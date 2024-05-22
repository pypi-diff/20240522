# Comparing `tmp/polarmints-0.1.8rc0.tar.gz` & `tmp/polarmints-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polarmints-0.1.8rc0.tar", max compression
+gzip compressed data, was "polarmints-0.1.9.tar", max compression
```

## Comparing `polarmints-0.1.8rc0.tar` & `polarmints-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1095 2023-07-15 15:46:38.393853 polarmints-0.1.8rc0/LICENSE
--rw-r--r--   0        0        0      639 2023-07-15 21:53:27.181490 polarmints-0.1.8rc0/polarmints/__init__.py
--rw-r--r--   0        0        0     2439 2023-11-13 08:52:17.986230 polarmints-0.1.8rc0/polarmints/aws.py
--rw-r--r--   0        0        0     4399 2023-11-13 09:15:08.913905 polarmints-0.1.8rc0/polarmints/core.py
--rw-r--r--   0        0        0     1386 2023-11-13 08:45:29.192739 polarmints-0.1.8rc0/polarmints/dateutils.py
--rw-r--r--   0        0        0     1132 2023-11-13 09:23:49.143462 polarmints-0.1.8rc0/polarmints/pandas.py
--rw-r--r--   0        0        0     1777 2023-08-31 21:42:20.285359 polarmints-0.1.8rc0/polarmints/pandas_mirror.py
--rw-r--r--   0        0        0      395 2023-07-15 21:58:08.349482 polarmints-0.1.8rc0/polarmints/sugar.py
--rw-r--r--   0        0        0     3733 2023-11-13 08:52:18.001859 polarmints-0.1.8rc0/polarmints/utils.py
--rw-r--r--   0        0        0      378 2023-11-13 09:24:43.043366 polarmints-0.1.8rc0/pyproject.toml
--rw-r--r--   0        0        0       12 2023-07-15 15:46:38.394854 polarmints-0.1.8rc0/README.md
--rw-r--r--   0        0        0      460 1970-01-01 00:00:00.000000 polarmints-0.1.8rc0/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-07-15 15:46:38.393853 polarmints-0.1.9/LICENSE
+-rw-r--r--   0        0        0      639 2023-07-15 21:53:27.181490 polarmints-0.1.9/polarmints/__init__.py
+-rw-r--r--   0        0        0     2710 2023-11-19 13:22:09.836836 polarmints-0.1.9/polarmints/aws.py
+-rw-r--r--   0        0        0     4399 2023-11-13 09:15:08.913905 polarmints-0.1.9/polarmints/core.py
+-rw-r--r--   0        0        0     1470 2023-11-19 13:20:43.882246 polarmints-0.1.9/polarmints/dateutils.py
+-rw-r--r--   0        0        0     1132 2023-11-13 09:23:49.143462 polarmints-0.1.9/polarmints/pandas.py
+-rw-r--r--   0        0        0     1777 2023-08-31 21:42:20.285359 polarmints-0.1.9/polarmints/pandas_mirror.py
+-rw-r--r--   0        0        0      399 2023-11-19 13:52:51.020287 polarmints-0.1.9/polarmints/sugar.py
+-rw-r--r--   0        0        0     4031 2023-11-19 13:52:51.040826 polarmints-0.1.9/polarmints/utils.py
+-rw-r--r--   0        0        0      376 2023-11-19 13:52:51.005559 polarmints-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-07-15 15:46:38.394854 polarmints-0.1.9/README.md
+-rw-r--r--   0        0        0      457 1970-01-01 00:00:00.000000 polarmints-0.1.9/PKG-INFO
```

### Comparing `polarmints-0.1.8rc0/LICENSE` & `polarmints-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polarmints-0.1.8rc0/polarmints/__init__.py` & `polarmints-0.1.9/polarmints/__init__.py`

 * *Files identical despite different names*

### Comparing `polarmints-0.1.8rc0/polarmints/aws.py` & `polarmints-0.1.9/polarmints/aws.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,23 @@
 import polars as pl
 from polars import DataFrame as DF
 try:
     from loguru import logger
 except:
     logger = logging.getLogger(__name__)
 
+######################################### HELPERS #########################################
 @lru_cache
 def fs3():
     return fs.S3FileSystem()
 
+def strip_s3_prefix(path: str) -> str:
+    return path.replace('s3://', '')
+
+######################################### MEAT #########################################
 def read_delta_s3(paths: str | list, exprs: list[list[tuple]] = [None], storage_options: dict = None, version: int = None,
                **kwargs) -> DF:
     """
 
     workaround until DeltaTable can read s3 as fast as pyarrow. and when it supports DNF predicates
     """
     if isinstance(paths, str):
@@ -44,14 +49,16 @@
 
     with timer(f'total s3 fetch {len(files)} files time: ' + '{cost}s'):
         df = pl.from_arrow(
             pq.read_table(files, filesystem=fs3(), **kwargs)
         )
     return df
 
+
+
 def get_paths(path: str | list[str], strip=True):
     if '*' in path:
         if not path.startswith('s3'):
             path = 's3://' + path
         with timer(f'listing files in {path} took ' + '{cost}s'):
             path = wr.s3.list_objects(path)
     if strip:
@@ -63,9 +70,9 @@
     path: str | list[str],
     **kwargs
 ) -> pl.DataFrame:
 
     path_ = get_paths(path)
     with timer(f'reading files {path} took ' + '{cost}s'):
         kwargs['use_pyarrow'] = True
-        kwargs['pyarrow_options'] = kwargs.get('pyarrow_options', {}) | {'filesystem': fs3()}
+        kwargs['pyarrow_options'] = (kwargs.get('pyarrow_options') or {}) | {'filesystem': fs3()}
         return pl.read_parquet(path_, **kwargs)
```

### Comparing `polarmints-0.1.8rc0/polarmints/core.py` & `polarmints-0.1.9/polarmints/core.py`

 * *Files identical despite different names*

### Comparing `polarmints-0.1.8rc0/polarmints/dateutils.py` & `polarmints-0.1.9/polarmints/dateutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,13 @@
             return pd.Series(res)
         case _:
             return res
 
 def start_end_pa_pred(col: str, start: date | str = None, end: date | str = None) -> list[tuple[str, str, pa.Date32Scalar]]:
     date_filter = []
     if start:
+        start = pd.Timestamp(start).date()
         date_filter.append((col, '>=', pa.scalar(start)))
     if end:
+        end = pd.Timestamp(end).date()
         date_filter.append((col, '<=', pa.scalar(end)))
     return date_filter
```

### Comparing `polarmints-0.1.8rc0/polarmints/pandas.py` & `polarmints-0.1.9/polarmints/pandas.py`

 * *Files identical despite different names*

### Comparing `polarmints-0.1.8rc0/polarmints/pandas_mirror.py` & `polarmints-0.1.9/polarmints/pandas_mirror.py`

 * *Files identical despite different names*

### Comparing `polarmints-0.1.8rc0/polarmints/utils.py` & `polarmints-0.1.9/polarmints/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+from contextlib import contextmanager
 from operator import and_
 from polarmints import c, DF
 import pyarrow.dataset as ds
 from typing import Iterable
 from functools import reduce
 import polars as pl
 from polars import lit, Expr, struct, DataFrame as DF
@@ -127,9 +128,17 @@
     res = primary_df.select([
         struct([df[col].rename(k)
             for k, df in dfs.items() if col in df
         ]).alias(col) if col in include else col
     for col in cols])
     return res
 
-
-
+def plv(cfg: pl.config.Config = None, rows=200, cols=25):
+    cfg = cfg or pl.Config()
+    cfg.set_tbl_rows(rows)
+    cfg.set_tbl_cols(cols)
+
+@contextmanager
+def plverbose(**kwargs):
+    with pl.Config() as cfg:
+        plv(cfg, **kwargs)
+        yield
```

