# Comparing `tmp/nonebot_plugin_orm-0.7.2.tar.gz` & `tmp/nonebot_plugin_orm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_orm-0.7.2.tar", last modified: Sun Apr 28 09:59:24 2024, max compression
+gzip compressed data, was "nonebot_plugin_orm-0.7.3.tar", last modified: Wed May 22 07:07:53 2024, max compression
```

## Comparing `nonebot_plugin_orm-0.7.2.tar` & `nonebot_plugin_orm-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1078 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/LICENSE
--rw-r--r--   0        0        0     7133 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/README.md
--rw-r--r--   0        0        0     7361 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__init__.py
--rw-r--r--   0        0        0     8161 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__main__.py
--rw-r--r--   0        0        0     1037 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/config.py
--rw-r--r--   0        0        0      416 2024-04-28 09:59:00.051276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/env.py
--rw-r--r--   0        0        0    31862 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/migrate.py
--rw-r--r--   0        0        0     3502 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/model.py
--rw-r--r--   0        0        0     5148 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/param.py
--rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/py.typed
--rw-r--r--   0        0        0       19 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/README
--rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/__init__.py
--rw-r--r--   0        0        0     2476 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/env.py
--rw-r--r--   0        0        0      667 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/versions/__init__.py
--rw-r--r--   0        0        0      654 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/README
--rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/__init__.py
--rw-r--r--   0        0        0     4426 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/env.py
--rw-r--r--   0        0        0      957 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/versions/__init__.py
--rw-r--r--   0        0        0    12946 2024-04-28 09:59:00.055276 nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/utils.py
--rw-r--r--   0        0        0     2119 2024-04-28 09:59:24.479448 nonebot_plugin_orm-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     8801 1970-01-01 00:00:00.000000 nonebot_plugin_orm-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/LICENSE
+-rw-r--r--   0        0        0     7133 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/README.md
+-rw-r--r--   0        0        0     7383 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/__init__.py
+-rw-r--r--   0        0        0     8161 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/__main__.py
+-rw-r--r--   0        0        0     1037 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/config.py
+-rw-r--r--   0        0        0      416 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/env.py
+-rw-r--r--   0        0        0    31862 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/migrate.py
+-rw-r--r--   0        0        0     3502 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/model.py
+-rw-r--r--   0        0        0     5148 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/param.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/py.typed
+-rw-r--r--   0        0        0       19 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/README
+-rw-r--r--   0        0        0        0 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/__init__.py
+-rw-r--r--   0        0        0     2476 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/env.py
+-rw-r--r--   0        0        0      667 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/script.py.mako
+-rw-r--r--   0        0        0        0 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/versions/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/README
+-rw-r--r--   0        0        0        0 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/__init__.py
+-rw-r--r--   0        0        0     4426 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/env.py
+-rw-r--r--   0        0        0      957 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/script.py.mako
+-rw-r--r--   0        0        0        0 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/versions/__init__.py
+-rw-r--r--   0        0        0    12946 2024-05-22 07:07:28.000619 nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/utils.py
+-rw-r--r--   0        0        0     2119 2024-05-22 07:07:53.008712 nonebot_plugin_orm-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     8801 1970-01-01 00:00:00.000000 nonebot_plugin_orm-0.7.3/PKG-INFO
```

### Comparing `nonebot_plugin_orm-0.7.2/LICENSE` & `nonebot_plugin_orm-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/README.md` & `nonebot_plugin_orm-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__init__.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,64 +78,68 @@
     with migrate.AlembicConfig(
         stdout=StreamToLogger(), cmd_opts=cmd_opts
     ) as alembic_config:
         if plugin_config.alembic_startup_check:
             cmd_opts.cmd = (migrate.check, [], [])
             try:
                 await greenlet_spawn(migrate.check, alembic_config)
-            except click.UsageError:
-                if not click.confirm("目标数据库未更新到最新迁移, 是否更新?"):
-                    raise
+            except click.UsageError as e:
+                try:
+                    click.confirm("目标数据库未更新到最新迁移, 是否更新?", abort=True)
+                except click.Abort:
+                    raise e
+
                 cmd_opts.cmd = (migrate.upgrade, [], [])
                 await greenlet_spawn(migrate.upgrade, alembic_config)
         else:
             logger.warning("跳过启动检查, 正在同步数据库模式...")
             cmd_opts.cmd = (migrate.sync, ["revision"], [])
             await greenlet_spawn(migrate.sync, alembic_config)
 
 
 def _init_orm():
     global _session_factory, _scoped_sessions
 
     _init_engines()
     _init_table()
     _session_factory = sa_async.async_sessionmaker(
-        **{
-            **dict(bind=_engines[""], binds=_binds),
-            **plugin_config.sqlalchemy_session_options,
-        }
+        _engines[""], binds=_binds, **plugin_config.sqlalchemy_session_options
     )
     _scoped_sessions = sa_async.async_scoped_session(
         _session_factory,
         lambda: (id(current_event.get(None)), current_matcher.get(None)),
     )
 
     run_postprocessor(_scoped_sessions.remove)
 
 
 def get_session(**local_kw: Any) -> sa_async.AsyncSession:
     try:
         return _session_factory(**local_kw)
     except NameError:
-        raise RuntimeError("nonebot-plugin-orm 未初始化") from None
+        _init_orm()
+
+    return _session_factory(**local_kw)
 
 
 # NOTE: NoneBot DI will run sync function in thread pool executor,
 # which is poor performance for this simple function, so we wrap it as a coroutine function.
 AsyncSession = Annotated[
     sa_async.AsyncSession,
     Depends(coroutine(wraps(lambda: None)(get_session)), use_cache=False),
 ]
 
 
 def get_scoped_session() -> sa_async.async_scoped_session[sa_async.AsyncSession]:
     try:
         return _scoped_sessions
     except NameError:
-        raise RuntimeError("nonebot-plugin-orm 未初始化") from None
+        _init_orm()
+
+    return _scoped_sessions
 
 
 async_scoped_session = Annotated[
     sa_async.async_scoped_session[sa_async.AsyncSession],
     Depends(coroutine(get_scoped_session)),
 ]
 
@@ -176,15 +180,17 @@
         del aiosqlite
     except (ImportError, RuntimeError):
         raise ValueError(
             '必须指定一个默认数据库 (SQLALCHEMY_DATABASE_URL 或 SQLALCHEMY_BINDS[""]). '
             "可以通过 `pip install nonebot-plugin-orm[default]` 获得开箱即用的数据库配置."
         ) from None
 
-    _engines[""] = _create_engine(f"sqlite+aiosqlite:///{_data_dir / 'db.sqlite3'}")
+    _engines[""] = _create_engine(
+        URL.create("sqlite+aiosqlite", database=str(_data_dir / "db.sqlite3"))
+    )
 
 
 def _init_table():
     global _binds, _metadatas, _plugins
 
     _binds = {}
     _plugins = {}
```

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/__main__.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/config.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/migrate.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/migrate.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/model.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/param.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from sqlalchemy import Row, Result, ScalarResult, select
 from sqlalchemy.sql.selectable import ExecutableReturnsRows
 from sqlalchemy.ext.asyncio import AsyncResult, AsyncScalarResult
 
 from .model import Model
 from .utils import Option, Dependency, generic_issubclass
 
-if sys.version_info >= (3, 10):
+if sys.version_info >= (3, 11):
     from typing import Annotated, get_args, get_origin
     from collections.abc import Iterator, Sequence, AsyncIterator
 
     Tuple = tuple
     Type = type
 else:
     from typing_extensions import Annotated, get_args, get_origin
```

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/env.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/env.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/generic/script.py.mako` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/generic/script.py.mako`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/README` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/README`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/env.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/env.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/templates/multidb/script.py.mako` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/templates/multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/nonebot_plugin_orm/utils.py` & `nonebot_plugin_orm-0.7.3/nonebot_plugin_orm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_orm-0.7.2/pyproject.toml` & `nonebot_plugin_orm-0.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-orm"
-version = "0.7.2"
+version = "0.7.3"
 description = "SQLAlchemy ORM support for nonebot"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
     { name = "ProgramRipper", email = "programripper@foxmail.com" },
 ]
 dependencies = [
     "alembic~=1.13",
```

### Comparing `nonebot_plugin_orm-0.7.2/PKG-INFO` & `nonebot_plugin_orm-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-orm
-Version: 0.7.2
+Version: 0.7.3
 Summary: SQLAlchemy ORM support for nonebot
 Keywords: nonebot,orm,sqlalchemy
 Home-page: https://github.com/nonebot/plugin-orm
 Author-Email: yanyongyu <yyy@nonebot.dev>, ProgramRipper <programripper@foxmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nonebot/plugin-orm
 Project-URL: Repository, https://github.com/nonebot/plugin-orm
```

