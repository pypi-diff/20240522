# Comparing `tmp/constellate-0.8.8.tar.gz` & `tmp/constellate-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "constellate-0.8.8.tar", last modified: Fri May 10 13:29:35 2024, max compression
+gzip compressed data, was "constellate-0.8.9.tar", last modified: Sun May 12 10:43:50 2024, max compression
```

## Comparing `constellate-0.8.8.tar` & `constellate-0.8.9.tar`

### file list

```diff
@@ -1,286 +1,286 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.589729 constellate-0.8.8/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-10 13:28:35.000000 constellate-0.8.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-10 13:28:35.000000 constellate-0.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3919 2024-05-10 13:29:35.589729 constellate-0.8.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-10 13:28:35.000000 constellate-0.8.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.557728 constellate-0.8.8/constellate/
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.557728 constellate-0.8.8/constellate/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/cli/argument/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cli/argument/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cli/argument/unparse.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/compression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/compression/zip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zip/zip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/compression/zstd/
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zstd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zstd/common.py
--rw-rw-rw-   0 root         (0) root         (0)     2102 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zstd/pyzstd.py
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/compression/zstd/zstandard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/concurrency/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/concurrency/asyncio/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/asyncio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3031 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/asyncio/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/concurrency/pebble/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/pebble/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2792 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/pebble/pool_cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/concurrency/simple/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/simple/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4057 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/simple/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/concurrency/std/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/std/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/concurrency/std/pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/constant/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/constant/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/constant/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/constant/debug.py
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/constant/platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/container/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/container/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/container/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/container/orchestration/k8s/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/container/orchestration/k8s/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/container/orchestration/k8s/probe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.561728 constellate-0.8.8/constellate/cryptography/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cryptography/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/cryptography/digest/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cryptography/digest/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/cryptography/digest/hexadecimal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/common/databasetype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/migration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     2220 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     6720 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/migrate.py
--rw-rw-rw-   0 root         (0) root         (0)     3429 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/migrationcontext.py
--rw-rw-rw-   0 root         (0) root         (0)     9700 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/migrationstep.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/migration/standard/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/standard/base.py
--rw-rw-rw-   0 root         (0) root         (0)    22342 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/standard/migrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/standard/table.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/migration/tablecontext.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/sparql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sparql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sparql/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/sparql/sparqlburger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sparql/sparqlburger/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sparql/sparqlburger/triple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.565728 constellate-0.8.8/constellate/database/sqlalchemy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/crud/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/crud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/crud/cru.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/exception/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/exception/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/exception/migrationexception.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/exception/vacumexception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/execution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7472 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/execution/execute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/expression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/create.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/drop.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/setsearchpath.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/drop.py
--rw-rw-rw-   0 root         (0) root         (0)     1641 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/lock.py
--rw-rw-rw-   0 root         (0) root         (0)     3546 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/presence.py
--rw-rw-rw-   0 root         (0) root         (0)     1105 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/expression/table/truncate.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/relationshiptype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/session/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/session/binder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/binder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/binder/binderresolver.py
--rw-rw-rw-   0 root         (0) root         (0)     6094 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/multienginesession.py
--rw-rw-rw-   0 root         (0) root         (0)     3781 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/syncmultienginesession.py
--rw-rw-rw-   0 root         (0) root         (0)     3097 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.569728 constellate-0.8.8/constellate/database/sqlalchemy/sharding/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sharding/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7054 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sharding/sharder.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sharding/shardoption.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sharding/simplesession.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sharding/unittoshardmixin.py
--rw-rw-rw-   0 root         (0) root         (0)    32171 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemydbconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1477 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemyengineconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    13143 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemypostgresql.py
--rw-rw-rw-   0 root         (0) root         (0)     9929 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemysqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enuminteger.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enumstring.py
--rw-rw-rw-   0 root         (0) root         (0)     2097 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enumvalue.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/timestamptz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/database/sqlalchemy/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16098 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/types/composite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/database/sqlalchemy/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/utils/sessioncommit.py
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlalchemy/utils/sql_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/database/sqlite3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlite3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/database/sqlite3/sqlite3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/datatype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/datatype/dictionary/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/dictionary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/dictionary/pop.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/dictionary/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/datatype/enum/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/enum/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datatype/enum/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/datetime/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datetime/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/datetime/timeinterval/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datetime/timeinterval/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/datetime/timeinterval/timeinterval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debug/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/debug/packages/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debug/packages/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debug/packages/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/debugger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debugger/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debugger/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)      737 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/debugger/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.573729 constellate-0.8.8/constellate/logger/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/logger/formatter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/formatter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/formatter/formatterfactory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/logger/handler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/handler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/handler/forwarderhandler.py
--rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/handler/stringhandler.py
--rw-rw-rw-   0 root         (0) root         (0)    20171 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/log.py
--rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/logmode.py
--rw-rw-rw-   0 root         (0) root         (0)     3048 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/logger/simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/network/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/network/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/network/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/network/download/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/network/url/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/network/url/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/network/url/unshortener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/package/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/package/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/pretty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/pretty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/pretty/log/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/pretty/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/pretty/log/line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/progression/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/progression/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/progression/progres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/project/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/project/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/project/version.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/resource/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/storage/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/storage/filesystem/anyfs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/anyfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/anyfs/availability.py
--rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/anyfs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/anyfs/size.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/storage/filesystem/tmpfs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/tmpfs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6635 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/tmpfs/memory_tempfile.py
--rw-rw-rw-   0 root         (0) root         (0)     2692 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/storage/filesystem/tmpfs/rambacked.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.577729 constellate-0.8.8/constellate/testing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/testing/mock/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/testing/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/testing/mock/argv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/numba/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/numba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/numba/progress/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/numba/progress/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/numba/progress/progress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/accessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/accessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3173 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/accessor/attribute_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/extra/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/extra/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/extra/sanitize/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/extra/sanitize/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11051 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/extra/sanitize/sanitize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/io/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/io/sql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/io/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/operation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/operation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/operation/introspection/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/operation/introspection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/operation/introspection/introspection.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandas/validation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/validation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/validation/pandera.py
--rw-rw-rw-   0 root         (0) root         (0)     7088 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandas/validation/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/thirdparty/pandera/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandera/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/thirdparty/pandera/inspector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/virtualization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/virtualization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/virtualization/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/virtualization/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/virtualization/common/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.581729 constellate-0.8.8/constellate/virtualization/docker/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-10 13:28:35.000000 constellate-0.8.8/constellate/virtualization/docker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.585729 constellate-0.8.8/constellate.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3919 2024-05-10 13:29:35.000000 constellate-0.8.8/constellate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8749 2024-05-10 13:29:35.000000 constellate-0.8.8/constellate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 13:29:35.000000 constellate-0.8.8/constellate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      904 2024-05-10 13:29:35.000000 constellate-0.8.8/constellate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-10 13:29:35.000000 constellate-0.8.8/constellate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     3085 2024-05-10 13:28:35.000000 constellate-0.8.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-10 13:29:35.589729 constellate-0.8.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 13:29:35.585729 constellate-0.8.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_cli_argument.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_compression.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_cryptography.py
--rw-rw-rw-   0 root         (0) root         (0)     1373 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     9700 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    19319 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_migration.py
--rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_pandas.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_pandera.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_progression.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_sparql.py
--rw-rw-rw-   0 root         (0) root         (0)    11500 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_sqlalchemy.py
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-10 13:28:35.000000 constellate-0.8.8/tests/test_storage_filesystem_tmpfs_rambacked.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.151869 constellate-0.8.9/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-12 10:42:51.000000 constellate-0.8.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-12 10:42:51.000000 constellate-0.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-12 10:43:50.151869 constellate-0.8.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-05-12 10:42:51.000000 constellate-0.8.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.111867 constellate-0.8.9/constellate/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.111867 constellate-0.8.9/constellate/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.111867 constellate-0.8.9/constellate/cli/argument/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cli/argument/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cli/argument/unparse.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/compression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/compression/zip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zip/zip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/compression/zstd/
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zstd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1630 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zstd/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     2102 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zstd/pyzstd.py
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/compression/zstd/zstandard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/concurrency/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/concurrency/asyncio/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/asyncio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3031 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/asyncio/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/concurrency/pebble/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/pebble/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2792 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/pebble/pool_cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/concurrency/simple/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/simple/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/simple/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/concurrency/std/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/std/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/concurrency/std/pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/constant/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/constant/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/constant/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/constant/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/constant/platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/container/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.115867 constellate-0.8.9/constellate/container/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/container/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/container/orchestration/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/container/orchestration/k8s/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/container/orchestration/k8s/probe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/cryptography/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cryptography/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/cryptography/digest/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cryptography/digest/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/cryptography/digest/hexadecimal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/common/databasetype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     2220 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     6720 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3429 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/migrationcontext.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/migrationstep.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/migration/standard/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/standard/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    22342 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/standard/migrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/standard/table.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/migration/tablecontext.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/sparql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sparql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sparql/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.119867 constellate-0.8.9/constellate/database/sparql/sparqlburger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sparql/sparqlburger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      553 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sparql/sparqlburger/triple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/crud/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/crud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/crud/cru.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/exception/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/exception/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       46 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/exception/migrationexception.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/exception/vacumexception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/execution/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7455 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/execution/execute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/expression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1510 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/drop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/setsearchpath.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.123868 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/drop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1641 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/lock.py
+-rw-rw-rw-   0 root         (0) root         (0)     3546 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/presence.py
+-rw-rw-rw-   0 root         (0) root         (0)     1105 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/expression/table/truncate.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/relationshiptype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/session/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/session/binder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/binder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/binder/binderresolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6094 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/multienginesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     3781 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/syncmultienginesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     3097 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/sharding/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sharding/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7054 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sharding/sharder.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sharding/shardoption.py
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sharding/simplesession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sharding/unittoshardmixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    32171 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemydbconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1477 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemyengineconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemymigrationconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    13143 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemypostgresql.py
+-rw-rw-rw-   0 root         (0) root         (0)     9929 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemysqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enuminteger.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enumstring.py
+-rw-rw-rw-   0 root         (0) root         (0)     2097 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enumvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/timestamptz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16098 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/types/composite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlalchemy/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/utils/sessioncommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlalchemy/utils/sql_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.127868 constellate-0.8.9/constellate/database/sqlite3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlite3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/database/sqlite3/sqlite3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/datatype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/datatype/dictionary/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/dictionary/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/dictionary/pop.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/dictionary/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/datatype/enum/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/enum/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datatype/enum/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/datetime/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datetime/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/datetime/timeinterval/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datetime/timeinterval/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10682 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/datetime/timeinterval/timeinterval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debug/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/debug/packages/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debug/packages/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debug/packages/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/debugger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debugger/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debugger/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)      737 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/debugger/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.131868 constellate-0.8.9/constellate/logger/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/logger/formatter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/formatter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      770 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/formatter/formatterfactory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/logger/handler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/handler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/handler/forwarderhandler.py
+-rw-rw-rw-   0 root         (0) root         (0)      572 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/handler/stringhandler.py
+-rw-rw-rw-   0 root         (0) root         (0)    20306 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/logmode.py
+-rw-rw-rw-   0 root         (0) root         (0)     3048 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/logger/simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/network/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/network/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/network/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/network/download/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/network/url/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/network/url/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/network/url/unshortener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/package/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/package/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/pretty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/pretty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/pretty/log/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/pretty/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/pretty/log/line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/progression/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/progression/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/progression/progres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/project/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/project/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/project/version.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/resource/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.135868 constellate-0.8.9/constellate/storage/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/storage/filesystem/anyfs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/anyfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/anyfs/availability.py
+-rw-rw-rw-   0 root         (0) root         (0)     3804 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/anyfs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/anyfs/size.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/storage/filesystem/tmpfs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/tmpfs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/tmpfs/memory_tempfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2692 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/storage/filesystem/tmpfs/rambacked.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/testing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/testing/mock/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/testing/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/testing/mock/argv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/numba/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/numba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/numba/progress/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/numba/progress/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/numba/progress/progress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/pandas/accessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/accessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3173 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/accessor/attribute_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/pandas/extra/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/extra/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/pandas/extra/sanitize/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/extra/sanitize/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10997 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/extra/sanitize/sanitize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.139869 constellate-0.8.9/constellate/thirdparty/pandas/io/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/thirdparty/pandas/io/sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/io/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/thirdparty/pandas/operation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/operation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/thirdparty/pandas/operation/introspection/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/operation/introspection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/operation/introspection/introspection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/thirdparty/pandas/validation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/validation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/validation/pandera.py
+-rw-rw-rw-   0 root         (0) root         (0)     7075 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandas/validation/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/thirdparty/pandera/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandera/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/thirdparty/pandera/inspector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/virtualization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/virtualization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/virtualization/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/virtualization/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/virtualization/common/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.143869 constellate-0.8.9/constellate/virtualization/docker/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 10:42:51.000000 constellate-0.8.9/constellate/virtualization/docker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.147869 constellate-0.8.9/constellate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3919 2024-05-12 10:43:50.000000 constellate-0.8.9/constellate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8749 2024-05-12 10:43:50.000000 constellate-0.8.9/constellate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-12 10:43:50.000000 constellate-0.8.9/constellate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      904 2024-05-12 10:43:50.000000 constellate-0.8.9/constellate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-12 10:43:50.000000 constellate-0.8.9/constellate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3085 2024-05-12 10:42:51.000000 constellate-0.8.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-05-12 10:43:50.151869 constellate-0.8.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-12 10:43:50.147869 constellate-0.8.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_cli_argument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_compression.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_cryptography.py
+-rw-rw-rw-   0 root         (0) root         (0)     1373 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     9700 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    19319 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)     8679 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_pandera.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_progression.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     1988 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_sparql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11501 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_sqlalchemy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1739 2024-05-12 10:42:51.000000 constellate-0.8.9/tests/test_storage_filesystem_tmpfs_rambacked.py
```

### Comparing `constellate-0.8.8/PKG-INFO` & `constellate-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellate
-Version: 0.8.8
+Version: 0.8.9
 Summary: A bunch of utilities aggregated over time
 Author-email: David Andreoletti <none@provided.yet>
 Project-URL: repository, https://github.com/davidandreoletti/constellate
 Keywords: constellate
 Classifier: License :: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: decorator>=5.1.0
 Requires-Dist: aioitertools>=0.8.0
 Requires-Dist: psutil>=5.7.0
-Requires-Dist: pendulum>=2.1.2
+Requires-Dist: pendulum>=3.0.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: memory-tempfile>=2.2.3
 Requires-Dist: bidict>=0.21.4
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: portion>=2.2.0
 Requires-Dist: jsonmerge>=1.8.0
 Requires-Dist: jsonschema>=4.7.2
```

### Comparing `constellate-0.8.8/README.rst` & `constellate-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/cli/argument/unparse.py` & `constellate-0.8.9/constellate/cli/argument/unparse.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/compression/zip/zip.py` & `constellate-0.8.9/constellate/compression/zip/zip.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/compression/zstd/common.py` & `constellate-0.8.9/constellate/compression/zstd/common.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/compression/zstd/pyzstd.py` & `constellate-0.8.9/constellate/compression/zstd/pyzstd.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/compression/zstd/zstandard.py` & `constellate-0.8.9/constellate/compression/zstd/zstandard.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/concurrency/asyncio/tasks.py` & `constellate-0.8.9/constellate/concurrency/asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/concurrency/pebble/pool_cleanup.py` & `constellate-0.8.9/constellate/concurrency/pebble/pool_cleanup.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/concurrency/simple/simple.py` & `constellate-0.8.9/constellate/concurrency/simple/simple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/concurrency/std/pool.py` & `constellate-0.8.9/constellate/concurrency/std/pool.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/cryptography/digest/hexadecimal.py` & `constellate-0.8.9/constellate/cryptography/digest/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/constant.py` & `constellate-0.8.9/constellate/database/migration/constant.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/metadata.py` & `constellate-0.8.9/constellate/database/migration/metadata.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/migrate.py` & `constellate-0.8.9/constellate/database/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/migrationcontext.py` & `constellate-0.8.9/constellate/database/migration/migrationcontext.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/migrationstep.py` & `constellate-0.8.9/constellate/database/migration/migrationstep.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 raise NotImplementedError("Migration script can have up to 1 dependencies only")
 
         def build_step_files(
             migration_files: List[Path] = None, previous_migration_files: List[Path] = None
         ) -> List[MigrationStepFile]:
             step_files = {}
             previous_mf = None
-            for index, mf in enumerate(migration_files):
+            for _index, mf in enumerate(migration_files):
                 if mf.name in step_files:
                     raise ValueError(
                         f"2+ migration files share the same name {mf.name}. Only 1 must be specified"
                     )
 
                 pymodule, metadata = _read_file_metadata(file=mf)
                 validate_metadata(metadata=metadata)
```

### Comparing `constellate-0.8.8/constellate/database/migration/standard/migrate.py` & `constellate-0.8.9/constellate/database/migration/standard/migrate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/migration/standard/table.py` & `constellate-0.8.9/constellate/database/migration/standard/table.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sparql/query.py` & `constellate-0.8.9/constellate/database/sparql/query.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sparql/sparqlburger/triple.py` & `constellate-0.8.9/constellate/database/sparql/sparqlburger/triple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/crud/cru.py` & `constellate-0.8.9/constellate/database/sqlalchemy/crud/cru.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/execution/execute.py` & `constellate-0.8.9/constellate/database/sqlalchemy/execution/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 if result_stream_max_row_buffer is not None
                 else result
             )
             # result's type: iter[X]
             # result = chain.from_iterable(result)
 
         return await __execute_select_return_iterable(result=result)
-    elif return_result_as_async_generator:
+    if return_result_as_async_generator:
         if result_stream:
             # result's type: iter[list[X]]
             result = (
                 result.partitions(result_stream_max_row_buffer)
                 if result_stream_max_row_buffer is not None
                 else result
             )
@@ -87,20 +87,20 @@
             # async generator
             return result
 
         # coroutine
         result = __execute_select_return_async_generator(result=result)
         # async generator
         return result
-    elif return_result_discard:
+    if return_result_discard:
         # 'Discard any rows left to fetch
         result.close()
         return None
-    else:
-        raise NotImplementedError()
+
+    raise NotImplementedError()
 
 
 async def __execute_select_return_sqlalchemy_native(
     result: AsyncResult = None,
 ) -> Union[X, Optional[X], List[X]]:
     return result
```

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/create.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/create.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/drop.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/drop.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/schema/setsearchpath.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/schema/setsearchpath.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/table/drop.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/table/drop.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/table/lock.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/table/lock.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/table/presence.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/table/presence.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/expression/table/truncate.py` & `constellate-0.8.9/constellate/database/sqlalchemy/expression/table/truncate.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/session/binder/binderresolver.py` & `constellate-0.8.9/constellate/database/sqlalchemy/session/binder/binderresolver.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/session/multienginesession.py` & `constellate-0.8.9/constellate/database/sqlalchemy/session/multienginesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/session/syncmultienginesession.py` & `constellate-0.8.9/constellate/database/sqlalchemy/session/syncmultienginesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py` & `constellate-0.8.9/constellate/database/sqlalchemy/session/syncmultiengineshardsession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sharding/sharder.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sharding/sharder.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sharding/shardoption.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sharding/shardoption.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sharding/simplesession.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sharding/simplesession.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sharding/unittoshardmixin.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sharding/unittoshardmixin.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemy.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemydbconfig.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemydbconfig.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemydbconfigmanager.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemyengineconfig.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemyengineconfig.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemypostgresql.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemypostgresql.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/sqlalchemysqlite3.py` & `constellate-0.8.9/constellate/database/sqlalchemy/sqlalchemysqlite3.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enuminteger.py` & `constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enuminteger.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enumstring.py` & `constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enumstring.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/enumvalue.py` & `constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/enumvalue.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/typedecorator/timestamptz.py` & `constellate-0.8.9/constellate/database/sqlalchemy/typedecorator/timestamptz.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/types/composite.py` & `constellate-0.8.9/constellate/database/sqlalchemy/types/composite.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/database/sqlalchemy/utils/sql_query.py` & `constellate-0.8.9/constellate/database/sqlalchemy/utils/sql_query.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 from sqlalchemy.sql import Select, Executable
 
 
 def stringify(
     query: Union[Select, Executable] = None,
     engine: Engine = None,
     dialect: DefaultDialect = None,
-    compile_kwargs: Dict = {},
+    compile_kwargs: Dict = None,
 ) -> str:
     """@query: Query object to get plain SQL query from
     @engine: Database type to know the SQL dialect to convert into
 
     src: https://stackoverflow.com/a/23835766/219728
 
     :param query: Union[Select:
     :param Executable]:  (Default value = None)
     :param engine: Engine:  (Default value = None)
     :param dialect: DefaultDialect:  (Default value = None)
     :param compile_kwargs: Dict:  (Default value = {})
 
     """
+    compile_kwargs = compile_kwargs or {}
     return (
         query.compile(engine)
         if engine is not None
         else query.compile(
             dialect=dialect, compile_kwargs={"literal_binds": True, **compile_kwargs}
         )
     )
@@ -41,11 +42,10 @@
     """
     # PERF: This will execute the query!!!! As of 2021 May, I did not find a way to get this info without executing the
     # query against the db
     result = await session.execute(query)
 
     # Fetch 1 or 0 result and **release the underlying cursor**, to prevent
     # virtual transaction to be held open on the database
-    ignored = result.scalars().all()
+    _ignored = result.scalars().all()
 
-    engine = result.raw.connection.engine
-    return engine
+    return result.raw.connection.engine
```

### Comparing `constellate-0.8.8/constellate/database/sqlite3/sqlite3.py` & `constellate-0.8.9/constellate/database/sqlite3/sqlite3.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/datatype/dictionary/update.py` & `constellate-0.8.9/constellate/datatype/dictionary/update.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/datetime/timeinterval/timeinterval.py` & `constellate-0.8.9/constellate/datetime/timeinterval/timeinterval.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import operator
 import sys
 from functools import reduce
 from typing import Generator, Any, Union, Tuple, List, Iterator
 
 import pandas
 import pendulum
+from pendulum import Interval as PendulumInterval
 import portion
-import portion as P
-from numpy import int64
-from pendulum import Period
 from portion import Interval, Bound, empty, IntervalDict
+from numpy import int64
+
 
 UTCTimestampMilliSec = int
 
 
 def __utctimestamp_millisec_converter(
     in_value: Union[int, int64, pendulum.DateTime, pendulum.Date, pandas.Timestamp],
 ):
     if isinstance(in_value, (int, int64)):
         return in_value
     if isinstance(in_value, (pendulum.DateTime, pendulum.Date)):
         return int(in_value.float_timestamp * 1000)
     if isinstance(in_value, pandas.Timestamp):
         return pendulum.instance(in_value.to_pydatetime()).int_timestamp * 1000
-    raise Exception(f"{in_value} not convertible to {type(UTCTimestampMilliSec)}")
+    raise ValueError(f"{in_value} not convertible to {type(UTCTimestampMilliSec)}")
 
 
 class TimeInterval(Interval):
     def __init__(
         self,
         *obj: Union[Interval, Tuple],  # Tuple==Tuple[Union[Interval, TimeInterval]]
     ):
@@ -39,15 +39,15 @@
         return self.lower
 
     @property
     def end(self):
         return self.upper
 
     # Conversion utilities
-    def to_pendulum_period(self, adjust_bounds: bool = False) -> Period:
+    def to_pendulum_period(self, adjust_bounds: bool = False) -> PendulumInterval:
         if self.start in [portion.inf, -portion.inf] or self.end in [portion.inf, -portion.inf]:
             raise ValueError("Infinite period cannot be computed")
 
         start = self.start - 1 if adjust_bounds and self.left is Bound.OPEN else self.start
         start = pendulum.from_timestamp(timestamp=start / 1000.0, tz="UTC")
         end = self.end + 1 if adjust_bounds and self.right is Bound.OPEN else self.end
         end = pendulum.from_timestamp(timestamp=end / 1000.0, tz="UTC")
@@ -63,41 +63,41 @@
         """
         if not self.intersection(other):
             raise ValueError()
 
         # )1,inf(
         inv_other = (~other)._intervals[-1]
         # [3, inf]
-        inv_other = P.closed(inv_other.lower, inv_other.upper)
+        inv_other = portion.closed(inv_other.lower, inv_other.upper)
         # [-5, 5] & [3, inf] => [3, 5]
         return TimeInterval(self & inv_other)
 
     def leftmost_intersected_complement(self, other):
         """leftmost_complement([-5, 5], [1,3]) => [-5,1]
 
         :param other:
 
         """
         if not self.intersection(other):
             raise ValueError()
         # -inf,1(
         inv_other = (~other)._intervals[0]
         # [-inf, 1]
-        inv_other = P.closed(inv_other.lower, inv_other.upper)
+        inv_other = portion.closed(inv_other.lower, inv_other.upper)
         # [-5, 5] & [-inf, 1] => [-5, 1]
         return TimeInterval(self & inv_other)
 
     # Sub range generators utilities
     def range(self, *args) -> Generator[Any, None, None]:
         for period in self.range_pendulum_period(*args):
             yield to_time_interval(
                 left=Bound.CLOSED, start=period.start, end=period.end, right=Bound.CLOSED
             )
 
-    def range_pendulum_period(self, *args) -> Generator[Period, None, None]:
+    def range_pendulum_period(self, *args) -> Generator[PendulumInterval, None, None]:
         period = self.to_pendulum_period()
         range_start = None
         for range_end in period.range(*args):
             if range_start is not None:
                 yield range_end - range_start
             range_start = range_end
 
@@ -132,23 +132,20 @@
 
     def difference(self, other):
         return self - other
 
     def __str__(self):
         def to_str(i):
             if i.empty:
-                return "Period []"
+                return "PendulumInterval []"
             return str(TimeInterval(i).to_pendulum_period())
 
         value = ",".join([to_str(i) for i in self])
         return f"{super().__str__()} ({value})"
 
-    def __hash__(self):
-        return super().__hash__()
-
 
 def to_time_interval(
     left: Bound = None,
     start: UTCTimestampMilliSec = None,
     end: UTCTimestampMilliSec = None,
     right: Bound = None,
 ):
@@ -157,15 +154,15 @@
         lower=__utctimestamp_millisec_converter(start),
         upper=__utctimestamp_millisec_converter(end),
         right=right,
     )
     return TimeInterval(interval)
 
 
-def to_time_interval_from_period(period: Period, left: Bound = None, right: Bound = None):
+def to_time_interval_from_period(period: PendulumInterval, left: Bound = None, right: Bound = None):
     interval = Interval.from_atomic(
         left=left,
         lower=__utctimestamp_millisec_converter(period.start),
         upper=__utctimestamp_millisec_converter(period.end),
         right=right,
     )
     return TimeInterval(interval)
@@ -249,16 +246,17 @@
             sub_time_interval = to_time_interval(
                 left=Bound.CLOSED, start=start, end=end, right=Bound.OPEN
             )
             if not sub_time_interval.empty:
                 yield sub_time_interval
 
 
-def to_sorted_atomic_intervals(intervals: Iterator[Interval] = []) -> List[Interval]:
-    return [i for i in to_time_interval_simplified(intervals)]
+def to_sorted_atomic_intervals(intervals: Iterator[Interval] = None) -> List[Interval]:
+    intervals = intervals or []
+    return list(to_time_interval_simplified(intervals))
 
 
 def to_sorted_time_intervals_from_intervals(
     intervals: Iterator[Interval] = None,
 ) -> List[TimeInterval]:
     intervals = intervals or []
     intervals = to_sorted_atomic_intervals(intervals)
@@ -324,9 +322,9 @@
     return list(mapped.keys())
 
 
 def to_sorted_atomic_intervals_from_time_intervals(
     instrument_time_intervals: List[TimeInterval] = None,
 ) -> List[Interval]:
     instrument_time_intervals = instrument_time_intervals or []
-    intervals = [time_interval for time_interval in instrument_time_intervals]
+    intervals = list(instrument_time_intervals)
     return to_sorted_atomic_intervals(intervals)
```

### Comparing `constellate-0.8.8/constellate/debugger/debugger.py` & `constellate-0.8.9/constellate/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/debugger/simple.py` & `constellate-0.8.9/constellate/debugger/simple.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/formatter/formatterfactory.py` & `constellate-0.8.9/constellate/logger/formatter/formatterfactory.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/handler/forwarderhandler.py` & `constellate-0.8.9/constellate/logger/handler/forwarderhandler.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/handler/stringhandler.py` & `constellate-0.8.9/constellate/logger/handler/stringhandler.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/log.py` & `constellate-0.8.9/constellate/logger/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,22 +59,23 @@
     _JOB_LOGGER_NAMES_LOCK = threading.Lock()
     _LOGS_DIRECTORY = _LogDefault.LOGS_DIRECTORY
     _ROOT_LOGGER_NAME = _LogDefault.ROOT_LOGGER_NAME
 
     def default_config_dict(
         root_name=None,
         mode: LogMode = _LogDefault.MODE,
-        template: Dict[str, object] = _LogDefault.TEMPLATE_CONFIG,
+        template: Dict[str, object] = None,
     ):
-        COLOR_MARKER = "%(log_color)s"
+        template = template or _LogDefault.TEMPLATE_CONFIG
+        color_marker = "%(log_color)s"
 
         def console_formatter(name=None, mode=None, normal_fmt=None, trace_fmt=None):
             remove_color = not has_flag(mode, LogMode.INTERACTIVE_YES)
             fmt = trace_fmt if has_flag(mode, LogMode.DETAIL_TRACE) else normal_fmt
-            fmt = fmt.replace(COLOR_MARKER, "") if remove_color else fmt
+            fmt = fmt.replace(color_marker, "") if remove_color else fmt
             colored = "colored" if not remove_color else "monocolor"
             key = f"console_{colored}_{name}"
             return (
                 key,
                 {
                     key: {
                         "()": ".".join([builder.__module__, builder.__name__]),
@@ -133,36 +134,39 @@
                         "stream": sys.stdout,
                     }
                 },
             )
 
         def logger(
             name=None,
-            handlers=[],
-            levelIFProd="INFO",
+            handlers=None,
+            level_if_prod="INFO",
             mode=None,
-            levelIfNotProd="DEBUG",
+            level_if_not_prod="DEBUG",
             propagate=False,
         ):
+            handlers = handlers or []
             return {
                 f"{name}": {
                     "handlers": handlers,
                     "level": (
-                        levelIFProd if has_flag(mode, LogMode.ENV_PRODUCTION) else levelIfNotProd
+                        level_if_prod
+                        if has_flag(mode, LogMode.ENV_PRODUCTION)
+                        else level_if_not_prod
                     ),
                     "propagate": propagate,
                 }
             }
 
         exception_str_attribute = "%(exception_str)s" if sys.version_info >= (3, 10, 0) else ""
         console_fmt_id, console_fmt = console_formatter(
             name="console",
             mode=mode,
-            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: {COLOR_MARKER}%(levelname)s: %(message)s {exception_str_attribute}",
-            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: {COLOR_MARKER}%(levelname)s: %(message)s {exception_str_attribute}",
+            normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: {color_marker}%(levelname)s: %(message)s {exception_str_attribute}",
+            trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(name)s: {color_marker}%(levelname)s: %(message)s {exception_str_attribute}",
         )
         file_fmt_id, file_fmt = file_formatter(
             name="detailed",
             mode=mode,
             normal_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s {exception_str_attribute}",
             trace_fmt=f"%(asctime)s: P%(process)d: %(processName)s: T%(thread)d: %(threadName)s: %(levelname)s: %(message)s {exception_str_attribute}",
         )
@@ -213,17 +217,17 @@
                 # Associate handler to config
                 config["handlers"].update(custom_fhd)
 
                 # Generate logger
                 custom_logger = logger(
                     name=f"{dot_name}",
                     handlers=[console_hd_id, custom_fhd_id] if is_root else [custom_fhd_id],
-                    levelIfNotProd=template_logger_obj.get("level", "DEBUG"),
+                    level_if_not_prod=template_logger_obj.get("level", "DEBUG"),
                     mode=mode,
-                    levelIFProd=template_logger_obj.get("level", "INFO"),
+                    level_if_prod=template_logger_obj.get("level", "INFO"),
                     propagate=not is_root,
                 )
 
                 # Associate logger to config
                 config["loggers"].update(custom_logger)
 
         def update_config_tree(config, template, previous_logger_parts):
@@ -387,20 +391,20 @@
                 ctx_manager=ctx_manager,
                 backend=backend,
                 message_dispatch_mode=dispatch_mode,
             )
 
             Log._FQDN_LOGGER_SETTINGS_EXTERNAL.update({name: client_handler_settings})
             return logger, client_handler_settings
-        elif has_flag(mode, LogMode.OPERATE_CLIENT):
+        if has_flag(mode, LogMode.OPERATE_CLIENT):
             setup_client_handlers(
                 logger=logger, handler_name_to_client_handler_settings=mode_settings
             )
             return logger, {}
-        elif has_flag(mode, LogMode.OPERATE_STANDALONE):
+        if has_flag(mode, LogMode.OPERATE_STANDALONE):
             return logger, {}
 
     @staticmethod
     def create_job_handler(capacity=sys.maxsize):
         """
 
         :param capacity:  (Default value = sys.maxsize)
```

### Comparing `constellate-0.8.8/constellate/logger/loggers.py` & `constellate-0.8.9/constellate/logger/loggers.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/logmode.py` & `constellate-0.8.9/constellate/logger/logmode.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/logger/simple.py` & `constellate-0.8.9/constellate/logger/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,9 +79,9 @@
     return Log.loggers(mode=LogMode.OPERATE_CLIENT, **kwargs)
 
 
 def teardown_loggers(loggers: Loggers = None, timeout: None = None) -> None:
     native_loggers = loggers.native_loggers() if loggers is not None else []
     logger_dispatch_remaining_messages(loggers=native_loggers)
     teardown_handlers(loggers=native_loggers, timeout=timeout)
-    "Free/Remove all loggers setup previously"
+    # Free/Remove all loggers setup previously
     Log.teardown_loggers(loggers=native_loggers)
```

### Comparing `constellate-0.8.8/constellate/progression/progres.py` & `constellate-0.8.9/constellate/progression/progres.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/resource/resource.py` & `constellate-0.8.9/constellate/resource/resource.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/storage/filesystem/anyfs/path.py` & `constellate-0.8.9/constellate/storage/filesystem/anyfs/path.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/storage/filesystem/tmpfs/memory_tempfile.py` & `constellate-0.8.9/constellate/storage/filesystem/tmpfs/memory_tempfile.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/storage/filesystem/tmpfs/rambacked.py` & `constellate-0.8.9/constellate/storage/filesystem/tmpfs/rambacked.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/numba/progress/progress.py` & `constellate-0.8.9/constellate/thirdparty/numba/progress/progress.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/__init__.py` & `constellate-0.8.9/constellate/thirdparty/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/accessor/attribute_accessor.py` & `constellate-0.8.9/constellate/thirdparty/pandas/accessor/attribute_accessor.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/extra/sanitize/sanitize.py` & `constellate-0.8.9/constellate/thirdparty/pandas/extra/sanitize/sanitize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import List, Union, Dict
+from typing import Any
+from typing_extensions import TypeAlias
+from typing import get_origin
 
 import inspect
 import itertools
 import pandas
 import pandas as pd
 import pandera.dtypes
 from pandas import DataFrame, Series
 from pandera.api.pandas.components import MultiIndex
-from typing import Any
-from typing_extensions import TypeAlias
-from typing import get_origin
+
 from constellate.thirdparty.pandas.validation.validation import (
     PanderaSchema,
     pandera_schema_from_pydantic_schema,
 )
 
 
 def fillnone(df: DataFrame = None, column_names: List[str] = None) -> None:
@@ -121,16 +122,15 @@
     ) -> pd.DataFrame:
         data[col_name] = data[col_name].astype(col_type)
         return data
 
     def _apply_dtype_series(
         data: pd.Series = None, col_name: str = None, col_type: Any = None
     ) -> pd.Series:
-        data = data.astype(col_type)
-        return data
+        return data.astype(col_type)
 
     def _apply_dtype(
         data: PandasData = None, col_name: str = None, col_type: Any = None
     ) -> PandasData:
         if isinstance(data, pd.DataFrame):
             return _apply_dtype_dataframe(data=data, col_name=col_name, col_type=col_type)
         if isinstance(data, pd.Series):
@@ -140,48 +140,48 @@
 
         raise NotImplementedError()
 
     def _to_numeric(data: PandasData = None, col_name: str = None) -> PandasData:
         if isinstance(data, pd.DataFrame):
             data[col_name] = pandas.to_numeric(data[col_name], errors="coerce", downcast=None)
             return data
-        elif isinstance(data, pd.Series):
+        if isinstance(data, pd.Series):
             data = pandas.to_numeric(data, errors="coerce", downcast=None)
             return data
-        elif isinstance(data, pd.Index):
+        if isinstance(data, pd.Index):
             data = pandas.to_numeric(data, errors="coerce", downcast=None)
             return data
-        else:
-            raise NotImplementedError()
+
+        raise NotImplementedError()
 
     def _to_datetime(data: PandasData = None, col_name: str = None) -> PandasData:
         if isinstance(data, pd.DataFrame):
             data[col_name] = pandas.to_datetime(data[col_name], errors="coerce")
             return data
-        elif isinstance(data, pd.Series):
+        if isinstance(data, pd.Series):
             data = pandas.to_datetime(data, errors="coerce")
             return data
-        elif isinstance(data, pd.Index):
+        if isinstance(data, pd.Index):
             data = pandas.to_datetime(data, errors="coerce")
             return data
-        else:
-            raise NotImplementedError()
+
+        raise NotImplementedError()
 
     def _to_timedelta(data: PandasData = None, col_name: str = None) -> PandasData:
         if isinstance(data, pd.DataFrame):
             data[col_name] = pandas.to_timedelta(data[col_name], errors="coerce")
             return data
-        elif isinstance(data, pd.Series):
+        if isinstance(data, pd.Series):
             data = pandas.to_timedelta(data, errors="coerce")
             return data
-        elif isinstance(data, pd.Index):
+        if isinstance(data, pd.Index):
             data = pandas.to_timedelta(data, errors="coerce")
             return data
-        else:
-            raise NotImplementedError()
+
+        raise NotImplementedError()
 
     col_type = col_info.dtype
 
     data_orig = data
     mono_index = None
     if index and multi_index:
         mono_index = data.get_level_values(col_name)
@@ -238,15 +238,17 @@
         pass
     else:
         raise NotImplementedError()
 
     return data
 
 
-def enum_to_value(data: Union[DataFrame, Series] = None, dtypes: Dict = {}) -> None:
+def enum_to_value(data: Union[DataFrame, Series] = None, dtypes: Dict = None) -> None:
+    dtypes = dtypes or {}
+
     def _enum_value(e):
         return e.value
 
     for col_name in list(data.columns):
         if col_name not in dtypes:
             continue
 
@@ -277,15 +279,15 @@
 
 
 def _get_index_name_and_dtypes(schema: PanderaSchema = None) -> Dict[str, Any]:
     schema2 = pandera_schema_from_pydantic_schema(schema=schema)
     if isinstance(schema2.index, pandera.api.pandas.components.MultiIndex):
         raise NotImplementedError("not implemented yet")
         # return list(schema2.index.columns.keys())
-    elif isinstance(schema2.index, pandera.api.pandas.components.Index):
+    if isinstance(schema2.index, pandera.api.pandas.components.Index):
         annotations = next(
             iter(filter(lambda m: m[0] == "__annotations__", inspect.getmembers(schema))),
             ("__annotations__", {}),
         )[1]
         name = next(
             iter(
                 [k for k, v in annotations.items() if get_origin(v) == pandera.typing.pandas.Index]
@@ -294,8 +296,9 @@
         )
         if name is None:
             raise ValueError()
         # get_origin(schema.__dict__['__annotations__']['some index name like timestamp']) does not seem to store the index name's dtype.
         # Hence, taking from dtype from schema2
         # Must return a <object> containing property path "dtype.type"
         return {name: schema2.index}
+
     raise NotImplementedError()
```

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy.py` & `constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py` & `constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy_engine.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py` & `constellate-0.8.9/constellate/thirdparty/pandas/io/sql/sqlalchemy_execution_option.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/validation/pandera.py` & `constellate-0.8.9/constellate/thirdparty/pandas/validation/pandera.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate/thirdparty/pandas/validation/validation.py` & `constellate-0.8.9/constellate/thirdparty/pandas/validation/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,14 @@
             pandera_schema = pandera_schema_from_pydantic_schema(schema=schema)
 
         # For list of checks carried out:
         # https://pandera.readthedocs.io/en/stable/lazy_validation.html
         return pandera_schema.validate(data, **schema_validation_options)
     except pandera.errors.SchemaError as e:
         # Case: lazy=False
-        i = 10
         msg = (
             f"\n\n------- Schema Error # --------\n"
             f"Schema:{schema.__name__}\n"
             f"Detail: {''.join(list(e.args))}\n"
             f"Failure Cases: {e.failure_cases}\n"
             f"Ruled failed:{e.schema}"
         )
@@ -198,15 +197,15 @@
             data = fn(*fn_args, **fn_kwargs)
             return fn_check(
                 data=data, schema=schema, schema_validation_options=schema_validation_options
             )
 
         fn_read_and_check = _read_and_check
 
-    return _read_and_check(
+    return fn_read_and_check(
         fn_check,
         fn,
         schema,
         schema_validation_options,
         *fn_args,
         **fn_kwargs,
     )
```

### Comparing `constellate-0.8.8/constellate/thirdparty/pandera/inspector.py` & `constellate-0.8.9/constellate/thirdparty/pandera/inspector.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate.egg-info/PKG-INFO` & `constellate-0.8.9/constellate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: constellate
-Version: 0.8.8
+Version: 0.8.9
 Summary: A bunch of utilities aggregated over time
 Author-email: David Andreoletti <none@provided.yet>
 Project-URL: repository, https://github.com/davidandreoletti/constellate
 Keywords: constellate
 Classifier: License :: Other/Proprietary License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: decorator>=5.1.0
 Requires-Dist: aioitertools>=0.8.0
 Requires-Dist: psutil>=5.7.0
-Requires-Dist: pendulum>=2.1.2
+Requires-Dist: pendulum>=3.0.0
 Requires-Dist: requests>=2.25.0
 Requires-Dist: memory-tempfile>=2.2.3
 Requires-Dist: bidict>=0.21.4
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: portion>=2.2.0
 Requires-Dist: jsonmerge>=1.8.0
 Requires-Dist: jsonschema>=4.7.2
```

### Comparing `constellate-0.8.8/constellate.egg-info/SOURCES.txt` & `constellate-0.8.9/constellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/constellate.egg-info/requires.txt` & `constellate-0.8.9/constellate.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 decorator>=5.1.0
 aioitertools>=0.8.0
 psutil>=5.7.0
-pendulum>=2.1.2
+pendulum>=3.0.0
 requests>=2.25.0
 memory-tempfile>=2.2.3
 bidict>=0.21.4
 attrs>=20.3.0
 portion>=2.2.0
 jsonmerge>=1.8.0
 jsonschema>=4.7.2
```

### Comparing `constellate-0.8.8/pyproject.toml` & `constellate-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
     "decorator>=5.1.0",
     "aioitertools>=0.8.0",
     "psutil>=5.7.0",
-    "pendulum>=2.1.2",
+    "pendulum>=3.0.0",
     "requests>=2.25.0",
     "memory-tempfile>=2.2.3",
     "bidict>=0.21.4",
     "attrs>=20.3.0",
     "portion>=2.2.0",
     "jsonmerge>=1.8.0",
     "jsonschema>=4.7.2",
```

### Comparing `constellate-0.8.8/tests/test_cli_argument.py` & `constellate-0.8.9/tests/test_cli_argument.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_compression.py` & `constellate-0.8.9/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_concurrency.py` & `constellate-0.8.9/tests/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_cryptography.py` & `constellate-0.8.9/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_enum.py` & `constellate-0.8.9/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_logger.py` & `constellate-0.8.9/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_migration.py` & `constellate-0.8.9/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_pandas.py` & `constellate-0.8.9/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_pandera.py` & `constellate-0.8.9/tests/test_pandera.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_progression.py` & `constellate-0.8.9/tests/test_progression.py`

 * *Files identical despite different names*

### Comparing `constellate-0.8.8/tests/test_sparql.py` & `constellate-0.8.9/tests/test_sparql.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from pytest_httpserver import HTTPServer
 from rdflib import Graph
 from rdflib.namespace import FOAF
 from rdflib.plugins.stores.sparqlstore import SPARQLStore
 from rdflib.term import URIRef, Literal
 
 from constellate.database.sparql.query import query
-from SPARQLBurger.SPARQLQueryBuilder import SPARQLSelectQuery, SPARQLGraphPattern
-
 from constellate.database.sparql.sparqlburger.triple import to_triple
 
+from SPARQLBurger.SPARQLQueryBuilder import SPARQLSelectQuery, SPARQLGraphPattern
+
 
 def test_query(httpserver: HTTPServer) -> None:
     # Fake SPARQL server endpoint result
     data = {
         "head": {
             "vars": ["name"],
         },
```

### Comparing `constellate-0.8.8/tests/test_sqlalchemy.py` & `constellate-0.8.9/tests/test_sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             async def read_one(text: str = None, **kwargs):
                 return await _read(conditions=[SQLAlchemyTestR.text == text], **kwargs)
 
             result = await read_one(session=session, text="foo")
             expect(isinstance(result, SQLAlchemyTestR)).equals(True)
             expect(result.id).equals(1)
 
-            with pytest.raises(NoResultFound) as excinfo:
+            with pytest.raises(NoResultFound) as _excinfo:
                 await read_one(session=session, text="do not exist")
 
             @execute_scalars_all_iterable
             async def read_all_iterable(**kwargs):
                 return await _read(conditions=[], **kwargs)
 
             result = await read_all_iterable(session=session)
```

### Comparing `constellate-0.8.8/tests/test_storage_filesystem_tmpfs_rambacked.py` & `constellate-0.8.9/tests/test_storage_filesystem_tmpfs_rambacked.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def case_data(keys):
         for key in keys:
             if key in data:
                 yield (key, data[key])
 
     # Create dir as required
-    for key, value in case_data(["dir"]):
+    for _key, value in case_data(["dir"]):
         Path(value).mkdir(exist_ok=True)
 
     # Create dir associated to env_tmpfs_dir as required
     for key, value in case_data(["env_tmpfs_dir"]):
         os.environ[value] = tempfile.mkdtemp()
 
     # Create tmpfs dir
```

