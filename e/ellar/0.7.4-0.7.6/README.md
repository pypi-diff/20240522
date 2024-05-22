# Comparing `tmp/ellar-0.7.4.tar.gz` & `tmp/ellar-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ellar-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ellar-0.7.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ellar-0.7.4.tar` & `ellar-0.7.6.tar`

### file list

```diff
@@ -1,311 +1,311 @@
--rw-r--r--   0        0        0     6789 2024-04-25 08:12:14.586263 ellar-0.7.4/README.md
--rw-r--r--   0        0        0      149 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/__init__.py
--rw-r--r--   0        0        0      182 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/__init__.py
--rw-r--r--   0        0        0     3281 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/context.py
--rw-r--r--   0        0        0     7931 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/factory.py
--rw-r--r--   0        0        0     2664 2024-04-25 08:12:14.626263 ellar-0.7.4/ellar/app/lifespan.py
--rw-r--r--   0        0        0    12053 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/app/main.py
--rw-r--r--   0        0        0     2267 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/app/services.py
--rw-r--r--   0        0        0      810 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/__init__.py
--rw-r--r--   0        0        0       55 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/constants.py
--rw-r--r--   0        0        0     2139 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/decorators.py
--rw-r--r--   0        0        0      411 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/__init__.py
--rw-r--r--   0        0        0     1281 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/apikey.py
--rw-r--r--   0        0        0     1405 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/auth_required.py
--rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/http.py
--rw-r--r--   0        0        0      356 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/guards/mixin.py
--rw-r--r--   0        0        0      575 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/__init__.py
--rw-r--r--   0        0        0      636 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/api_key.py
--rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/http.py
--rw-r--r--   0        0        0      698 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/mixin.py
--rw-r--r--   0        0        0      683 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/model.py
--rw-r--r--   0        0        0      371 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/__init__.py
--rw-r--r--   0        0        0      781 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/api_key.py
--rw-r--r--   0        0        0     5205 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/base.py
--rw-r--r--   0        0        0     3634 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/handlers/schemes/http.py
--rw-r--r--   0        0        0      223 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/identity.py
--rw-r--r--   0        0        0     1750 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/interceptor.py
--rw-r--r--   0        0        0      142 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/__init__.py
--rw-r--r--   0        0        0     1625 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/auth.py
--rw-r--r--   0        0        0     2239 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/middleware/session.py
--rw-r--r--   0        0        0      370 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/__init__.py
--rw-r--r--   0        0        0     5189 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/base.py
--rw-r--r--   0        0        0      940 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/policy/common.py
--rw-r--r--   0        0        0      177 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/__init__.py
--rw-r--r--   0        0        0     1046 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/auth_schemes.py
--rw-r--r--   0        0        0     1637 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/services/middleware.py
--rw-r--r--   0        0        0      934 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/base.py
--rw-r--r--   0        0        0     1699 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/cookie_dict.py
--rw-r--r--   0        0        0      384 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/options.py
--rw-r--r--   0        0        0     2174 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/auth/session/strategy.py
--rw-r--r--   0        0        0      257 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/__init__.py
--rw-r--r--   0        0        0      109 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/__init__.py
--rw-r--r--   0        0        0     4841 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/_aio_cache.py.ellar
--rw-r--r--   0        0        0     4633 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/base.py
--rw-r--r--   0        0        0     5406 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/local_cache.py
--rw-r--r--   0        0        0      971 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/pylib_cache.py
--rw-r--r--   0        0        0     2240 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/pymem_cache.py
--rw-r--r--   0        0        0       72 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/redis/__init__.py
--rw-r--r--   0        0        0     6813 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/redis/backend.py
--rw-r--r--   0        0        0     1413 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/backends/serializer.py
--rw-r--r--   0        0        0     3018 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/decorator.py
--rw-r--r--   0        0        0    11819 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/interface.py
--rw-r--r--   0        0        0     2045 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/make_key_decorator.py
--rw-r--r--   0        0        0     2657 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/model.py
--rw-r--r--   0        0        0     1882 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/module.py
--rw-r--r--   0        0        0      867 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/schema.py
--rw-r--r--   0        0        0     5077 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/cache/service.py
--rw-r--r--   0        0        0     3791 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/__init__.py
--rw-r--r--   0        0        0      195 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/__init__.py
--rw-r--r--   0        0        0     1163 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/cache_properties.py
--rw-r--r--   0        0        0      891 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/compatible/dict.py
--rw-r--r--   0        0        0     4901 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/constants.py
--rw-r--r--   0        0        0     1672 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/converters.py
--rw-r--r--   0        0        0     2829 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/datastructures.py
--rw-r--r--   0        0        0      811 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/__init__.py
--rw-r--r--   0        0        0      628 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/base.py
--rw-r--r--   0        0        0     3850 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/controller.py
--rw-r--r--   0        0        0     1042 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/exception.py
--rw-r--r--   0        0        0      610 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/extra_args.py
--rw-r--r--   0        0        0     2528 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/file.py
--rw-r--r--   0        0        0     1026 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/guards.py
--rw-r--r--   0        0        0     4740 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/html.py
--rw-r--r--   0        0        0     1085 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/interceptor.py
--rw-r--r--   0        0        0      928 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/middleware.py
--rw-r--r--   0        0        0     3335 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/modules.py
--rw-r--r--   0        0        0     1184 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/serializer.py
--rw-r--r--   0        0        0      397 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/decorators/versioning.py
--rw-r--r--   0        0        0      930 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/__init__.py
--rw-r--r--   0        0        0      472 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/__init__.py
--rw-r--r--   0        0        0     1519 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/base.py
--rw-r--r--   0        0        0     1251 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/api/exceptions_types.py
--rw-r--r--   0        0        0     2588 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/callable_exceptions.py
--rw-r--r--   0        0        0      103 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/context.py
--rw-r--r--   0        0        0     2537 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/handlers.py
--rw-r--r--   0        0        0      768 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/exceptions/validation.py
--rw-r--r--   0        0        0     1325 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/__init__.py
--rw-r--r--   0        0        0      398 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/application.py
--rw-r--r--   0        0        0     3971 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/context.py
--rw-r--r--   0        0        0     1769 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/exceptions.py
--rw-r--r--   0        0        0      400 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/guard_consumer.py
--rw-r--r--   0        0        0      684 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/identity_schemes.py
--rw-r--r--   0        0        0      406 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/interceptor_consumer.py
--rw-r--r--   0        0        0      404 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/middleware.py
--rw-r--r--   0        0        0     1771 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/module.py
--rw-r--r--   0        0        0      748 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/response_model.py
--rw-r--r--   0        0        0      907 2024-04-25 08:12:14.630263 ellar-0.7.4/ellar/common/interfaces/templating.py
--rw-r--r--   0        0        0      774 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/interfaces/versioning.py
--rw-r--r--   0        0        0      104 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/logging.py
--rw-r--r--   0        0        0      363 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/__init__.py
--rw-r--r--   0        0        0      877 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/controller.py
--rw-r--r--   0        0        0      803 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/guard.py
--rw-r--r--   0        0        0      851 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/identity.py
--rw-r--r--   0        0        0      320 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/models/interceptor.py
--rw-r--r--   0        0        0      802 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/__init__.py
--rw-r--r--   0        0        0     9663 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/base.py
--rw-r--r--   0        0        0     2759 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/router.py
--rw-r--r--   0        0        0     3632 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/operations/schema.py
--rw-r--r--   0        0        0      555 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/__init__.py
--rw-r--r--   0        0        0      315 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/__init__.py
--rw-r--r--   0        0        0    14710 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/base.py
--rw-r--r--   0        0        0     1657 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/extra_args.py
--rw-r--r--   0        0        0     1994 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/factory.py
--rw-r--r--   0        0        0     6837 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/request_model.py
--rw-r--r--   0        0        0     6180 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/resolver_generators.py
--rw-r--r--   0        0        0     2429 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/args/websocket_model.py
--rw-r--r--   0        0        0     4165 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/__init__.py
--rw-r--r--   0        0        0     2366 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/inject.py
--rw-r--r--   0        0        0    16837 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/decorators/models.py
--rw-r--r--   0        0        0    15753 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/params.py
--rw-r--r--   0        0        0     1106 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/__init__.py
--rw-r--r--   0        0        0     1702 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/base.py
--rw-r--r--   0        0        0     5758 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/bulk_parameter.py
--rw-r--r--   0        0        0    11220 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/parameter.py
--rw-r--r--   0        0        0      776 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/__init__.py
--rw-r--r--   0        0        0      873 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/background.py
--rw-r--r--   0        0        0     2726 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/base.py
--rw-r--r--   0        0        0      397 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/connection.py
--rw-r--r--   0        0        0      334 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/context.py
--rw-r--r--   0        0        0     1547 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/provider.py
--rw-r--r--   0        0        0      393 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/request.py
--rw-r--r--   0        0        0      400 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/response.py
--rw-r--r--   0        0        0      524 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/session.py
--rw-r--r--   0        0        0      392 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/params/resolvers/system_parameters/websocket.py
--rw-r--r--   0        0        0      415 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/__init__.py
--rw-r--r--   0        0        0      839 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/__init__.py
--rw-r--r--   0        0        0     7921 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/base.py
--rw-r--r--   0        0        0       50 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/exceptions.py
--rw-r--r--   0        0        0     4305 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/file.py
--rw-r--r--   0        0        0      726 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/helper.py
--rw-r--r--   0        0        0     2129 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/html.py
--rw-r--r--   0        0        0     2935 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/json.py
--rw-r--r--   0        0        0     4865 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/route.py
--rw-r--r--   0        0        0     1688 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/models/type_converter.py
--rw-r--r--   0        0        0     1253 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/responses/response_types.py
--rw-r--r--   0        0        0      357 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/__init__.py
--rw-r--r--   0        0        0     5633 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/base.py
--rw-r--r--   0        0        0      194 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/serializer/guard.py
--rw-r--r--   0        0        0      454 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/shortcuts.py
--rw-r--r--   0        0        0      613 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/__init__.py
--rw-r--r--   0        0        0      593 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/environment.py
--rw-r--r--   0        0        0     2020 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/loader.py
--rw-r--r--   0        0        0      835 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/model.py
--rw-r--r--   0        0        0     2584 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/renderer.py
--rw-r--r--   0        0        0      110 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/templating/schema.py
--rw-r--r--   0        0        0      713 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/common/types.py
--rw-r--r--   0        0        0      928 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/__init__.py
--rw-r--r--   0        0        0      162 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/__init__.py
--rw-r--r--   0        0        0     5454 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/app_settings_models.py
--rw-r--r--   0        0        0     2397 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/config.py
--rw-r--r--   0        0        0     3270 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/conf/mixins.py
--rw-r--r--   0        0        0      469 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/__init__.py
--rw-r--r--   0        0        0      855 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/http.py
--rw-r--r--   0        0        0      245 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/connection/websocket.py
--rw-r--r--   0        0        0       97 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/exceptions/__init__.py
--rw-r--r--   0        0        0     2157 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/exceptions/service.py
--rw-r--r--   0        0        0      457 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/__init__.py
--rw-r--r--   0        0        0     1327 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/execution.py
--rw-r--r--   0        0        0     2581 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/factory.py
--rw-r--r--   0        0        0     2280 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/host.py
--rw-r--r--   0        0        0     2089 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/http.py
--rw-r--r--   0        0        0      801 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/execution_context/websocket.py
--rw-r--r--   0        0        0       72 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/guards/__init__.py
--rw-r--r--   0        0        0     1729 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/guards/consumer.py
--rw-r--r--   0        0        0       87 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/interceptors/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/interceptors/consumer.py
--rw-r--r--   0        0        0     1050 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/__init__.py
--rw-r--r--   0        0        0     2905 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/di.py
--rw-r--r--   0        0        0     2689 2024-04-25 08:12:14.634263 ellar-0.7.4/ellar/core/middleware/exceptions.py
--rw-r--r--   0        0        0     2577 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/function.py
--rw-r--r--   0        0        0      917 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/middleware.py
--rw-r--r--   0        0        0     1049 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/middleware/versioning.py
--rw-r--r--   0        0        0      363 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/__init__.py
--rw-r--r--   0        0        0     1302 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/base.py
--rw-r--r--   0        0        0     3082 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/builder.py
--rw-r--r--   0        0        0     7921 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/config.py
--rw-r--r--   0        0        0      787 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/helper.py
--rw-r--r--   0        0        0     9438 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/modules/ref.py
--rw-r--r--   0        0        0      291 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/base.py
--rw-r--r--   0        0        0     4821 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/controller.py
--rw-r--r--   0        0        0     1251 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/router_builders/module_router.py
--rw-r--r--   0        0        0      963 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/__init__.py
--rw-r--r--   0        0        0     5427 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/base.py
--rw-r--r--   0        0        0      272 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/__init__.py
--rw-r--r--   0        0        0     1068 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/base.py
--rw-r--r--   0        0        0      852 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/route.py
--rw-r--r--   0        0        0      190 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/handler.py
--rw-r--r--   0        0        0     1564 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/controller/websocket/route.py
--rw-r--r--   0        0        0     2566 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/file_mount.py
--rw-r--r--   0        0        0     7056 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/mount.py
--rw-r--r--   0        0        0     5321 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/route.py
--rw-r--r--   0        0        0     3046 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/route_collections.py
--rw-r--r--   0        0        0     2324 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/utils.py
--rw-r--r--   0        0        0      161 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/__init__.py
--rw-r--r--   0        0        0     6628 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/handler.py
--rw-r--r--   0        0        0     5618 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/routing/websocket/route.py
--rw-r--r--   0        0        0        0 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/__init__.py
--rw-r--r--   0        0        0     4074 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/__init__.py
--rw-r--r--   0        0        0     1811 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/argon2.py
--rw-r--r--   0        0        0     3002 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/base.py
--rw-r--r--   0        0        0     1739 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/bcrypt.py
--rw-r--r--   0        0        0     1418 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/md5.py
--rw-r--r--   0        0        0     1282 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/pbkdf.py
--rw-r--r--   0        0        0     2774 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/security/hashers/scrypt.py
--rw-r--r--   0        0        0       82 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/services/__init__.py
--rw-r--r--   0        0        0     1977 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/services/reflector.py
--rw-r--r--   0        0        0      392 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/shortcuts.py
--rw-r--r--   0        0        0     1805 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/staticfiles.py
--rw-r--r--   0        0        0      673 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/base.py
--rw-r--r--   0        0        0     6176 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/core/versioning/resolver.py
--rw-r--r--   0        0        0     1220 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/__init__.py
--rw-r--r--   0        0        0      344 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/asgi_args.py
--rw-r--r--   0        0        0     1120 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/constants.py
--rw-r--r--   0        0        0        0 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/context.py
--rw-r--r--   0        0        0      400 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/exceptions.py
--rw-r--r--   0        0        0      117 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/__init__.py
--rw-r--r--   0        0        0     8754 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/container.py
--rw-r--r--   0        0        0     5912 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/injector/ellar_injector.py
--rw-r--r--   0        0        0      154 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/logger.py
--rw-r--r--   0        0        0     1001 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/providers.py
--rw-r--r--   0        0        0     2050 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/scopes.py
--rw-r--r--   0        0        0     5969 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/service_config.py
--rw-r--r--   0        0        0       39 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/types.py
--rw-r--r--   0        0        0      406 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/di/utils.py
--rw-r--r--   0        0        0      231 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/events/__init__.py
--rw-r--r--   0        0        0     1951 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/events/base.py
--rw-r--r--   0        0        0      579 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/__init__.py
--rw-r--r--   0        0        0    10854 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/builder.py
--rw-r--r--   0        0        0      243 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/constants.py
--rw-r--r--   0        0        0       94 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/__init__.py
--rw-r--r--   0        0        0     1199 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/extra_info.py
--rw-r--r--   0        0        0      731 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/decorators/tags.py
--rw-r--r--   0        0        0      219 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/__init__.py
--rw-r--r--   0        0        0     1138 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/base.py
--rw-r--r--   0        0        0      932 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/redocs.py
--rw-r--r--   0        0        0     2226 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/stoplight.py
--rw-r--r--   0        0        0     1078 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/docs_ui/swagger.py
--rw-r--r--   0        0        0     5497 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/module.py
--rw-r--r--   0        0        0    13873 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/openapi_v3.py
--rw-r--r--   0        0        0    16040 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/route_doc_models.py
--rw-r--r--   0        0        0      115 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/schemas/__init__.py
--rw-r--r--   0        0        0      348 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/schemas/validation.py
--rw-r--r--   0        0        0    50277 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/static/swagger/SwaggerDark.css
--rw-r--r--   0        0        0      702 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/templates/redocs.html
--rw-r--r--   0        0        0      895 2024-04-25 08:12:14.638263 ellar-0.7.4/ellar/openapi/templates/swagger.html
--rw-r--r--   0        0        0        0 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/py.typed
--rw-r--r--   0        0        0     2082 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/__init__.py
--rw-r--r--   0        0        0     1528 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/decorator.py
--rw-r--r--   0        0        0      764 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/emails.py
--rw-r--r--   0        0        0     1798 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/encoder.py
--rw-r--r--   0        0        0     1718 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/exceptions.py
--rw-r--r--   0        0        0      692 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/field_constraints.py
--rw-r--r--   0        0        0     2850 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/fields.py
--rw-r--r--   0        0        0      397 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/types.py
--rw-r--r--   0        0        0     8596 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/pydantic/utils.py
--rw-r--r--   0        0        0      105 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/__init__.py
--rw-r--r--   0        0        0     5258 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/_reflect.py
--rw-r--r--   0        0        0       34 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/reflect/constants.py
--rw-r--r--   0        0        0       58 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/__init__.py
--rw-r--r--   0        0        0      232 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/guard.py
--rw-r--r--   0        0        0      704 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/controllers/home.py
--rw-r--r--   0        0        0      211 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/modules.py
--rw-r--r--   0        0        0   232915 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/css/bootstrap.min.css
--rw-r--r--   0        0        0      721 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/css/cover.css
--rwxr-xr-x   0        0        0    25915 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/EllarLogoB.png
--rwxr-xr-x   0        0        0    36744 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/EllarLogoIconOnly.png
--rwxr-xr-x   0        0        0     3888 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/static/img/Icon.svg
--rw-r--r--   0        0        0     2575 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/samples/templates/home/index.html
--rw-r--r--   0        0        0      629 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/__init__.py
--rw-r--r--   0        0        0      422 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/adapter.py
--rw-r--r--   0        0        0      543 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/constants.py
--rw-r--r--   0        0        0     1914 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/context.py
--rw-r--r--   0        0        0      225 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/__init__.py
--rw-r--r--   0        0        0      667 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/events.py
--rw-r--r--   0        0        0     3034 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/gateway.py
--rw-r--r--   0        0        0      570 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/decorators/subscribe_message.py
--rw-r--r--   0        0        0     4177 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/factory.py
--rw-r--r--   0        0        0     9619 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/gateway.py
--rw-r--r--   0        0        0      144 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/model.py
--rw-r--r--   0        0        0      532 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/responses.py
--rw-r--r--   0        0        0      107 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/testing/__init__.py
--rw-r--r--   0        0        0     1700 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/socket_io/testing/module.py
--rw-r--r--   0        0        0      129 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/__init__.py
--rw-r--r--   0        0        0     4656 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/module.py
--rw-r--r--   0        0        0     1236 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/testing/uvicorn_server.py
--rw-r--r--   0        0        0       60 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/__init__.py
--rw-r--r--   0        0        0     8476 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/sync_worker.py
--rw-r--r--   0        0        0      664 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/threading/utils.py
--rw-r--r--   0        0        0     2386 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/__init__.py
--rw-r--r--   0        0        0      870 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/crypto.py
--rw-r--r--   0        0        0      658 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/enums.py
--rw-r--r--   0        0        0      389 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/event_loop.py
--rw-r--r--   0        0        0     7692 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/functional.py
--rw-r--r--   0        0        0     3810 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/importer.py
--rw-r--r--   0        0        0      723 2024-04-25 08:12:14.642263 ellar-0.7.4/ellar/utils/module_loading.py
--rw-r--r--   0        0        0     3363 2024-04-25 08:12:14.642263 ellar-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     9083 1970-01-01 00:00:00.000000 ellar-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     6789 2024-05-22 21:06:47.163232 ellar-0.7.6/README.md
+-rw-r--r--   0        0        0      149 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/__init__.py
+-rw-r--r--   0        0        0     3281 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/context.py
+-rw-r--r--   0        0        0     8186 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/factory.py
+-rw-r--r--   0        0        0     2590 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/lifespan.py
+-rw-r--r--   0        0        0    12053 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/main.py
+-rw-r--r--   0        0        0     2267 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/app/services.py
+-rw-r--r--   0        0        0      810 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/constants.py
+-rw-r--r--   0        0        0     2139 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/decorators.py
+-rw-r--r--   0        0        0      411 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/guards/__init__.py
+-rw-r--r--   0        0        0     1281 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/guards/apikey.py
+-rw-r--r--   0        0        0     1405 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/guards/auth_required.py
+-rw-r--r--   0        0        0      472 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/guards/http.py
+-rw-r--r--   0        0        0      356 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/guards/mixin.py
+-rw-r--r--   0        0        0      575 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/api_key.py
+-rw-r--r--   0        0        0      472 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/http.py
+-rw-r--r--   0        0        0      698 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/mixin.py
+-rw-r--r--   0        0        0      683 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/model.py
+-rw-r--r--   0        0        0      371 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/schemes/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/schemes/api_key.py
+-rw-r--r--   0        0        0     5205 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/schemes/base.py
+-rw-r--r--   0        0        0     3634 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/handlers/schemes/http.py
+-rw-r--r--   0        0        0      223 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/identity.py
+-rw-r--r--   0        0        0     1750 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/interceptor.py
+-rw-r--r--   0        0        0      142 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/middleware/__init__.py
+-rw-r--r--   0        0        0     1625 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/middleware/auth.py
+-rw-r--r--   0        0        0     2239 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/middleware/session.py
+-rw-r--r--   0        0        0      370 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/policy/__init__.py
+-rw-r--r--   0        0        0     5189 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/policy/base.py
+-rw-r--r--   0        0        0      940 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/policy/common.py
+-rw-r--r--   0        0        0      177 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/services/__init__.py
+-rw-r--r--   0        0        0     1046 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/services/auth_schemes.py
+-rw-r--r--   0        0        0     1637 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/services/middleware.py
+-rw-r--r--   0        0        0      934 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/session/__init__.py
+-rw-r--r--   0        0        0     1622 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/session/base.py
+-rw-r--r--   0        0        0     1699 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/session/cookie_dict.py
+-rw-r--r--   0        0        0      384 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/session/options.py
+-rw-r--r--   0        0        0     2174 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/auth/session/strategy.py
+-rw-r--r--   0        0        0      257 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/__init__.py
+-rw-r--r--   0        0        0      109 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/__init__.py
+-rw-r--r--   0        0        0     4841 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/_aio_cache.py.ellar
+-rw-r--r--   0        0        0     4633 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/base.py
+-rw-r--r--   0        0        0     5406 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/local_cache.py
+-rw-r--r--   0        0        0      971 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/pylib_cache.py
+-rw-r--r--   0        0        0     2240 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/pymem_cache.py
+-rw-r--r--   0        0        0       72 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/redis/__init__.py
+-rw-r--r--   0        0        0     6813 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/redis/backend.py
+-rw-r--r--   0        0        0     1413 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/backends/serializer.py
+-rw-r--r--   0        0        0     3018 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/decorator.py
+-rw-r--r--   0        0        0    11819 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/interface.py
+-rw-r--r--   0        0        0     2045 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/make_key_decorator.py
+-rw-r--r--   0        0        0     2657 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/model.py
+-rw-r--r--   0        0        0     1882 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/module.py
+-rw-r--r--   0        0        0      867 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/schema.py
+-rw-r--r--   0        0        0     5077 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/cache/service.py
+-rw-r--r--   0        0        0     3839 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/__init__.py
+-rw-r--r--   0        0        0      195 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/compatible/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/compatible/cache_properties.py
+-rw-r--r--   0        0        0      891 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/compatible/dict.py
+-rw-r--r--   0        0        0     4901 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/constants.py
+-rw-r--r--   0        0        0     1672 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/converters.py
+-rw-r--r--   0        0        0     2829 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/datastructures.py
+-rw-r--r--   0        0        0      811 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/__init__.py
+-rw-r--r--   0        0        0      628 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/base.py
+-rw-r--r--   0        0        0     3850 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/controller.py
+-rw-r--r--   0        0        0     1042 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/exception.py
+-rw-r--r--   0        0        0      610 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/extra_args.py
+-rw-r--r--   0        0        0     2528 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/file.py
+-rw-r--r--   0        0        0     1026 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/guards.py
+-rw-r--r--   0        0        0     4740 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/html.py
+-rw-r--r--   0        0        0     1085 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/interceptor.py
+-rw-r--r--   0        0        0      928 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/middleware.py
+-rw-r--r--   0        0        0     3335 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/modules.py
+-rw-r--r--   0        0        0     1184 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/serializer.py
+-rw-r--r--   0        0        0      397 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/decorators/versioning.py
+-rw-r--r--   0        0        0      930 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/__init__.py
+-rw-r--r--   0        0        0      472 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/api/__init__.py
+-rw-r--r--   0        0        0     1519 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/api/base.py
+-rw-r--r--   0        0        0     1251 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/api/exceptions_types.py
+-rw-r--r--   0        0        0     2588 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/callable_exceptions.py
+-rw-r--r--   0        0        0      103 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/context.py
+-rw-r--r--   0        0        0     2537 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/handlers.py
+-rw-r--r--   0        0        0      768 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/exceptions/validation.py
+-rw-r--r--   0        0        0     1369 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/interfaces/__init__.py
+-rw-r--r--   0        0        0      818 2024-05-22 21:06:47.207232 ellar-0.7.6/ellar/common/interfaces/application.py
+-rw-r--r--   0        0        0     3971 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/context.py
+-rw-r--r--   0        0        0     1769 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/exceptions.py
+-rw-r--r--   0        0        0      400 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/guard_consumer.py
+-rw-r--r--   0        0        0      684 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/identity_schemes.py
+-rw-r--r--   0        0        0      406 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/interceptor_consumer.py
+-rw-r--r--   0        0        0      404 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/middleware.py
+-rw-r--r--   0        0        0     1771 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/module.py
+-rw-r--r--   0        0        0      748 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/response_model.py
+-rw-r--r--   0        0        0      907 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/templating.py
+-rw-r--r--   0        0        0      774 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/interfaces/versioning.py
+-rw-r--r--   0        0        0      104 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/logging.py
+-rw-r--r--   0        0        0      363 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/models/__init__.py
+-rw-r--r--   0        0        0      877 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/models/controller.py
+-rw-r--r--   0        0        0      803 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/models/guard.py
+-rw-r--r--   0        0        0      851 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/models/identity.py
+-rw-r--r--   0        0        0      320 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/models/interceptor.py
+-rw-r--r--   0        0        0      802 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/operations/__init__.py
+-rw-r--r--   0        0        0     9663 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/operations/base.py
+-rw-r--r--   0        0        0     2759 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/operations/router.py
+-rw-r--r--   0        0        0     3632 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/operations/schema.py
+-rw-r--r--   0        0        0      555 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/__init__.py
+-rw-r--r--   0        0        0    14710 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/base.py
+-rw-r--r--   0        0        0     1657 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/extra_args.py
+-rw-r--r--   0        0        0     1994 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/factory.py
+-rw-r--r--   0        0        0     6837 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/request_model.py
+-rw-r--r--   0        0        0     6180 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/resolver_generators.py
+-rw-r--r--   0        0        0     2429 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/args/websocket_model.py
+-rw-r--r--   0        0        0     4165 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/decorators/__init__.py
+-rw-r--r--   0        0        0     2366 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/decorators/inject.py
+-rw-r--r--   0        0        0    16837 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/decorators/models.py
+-rw-r--r--   0        0        0    15753 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/params.py
+-rw-r--r--   0        0        0     1106 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/__init__.py
+-rw-r--r--   0        0        0     1702 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/base.py
+-rw-r--r--   0        0        0     5830 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/bulk_parameter.py
+-rw-r--r--   0        0        0    11220 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/parameter.py
+-rw-r--r--   0        0        0      776 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/__init__.py
+-rw-r--r--   0        0        0      873 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/background.py
+-rw-r--r--   0        0        0     2726 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/base.py
+-rw-r--r--   0        0        0      397 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/connection.py
+-rw-r--r--   0        0        0      334 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/context.py
+-rw-r--r--   0        0        0     1547 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/provider.py
+-rw-r--r--   0        0        0      393 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/request.py
+-rw-r--r--   0        0        0      400 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/response.py
+-rw-r--r--   0        0        0      524 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/session.py
+-rw-r--r--   0        0        0      392 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/params/resolvers/system_parameters/websocket.py
+-rw-r--r--   0        0        0      415 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/__init__.py
+-rw-r--r--   0        0        0     7921 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/base.py
+-rw-r--r--   0        0        0       50 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/exceptions.py
+-rw-r--r--   0        0        0     4305 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/file.py
+-rw-r--r--   0        0        0      726 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/helper.py
+-rw-r--r--   0        0        0     2129 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/html.py
+-rw-r--r--   0        0        0     2935 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/json.py
+-rw-r--r--   0        0        0     4865 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/route.py
+-rw-r--r--   0        0        0     1688 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/models/type_converter.py
+-rw-r--r--   0        0        0     1253 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/responses/response_types.py
+-rw-r--r--   0        0        0      357 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/serializer/__init__.py
+-rw-r--r--   0        0        0     5633 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/serializer/base.py
+-rw-r--r--   0        0        0      194 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/serializer/guard.py
+-rw-r--r--   0        0        0      454 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/shortcuts.py
+-rw-r--r--   0        0        0      613 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/__init__.py
+-rw-r--r--   0        0        0      593 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/environment.py
+-rw-r--r--   0        0        0     2020 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/loader.py
+-rw-r--r--   0        0        0      835 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/model.py
+-rw-r--r--   0        0        0     3018 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/renderer.py
+-rw-r--r--   0        0        0      110 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/templating/schema.py
+-rw-r--r--   0        0        0      713 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/common/types.py
+-rw-r--r--   0        0        0      928 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/conf/__init__.py
+-rw-r--r--   0        0        0     5454 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/conf/app_settings_models.py
+-rw-r--r--   0        0        0     2397 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/conf/config.py
+-rw-r--r--   0        0        0     3270 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/conf/mixins.py
+-rw-r--r--   0        0        0      469 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/connection/__init__.py
+-rw-r--r--   0        0        0      855 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/connection/http.py
+-rw-r--r--   0        0        0      245 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/connection/websocket.py
+-rw-r--r--   0        0        0       97 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/exceptions/__init__.py
+-rw-r--r--   0        0        0     2157 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/exceptions/service.py
+-rw-r--r--   0        0        0      457 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/__init__.py
+-rw-r--r--   0        0        0     1327 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/execution.py
+-rw-r--r--   0        0        0     2581 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/factory.py
+-rw-r--r--   0        0        0     2280 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/host.py
+-rw-r--r--   0        0        0     2089 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/http.py
+-rw-r--r--   0        0        0      801 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/execution_context/websocket.py
+-rw-r--r--   0        0        0       72 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/guards/__init__.py
+-rw-r--r--   0        0        0     1729 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/guards/consumer.py
+-rw-r--r--   0        0        0       87 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/interceptors/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-22 21:06:47.211232 ellar-0.7.6/ellar/core/interceptors/consumer.py
+-rw-r--r--   0        0        0     1050 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/__init__.py
+-rw-r--r--   0        0        0     2905 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/di.py
+-rw-r--r--   0        0        0     2689 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/exceptions.py
+-rw-r--r--   0        0        0     2577 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/function.py
+-rw-r--r--   0        0        0      917 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/middleware.py
+-rw-r--r--   0        0        0     1049 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/middleware/versioning.py
+-rw-r--r--   0        0        0      363 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/base.py
+-rw-r--r--   0        0        0     3082 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/builder.py
+-rw-r--r--   0        0        0     7921 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/config.py
+-rw-r--r--   0        0        0      787 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/helper.py
+-rw-r--r--   0        0        0     9438 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/modules/ref.py
+-rw-r--r--   0        0        0      291 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/router_builders/__init__.py
+-rw-r--r--   0        0        0     2094 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/router_builders/base.py
+-rw-r--r--   0        0        0     4821 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/router_builders/controller.py
+-rw-r--r--   0        0        0     1251 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/router_builders/module_router.py
+-rw-r--r--   0        0        0      963 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/__init__.py
+-rw-r--r--   0        0        0     5427 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/base.py
+-rw-r--r--   0        0        0      272 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/__init__.py
+-rw-r--r--   0        0        0     1068 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/base.py
+-rw-r--r--   0        0        0      852 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/route.py
+-rw-r--r--   0        0        0      190 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/websocket/__init__.py
+-rw-r--r--   0        0        0     1844 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/websocket/handler.py
+-rw-r--r--   0        0        0     1564 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/controller/websocket/route.py
+-rw-r--r--   0        0        0     2566 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/file_mount.py
+-rw-r--r--   0        0        0     7056 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/mount.py
+-rw-r--r--   0        0        0     5321 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/route.py
+-rw-r--r--   0        0        0     3046 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/route_collections.py
+-rw-r--r--   0        0        0     2324 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/utils.py
+-rw-r--r--   0        0        0      161 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/websocket/__init__.py
+-rw-r--r--   0        0        0     6628 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/websocket/handler.py
+-rw-r--r--   0        0        0     5618 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/routing/websocket/route.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/__init__.py
+-rw-r--r--   0        0        0     4074 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/__init__.py
+-rw-r--r--   0        0        0     1811 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/argon2.py
+-rw-r--r--   0        0        0     3002 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/base.py
+-rw-r--r--   0        0        0     1739 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/bcrypt.py
+-rw-r--r--   0        0        0     1418 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/md5.py
+-rw-r--r--   0        0        0     1282 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/pbkdf.py
+-rw-r--r--   0        0        0     2774 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/security/hashers/scrypt.py
+-rw-r--r--   0        0        0       82 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/services/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/services/reflector.py
+-rw-r--r--   0        0        0      392 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/shortcuts.py
+-rw-r--r--   0        0        0     1805 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/staticfiles.py
+-rw-r--r--   0        0        0      673 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/versioning/__init__.py
+-rw-r--r--   0        0        0     2569 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/versioning/base.py
+-rw-r--r--   0        0        0     6171 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/core/versioning/resolver.py
+-rw-r--r--   0        0        0     1220 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/asgi_args.py
+-rw-r--r--   0        0        0     1120 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/constants.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/context.py
+-rw-r--r--   0        0        0      400 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/exceptions.py
+-rw-r--r--   0        0        0      117 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/injector/__init__.py
+-rw-r--r--   0        0        0     8754 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/injector/container.py
+-rw-r--r--   0        0        0     5912 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/injector/ellar_injector.py
+-rw-r--r--   0        0        0      154 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/logger.py
+-rw-r--r--   0        0        0     1001 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/providers.py
+-rw-r--r--   0        0        0     2050 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/scopes.py
+-rw-r--r--   0        0        0     5969 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/service_config.py
+-rw-r--r--   0        0        0       39 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/types.py
+-rw-r--r--   0        0        0      406 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/di/utils.py
+-rw-r--r--   0        0        0      231 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/events/__init__.py
+-rw-r--r--   0        0        0     1951 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/events/base.py
+-rw-r--r--   0        0        0      579 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/__init__.py
+-rw-r--r--   0        0        0    10854 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/builder.py
+-rw-r--r--   0        0        0      243 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/constants.py
+-rw-r--r--   0        0        0       94 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/decorators/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/decorators/extra_info.py
+-rw-r--r--   0        0        0      731 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/decorators/tags.py
+-rw-r--r--   0        0        0      219 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/docs_ui/__init__.py
+-rw-r--r--   0        0        0     1138 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/docs_ui/base.py
+-rw-r--r--   0        0        0      932 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/docs_ui/redocs.py
+-rw-r--r--   0        0        0     2226 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/docs_ui/stoplight.py
+-rw-r--r--   0        0        0     1078 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/docs_ui/swagger.py
+-rw-r--r--   0        0        0     5497 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/module.py
+-rw-r--r--   0        0        0    13873 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/openapi_v3.py
+-rw-r--r--   0        0        0    16040 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/route_doc_models.py
+-rw-r--r--   0        0        0      115 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/schemas/__init__.py
+-rw-r--r--   0        0        0      348 2024-05-22 21:06:47.215232 ellar-0.7.6/ellar/openapi/schemas/validation.py
+-rw-r--r--   0        0        0    50277 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/openapi/static/swagger/SwaggerDark.css
+-rw-r--r--   0        0        0      702 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/openapi/templates/redocs.html
+-rw-r--r--   0        0        0      895 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/openapi/templates/swagger.html
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/py.typed
+-rw-r--r--   0        0        0     2082 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/__init__.py
+-rw-r--r--   0        0        0     1528 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/decorator.py
+-rw-r--r--   0        0        0      764 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/emails.py
+-rw-r--r--   0        0        0     1798 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/encoder.py
+-rw-r--r--   0        0        0     1718 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/exceptions.py
+-rw-r--r--   0        0        0      692 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/field_constraints.py
+-rw-r--r--   0        0        0     2850 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/fields.py
+-rw-r--r--   0        0        0      397 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/types.py
+-rw-r--r--   0        0        0     8596 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/pydantic/utils.py
+-rw-r--r--   0        0        0      105 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/reflect/__init__.py
+-rw-r--r--   0        0        0     5258 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/reflect/_reflect.py
+-rw-r--r--   0        0        0       34 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/reflect/constants.py
+-rw-r--r--   0        0        0       58 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/controllers/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/controllers/guard.py
+-rw-r--r--   0        0        0      704 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/controllers/home.py
+-rw-r--r--   0        0        0      211 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/modules.py
+-rw-r--r--   0        0        0   232915 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0      721 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/static/css/cover.css
+-rwxr-xr-x   0        0        0    25915 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/static/img/EllarLogoB.png
+-rwxr-xr-x   0        0        0    36744 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/static/img/EllarLogoIconOnly.png
+-rwxr-xr-x   0        0        0     3888 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/static/img/Icon.svg
+-rw-r--r--   0        0        0     2575 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/samples/templates/home/index.html
+-rw-r--r--   0        0        0      629 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/adapter.py
+-rw-r--r--   0        0        0      543 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/constants.py
+-rw-r--r--   0        0        0     1914 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/context.py
+-rw-r--r--   0        0        0      225 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/decorators/__init__.py
+-rw-r--r--   0        0        0      667 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/decorators/events.py
+-rw-r--r--   0        0        0     3034 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/decorators/gateway.py
+-rw-r--r--   0        0        0      570 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/decorators/subscribe_message.py
+-rw-r--r--   0        0        0     4177 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/factory.py
+-rw-r--r--   0        0        0     9619 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/gateway.py
+-rw-r--r--   0        0        0      144 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/model.py
+-rw-r--r--   0        0        0      532 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/responses.py
+-rw-r--r--   0        0        0      107 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/testing/__init__.py
+-rw-r--r--   0        0        0     1700 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/socket_io/testing/module.py
+-rw-r--r--   0        0        0      129 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/testing/__init__.py
+-rw-r--r--   0        0        0     4438 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/testing/module.py
+-rw-r--r--   0        0        0     1236 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/testing/uvicorn_server.py
+-rw-r--r--   0        0        0       60 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/threading/__init__.py
+-rw-r--r--   0        0        0     8476 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/threading/sync_worker.py
+-rw-r--r--   0        0        0      664 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/threading/utils.py
+-rw-r--r--   0        0        0     2386 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/__init__.py
+-rw-r--r--   0        0        0      870 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/crypto.py
+-rw-r--r--   0        0        0      658 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/enums.py
+-rw-r--r--   0        0        0      389 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/event_loop.py
+-rw-r--r--   0        0        0     7692 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/functional.py
+-rw-r--r--   0        0        0     3810 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/importer.py
+-rw-r--r--   0        0        0      723 2024-05-22 21:06:47.219232 ellar-0.7.6/ellar/utils/module_loading.py
+-rw-r--r--   0        0        0     3363 2024-05-22 21:06:47.219232 ellar-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     9083 1970-01-01 00:00:00.000000 ellar-0.7.6/PKG-INFO
```

### Comparing `ellar-0.7.4/README.md` & `ellar-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/app/context.py` & `ellar-0.7.6/ellar/app/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/app/factory.py` & `ellar-0.7.6/ellar/app/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing as t
 from collections import OrderedDict
 from pathlib import Path
 
 import click
-from ellar.common import Module
+from ellar.common import IApplicationReady, Module
 from ellar.common.constants import MODULE_METADATA, MODULE_WATERMARK
 from ellar.common.models import GuardCanActivate
 from ellar.core import Config, DynamicModule, LazyModuleImport, ModuleBase, ModuleSetup
 from ellar.core.modules import ModuleRefBase
 from ellar.di import EllarInjector, ProviderConfig
 from ellar.reflect import reflect
 from ellar.utils import get_unique_type
@@ -170,14 +170,21 @@
             ), f"{module_config.module} is not properly configured."
 
             injector.add_module(module_ref)
             app.router.extend(module_ref.routes)
 
         # app.setup_jinja_environment
         app.setup_jinja_environment()
+
+        for module, module_ref in app.injector.get_modules().items():
+            module_ref.run_module_register_services()
+
+            if issubclass(module, IApplicationReady):
+                app.injector.get(module).on_ready(app)
+
         return app
 
     @classmethod
     def create_app(
         cls,
         controllers: t.Sequence[t.Union[t.Type]] = (),
         routers: t.Sequence[t.Union["ModuleRouter", "EllarMount", Mount, Host]] = (),
```

### Comparing `ellar-0.7.4/ellar/app/lifespan.py` & `ellar-0.7.6/ellar/app/lifespan.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         ] = None,
     ) -> None:
         self._lifespan_context = (
             _default_lifespan_context if lifespan_context is None else lifespan_context
         )
 
     def _get_startup_modules(self, app: "App") -> t.Iterator[IApplicationStartup]:
-        for module, module_ref in app.injector.get_modules().items():
-            module_ref.run_module_register_services()
+        for module in app.injector.get_modules():
             if issubclass(module, IApplicationStartup):
                 yield app.injector.get(module)
 
     def _get_shutdown_modules(self, app: "App") -> t.Iterator[IApplicationShutdown]:
         for module in app.injector.get_modules():
             if issubclass(module, IApplicationShutdown):
                 yield app.injector.get(module)
```

### Comparing `ellar-0.7.4/ellar/app/main.py` & `ellar-0.7.6/ellar/app/main.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/app/services.py` & `ellar-0.7.6/ellar/app/services.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/__init__.py` & `ellar-0.7.6/ellar/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/decorators.py` & `ellar-0.7.6/ellar/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/guards/apikey.py` & `ellar-0.7.6/ellar/auth/guards/apikey.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/guards/auth_required.py` & `ellar-0.7.6/ellar/auth/guards/auth_required.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/__init__.py` & `ellar-0.7.6/ellar/auth/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/api_key.py` & `ellar-0.7.6/ellar/auth/handlers/api_key.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/mixin.py` & `ellar-0.7.6/ellar/auth/handlers/mixin.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/model.py` & `ellar-0.7.6/ellar/auth/handlers/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/schemes/api_key.py` & `ellar-0.7.6/ellar/auth/handlers/schemes/api_key.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/schemes/base.py` & `ellar-0.7.6/ellar/auth/handlers/schemes/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/handlers/schemes/http.py` & `ellar-0.7.6/ellar/auth/handlers/schemes/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/interceptor.py` & `ellar-0.7.6/ellar/auth/interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/middleware/auth.py` & `ellar-0.7.6/ellar/auth/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/middleware/session.py` & `ellar-0.7.6/ellar/auth/middleware/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/policy/base.py` & `ellar-0.7.6/ellar/auth/policy/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/policy/common.py` & `ellar-0.7.6/ellar/auth/policy/common.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/services/auth_schemes.py` & `ellar-0.7.6/ellar/auth/services/auth_schemes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/services/middleware.py` & `ellar-0.7.6/ellar/auth/services/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/session/__init__.py` & `ellar-0.7.6/ellar/auth/session/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/session/base.py` & `ellar-0.7.6/ellar/auth/session/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/session/cookie_dict.py` & `ellar-0.7.6/ellar/auth/session/cookie_dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/auth/session/strategy.py` & `ellar-0.7.6/ellar/auth/session/strategy.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/_aio_cache.py.ellar` & `ellar-0.7.6/ellar/cache/backends/_aio_cache.py.ellar`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/base.py` & `ellar-0.7.6/ellar/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/local_cache.py` & `ellar-0.7.6/ellar/cache/backends/local_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/pylib_cache.py` & `ellar-0.7.6/ellar/cache/backends/pylib_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/pymem_cache.py` & `ellar-0.7.6/ellar/cache/backends/pymem_cache.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/redis/backend.py` & `ellar-0.7.6/ellar/cache/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/backends/serializer.py` & `ellar-0.7.6/ellar/cache/backends/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/decorator.py` & `ellar-0.7.6/ellar/cache/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/interface.py` & `ellar-0.7.6/ellar/cache/interface.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/make_key_decorator.py` & `ellar-0.7.6/ellar/cache/make_key_decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/model.py` & `ellar-0.7.6/ellar/cache/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/module.py` & `ellar-0.7.6/ellar/cache/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/schema.py` & `ellar-0.7.6/ellar/cache/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/cache/service.py` & `ellar-0.7.6/ellar/cache/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/__init__.py` & `ellar-0.7.6/ellar/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     NotAuthenticated,
     NotFound,
     PermissionDenied,
     UnsupportedMediaType,
     WebSocketException,
 )
 from .interfaces import (
+    IApplicationReady,
     IApplicationShutdown,
     IApplicationStartup,
     IExceptionHandler,
     IExceptionMiddlewareService,
     IExecutionContext,
     IExecutionContextFactory,
     IGuardsConsumer,
@@ -181,12 +182,13 @@
     "IInterceptorsConsumer",
     "IGuardsConsumer",
     "EllarInterceptor",
     "UseInterceptors",
     "IApplicationStartup",
     "IApplicationShutdown",
     "IIdentitySchemes",
+    "IApplicationReady",
 ]
 
 
 def __dir__() -> t.List[str]:
     return sorted(__all__)  # pragma: no cover
```

### Comparing `ellar-0.7.4/ellar/common/compatible/cache_properties.py` & `ellar-0.7.6/ellar/common/compatible/cache_properties.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/compatible/dict.py` & `ellar-0.7.6/ellar/common/compatible/dict.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/constants.py` & `ellar-0.7.6/ellar/common/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/converters.py` & `ellar-0.7.6/ellar/common/converters.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/datastructures.py` & `ellar-0.7.6/ellar/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/__init__.py` & `ellar-0.7.6/ellar/common/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/base.py` & `ellar-0.7.6/ellar/common/decorators/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/controller.py` & `ellar-0.7.6/ellar/common/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/exception.py` & `ellar-0.7.6/ellar/common/decorators/exception.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/extra_args.py` & `ellar-0.7.6/ellar/common/decorators/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/file.py` & `ellar-0.7.6/ellar/common/decorators/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/guards.py` & `ellar-0.7.6/ellar/common/decorators/guards.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/html.py` & `ellar-0.7.6/ellar/common/decorators/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/interceptor.py` & `ellar-0.7.6/ellar/common/decorators/interceptor.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/middleware.py` & `ellar-0.7.6/ellar/common/decorators/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/modules.py` & `ellar-0.7.6/ellar/common/decorators/modules.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/decorators/serializer.py` & `ellar-0.7.6/ellar/common/decorators/serializer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/__init__.py` & `ellar-0.7.6/ellar/common/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/api/base.py` & `ellar-0.7.6/ellar/common/exceptions/api/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/api/exceptions_types.py` & `ellar-0.7.6/ellar/common/exceptions/api/exceptions_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/callable_exceptions.py` & `ellar-0.7.6/ellar/common/exceptions/callable_exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/handlers.py` & `ellar-0.7.6/ellar/common/exceptions/handlers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/exceptions/validation.py` & `ellar-0.7.6/ellar/common/exceptions/validation.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/__init__.py` & `ellar-0.7.6/ellar/common/interfaces/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .application import IApplicationShutdown, IApplicationStartup
+from .application import IApplicationReady, IApplicationShutdown, IApplicationStartup
 from .context import (
     IExecutionContext,
     IExecutionContextFactory,
     IHostContext,
     IHostContextFactory,
     IHTTPConnectionContextFactory,
     IHTTPHostContext,
@@ -37,8 +37,9 @@
     "IGuardsConsumer",
     "IApplicationShutdown",
     "IApplicationStartup",
     "IAPIVersioning",
     "IAPIVersioningResolver",
     "IEllarMiddleware",
     "IIdentitySchemes",
+    "IApplicationReady",
 ]
```

### Comparing `ellar-0.7.4/ellar/common/interfaces/context.py` & `ellar-0.7.6/ellar/common/interfaces/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/exceptions.py` & `ellar-0.7.6/ellar/common/interfaces/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/identity_schemes.py` & `ellar-0.7.6/ellar/common/interfaces/identity_schemes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/module.py` & `ellar-0.7.6/ellar/common/interfaces/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/response_model.py` & `ellar-0.7.6/ellar/common/interfaces/response_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/templating.py` & `ellar-0.7.6/ellar/common/interfaces/templating.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/interfaces/versioning.py` & `ellar-0.7.6/ellar/common/interfaces/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/models/controller.py` & `ellar-0.7.6/ellar/common/models/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/models/guard.py` & `ellar-0.7.6/ellar/common/models/guard.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/models/identity.py` & `ellar-0.7.6/ellar/common/models/identity.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/operations/__init__.py` & `ellar-0.7.6/ellar/common/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/operations/base.py` & `ellar-0.7.6/ellar/common/operations/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/operations/router.py` & `ellar-0.7.6/ellar/common/operations/router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/operations/schema.py` & `ellar-0.7.6/ellar/common/operations/schema.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/__init__.py` & `ellar-0.7.6/ellar/common/params/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/base.py` & `ellar-0.7.6/ellar/common/params/args/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/extra_args.py` & `ellar-0.7.6/ellar/common/params/args/extra_args.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/factory.py` & `ellar-0.7.6/ellar/common/params/args/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/request_model.py` & `ellar-0.7.6/ellar/common/params/args/request_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/resolver_generators.py` & `ellar-0.7.6/ellar/common/params/args/resolver_generators.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/args/websocket_model.py` & `ellar-0.7.6/ellar/common/params/args/websocket_model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/decorators/__init__.py` & `ellar-0.7.6/ellar/common/params/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/decorators/inject.py` & `ellar-0.7.6/ellar/common/params/decorators/inject.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/decorators/models.py` & `ellar-0.7.6/ellar/common/params/decorators/models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/params.py` & `ellar-0.7.6/ellar/common/params/params.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/__init__.py` & `ellar-0.7.6/ellar/common/params/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/base.py` & `ellar-0.7.6/ellar/common/params/resolvers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/bulk_parameter.py` & `ellar-0.7.6/ellar/common/params/resolvers/bulk_parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,20 +78,22 @@
 
     async def resolve_grouped_fields(
         self, ctx: IExecutionContext, body: t.Any
     ) -> t.Tuple:
         request_logger.debug(
             f"Resolving Form Grouped Field - '{self.__class__.__name__}'"
         )
-        value, resolver_errors = await self._get_resolver_data(ctx, body, by_alias=True)
+        values, resolver_errors = await self._get_resolver_data(
+            ctx, body, by_alias=True
+        )
         if resolver_errors:
-            return value, resolver_errors
+            return values, resolver_errors
         # Combining resolved values into one pydantic model specified by the user in Route function parameter
         processed_value, processed_errors = self.model_field.validate(
-            value,
+            values,
             {},
             loc=(self.model_field.field_info.in_.value, self.model_field.alias),
         )
 
         if processed_errors:  # pragma: no cover
             # Just in case error still happened after combining each field to one pydantic model.
             processed_errors = self.validate_error_sequence(processed_errors)
@@ -144,8 +146,8 @@
 
         values, errors = await super().resolve_handle(ctx, *args, body=_body, **kwargs)
 
         if errors:
             return values, self.validate_error_sequence(errors)
 
         _, body_value = values.popitem()
-        return body_value.dict(), []
+        return {k: getattr(body_value, k) for k in body_value.model_fields_set}, []
```

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/parameter.py` & `ellar-0.7.6/ellar/common/params/resolvers/parameter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/__init__.py` & `ellar-0.7.6/ellar/common/params/resolvers/system_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/background.py` & `ellar-0.7.6/ellar/common/params/resolvers/system_parameters/background.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/base.py` & `ellar-0.7.6/ellar/common/params/resolvers/system_parameters/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/provider.py` & `ellar-0.7.6/ellar/common/params/resolvers/system_parameters/provider.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/params/resolvers/system_parameters/session.py` & `ellar-0.7.6/ellar/common/params/resolvers/system_parameters/session.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/__init__.py` & `ellar-0.7.6/ellar/common/responses/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/base.py` & `ellar-0.7.6/ellar/common/responses/models/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/file.py` & `ellar-0.7.6/ellar/common/responses/models/file.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/helper.py` & `ellar-0.7.6/ellar/common/responses/models/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/html.py` & `ellar-0.7.6/ellar/common/responses/models/html.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/json.py` & `ellar-0.7.6/ellar/common/responses/models/json.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/route.py` & `ellar-0.7.6/ellar/common/responses/models/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/models/type_converter.py` & `ellar-0.7.6/ellar/common/responses/models/type_converter.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/responses/response_types.py` & `ellar-0.7.6/ellar/common/responses/response_types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/serializer/base.py` & `ellar-0.7.6/ellar/common/serializer/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/templating/__init__.py` & `ellar-0.7.6/ellar/common/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/templating/environment.py` & `ellar-0.7.6/ellar/common/templating/environment.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/templating/loader.py` & `ellar-0.7.6/ellar/common/templating/loader.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/templating/model.py` & `ellar-0.7.6/ellar/common/templating/model.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/common/templating/renderer.py` & `ellar-0.7.6/ellar/common/templating/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,37 +37,50 @@
     template_string: str, request: "Request", **template_context: t.Any
 ) -> str:
     """Renders a template to string.
     :param request: Request instance
     :param template_string: Template String
     :param template_context: variables that should be available in the context of the template.
     """
-    jinja_environment = request.service_provider.get(Environment)
-    jinja_template = jinja_environment.from_string(template_string)
+    try:
+        jinja_template, template_context_ = _get_jinja_and_template_context(
+            template_name=template_string,
+            request=request,
+            **process_view_model(template_context),
+        )
+        return jinja_template.render(template_context_)
+    except jinja2.TemplateNotFound:
+        jinja_environment = request.service_provider.get(Environment)
+        jinja_template = jinja_environment.from_string(template_string)
 
-    _template_context = dict(template_context)
-    _template_context.update(request=request)
+        _template_context = dict(template_context)
+        _template_context.update(request=request)
 
-    return jinja_template.render(_template_context)  # type:ignore[no-any-return]
+        return jinja_template.render(_template_context)
 
 
 def render_template(
     template_name: str,
     request: "Request",
     background: t.Optional[BackgroundTask] = None,
+    status_code: int = 200,
     **template_kwargs: t.Any,
 ) -> TemplateResponse:
     """Renders a template from the template folder with the given context.
+    :param status_code: Template Response status code
     :param request: Request instance
     :param template_name: the name of the template to be rendered
     :param template_kwargs: variables that should be available in the context of the template.
     :param background: any background task to be executed after render.
     :return TemplateResponse
     """
     jinja_template, template_context = _get_jinja_and_template_context(
         template_name=template_name,
         request=request,
         **process_view_model(template_kwargs),
     )
     return TemplateResponse(
-        template=jinja_template, context=template_context, background=background
+        template=jinja_template,
+        context=template_context,
+        background=background,
+        status_code=status_code,
     )
```

### Comparing `ellar-0.7.4/ellar/common/types.py` & `ellar-0.7.6/ellar/common/types.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/__init__.py` & `ellar-0.7.6/ellar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/conf/app_settings_models.py` & `ellar-0.7.6/ellar/core/conf/app_settings_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/conf/config.py` & `ellar-0.7.6/ellar/core/conf/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/conf/mixins.py` & `ellar-0.7.6/ellar/core/conf/mixins.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/connection/http.py` & `ellar-0.7.6/ellar/core/connection/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/exceptions/service.py` & `ellar-0.7.6/ellar/core/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/execution_context/execution.py` & `ellar-0.7.6/ellar/core/execution_context/execution.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/execution_context/factory.py` & `ellar-0.7.6/ellar/core/execution_context/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/execution_context/host.py` & `ellar-0.7.6/ellar/core/execution_context/host.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/execution_context/http.py` & `ellar-0.7.6/ellar/core/execution_context/http.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/execution_context/websocket.py` & `ellar-0.7.6/ellar/core/execution_context/websocket.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/guards/consumer.py` & `ellar-0.7.6/ellar/core/guards/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/interceptors/consumer.py` & `ellar-0.7.6/ellar/core/interceptors/consumer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/__init__.py` & `ellar-0.7.6/ellar/core/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/di.py` & `ellar-0.7.6/ellar/core/middleware/di.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/exceptions.py` & `ellar-0.7.6/ellar/core/middleware/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/function.py` & `ellar-0.7.6/ellar/core/middleware/function.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/middleware.py` & `ellar-0.7.6/ellar/core/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/middleware/versioning.py` & `ellar-0.7.6/ellar/core/middleware/versioning.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/modules/base.py` & `ellar-0.7.6/ellar/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/modules/builder.py` & `ellar-0.7.6/ellar/core/modules/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/modules/config.py` & `ellar-0.7.6/ellar/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/modules/helper.py` & `ellar-0.7.6/ellar/core/modules/helper.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/modules/ref.py` & `ellar-0.7.6/ellar/core/modules/ref.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/router_builders/base.py` & `ellar-0.7.6/ellar/core/router_builders/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/router_builders/controller.py` & `ellar-0.7.6/ellar/core/router_builders/controller.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/router_builders/module_router.py` & `ellar-0.7.6/ellar/core/router_builders/module_router.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/__init__.py` & `ellar-0.7.6/ellar/core/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/base.py` & `ellar-0.7.6/ellar/core/routing/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/controller/base.py` & `ellar-0.7.6/ellar/core/routing/controller/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/controller/route.py` & `ellar-0.7.6/ellar/core/routing/controller/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/controller/websocket/handler.py` & `ellar-0.7.6/ellar/core/routing/controller/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/controller/websocket/route.py` & `ellar-0.7.6/ellar/core/routing/controller/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/file_mount.py` & `ellar-0.7.6/ellar/core/routing/file_mount.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/mount.py` & `ellar-0.7.6/ellar/core/routing/mount.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/route.py` & `ellar-0.7.6/ellar/core/routing/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/route_collections.py` & `ellar-0.7.6/ellar/core/routing/route_collections.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/utils.py` & `ellar-0.7.6/ellar/core/routing/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/websocket/handler.py` & `ellar-0.7.6/ellar/core/routing/websocket/handler.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/routing/websocket/route.py` & `ellar-0.7.6/ellar/core/routing/websocket/route.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/__init__.py` & `ellar-0.7.6/ellar/core/security/hashers/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/argon2.py` & `ellar-0.7.6/ellar/core/security/hashers/argon2.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/base.py` & `ellar-0.7.6/ellar/core/security/hashers/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/bcrypt.py` & `ellar-0.7.6/ellar/core/security/hashers/bcrypt.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/md5.py` & `ellar-0.7.6/ellar/core/security/hashers/md5.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/pbkdf.py` & `ellar-0.7.6/ellar/core/security/hashers/pbkdf.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/security/hashers/scrypt.py` & `ellar-0.7.6/ellar/core/security/hashers/scrypt.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/services/reflector.py` & `ellar-0.7.6/ellar/core/services/reflector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/staticfiles.py` & `ellar-0.7.6/ellar/core/staticfiles.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/versioning/__init__.py` & `ellar-0.7.6/ellar/core/versioning/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/versioning/base.py` & `ellar-0.7.6/ellar/core/versioning/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/core/versioning/resolver.py` & `ellar-0.7.6/ellar/core/versioning/resolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,17 +119,19 @@
     def raise_exception(self) -> None:
         raise NotAcceptable(
             self.invalid_version_message.format(parameter=self.header_parameter)
         )
 
     def resolve_version(self) -> str:
         message = email.message.Message()
-        message[self.header_parameter] = self.connection.headers.get(  # type: ignore[assignment]
-            self.header_parameter
-        )
+
+        value = self.connection.headers.get(self.header_parameter)
+        assert value
+
+        message[self.header_parameter] = value
         accept = dict(message.get_params(header=self.header_parameter))  # type: ignore[arg-type]
         version = accept.get(self.version_parameter, self.default_version)
         return str(version)
 
 
 class QueryParameterAPIVersionResolver(DefaultAPIVersionResolver):
     invalid_version_message = "Invalid version in query parameter."
```

### Comparing `ellar-0.7.4/ellar/di/__init__.py` & `ellar-0.7.6/ellar/di/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/constants.py` & `ellar-0.7.6/ellar/di/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/injector/container.py` & `ellar-0.7.6/ellar/di/injector/container.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/injector/ellar_injector.py` & `ellar-0.7.6/ellar/di/injector/ellar_injector.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/providers.py` & `ellar-0.7.6/ellar/di/providers.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/scopes.py` & `ellar-0.7.6/ellar/di/scopes.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/di/service_config.py` & `ellar-0.7.6/ellar/di/service_config.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/events/base.py` & `ellar-0.7.6/ellar/events/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/__init__.py` & `ellar-0.7.6/ellar/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/builder.py` & `ellar-0.7.6/ellar/openapi/builder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/decorators/extra_info.py` & `ellar-0.7.6/ellar/openapi/decorators/extra_info.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/decorators/tags.py` & `ellar-0.7.6/ellar/openapi/decorators/tags.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/docs_ui/base.py` & `ellar-0.7.6/ellar/openapi/docs_ui/base.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/docs_ui/redocs.py` & `ellar-0.7.6/ellar/openapi/docs_ui/redocs.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/docs_ui/stoplight.py` & `ellar-0.7.6/ellar/openapi/docs_ui/stoplight.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/docs_ui/swagger.py` & `ellar-0.7.6/ellar/openapi/docs_ui/swagger.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/module.py` & `ellar-0.7.6/ellar/openapi/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/openapi_v3.py` & `ellar-0.7.6/ellar/openapi/openapi_v3.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/route_doc_models.py` & `ellar-0.7.6/ellar/openapi/route_doc_models.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/static/swagger/SwaggerDark.css` & `ellar-0.7.6/ellar/openapi/static/swagger/SwaggerDark.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/templates/redocs.html` & `ellar-0.7.6/ellar/openapi/templates/redocs.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/openapi/templates/swagger.html` & `ellar-0.7.6/ellar/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/__init__.py` & `ellar-0.7.6/ellar/pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/decorator.py` & `ellar-0.7.6/ellar/pydantic/decorator.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/emails.py` & `ellar-0.7.6/ellar/pydantic/emails.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/encoder.py` & `ellar-0.7.6/ellar/pydantic/encoder.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/exceptions.py` & `ellar-0.7.6/ellar/pydantic/exceptions.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/field_constraints.py` & `ellar-0.7.6/ellar/pydantic/field_constraints.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/fields.py` & `ellar-0.7.6/ellar/pydantic/fields.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/pydantic/utils.py` & `ellar-0.7.6/ellar/pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/reflect/_reflect.py` & `ellar-0.7.6/ellar/reflect/_reflect.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/controllers/home.py` & `ellar-0.7.6/ellar/samples/controllers/home.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/static/css/bootstrap.min.css` & `ellar-0.7.6/ellar/samples/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/static/css/cover.css` & `ellar-0.7.6/ellar/samples/static/css/cover.css`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/static/img/EllarLogoB.png` & `ellar-0.7.6/ellar/samples/static/img/EllarLogoB.png`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/static/img/EllarLogoIconOnly.png` & `ellar-0.7.6/ellar/samples/static/img/EllarLogoIconOnly.png`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/static/img/Icon.svg` & `ellar-0.7.6/ellar/samples/static/img/Icon.svg`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/samples/templates/home/index.html` & `ellar-0.7.6/ellar/samples/templates/home/index.html`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/__init__.py` & `ellar-0.7.6/ellar/socket_io/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/constants.py` & `ellar-0.7.6/ellar/socket_io/constants.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/context.py` & `ellar-0.7.6/ellar/socket_io/context.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/decorators/events.py` & `ellar-0.7.6/ellar/socket_io/decorators/events.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/decorators/gateway.py` & `ellar-0.7.6/ellar/socket_io/decorators/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/decorators/subscribe_message.py` & `ellar-0.7.6/ellar/socket_io/decorators/subscribe_message.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/factory.py` & `ellar-0.7.6/ellar/socket_io/factory.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/gateway.py` & `ellar-0.7.6/ellar/socket_io/gateway.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/responses.py` & `ellar-0.7.6/ellar/socket_io/responses.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/socket_io/testing/module.py` & `ellar-0.7.6/ellar/socket_io/testing/module.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/testing/module.py` & `ellar-0.7.6/ellar/testing/module.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,25 +46,22 @@
         )
         self._providers.append(provider_config)
         return self
 
     def create_application(self) -> App:
         if self._app:
             return self._app
+
         self._app = AppFactory.create_app(
             modules=[self._testing_module],
             global_guards=self._global_guards,
             config_module=self._config_module,
             providers=self._providers,
         )
 
-        for _, module_ref in self._app.injector.get_modules().items():
-            # setup module just in case lifespan function will not be called during testing.
-            module_ref.run_module_register_services()
-
         return self._app
 
     def get_test_client(
         self,
         base_url: str = "http://testserver",
         raise_server_exceptions: bool = True,
         root_path: str = "",
```

### Comparing `ellar-0.7.4/ellar/testing/uvicorn_server.py` & `ellar-0.7.6/ellar/testing/uvicorn_server.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/threading/sync_worker.py` & `ellar-0.7.6/ellar/threading/sync_worker.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/threading/utils.py` & `ellar-0.7.6/ellar/threading/utils.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/__init__.py` & `ellar-0.7.6/ellar/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/crypto.py` & `ellar-0.7.6/ellar/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/enums.py` & `ellar-0.7.6/ellar/utils/enums.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/functional.py` & `ellar-0.7.6/ellar/utils/functional.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/importer.py` & `ellar-0.7.6/ellar/utils/importer.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/ellar/utils/module_loading.py` & `ellar-0.7.6/ellar/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/pyproject.toml` & `ellar-0.7.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ellar-0.7.4/PKG-INFO` & `ellar-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ellar
-Version: 0.7.4
+Version: 0.7.6
 Summary: Ellar - Python ASGI web framework for building fast, efficient, and scalable RESTful APIs and server-side applications.
 Author-email: Ezeudoh Tochukwu <tochukwu.ezeudoh@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

