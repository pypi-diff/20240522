# Comparing `tmp/clickhouse-connect-0.7.8.tar.gz` & `tmp/clickhouse-connect-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.7.8.tar", last modified: Sun Apr 14 23:04:37 2024, max compression
+gzip compressed data, was "clickhouse-connect-0.7.9.tar", last modified: Tue May 21 18:07:32 2024, max compression
```

## Comparing `clickhouse-connect-0.7.8.tar` & `clickhouse-connect-0.7.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.760663 clickhouse-connect-0.7.8/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.768664 clickhouse-connect-0.7.8/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43035 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    23393 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driver/tzutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/dataconv.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/driverc/npconv.pyx
--rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/json_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 23:04:37.764664 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 23:04:37.000000 clickhouse-connect-0.7.8/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 23:04:37.772664 clickhouse-connect-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-14 23:04:36.000000 clickhouse-connect-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.295633 clickhouse-connect-0.7.9/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.295633 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.295633 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13684 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.295633 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.299633 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.299633 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14783 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.299633 clickhouse-connect-0.7.9/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23637 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driver/tzutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/dataconv.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/driverc/npconv.pyx
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1163 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/json_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8182 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:07:32.295633 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:07:32.303633 clickhouse-connect-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-21 18:07:32.000000 clickhouse-connect-0.7.9/setup.py
```

### Comparing `clickhouse-connect-0.7.8/LICENSE` & `clickhouse-connect-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/PKG-INFO` & `clickhouse-connect-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.7.8
+Version: 0.7.9
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.7.8/README.md` & `clickhouse-connect-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.7.9/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/common.py` & `clickhouse-connect-0.7.9/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.7.9/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.7.9/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.7.9/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.7.9/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
         username = username or parsed.username
         password = password or parsed.password
         host = host or parsed.hostname
         port = port or parsed.port
         if parsed.path and (not database or database == '__default__'):
             database = parsed.path[1:].split('/')[0]
         database = database or parsed.path
-        kwargs.update(dict(parse_qs(parsed.query)))
+        for k, v in parse_qs(parsed.query).items():
+            kwargs[k] = v[0]
     use_tls = str(secure).lower() == 'true' or interface == 'https' or (not interface and port in (443, 8443))
     if not host:
         host = 'localhost'
     if not interface:
         interface = 'https' if use_tls else 'http'
     port = port or default_port(interface, use_tls)
     if username is None and 'user' in kwargs:
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,30 +37,34 @@
     write_compression: str = None
     protocol_version = 0
     valid_transport_settings = set()
     optional_transport_settings = set()
     database = None
     max_error_message = 0
     apply_server_timezone = False
+    show_clickhouse_errors = True
 
     def __init__(self,
                  database: str,
                  query_limit: int,
                  uri: str,
                  query_retries: int,
                  server_host_name: Optional[str],
-                 apply_server_timezone: Optional[Union[str, bool]]):
+                 apply_server_timezone: Optional[Union[str, bool]],
+                 show_clickhouse_errors: Optional[bool]):
         """
         Shared initialization of ClickHouse Connect client
         :param database: database name
         :param query_limit: default LIMIT for queries
         :param uri: uri for error messages
         """
         self.query_limit = coerce_int(query_limit)
         self.query_retries = coerce_int(query_retries)
+        if show_clickhouse_errors is not None:
+            self.show_clickhouse_errors = coerce_bool(show_clickhouse_errors)
         self.server_host_name = server_host_name
         self.server_tz, dst_safe = pytz.UTC, True
         self.server_version, server_tz = \
             tuple(self.command('SELECT version(), timezone()', use_database=False))
         try:
             server_tz = pytz.timezone(server_tz)
             server_tz, dst_safe = tzutil.normalize_timezone(server_tz)
@@ -68,15 +72,15 @@
                 apply_server_timezone = dst_safe
             self.apply_server_timezone = apply_server_timezone == 'always' or coerce_bool(apply_server_timezone)
         except UnknownTimeZoneError:
             logger.warning('Warning, server is using an unrecognized timezone %s, will use UTC default', server_tz)
 
         if not self.apply_server_timezone and not tzutil.local_tz_dst_safe:
             logger.warning('local timezone %s may return unexpected times due to Daylight Savings Time/' +
-                           'Summer Time differences', tzutil.local_tz.tzname())
+                           'Summer Time differences', tzutil.local_tz.tzname(None))
         readonly = 'readonly'
         if not self.min_version('19.17'):
             readonly = common.get_setting('readonly')
         server_settings = self.query(f'SELECT name, value, {readonly} as readonly FROM system.settings LIMIT 10000')
         self.server_settings = {row['name']: SettingDef(**row) for row in server_settings.named_results()}
         if database and not database == '__default__':
             self.database = database
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/httpclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from clickhouse_connect.driver.ctypes import RespBuffCls
 from clickhouse_connect.driver.client import Client
 from clickhouse_connect.driver.common import dict_copy, coerce_bool, coerce_int
 from clickhouse_connect.driver.compression import available_compression
 from clickhouse_connect.driver.exceptions import DatabaseError, OperationalError, ProgrammingError
 from clickhouse_connect.driver.external import ExternalData
 from clickhouse_connect.driver.httputil import ResponseSource, get_pool_manager, get_response_data, \
-    default_pool_manager, get_proxy_manager, all_managers, check_env_proxy, check_conn_reset
+    default_pool_manager, get_proxy_manager, all_managers, check_env_proxy, check_conn_expiration
 from clickhouse_connect.driver.insert import InsertContext
 from clickhouse_connect.driver.summary import QuerySummary
 from clickhouse_connect.driver.query import QueryResult, QueryContext, quote_identifier, bind_query
 from clickhouse_connect.driver.transform import NativeTransform
 
 logger = logging.getLogger(__name__)
 columns_only_re = re.compile(r'LIMIT 0\s*$', re.IGNORECASE)
@@ -64,15 +64,16 @@
                  client_cert_key: Optional[str] = None,
                  session_id: Optional[str] = None,
                  settings: Optional[Dict[str, Any]] = None,
                  pool_mgr: Optional[PoolManager] = None,
                  http_proxy: Optional[str] = None,
                  https_proxy: Optional[str] = None,
                  server_host_name: Optional[str] = None,
-                 apply_server_timezone: Optional[Union[str, bool]] = None):
+                 apply_server_timezone: Optional[Union[str, bool]] = None,
+                 show_clickhouse_errors: Optional[bool] = None):
         """
         Create an HTTP ClickHouse Connect client
         See clickhouse_connect.get_client for parameters
         """
         self.url = f'{interface}://{host}:{port}'
         self.headers = {}
         ch_settings = dict_copy(settings, self.params)
@@ -110,15 +111,15 @@
 
         if not client_cert and username:
             self.headers['Authorization'] = 'Basic ' + b64encode(f'{username}:{password}'.encode()).decode()
         self.headers['User-Agent'] = common.build_client_name(client_name)
         self._read_format = self._write_format = 'Native'
         self._transform = NativeTransform()
 
-        # There is use cases when client need to disable timeouts.
+        # There are use cases when the client needs to disable timeouts.
         if connect_timeout is not None:
             connect_timeout = coerce_int(connect_timeout)
         if send_receive_timeout is not None:
             send_receive_timeout = coerce_int(send_receive_timeout)
         self.timeout = Timeout(connect=connect_timeout, read=send_receive_timeout)
         self.http_retries = 1
         self._send_progress = None
@@ -143,15 +144,16 @@
             compression = None
 
         super().__init__(database=database,
                          uri=self.url,
                          query_limit=query_limit,
                          query_retries=query_retries,
                          server_host_name=server_host_name,
-                         apply_server_timezone=apply_server_timezone)
+                         apply_server_timezone=apply_server_timezone,
+                         show_clickhouse_errors=show_clickhouse_errors)
         self.params = self._validate_settings(ch_settings)
         comp_setting = self._setting_status('enable_http_compression')
         self._send_comp_setting = not comp_setting.is_set and comp_setting.is_writable
         if comp_setting.is_set or comp_setting.is_writable:
             self.compression = compression
         send_setting = self._setting_status('send_progress_in_http_headers')
         self._send_progress = not send_setting.is_set and send_setting.is_writable
@@ -161,16 +163,15 @@
 
     def set_client_setting(self, key, value):
         str_value = self._validate_setting(key, value, common.get_setting('invalid_setting_action'))
         if str_value is not None:
             self.params[key] = str_value
 
     def get_client_setting(self, key) -> Optional[str]:
-        values = self.params.get(key)
-        return values[0] if values else None
+        return self.params.get(key)
 
     def _prep_query(self, context: QueryContext):
         final_query = super()._prep_query(context)
         if context.is_insert:
             return final_query
         return f'{final_query}\n FORMAT {self._read_format}'
 
@@ -353,16 +354,19 @@
             err_content = get_response_data(response)
         except Exception: # pylint: disable=broad-except
             err_content = None
         finally:
             response.close()
 
         if err_content:
-            err_msg = common.format_error(err_content.decode(errors='backslashreplace'))
-            err_str = f':{err_str}\n {err_msg}'
+            if self.show_clickhouse_errors:
+                err_msg = common.format_error(err_content.decode(errors='backslashreplace'))
+                err_str = f':{err_str}\n {err_msg}'
+            else:
+                err_str = 'The ClickHouse server returned an error.'
         raise OperationalError(err_str) if retried else DatabaseError(err_str) from None
 
     def _raw_request(self,
                      data,
                      params: Dict[str, str],
                      headers: Optional[Dict[str, Any]] = None,
                      method: str = 'POST',
@@ -395,15 +399,15 @@
         if self.server_host_name:
             kwargs['assert_same_host'] = False
             kwargs['headers'].update({'Host': self.server_host_name})
         if fields:
             kwargs['fields'] = fields
         else:
             kwargs['body'] = data
-        check_conn_reset(self.http)
+        check_conn_expiration(self.http)
         query_session = final_params.get('session_id')
         while True:
             attempts += 1
             if query_session:
                 if query_session == self._active_session:
                     raise ProgrammingError('Attempt to execute concurrent queries within the same session.' +
                                            'Please use a separate client instance per thread/process.')
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/httputil.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from urllib3.response import HTTPResponse
 
 from clickhouse_connect.driver.exceptions import ProgrammingError
 from clickhouse_connect import common
 
 logger = logging.getLogger(__name__)
 
-# We disable this warning.  Verify must explicitly set to false, so we assume the user knows what they're doing
+# We disable this warning.  Verify must be explicitly set to false, so we assume the user knows what they're doing
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 # Increase this number just to be safe when ClickHouse is returning progress headers
 http.client._MAXHEADERS = 10000  # pylint: disable=protected-access
 
 DEFAULT_KEEP_INTERVAL = 30
 DEFAULT_KEEP_COUNT = 3
@@ -114,21 +114,21 @@
         manager = ProxyManager(https_proxy, **options)
     else:
         manager = PoolManager(**options)
     all_managers[manager] = int(time.time())
     return manager
 
 
-def check_conn_reset(manager: PoolManager):
+def check_conn_expiration(manager: PoolManager):
     reset_seconds = common.get_setting('max_connection_age')
     if reset_seconds:
         last_reset = all_managers.get(manager, 0)
         now = int(time.time())
         if last_reset < now - reset_seconds:
-            logger.debug('connection reset')
+            logger.debug('connection expiration')
             manager.clear()
             all_managers[manager] = now
 
 
 def get_proxy_manager(host: str, http_proxy):
     key = f'{host}__{http_proxy}'
     if key in _proxy_managers:
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/npquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         if self._block_gen is None:
             raise StreamClosedError
         bg = self._block_gen
         chain = itertools.chain
         chains = [chain(b) for b in zip(*bg)]
         new_df_series = []
         for c in chains:
-            new_df_series.append(pd.concat([pd.Series(piece, copy=False) for piece in c],
+            new_df_series.append(pd.concat([pd.Series(piece, copy=False) for piece in c if len(piece) > 0],
                                            copy=False, ignore_index=True))
         self._df_result = pd.DataFrame(dict(zip(self.column_names, new_df_series)))
         self.close()
         return self
 
     @property
     def np_result(self):
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/summary.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/summary.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driver/tzutil.py` & `clickhouse-connect-0.7.9/clickhouse_connect/driver/tzutil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driverc/buffer.pxd` & `clickhouse-connect-0.7.9/clickhouse_connect/driverc/buffer.pxd`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driverc/buffer.pyx` & `clickhouse-connect-0.7.9/clickhouse_connect/driverc/buffer.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/driverc/dataconv.pyx` & `clickhouse-connect-0.7.9/clickhouse_connect/driverc/dataconv.pyx`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.7.9/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.7.9/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.7.9/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.7.9/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.7.9/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.7.8
+Version: 0.7.9
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.7.8/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.7.9/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.7.8/setup.py` & `clickhouse-connect-0.7.9/setup.py`

 * *Files identical despite different names*

