# Comparing `tmp/frontegg-3.0.1.tar.gz` & `tmp/frontegg-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontegg-3.0.1.tar", max compression
+gzip compressed data, was "frontegg-3.0.2.tar", max compression
```

## Comparing `frontegg-3.0.1.tar` & `frontegg-3.0.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2023-06-14 11:56:36.715998 frontegg-3.0.1/LICENSE
--rw-r--r--   0        0        0      406 2023-06-14 11:56:36.716739 frontegg-3.0.1/README-PYPI.rst
--rw-r--r--   0        0        0      213 2023-06-14 11:56:36.717131 frontegg-3.0.1/frontegg/__init__.py
--rw-r--r--   0        0        0      490 2024-01-25 12:44:31.271000 frontegg-3.0.1/frontegg/common/__init__.py
--rw-r--r--   0        0        0     4437 2024-01-25 12:44:31.271240 frontegg-3.0.1/frontegg/common/async_identity_mixin.py
--rw-r--r--   0        0        0      489 2023-06-14 11:56:36.717345 frontegg-3.0.1/frontegg/common/cache/cache_manager.py
--rw-r--r--   0        0        0     1206 2023-10-18 11:04:26.986677 frontegg-3.0.1/frontegg/common/cache/local_cache_manager.py
--rw-r--r--   0        0        0     1147 2023-10-18 11:04:26.986809 frontegg-3.0.1/frontegg/common/cache/redis_cache_manager.py
--rw-r--r--   0        0        0      291 2024-01-25 12:44:31.271548 frontegg-3.0.1/frontegg/common/clients/__init__.py
--rw-r--r--   0        0        0     3997 2024-01-25 12:44:31.271833 frontegg-3.0.1/frontegg/common/clients/async_http_client.py
--rw-r--r--   0        0        0     1738 2023-06-14 11:56:36.717631 frontegg-3.0.1/frontegg/common/clients/audits_client.py
--rw-r--r--   0        0        0     3506 2023-06-21 09:07:06.988528 frontegg-3.0.1/frontegg/common/clients/http_client.py
--rw-r--r--   0        0        0     4338 2023-10-18 11:04:26.987093 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_resolver.py
--rw-r--r--   0        0        0      702 2024-01-24 13:51:22.312418 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
--rw-r--r--   0        0        0     2840 2024-01-25 12:44:31.272104 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_access_token_service.py
--rw-r--r--   0        0        0     1163 2024-01-25 12:44:31.272333 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_tenant_access_token_service.py
--rw-r--r--   0        0        0     1151 2024-01-25 12:44:31.272585 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_user_access_token_service.py
--rw-r--r--   0        0        0     2658 2023-10-18 11:04:26.987602 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
--rw-r--r--   0        0        0      985 2023-06-14 11:56:36.718125 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
--rw-r--r--   0        0        0      989 2023-06-14 11:56:36.718199 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
--rw-r--r--   0        0        0     1801 2023-06-21 09:07:06.988796 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
--rw-r--r--   0        0        0     1842 2024-01-25 12:44:31.272830 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_access_token_service.py
--rw-r--r--   0        0        0     1457 2024-01-25 12:44:31.273291 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_tenant_access_token_service.py
--rw-r--r--   0        0        0     1405 2024-01-25 12:44:31.273584 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_user_access_token_service.py
--rw-r--r--   0        0        0     1364 2023-10-18 11:04:26.987753 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
--rw-r--r--   0        0        0     1274 2023-10-18 11:04:26.988262 frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
--rw-r--r--   0        0        0     4796 2024-01-25 12:44:31.274024 frontegg-3.0.1/frontegg/common/clients/token_resolvers/async_access_token_resolver.py
--rw-r--r--   0        0        0      979 2024-01-25 12:44:31.274270 frontegg-3.0.1/frontegg/common/clients/token_resolvers/async_authorization_token_resolver.py
--rw-r--r--   0        0        0      968 2023-10-18 11:04:26.988412 frontegg-3.0.1/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
--rw-r--r--   0        0        0     3563 2023-10-18 11:04:26.988509 frontegg-3.0.1/frontegg/common/clients/token_resolvers/token_resolver.py
--rw-r--r--   0        0        0     1382 2023-10-18 11:04:26.988671 frontegg-3.0.1/frontegg/common/clients/types.py
--rw-r--r--   0        0        0     1696 2024-01-25 12:44:31.274423 frontegg-3.0.1/frontegg/common/frontegg_async_authenticator.py
--rw-r--r--   0        0        0     1720 2024-01-25 12:44:31.274945 frontegg-3.0.1/frontegg/common/frontegg_authenticator.py
--rw-r--r--   0        0        0      351 2023-10-18 11:04:26.989183 frontegg-3.0.1/frontegg/common/frontegg_config.py
--rw-r--r--   0        0        0     1518 2023-10-18 11:04:26.989272 frontegg-3.0.1/frontegg/common/frontegg_context.py
--rw-r--r--   0        0        0     4236 2024-01-24 11:40:35.720581 frontegg-3.0.1/frontegg/common/identity_mixin.py
--rw-r--r--   0        0        0      250 2023-10-18 11:04:26.989536 frontegg-3.0.1/frontegg/common/package_utils.py
--rw-r--r--   0        0        0     4571 2024-01-25 16:44:45.112235 frontegg-3.0.1/frontegg/fastapi/README.md
--rw-r--r--   0        0        0       53 2023-06-14 11:56:36.719232 frontegg-3.0.1/frontegg/fastapi/__init__.py
--rw-r--r--   0        0        0       43 2023-10-18 12:34:50.114111 frontegg-3.0.1/frontegg/fastapi/__init__.pyi
--rw-r--r--   0        0        0     1863 2024-01-25 12:44:31.275175 frontegg-3.0.1/frontegg/fastapi/frontegg.py
--rw-r--r--   0        0        0      997 2024-01-25 12:44:31.275419 frontegg-3.0.1/frontegg/fastapi/frontegg.pyi
--rw-r--r--   0        0        0        0 2023-10-18 12:21:48.461872 frontegg-3.0.1/frontegg/fastapi/py.typed
--rw-r--r--   0        0        0      152 2023-06-14 11:56:36.719402 frontegg-3.0.1/frontegg/fastapi/secure_access/__init__.py
--rw-r--r--   0        0        0      140 2023-10-18 12:34:50.114214 frontegg-3.0.1/frontegg/fastapi/secure_access/__init__.pyi
--rw-r--r--   0        0        0     4866 2024-01-25 12:44:31.275785 frontegg-3.0.1/frontegg/fastapi/secure_access/frontegg_security.py
--rw-r--r--   0        0        0     1857 2023-10-18 12:34:50.114395 frontegg-3.0.1/frontegg/fastapi/secure_access/frontegg_security.pyi
--rw-r--r--   0        0        0     4164 2023-06-14 11:56:36.719602 frontegg-3.0.1/frontegg/flask/README.md
--rw-r--r--   0        0        0       53 2023-06-14 11:56:36.719657 frontegg-3.0.1/frontegg/flask/__init__.py
--rw-r--r--   0        0        0     1620 2023-06-14 11:56:36.719709 frontegg-3.0.1/frontegg/flask/frontegg.py
--rw-r--r--   0        0        0       86 2023-06-14 11:56:36.719797 frontegg-3.0.1/frontegg/flask/secure_access/__init__.py
--rw-r--r--   0        0        0     1820 2023-10-18 11:04:26.990281 frontegg-3.0.1/frontegg/flask/secure_access/with_authentication.py
--rw-r--r--   0        0        0      589 2023-10-18 11:04:26.990469 frontegg-3.0.1/frontegg/helpers/exceptions.py
--rw-r--r--   0        0        0     1669 2024-02-29 15:21:00.316252 frontegg-3.0.1/frontegg/helpers/frontegg_urls.py
--rw-r--r--   0        0        0      295 2023-06-14 11:56:36.720125 frontegg-3.0.1/frontegg/helpers/logger.py
--rw-r--r--   0        0        0      984 2023-10-18 11:04:26.990718 frontegg-3.0.1/frontegg/helpers/retry.py
--rw-r--r--   0        0        0     1601 2024-02-29 15:23:04.080881 frontegg-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 frontegg-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-14 11:56:36.715998 frontegg-3.0.2/LICENSE
+-rw-r--r--   0        0        0      406 2023-06-14 11:56:36.716739 frontegg-3.0.2/README-PYPI.rst
+-rw-r--r--   0        0        0      213 2023-06-14 11:56:36.717131 frontegg-3.0.2/frontegg/__init__.py
+-rw-r--r--   0        0        0      490 2024-01-25 12:44:31.271000 frontegg-3.0.2/frontegg/common/__init__.py
+-rw-r--r--   0        0        0     4437 2024-01-25 12:44:31.271240 frontegg-3.0.2/frontegg/common/async_identity_mixin.py
+-rw-r--r--   0        0        0      489 2023-06-14 11:56:36.717345 frontegg-3.0.2/frontegg/common/cache/cache_manager.py
+-rw-r--r--   0        0        0     1206 2023-10-18 11:04:26.986677 frontegg-3.0.2/frontegg/common/cache/local_cache_manager.py
+-rw-r--r--   0        0        0     1147 2023-10-18 11:04:26.986809 frontegg-3.0.2/frontegg/common/cache/redis_cache_manager.py
+-rw-r--r--   0        0        0      291 2024-01-25 12:44:31.271548 frontegg-3.0.2/frontegg/common/clients/__init__.py
+-rw-r--r--   0        0        0     3997 2024-01-25 12:44:31.271833 frontegg-3.0.2/frontegg/common/clients/async_http_client.py
+-rw-r--r--   0        0        0     1738 2023-06-14 11:56:36.717631 frontegg-3.0.2/frontegg/common/clients/audits_client.py
+-rw-r--r--   0        0        0     3506 2023-06-21 09:07:06.988528 frontegg-3.0.2/frontegg/common/clients/http_client.py
+-rw-r--r--   0        0        0     4338 2023-10-18 11:04:26.987093 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_resolver.py
+-rw-r--r--   0        0        0      702 2024-01-24 13:51:22.312418 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py
+-rw-r--r--   0        0        0     2840 2024-01-25 12:44:31.272104 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_access_token_service.py
+-rw-r--r--   0        0        0     1163 2024-01-25 12:44:31.272333 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_tenant_access_token_service.py
+-rw-r--r--   0        0        0     1151 2024-01-25 12:44:31.272585 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_user_access_token_service.py
+-rw-r--r--   0        0        0     2658 2023-10-18 11:04:26.987602 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py
+-rw-r--r--   0        0        0      985 2023-06-14 11:56:36.718125 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py
+-rw-r--r--   0        0        0      989 2023-06-14 11:56:36.718199 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py
+-rw-r--r--   0        0        0     1801 2023-06-21 09:07:06.988796 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py
+-rw-r--r--   0        0        0     1842 2024-01-25 12:44:31.272830 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_access_token_service.py
+-rw-r--r--   0        0        0     1457 2024-01-25 12:44:31.273291 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_tenant_access_token_service.py
+-rw-r--r--   0        0        0     1405 2024-01-25 12:44:31.273584 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_user_access_token_service.py
+-rw-r--r--   0        0        0     1364 2023-10-18 11:04:26.987753 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py
+-rw-r--r--   0        0        0     1274 2023-10-18 11:04:26.988262 frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py
+-rw-r--r--   0        0        0     4796 2024-01-25 12:44:31.274024 frontegg-3.0.2/frontegg/common/clients/token_resolvers/async_access_token_resolver.py
+-rw-r--r--   0        0        0      979 2024-01-25 12:44:31.274270 frontegg-3.0.2/frontegg/common/clients/token_resolvers/async_authorization_token_resolver.py
+-rw-r--r--   0        0        0      968 2023-10-18 11:04:26.988412 frontegg-3.0.2/frontegg/common/clients/token_resolvers/authorization_header_resolver.py
+-rw-r--r--   0        0        0     3563 2023-10-18 11:04:26.988509 frontegg-3.0.2/frontegg/common/clients/token_resolvers/token_resolver.py
+-rw-r--r--   0        0        0     1382 2023-10-18 11:04:26.988671 frontegg-3.0.2/frontegg/common/clients/types.py
+-rw-r--r--   0        0        0     1696 2024-01-25 12:44:31.274423 frontegg-3.0.2/frontegg/common/frontegg_async_authenticator.py
+-rw-r--r--   0        0        0     1720 2024-01-25 12:44:31.274945 frontegg-3.0.2/frontegg/common/frontegg_authenticator.py
+-rw-r--r--   0        0        0      351 2023-10-18 11:04:26.989183 frontegg-3.0.2/frontegg/common/frontegg_config.py
+-rw-r--r--   0        0        0     1518 2023-10-18 11:04:26.989272 frontegg-3.0.2/frontegg/common/frontegg_context.py
+-rw-r--r--   0        0        0     4236 2024-01-24 11:40:35.720581 frontegg-3.0.2/frontegg/common/identity_mixin.py
+-rw-r--r--   0        0        0      250 2023-10-18 11:04:26.989536 frontegg-3.0.2/frontegg/common/package_utils.py
+-rw-r--r--   0        0        0     4571 2024-01-25 16:44:45.112235 frontegg-3.0.2/frontegg/fastapi/README.md
+-rw-r--r--   0        0        0       53 2023-06-14 11:56:36.719232 frontegg-3.0.2/frontegg/fastapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-10-18 12:34:50.114111 frontegg-3.0.2/frontegg/fastapi/__init__.pyi
+-rw-r--r--   0        0        0     1863 2024-01-25 12:44:31.275175 frontegg-3.0.2/frontegg/fastapi/frontegg.py
+-rw-r--r--   0        0        0      997 2024-01-25 12:44:31.275419 frontegg-3.0.2/frontegg/fastapi/frontegg.pyi
+-rw-r--r--   0        0        0        0 2023-10-18 12:21:48.461872 frontegg-3.0.2/frontegg/fastapi/py.typed
+-rw-r--r--   0        0        0      152 2023-06-14 11:56:36.719402 frontegg-3.0.2/frontegg/fastapi/secure_access/__init__.py
+-rw-r--r--   0        0        0      140 2023-10-18 12:34:50.114214 frontegg-3.0.2/frontegg/fastapi/secure_access/__init__.pyi
+-rw-r--r--   0        0        0     4866 2024-04-02 09:03:05.790567 frontegg-3.0.2/frontegg/fastapi/secure_access/frontegg_security.py
+-rw-r--r--   0        0        0     1857 2023-10-18 12:34:50.114395 frontegg-3.0.2/frontegg/fastapi/secure_access/frontegg_security.pyi
+-rw-r--r--   0        0        0     4164 2023-06-14 11:56:36.719602 frontegg-3.0.2/frontegg/flask/README.md
+-rw-r--r--   0        0        0       53 2023-06-14 11:56:36.719657 frontegg-3.0.2/frontegg/flask/__init__.py
+-rw-r--r--   0        0        0     1620 2023-06-14 11:56:36.719709 frontegg-3.0.2/frontegg/flask/frontegg.py
+-rw-r--r--   0        0        0       86 2023-06-14 11:56:36.719797 frontegg-3.0.2/frontegg/flask/secure_access/__init__.py
+-rw-r--r--   0        0        0     1820 2023-10-18 11:04:26.990281 frontegg-3.0.2/frontegg/flask/secure_access/with_authentication.py
+-rw-r--r--   0        0        0      589 2023-10-18 11:04:26.990469 frontegg-3.0.2/frontegg/helpers/exceptions.py
+-rw-r--r--   0        0        0     1669 2024-02-29 15:21:00.316252 frontegg-3.0.2/frontegg/helpers/frontegg_urls.py
+-rw-r--r--   0        0        0      295 2023-06-14 11:56:36.720125 frontegg-3.0.2/frontegg/helpers/logger.py
+-rw-r--r--   0        0        0      984 2023-10-18 11:04:26.990718 frontegg-3.0.2/frontegg/helpers/retry.py
+-rw-r--r--   0        0        0     1602 2024-05-22 08:21:39.720297 frontegg-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 frontegg-3.0.2/PKG-INFO
```

### Comparing `frontegg-3.0.1/LICENSE` & `frontegg-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/async_identity_mixin.py` & `frontegg-3.0.2/frontegg/common/async_identity_mixin.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/cache/local_cache_manager.py` & `frontegg-3.0.2/frontegg/common/cache/local_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/cache/redis_cache_manager.py` & `frontegg-3.0.2/frontegg/common/cache/redis_cache_manager.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/async_http_client.py` & `frontegg-3.0.2/frontegg/common/clients/async_http_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/audits_client.py` & `frontegg-3.0.2/frontegg/common/clients/audits_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/http_client.py` & `frontegg-3.0.2/frontegg/common/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_resolver.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/base_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_tenant_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_user_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/async_impl/async_cache_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/cache_services/cache_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_tenant_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_user_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/async_impl/async_user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/tenant_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/access_token_services/services/user_access_token_service.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/async_access_token_resolver.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/async_access_token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/async_authorization_token_resolver.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/async_authorization_token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/authorization_header_resolver.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/authorization_header_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/token_resolvers/token_resolver.py` & `frontegg-3.0.2/frontegg/common/clients/token_resolvers/token_resolver.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/clients/types.py` & `frontegg-3.0.2/frontegg/common/clients/types.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/frontegg_async_authenticator.py` & `frontegg-3.0.2/frontegg/common/frontegg_async_authenticator.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/frontegg_authenticator.py` & `frontegg-3.0.2/frontegg/common/frontegg_authenticator.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/frontegg_context.py` & `frontegg-3.0.2/frontegg/common/frontegg_context.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/common/identity_mixin.py` & `frontegg-3.0.2/frontegg/common/identity_mixin.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/fastapi/README.md` & `frontegg-3.0.2/frontegg/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/fastapi/frontegg.py` & `frontegg-3.0.2/frontegg/fastapi/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/fastapi/frontegg.pyi` & `frontegg-3.0.2/frontegg/fastapi/frontegg.pyi`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/fastapi/secure_access/frontegg_security.py` & `frontegg-3.0.2/frontegg/fastapi/secure_access/frontegg_security.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/fastapi/secure_access/frontegg_security.pyi` & `frontegg-3.0.2/frontegg/fastapi/secure_access/frontegg_security.pyi`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/flask/README.md` & `frontegg-3.0.2/frontegg/flask/README.md`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/flask/frontegg.py` & `frontegg-3.0.2/frontegg/flask/frontegg.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/flask/secure_access/with_authentication.py` & `frontegg-3.0.2/frontegg/flask/secure_access/with_authentication.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/helpers/exceptions.py` & `frontegg-3.0.2/frontegg/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/helpers/frontegg_urls.py` & `frontegg-3.0.2/frontegg/helpers/frontegg_urls.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/frontegg/helpers/retry.py` & `frontegg-3.0.2/frontegg/helpers/retry.py`

 * *Files identical despite different names*

### Comparing `frontegg-3.0.1/pyproject.toml` & `frontegg-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "frontegg"
-version = "3.0.1"
+version = "3.0.2"
 description = "Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code."
 homepage = "https://frontegg.com/"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
@@ -23,15 +23,15 @@
 fastapi = { version = "*", optional = true }
 requests = "^2.28.2"
 arrow = "^1.2.3"
 aiohttp = {version = "^3.6.2", optional = true}
 PyJWT = "^2.6.0"
 cryptography = ">=42.0.5"
 typing-extensions = "^4.4.0"
-httpx = "^0.26.0"
+httpx = ">=0.26.0"
 
 [tool.poetry.extras]
 flask = ["flask"]
 fastapi = ["fastapi"]
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.3.2"
```

### Comparing `frontegg-3.0.1/PKG-INFO` & `frontegg-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontegg
-Version: 3.0.1
+Version: 3.0.2
 Summary: Frontegg is a web platform where SaaS companies can set up their fully managed, scalable and brand aware - SaaS features and integrate them into their SaaS portals in up to 5 lines of code.
 Home-page: https://frontegg.com/
 Author: Frontegg LTD
 Author-email: hello@frontegg.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 Provides-Extra: flask
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: aiohttp (>=3.6.2,<4.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: cryptography (>=42.0.5)
 Requires-Dist: fastapi ; extra == "fastapi"
 Requires-Dist: flask (>=2.0,<3.0) ; extra == "flask"
-Requires-Dist: httpx (>=0.26.0,<0.27.0)
+Requires-Dist: httpx (>=0.26.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Description-Content-Type: text/x-rst
 
 .. image:: https://fronteggstuff.blob.core.windows.net/frongegg-logos/logo-transparent.png
    :alt: Frontegg
```

