# Comparing `tmp/logfire-0.33.0.tar.gz` & `tmp/logfire-0.34.0.tar.gz`

## Comparing `logfire-0.33.0.tar` & `logfire-0.34.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.33.0/Makefile
--rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/__main__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/cli.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/exceptions.py
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/propagate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/py.typed
--rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/testing.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/version.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/__init__.py
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/ast_utils.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/async_.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auth.py
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/backfill.py
--rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/cli.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/collect_system_info.py
--rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/config.py
--rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/config_params.py
--rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/constants.py
--rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/formatter.py
--rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/instrument.py
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_encoder.py
--rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_formatter.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_schema.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/json_types.py
--rw-r--r--   0        0        0    58309 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/main.py
--rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/metrics.py
--rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/scrubbing.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/stack_info.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/tracer.py
--rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/utils.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/__init__.py
--rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/import_hook.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/rewrite_ast.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/auto_trace/types.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/__init__.py
--rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/console.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/fallback.py
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/file.py
--rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/otlp.py
--rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/processor_wrapper.py
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/remove_pending.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/exporters/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/asyncpg.py
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/executors.py
--rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/fastapi.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/psycopg.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/anthropic.py
--rw-r--r--   0        0        0     6063 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/llm_provider.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/openai.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/_internal/integrations/llm_providers/types.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/__init__.py
--rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/logging.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/loguru.py
--rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/pydantic.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 logfire-0.33.0/logfire/integrations/structlog.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/conftest.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/module_used_for_tests.py
--rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_auto_trace.py
--rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_backfill.py
--rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_cli.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_collect_package_resources.py
--rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_configure.py
--rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_console_exporter.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_formatter.py
--rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_json_args.py
--rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_json_args_formatting.py
--rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_logfire.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_loguru.py
--rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_metrics.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_no_production.py
--rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_pydantic_plugin.py
--rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_sampling.py
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_secret_scrubbing.py
--rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_slow_async_callbacks.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_source_code_extraction.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_stdlib_logging.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_structlog.py
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_testing.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/test_utils.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/__init__.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/foo.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/auto_trace_samples/simple_nesting.py
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_fallback_exporter.py
--rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_file_exporter.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_otlp_session.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_remove_pending.py
--rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/exporters/test_retry_fewer_spans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/slow_async_callbacks_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/a/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/import_used_for_tests/a/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/__init__.py
--rw-r--r--   0        0        0    24452 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_anthropic.py
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_asgi.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_asyncpg.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_django.py
--rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_fastapi.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_flask.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_httpx.py
--rw-r--r--   0        0        0    44176 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_openai.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_psycopg.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_requests.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_sqlalchemy.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_starlette.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/test_wsgi.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/__init__.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/models.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.33.0/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.33.0/LICENSE
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.33.0/README.md
--rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.33.0/pyproject.toml
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.33.0/PKG-INFO
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 logfire-0.34.0/Makefile
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/__main__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/cli.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/exceptions.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/propagate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/py.typed
+-rw-r--r--   0        0        0     9570 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/testing.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/version.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/__init__.py
+-rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/ast_utils.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/async_.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/auth.py
+-rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/backfill.py
+-rw-r--r--   0        0        0    18512 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/cli.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/collect_system_info.py
+-rw-r--r--   0        0        0    56181 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/config.py
+-rw-r--r--   0        0        0    11225 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/config_params.py
+-rw-r--r--   0        0        0     5501 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/constants.py
+-rw-r--r--   0        0        0    19127 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/formatter.py
+-rw-r--r--   0        0        0     5716 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/instrument.py
+-rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/json_encoder.py
+-rw-r--r--   0        0        0    11646 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/json_formatter.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/json_schema.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/json_types.py
+-rw-r--r--   0        0        0    59310 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/main.py
+-rw-r--r--   0        0        0    13153 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/metrics.py
+-rw-r--r--   0        0        0     8756 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/scrubbing.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/stack_info.py
+-rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/tracer.py
+-rw-r--r--   0        0        0     6384 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/utils.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/auto_trace/__init__.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/auto_trace/import_hook.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/auto_trace/rewrite_ast.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/auto_trace/types.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/__init__.py
+-rw-r--r--   0        0        0    18968 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/console.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/fallback.py
+-rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/file.py
+-rw-r--r--   0        0        0     4035 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/otlp.py
+-rw-r--r--   0        0        0     9014 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/processor_wrapper.py
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/remove_pending.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/exporters/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/asyncpg.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/executors.py
+-rw-r--r--   0        0        0    10599 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/fastapi.py
+-rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/psycopg.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/llm_providers/anthropic.py
+-rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/llm_providers/llm_provider.py
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/llm_providers/openai.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/_internal/integrations/llm_providers/types.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/integrations/__init__.py
+-rw-r--r--   0        0        0     4707 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/integrations/logging.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/integrations/loguru.py
+-rw-r--r--   0        0        0    19169 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/integrations/pydantic.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 logfire-0.34.0/logfire/integrations/structlog.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/__init__.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/conftest.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/module_used_for_tests.py
+-rw-r--r--   0        0        0    19034 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_auto_trace.py
+-rw-r--r--   0        0        0     9988 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_backfill.py
+-rw-r--r--   0        0        0    47077 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_cli.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_collect_package_resources.py
+-rw-r--r--   0        0        0    53700 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_configure.py
+-rw-r--r--   0        0        0    29388 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_console_exporter.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_formatter.py
+-rw-r--r--   0        0        0    45893 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_json_args.py
+-rw-r--r--   0        0        0    19936 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_json_args_formatting.py
+-rw-r--r--   0        0        0   105498 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_logfire.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_loguru.py
+-rw-r--r--   0        0        0    11914 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_metrics.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_no_production.py
+-rw-r--r--   0        0        0    54162 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_pydantic_plugin.py
+-rw-r--r--   0        0        0     7061 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_sampling.py
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_secret_scrubbing.py
+-rw-r--r--   0        0        0     7270 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_slow_async_callbacks.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_source_code_extraction.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_stdlib_logging.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_structlog.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_testing.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/auto_trace_samples/__init__.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/auto_trace_samples/foo.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/auto_trace_samples/simple_nesting.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/exporters/test_fallback_exporter.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/exporters/test_file_exporter.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/exporters/test_otlp_session.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/exporters/test_remove_pending.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/exporters/test_retry_fewer_spans.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/import_used_for_tests/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/import_used_for_tests/slow_async_callbacks_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/import_used_for_tests/a/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/import_used_for_tests/a/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/__init__.py
+-rw-r--r--   0        0        0    24476 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_anthropic.py
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_asgi.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_asyncpg.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_django.py
+-rw-r--r--   0        0        0    44449 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_fastapi.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_flask.py
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_httpx.py
+-rw-r--r--   0        0        0    44469 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_openai.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_psycopg.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_requests.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_sqlalchemy.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_starlette.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/test_wsgi.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/__init__.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/admin.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/apps.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/models.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/urls.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_app/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_site/__init__.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_site/settings.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_site/urls.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_site/wsgi.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 logfire-0.34.0/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 logfire-0.34.0/LICENSE
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 logfire-0.34.0/README.md
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 logfire-0.34.0/pyproject.toml
+-rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 logfire-0.34.0/PKG-INFO
```

### Comparing `logfire-0.33.0/Makefile` & `logfire-0.34.0/Makefile`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/__init__.py` & `logfire-0.34.0/logfire/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/propagate.py` & `logfire-0.34.0/logfire/propagate.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/testing.py` & `logfire-0.34.0/logfire/testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/ast_utils.py` & `logfire-0.34.0/logfire/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/async_.py` & `logfire-0.34.0/logfire/_internal/async_.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/auth.py` & `logfire-0.34.0/logfire/_internal/auth.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/backfill.py` & `logfire-0.34.0/logfire/_internal/backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/cli.py` & `logfire-0.34.0/logfire/_internal/cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/config.py` & `logfire-0.34.0/logfire/_internal/config.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/config_params.py` & `logfire-0.34.0/logfire/_internal/config_params.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/constants.py` & `logfire-0.34.0/logfire/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/formatter.py` & `logfire-0.34.0/logfire/_internal/formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/instrument.py` & `logfire-0.34.0/logfire/_internal/instrument.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/json_encoder.py` & `logfire-0.34.0/logfire/_internal/json_encoder.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/json_formatter.py` & `logfire-0.34.0/logfire/_internal/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/json_schema.py` & `logfire-0.34.0/logfire/_internal/json_schema.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/json_types.py` & `logfire-0.34.0/logfire/_internal/json_types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/main.py` & `logfire-0.34.0/logfire/_internal/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -818,15 +818,22 @@
             app,
             request_attributes_mapper=request_attributes_mapper,
             excluded_urls=excluded_urls,
             use_opentelemetry_instrumentation=use_opentelemetry_instrumentation,
         )
 
     def instrument_openai(
-        self, openai_client: openai.OpenAI | openai.AsyncOpenAI, *, suppress_other_instrumentation: bool = True
+        self,
+        openai_client: openai.OpenAI
+        | openai.AsyncOpenAI
+        | type[openai.OpenAI]
+        | type[openai.AsyncOpenAI]
+        | None = None,
+        *,
+        suppress_other_instrumentation: bool = True,
     ) -> ContextManager[None]:
         """Instrument an OpenAI client so that spans are automatically created for each request.
 
         The following methods are instrumented for both the sync and the async clients:
 
         - [`client.chat.completions.create`](https://platform.openai.com/docs/guides/text-generation/chat-completions-api) — with and without `stream=True`
         - [`client.completions.create`](https://platform.openai.com/docs/guides/text-generation/completions-api) — with and without `stream=True`
@@ -851,48 +858,62 @@
                 {'role': 'user', 'content': 'What is four plus five?'},
             ],
         )
         print('answer:', response.choices[0].message.content)
         ```
 
         Args:
-            openai_client: The OpenAI client to instrument, either `openai.OpenAI` or `openai.AsyncOpenAI`.
+            openai_client: The OpenAI client or class to instrument:
+
+                - `None` (the default) to instrument both the `openai.OpenAI` and `openai.AsyncOpenAI` classes.
+                - The `openai.OpenAI` class or a subclass
+                - The `openai.AsyncOpenAI` class or a subclass
+                - An instance of `openai.OpenAI`
+                - An instance of `openai.AsyncOpenAI`
+
             suppress_other_instrumentation: If True, suppress any other OTEL instrumentation that may be otherwise
                 enabled. In reality, this means the HTTPX instrumentation, which could otherwise be called since
                 OpenAI uses HTTPX to make HTTP requests.
 
         Returns:
             A context manager that will revert the instrumentation when exited.
                 Use of this context manager is optional.
         """
+        import openai
+
         from .integrations.llm_providers.llm_provider import instrument_llm_provider
         from .integrations.llm_providers.openai import get_endpoint_config, is_async_client, on_response
 
         return instrument_llm_provider(
             self,
-            openai_client,
+            openai_client or (openai.OpenAI, openai.AsyncOpenAI),
             suppress_other_instrumentation,
             'OpenAI',
             get_endpoint_config,
             on_response,
             is_async_client,
         )
 
     def instrument_anthropic(
         self,
-        anthropic_client: anthropic.Anthropic | anthropic.AsyncAnthropic,
+        anthropic_client: anthropic.Anthropic
+        | anthropic.AsyncAnthropic
+        | type[anthropic.Anthropic]
+        | type[anthropic.AsyncAnthropic]
+        | None = None,
         *,
         suppress_other_instrumentation: bool = True,
     ) -> ContextManager[None]:
         """Instrument an Anthropic client so that spans are automatically created for each request.
 
         The following methods are instrumented for both the sync and the async clients:
 
-        - [`client.messages.create`](https://docs.anthropic.com/claude/reference/messages_post) — with and without `stream=True`
-        - [`client.beta.tools.messages.create`](https://docs.anthropic.com/claude/docs/tool-use-examples) — with and without `stream=True`
+        - [`client.messages.create`](https://docs.anthropic.com/en/api/messages)
+        - [`client.messages.stream`](https://docs.anthropic.com/en/api/messages-streaming)
+        - [`client.beta.tools.messages.create`](https://docs.anthropic.com/en/docs/tool-use)
 
         When `stream=True` a second span is created to instrument the streamed response.
 
         Example usage:
 
         ```python
         import logfire
@@ -908,29 +929,39 @@
                 {'role': 'user', 'content': 'What is four plus five?'},
             ],
         )
         print('answer:', response.content[0].text)
         ```
 
         Args:
-            anthropic_client: The Anthropic client to instrument, either `anthropic.Anthropic` or `anthropic.AsyncAnthropic`.
+            anthropic_client: The Anthropic client or class to instrument:
+
+                - `None` (the default) to instrument both the
+                    `anthropic.Anthropic` and `anthropic.AsyncAnthropic` classes.
+                - The `anthropic.Anthropic` class or a subclass
+                - The `anthropic.AsyncAnthropic` class or a subclass
+                - An instance of `anthropic.Anthropic`
+                - An instance of `anthropic.AsyncAnthropic`
+
             suppress_other_instrumentation: If True, suppress any other OTEL instrumentation that may be otherwise
                 enabled. In reality, this means the HTTPX instrumentation, which could otherwise be called since
                 OpenAI uses HTTPX to make HTTP requests.
 
         Returns:
             A context manager that will revert the instrumentation when exited.
                 Use of this context manager is optional.
         """
+        import anthropic
+
         from .integrations.llm_providers.anthropic import get_endpoint_config, is_async_client, on_response
         from .integrations.llm_providers.llm_provider import instrument_llm_provider
 
         return instrument_llm_provider(
             self,
-            anthropic_client,
+            anthropic_client or (anthropic.Anthropic, anthropic.AsyncAnthropic),
             suppress_other_instrumentation,
             'Anthropic',
             get_endpoint_config,
             on_response,
             is_async_client,
         )
```

### Comparing `logfire-0.33.0/logfire/_internal/metrics.py` & `logfire-0.34.0/logfire/_internal/metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/scrubbing.py` & `logfire-0.34.0/logfire/_internal/scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/stack_info.py` & `logfire-0.34.0/logfire/_internal/stack_info.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/tracer.py` & `logfire-0.34.0/logfire/_internal/tracer.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/utils.py` & `logfire-0.34.0/logfire/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/auto_trace/__init__.py` & `logfire-0.34.0/logfire/_internal/auto_trace/__init__.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/auto_trace/import_hook.py` & `logfire-0.34.0/logfire/_internal/auto_trace/import_hook.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/auto_trace/rewrite_ast.py` & `logfire-0.34.0/logfire/_internal/auto_trace/rewrite_ast.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/auto_trace/types.py` & `logfire-0.34.0/logfire/_internal/auto_trace/types.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/console.py` & `logfire-0.34.0/logfire/_internal/exporters/console.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/fallback.py` & `logfire-0.34.0/logfire/_internal/exporters/fallback.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/file.py` & `logfire-0.34.0/logfire/_internal/exporters/file.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/otlp.py` & `logfire-0.34.0/logfire/_internal/exporters/otlp.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/processor_wrapper.py` & `logfire-0.34.0/logfire/_internal/exporters/processor_wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/remove_pending.py` & `logfire-0.34.0/logfire/_internal/exporters/remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/exporters/wrapper.py` & `logfire-0.34.0/logfire/_internal/exporters/wrapper.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/integrations/executors.py` & `logfire-0.34.0/logfire/_internal/integrations/executors.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/integrations/fastapi.py` & `logfire-0.34.0/logfire/_internal/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/integrations/psycopg.py` & `logfire-0.34.0/logfire/_internal/integrations/psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/_internal/integrations/llm_providers/anthropic.py` & `logfire-0.34.0/logfire/_internal/integrations/llm_providers/anthropic.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,13 +64,13 @@
                 }
                 for block in response.content
             ]
         span.set_attribute('response_data', {'message': message, 'usage': response.usage})
     return response
 
 
-def is_async_client(client: anthropic.Anthropic | anthropic.AsyncAnthropic):
-    """Returns whether or not `client` is async."""
-    if isinstance(client, anthropic.Anthropic):
+def is_async_client(client: type[anthropic.Anthropic] | type[anthropic.AsyncAnthropic]):
+    """Returns whether or not the `client` class is async."""
+    if issubclass(client, anthropic.Anthropic):
         return False
-    assert isinstance(client, anthropic.AsyncAnthropic), f'Unexpected Anthropic or AsyncAnthropic type, got: {client}'
+    assert issubclass(client, anthropic.AsyncAnthropic), f'Expected Anthropic or AsyncAnthropic type, got: {client}'
     return True
```

### Comparing `logfire-0.33.0/logfire/_internal/integrations/llm_providers/llm_provider.py` & `logfire-0.34.0/logfire/_internal/integrations/llm_providers/llm_provider.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
-from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, ContextManager, Iterator
+from collections.abc import Iterable
+from contextlib import ExitStack, contextmanager, nullcontext
+from typing import TYPE_CHECKING, Any, AsyncIterator, Callable, ContextManager, Iterator, cast
 
 from opentelemetry import context
 
 from ...constants import ONE_SECOND_IN_NANOSECONDS
 
 if TYPE_CHECKING:
     from ...main import Logfire, LogfireSpan
@@ -18,23 +19,63 @@
 def instrument_llm_provider(
     logfire: Logfire,
     client: Any,
     suppress_otel: bool,
     scope_suffix: str,
     get_endpoint_config_fn: Callable[[Any], EndpointConfig],
     on_response_fn: Callable[[Any, LogfireSpan], Any],
-    is_async_client_fn: Callable[[Any], bool],
+    is_async_client_fn: Callable[[type[Any]], bool],
 ) -> ContextManager[None]:
-    """Instruments the provided `client` with `logfire`."""
+    """Instruments the provided `client` (or clients) with `logfire`.
+
+    The `client` argument can be:
+    - a single client instance, e.g. an instance of `openai.OpenAI`,
+    - a class of a client, or
+    - an iterable of clients/classes.
+
+    Returns:
+        A context manager that will revert the instrumentation when exited.
+            Use of this context manager is optional.
+    """
+    if isinstance(client, Iterable):
+        # Eagerly instrument each client, but only open the returned context managers
+        # in another context manager which the user needs to open if they want.
+        # Otherwise the garbage collector will close them and uninstrument.
+        context_managers = [
+            instrument_llm_provider(
+                logfire,
+                c,
+                suppress_otel,
+                scope_suffix,
+                get_endpoint_config_fn,
+                on_response_fn,
+                is_async_client_fn,
+            )
+            for c in cast('Iterable[Any]', client)
+        ]
+
+        @contextmanager
+        def uninstrument_context():
+            with ExitStack() as exit_stack:
+                for context_manager in context_managers:
+                    exit_stack.enter_context(context_manager)
+                yield
+
+        return uninstrument_context()
+
+    if getattr(client, '_is_instrumented_by_logfire', False):
+        # Do nothing if already instrumented.
+        return nullcontext()
+
     logfire_llm = logfire.with_settings(custom_scope_suffix=scope_suffix.lower(), tags=['LLM'])
 
     client._is_instrumented_by_logfire = True
     client._original_request_method = original_request_method = client._request
 
-    is_async = is_async_client_fn(client)
+    is_async = is_async_client_fn(client if isinstance(client, type) else type(client))
 
     def _instrumentation_setup(**kwargs: Any) -> Any:
         if context.get_value('suppress_instrumentation'):
             return None, None, kwargs
 
         options = kwargs['options']
         try:
@@ -72,38 +113,41 @@
                                 record_chunk(chunk)
                                 yield chunk
 
                 kwargs['stream_cls'] = LogfireInstrumentedStream
 
         return message_template, span_data, kwargs
 
-    def instrumented_llm_request_sync(**kwargs: Any) -> Any:
+    # In these methods, `*args` is only expected to be `(self,)`
+    # in the case where we instrument classes rather than client instances.
+
+    def instrumented_llm_request_sync(*args: Any, **kwargs: Any) -> Any:
         message_template, span_data, kwargs = _instrumentation_setup(**kwargs)
         if message_template is None:
-            return original_request_method(**kwargs)
+            return original_request_method(*args, **kwargs)
         stream = kwargs['stream']
         with logfire_llm.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
-                    return original_request_method(**kwargs)
+                    return original_request_method(*args, **kwargs)
                 else:
-                    response = on_response_fn(original_request_method(**kwargs), span)
+                    response = on_response_fn(original_request_method(*args, **kwargs), span)
                     return response
 
-    async def instrumented_llm_request_async(**kwargs: Any) -> Any:
+    async def instrumented_llm_request_async(*args: Any, **kwargs: Any) -> Any:
         message_template, span_data, kwargs = _instrumentation_setup(**kwargs)
         if message_template is None:
-            return await original_request_method(**kwargs)
+            return await original_request_method(*args, **kwargs)
         stream = kwargs['stream']
         with logfire_llm.span(message_template, **span_data) as span:
             with maybe_suppress_instrumentation(suppress_otel):
                 if stream:
-                    return await original_request_method(**kwargs)
+                    return await original_request_method(*args, **kwargs)
                 else:
-                    response = on_response_fn(await original_request_method(**kwargs), span)
+                    response = on_response_fn(await original_request_method(*args, **kwargs), span)
                     return response
 
     if is_async:
         client._request = instrumented_llm_request_async
     else:
         client._request = instrumented_llm_request_sync
 
@@ -114,15 +158,15 @@
         The user isn't required (or even expected) to use this context manager,
         which is why the instrumenting has already happened before.
         It exists mostly for tests and just in case users want it.
         """
         try:
             yield
         finally:
-            client._request = client._original_request_method
+            client._request = client._original_request_method  # type: ignore
             del client._original_request_method
             client._is_instrumented_by_logfire = False
 
     return uninstrument_context()
 
 
 @contextmanager
```

### Comparing `logfire-0.33.0/logfire/_internal/integrations/llm_providers/openai.py` & `logfire-0.34.0/logfire/_internal/integrations/llm_providers/openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,13 +95,13 @@
     elif isinstance(response, CreateEmbeddingResponse):
         span.set_attribute('response_data', {'usage': response.usage})
     elif isinstance(response, ImagesResponse):  # pragma: no branch
         span.set_attribute('response_data', {'images': response.data})
     return response
 
 
-def is_async_client(client: openai.OpenAI | openai.AsyncOpenAI):
-    """Returns whether or not `client` is async."""
-    if isinstance(client, openai.OpenAI):
+def is_async_client(client: type[openai.OpenAI] | type[openai.AsyncOpenAI]):
+    """Returns whether or not the `client` class is async."""
+    if issubclass(client, openai.OpenAI):
         return False
-    assert isinstance(client, openai.AsyncOpenAI), f'Unexpected OpenAI or AsyncOpenAI type, got: {client}'
+    assert issubclass(client, openai.AsyncOpenAI), f'Expected OpenAI or AsyncOpenAI type, got: {client}'
     return True
```

### Comparing `logfire-0.33.0/logfire/integrations/logging.py` & `logfire-0.34.0/logfire/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/integrations/loguru.py` & `logfire-0.34.0/logfire/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/integrations/pydantic.py` & `logfire-0.34.0/logfire/integrations/pydantic.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/logfire/integrations/structlog.py` & `logfire-0.34.0/logfire/integrations/structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/conftest.py` & `logfire-0.34.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_auto_trace.py` & `logfire-0.34.0/tests/test_auto_trace.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_backfill.py` & `logfire-0.34.0/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_cli.py` & `logfire-0.34.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_collect_package_resources.py` & `logfire-0.34.0/tests/test_collect_package_resources.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_configure.py` & `logfire-0.34.0/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_console_exporter.py` & `logfire-0.34.0/tests/test_console_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_formatter.py` & `logfire-0.34.0/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_json_args.py` & `logfire-0.34.0/tests/test_json_args.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_json_args_formatting.py` & `logfire-0.34.0/tests/test_json_args_formatting.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_logfire.py` & `logfire-0.34.0/tests/test_logfire.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_loguru.py` & `logfire-0.34.0/tests/test_loguru.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_metrics.py` & `logfire-0.34.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_no_production.py` & `logfire-0.34.0/tests/test_no_production.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_pydantic_plugin.py` & `logfire-0.34.0/tests/test_pydantic_plugin.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_sampling.py` & `logfire-0.34.0/tests/test_sampling.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_secret_scrubbing.py` & `logfire-0.34.0/tests/test_secret_scrubbing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_slow_async_callbacks.py` & `logfire-0.34.0/tests/test_slow_async_callbacks.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_source_code_extraction.py` & `logfire-0.34.0/tests/test_source_code_extraction.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_stdlib_logging.py` & `logfire-0.34.0/tests/test_stdlib_logging.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_structlog.py` & `logfire-0.34.0/tests/test_structlog.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_testing.py` & `logfire-0.34.0/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/test_utils.py` & `logfire-0.34.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/utils.py` & `logfire-0.34.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/exporters/test_fallback_exporter.py` & `logfire-0.34.0/tests/exporters/test_fallback_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/exporters/test_file_exporter.py` & `logfire-0.34.0/tests/exporters/test_file_exporter.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/exporters/test_otlp_session.py` & `logfire-0.34.0/tests/exporters/test_otlp_session.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/exporters/test_remove_pending.py` & `logfire-0.34.0/tests/exporters/test_remove_pending.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/exporters/test_retry_fewer_spans.py` & `logfire-0.34.0/tests/exporters/test_retry_fewer_spans.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/import_used_for_tests/slow_async_callbacks_example.py` & `logfire-0.34.0/tests/import_used_for_tests/slow_async_callbacks_example.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_anthropic.py` & `logfire-0.34.0/tests/otel_integrations/test_anthropic.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,16 @@
 
 @pytest.fixture
 async def instrumented_async_client() -> AsyncIterator[anthropic.AsyncAnthropic]:
     async with httpx.AsyncClient(transport=MockTransport(request_handler)) as httpx_client:
         # use a hardcoded API key to make sure one in the environment is never used
         anthropic_client = anthropic.AsyncAnthropic(api_key='foobar', http_client=httpx_client)
 
-        with logfire.instrument_anthropic(anthropic_client):
+        # Test instrumenting EVERYTHING
+        with logfire.instrument_anthropic():
             yield anthropic_client
 
 
 def test_sync_messages(instrumented_client: anthropic.Anthropic, exporter: TestExporter) -> None:
     response = instrumented_client.messages.create(
         max_tokens=1000,
         model='claude-3-haiku-20240307',
```

### Comparing `logfire-0.33.0/tests/otel_integrations/test_asgi.py` & `logfire-0.34.0/tests/otel_integrations/test_asgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_asyncpg.py` & `logfire-0.34.0/tests/otel_integrations/test_asyncpg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_django.py` & `logfire-0.34.0/tests/otel_integrations/test_django.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_fastapi.py` & `logfire-0.34.0/tests/otel_integrations/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_flask.py` & `logfire-0.34.0/tests/otel_integrations/test_flask.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_httpx.py` & `logfire-0.34.0/tests/otel_integrations/test_httpx.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_openai.py` & `logfire-0.34.0/tests/otel_integrations/test_openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,22 @@
 
 @pytest.fixture
 def instrumented_client() -> Iterator[openai.Client]:
     with httpx.Client(transport=MockTransport(request_handler)) as httpx_client:
         # use a hardcoded API key to make sure one in the environment is never used
         openai_client = openai.Client(api_key='foobar', http_client=httpx_client)
 
-        with logfire.instrument_openai(openai_client):
+        # Test instrumenting a class
+        with logfire.instrument_openai(openai.Client):
+            # Test repeatedly instrumenting something already instrumented (should do nothing)
+            with logfire.instrument_openai(openai.Client):
+                pass
+            with logfire.instrument_openai(openai_client):
+                pass
+
             yield openai_client
 
 
 @pytest.fixture
 async def instrumented_async_client() -> AsyncIterator[openai.AsyncClient]:
     async with httpx.AsyncClient(transport=MockTransport(request_handler)) as httpx_client:
         # use a hardcoded API key to make sure one in the environment is never used
```

### Comparing `logfire-0.33.0/tests/otel_integrations/test_psycopg.py` & `logfire-0.34.0/tests/otel_integrations/test_psycopg.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_requests.py` & `logfire-0.34.0/tests/otel_integrations/test_requests.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_sqlalchemy.py` & `logfire-0.34.0/tests/otel_integrations/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_starlette.py` & `logfire-0.34.0/tests/otel_integrations/test_starlette.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/test_wsgi.py` & `logfire-0.34.0/tests/otel_integrations/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/django_test_project/manage.py` & `logfire-0.34.0/tests/otel_integrations/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/tests/otel_integrations/django_test_project/django_test_site/settings.py` & `logfire-0.34.0/tests/otel_integrations/django_test_project/django_test_site/settings.py`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/LICENSE` & `logfire-0.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/README.md` & `logfire-0.34.0/README.md`

 * *Files identical despite different names*

### Comparing `logfire-0.33.0/pyproject.toml` & `logfire-0.34.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "logfire"
-version = "0.33.0"
+version = "0.34.0"
 description = "The best Python observability tool! 🪵🔥"
 authors = [
     { name = "Pydantic Team", email = "engineering@pydantic.dev" },
     { name = "Samuel Colvin", email = "samuel@pydantic.dev" },
     { name = "Hasan Ramezani", email = "hasan@pydantic.dev" },
     { name = "Adrian Garcia Badaracco", email = "adrian@pydantic.dev" },
     { name = "David Montague", email = "david@pydantic.dev" },
```

### Comparing `logfire-0.33.0/PKG-INFO` & `logfire-0.34.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: logfire
-Version: 0.33.0
+Version: 0.34.0
 Summary: The best Python observability tool! 🪵🔥
 Author-email: Pydantic Team <engineering@pydantic.dev>, Samuel Colvin <samuel@pydantic.dev>, Hasan Ramezani <hasan@pydantic.dev>, Adrian Garcia Badaracco <adrian@pydantic.dev>, David Montague <david@pydantic.dev>, Marcelo Trylesinski <marcelo@pydantic.dev>, David Hewitt <david.hewitt@pydantic.dev>, Alex Hall <alex@pydantic.dev>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

