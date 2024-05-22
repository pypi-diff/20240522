# Comparing `tmp/stac_fastapi_pgstac-3.0.0a0.tar.gz` & `tmp/stac_fastapi_pgstac-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_pgstac-3.0.0a0.tar", last modified: Fri May 10 14:19:33 2024, max compression
+gzip compressed data, was "stac_fastapi_pgstac-3.0.0a1.tar", last modified: Wed May 22 16:59:35 2024, max compression
```

## Comparing `stac_fastapi_pgstac-3.0.0a0.tar` & `stac_fastapi_pgstac-3.0.0a1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.665520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/base_item_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 14:19:33.000000 stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.665520 stac_fastapi_pgstac-3.0.0a0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24803 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/api/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.669520 stac_fastapi_pgstac-3.0.0a0/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/clients/test_postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:33.673520 stac_fastapi_pgstac-3.0.0a0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    51039 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-10 14:19:23.000000 stac_fastapi_pgstac-3.0.0a0/tests/resources/test_mgmt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.425942 stac_fastapi_pgstac-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 16:59:35.425942 stac_fastapi_pgstac-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.413942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.417942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15142 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.417942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.417942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/types/base_item_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 16:59:35.000000 stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.413942 stac_fastapi_pgstac-3.0.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24803 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/api/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/clients/test_postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:35.421942 stac_fastapi_pgstac-3.0.0a1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/resources/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/resources/test_conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51039 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/resources/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 16:59:26.000000 stac_fastapi_pgstac-3.0.0a1/tests/resources/test_mgmt.py
```

### Comparing `stac_fastapi_pgstac-3.0.0a0/LICENSE` & `stac_fastapi_pgstac-3.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/PKG-INFO` & `stac_fastapi_pgstac-3.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,18 +14,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: orjson
 Requires-Dist: pydantic
-Requires-Dist: stac_pydantic==3.0.*
-Requires-Dist: stac-fastapi.api~=3.0.0a0
-Requires-Dist: stac-fastapi.extensions~=3.0.0a0
-Requires-Dist: stac-fastapi.types~=3.0.0a0
+Requires-Dist: stac_pydantic==3.1.*
+Requires-Dist: stac-fastapi.api~=3.0.0a1
+Requires-Dist: stac-fastapi.extensions~=3.0.0a1
+Requires-Dist: stac-fastapi.types~=3.0.0a1
 Requires-Dist: asyncpg
 Requires-Dist: buildpg
 Requires-Dist: brotli_asgi
 Requires-Dist: pygeofilter>=0.2
 Requires-Dist: pypgstac==0.8.*
 Provides-Extra: dev
 Requires-Dist: pystac[validation]; extra == "dev"
@@ -100,15 +100,15 @@
 See [CONTRIBUTING](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/CONTRIBUTING.md) for detailed contribution instructions.
 
 To install:
 
 ```shell
 git clone https://github.com/stac-utils/stac-fastapi-pgstac
 cd stac-fastapi-pgstac
-pip install -e ".[dev,server,docs]"
+python -m pip install -e ".[dev,server,docs]"
 ```
 
 To test:
 
 ```shell
 make test
 ```
```

### Comparing `stac_fastapi_pgstac-3.0.0a0/README.md` & `stac_fastapi_pgstac-3.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 See [CONTRIBUTING](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/CONTRIBUTING.md) for detailed contribution instructions.
 
 To install:
 
 ```shell
 git clone https://github.com/stac-utils/stac-fastapi-pgstac
 cd stac-fastapi-pgstac
-pip install -e ".[dev,server,docs]"
+python -m pip install -e ".[dev,server,docs]"
 ```
 
 To test:
 
 ```shell
 make test
 ```
```

### Comparing `stac_fastapi_pgstac-3.0.0a0/pyproject.toml` & `stac_fastapi_pgstac-3.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/setup.py` & `stac_fastapi_pgstac-3.0.0a1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
     "attrs",
     "orjson",
     "pydantic",
-    "stac_pydantic==3.0.*",
-    "stac-fastapi.api~=3.0.0a0",
-    "stac-fastapi.extensions~=3.0.0a0",
-    "stac-fastapi.types~=3.0.0a0",
+    "stac_pydantic==3.1.*",
+    "stac-fastapi.api~=3.0.0a1",
+    "stac-fastapi.extensions~=3.0.0a1",
+    "stac-fastapi.types~=3.0.0a1",
     "asyncpg",
     "buildpg",
     "brotli_asgi",
     "pygeofilter>=0.2",
     "pypgstac==0.8.*",
 ]
```

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/app.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/config.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/core.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/core.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/db.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/db.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/filter.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/extensions/query.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/extensions/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/models/links.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/models/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/transactions.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/transactions.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/base_item_cache.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/types/base_item_cache.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/types/search.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/types/search.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi/pgstac/utils.py` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi/pgstac/utils.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/PKG-INFO` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.pgstac
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework and using the pgstac backend.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: David Bitner
 Author-email: david@developmentseed.org
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,18 +14,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: attrs
 Requires-Dist: orjson
 Requires-Dist: pydantic
-Requires-Dist: stac_pydantic==3.0.*
-Requires-Dist: stac-fastapi.api~=3.0.0a0
-Requires-Dist: stac-fastapi.extensions~=3.0.0a0
-Requires-Dist: stac-fastapi.types~=3.0.0a0
+Requires-Dist: stac_pydantic==3.1.*
+Requires-Dist: stac-fastapi.api~=3.0.0a1
+Requires-Dist: stac-fastapi.extensions~=3.0.0a1
+Requires-Dist: stac-fastapi.types~=3.0.0a1
 Requires-Dist: asyncpg
 Requires-Dist: buildpg
 Requires-Dist: brotli_asgi
 Requires-Dist: pygeofilter>=0.2
 Requires-Dist: pypgstac==0.8.*
 Provides-Extra: dev
 Requires-Dist: pystac[validation]; extra == "dev"
@@ -100,15 +100,15 @@
 See [CONTRIBUTING](https://github.com/stac-utils/stac-fastapi-pgstac/blob/main/CONTRIBUTING.md) for detailed contribution instructions.
 
 To install:
 
 ```shell
 git clone https://github.com/stac-utils/stac-fastapi-pgstac
 cd stac-fastapi-pgstac
-pip install -e ".[dev,server,docs]"
+python -m pip install -e ".[dev,server,docs]"
 ```
 
 To test:
 
 ```shell
 make test
 ```
```

### Comparing `stac_fastapi_pgstac-3.0.0a0/stac_fastapi.pgstac.egg-info/SOURCES.txt` & `stac_fastapi_pgstac-3.0.0a1/stac_fastapi.pgstac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/tests/api/test_api.py` & `stac_fastapi_pgstac-3.0.0a1/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/tests/clients/test_postgres.py` & `stac_fastapi_pgstac-3.0.0a1/tests/clients/test_postgres.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_collection.py` & `stac_fastapi_pgstac-3.0.0a1/tests/resources/test_collection.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_conformance.py` & `stac_fastapi_pgstac-3.0.0a1/tests/resources/test_conformance.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_pgstac-3.0.0a0/tests/resources/test_item.py` & `stac_fastapi_pgstac-3.0.0a1/tests/resources/test_item.py`

 * *Files identical despite different names*

