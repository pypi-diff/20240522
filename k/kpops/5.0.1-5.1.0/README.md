# Comparing `tmp/kpops-5.0.1.tar.gz` & `tmp/kpops-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-5.0.1.tar", max compression
+gzip compressed data, was "kpops-5.1.0.tar", max compression
```

## Comparing `kpops-5.0.1.tar` & `kpops-5.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1064 2024-05-15 09:41:48.275024 kpops-5.0.1/LICENSE
--rw-r--r--   0        0        0     2675 2024-05-15 09:41:48.275024 kpops-5.0.1/README.md
--rw-r--r--   0        0        0      250 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      124 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/exception.py
--rw-r--r--   0        0        0    16061 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/main.py
--rw-r--r--   0        0        0      101 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/options.py
--rw-r--r--   0        0        0     2512 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/cli/registry.py
--rw-r--r--   0        0        0      699 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0     1168 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py
--rw-r--r--   0        0        0       92 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     8950 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2125 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     7072 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      974 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     7434 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      229 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     4839 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     3543 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      797 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kubernetes/__init__.py
--rw-r--r--   0        0        0      841 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kubernetes/model.py
--rw-r--r--   0        0        0     1799 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kubernetes/pvc_handler.py
--rw-r--r--   0        0        0     1116 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/kubernetes/utils.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6872 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      491 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      225 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9534 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2420 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     7389 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      906 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0    10674 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     1061 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/cleaner.py
--rw-r--r--   0        0        0     7237 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/helm_app.py
--rw-r--r--   0        0        0     4748 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0     9178 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     1828 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0      149 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     1882 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0      217 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/models/resource.py
--rw-r--r--   0        0        0      994 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0     3801 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/models/topic.py
--rw-r--r--   0        0        0     8324 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0     1031 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0      595 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2873 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0    10245 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     4178 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0     5299 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/config.py
--rw-r--r--   0        0        0    15340 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/pipeline.py
--rw-r--r--   0        0        0      278 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/__init__.py
--rw-r--r--   0        0        0     3060 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/cli_commands.py
--rw-r--r--   0        0        0      375 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3178 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     4996 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/dict_ops.py
--rw-r--r--   0        0        0     2431 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/docstring.py
--rw-r--r--   0        0        0     1176 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/environment.py
--rw-r--r--   0        0        0     5924 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      298 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/json.py
--rw-r--r--   0        0        0     6533 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/pydantic.py
--rw-r--r--   0        0        0      238 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/types.py
--rw-r--r--   0        0        0     4332 2024-05-15 09:41:48.283024 kpops-5.0.1/kpops/utils/yaml.py
--rw-r--r--   0        0        0     7443 2024-05-15 09:41:48.287024 kpops-5.0.1/pyproject.toml
--rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kpops-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-22 08:41:53.709716 kpops-5.1.0/LICENSE
+-rw-r--r--   0        0        0     2675 2024-05-22 08:41:53.709716 kpops-5.1.0/README.md
+-rw-r--r--   0        0        0      250 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      124 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/exception.py
+-rw-r--r--   0        0        0    16061 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/main.py
+-rw-r--r--   0        0        0      101 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/options.py
+-rw-r--r--   0        0        0     2512 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/cli/registry.py
+-rw-r--r--   0        0        0      699 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0     1168 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py
+-rw-r--r--   0        0        0       92 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     8950 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2125 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     7072 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      974 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     7434 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      229 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     4839 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     3543 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      797 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kubernetes/__init__.py
+-rw-r--r--   0        0        0      841 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kubernetes/model.py
+-rw-r--r--   0        0        0     1799 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kubernetes/pvc_handler.py
+-rw-r--r--   0        0        0     1116 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/kubernetes/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6872 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      491 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      225 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9534 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2420 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     7389 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      906 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0    10674 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     1061 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/cleaner.py
+-rw-r--r--   0        0        0     7293 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/helm_app.py
+-rw-r--r--   0        0        0     4748 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0     9178 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     1828 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0      149 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0      217 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/models/resource.py
+-rw-r--r--   0        0        0      994 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0     3801 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/models/topic.py
+-rw-r--r--   0        0        0     8324 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0     1031 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0      595 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2873 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0    10245 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     4178 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0     5299 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/config.py
+-rw-r--r--   0        0        0    15340 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/pipeline.py
+-rw-r--r--   0        0        0      278 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/__init__.py
+-rw-r--r--   0        0        0     3060 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/cli_commands.py
+-rw-r--r--   0        0        0      375 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3178 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     4996 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/dict_ops.py
+-rw-r--r--   0        0        0     2431 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1176 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5924 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      298 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/json.py
+-rw-r--r--   0        0        0     6533 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0      238 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/types.py
+-rw-r--r--   0        0        0     4332 2024-05-22 08:41:53.717716 kpops-5.1.0/kpops/utils/yaml.py
+-rw-r--r--   0        0        0     7443 2024-05-22 08:41:53.721716 kpops-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4326 1970-01-01 00:00:00.000000 kpops-5.1.0/PKG-INFO
```

### Comparing `kpops-5.0.1/LICENSE` & `kpops-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/README.md` & `kpops-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/cli/custom_formatter.py` & `kpops-5.1.0/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/cli/main.py` & `kpops-5.1.0/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/cli/registry.py` & `kpops-5.1.0/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/__init__.py` & `kpops-5.1.0/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/helm_wrapper/dry_run_handler.py` & `kpops-5.1.0/kpops/component_handlers/helm_wrapper/dry_run_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-5.1.0/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-5.1.0/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/helm_wrapper/model.py` & `kpops-5.1.0/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-5.1.0/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-5.1.0/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-5.1.0/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kafka_connect/model.py` & `kpops-5.1.0/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-5.1.0/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kubernetes/model.py` & `kpops-5.1.0/kpops/component_handlers/kubernetes/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kubernetes/pvc_handler.py` & `kpops-5.1.0/kpops/component_handlers/kubernetes/pvc_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/kubernetes/utils.py` & `kpops-5.1.0/kpops/component_handlers/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-5.1.0/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/topic/handler.py` & `kpops-5.1.0/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/topic/model.py` & `kpops-5.1.0/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-5.1.0/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/topic/utils.py` & `kpops-5.1.0/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/component_handlers/utils/exception.py` & `kpops-5.1.0/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/__init__.py` & `kpops-5.1.0/kpops/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/base_defaults_component.py` & `kpops-5.1.0/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/cleaner.py` & `kpops-5.1.0/kpops/components/base_components/cleaner.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/helm_app.py` & `kpops-5.1.0/kpops/components/base_components/helm_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import logging
 from functools import cached_property
 from typing import Annotated, Any
 
 import pydantic
-from pydantic import Field, SerializationInfo, model_serializer
+from pydantic import Field, SerializationInfo, computed_field, model_serializer
 from typing_extensions import override
 
 from kpops.component_handlers.helm_wrapper.dry_run_handler import DryRunHandler
 from kpops.component_handlers.helm_wrapper.helm import Helm
 from kpops.component_handlers.helm_wrapper.helm_diff import HelmDiff
 from kpops.component_handlers.helm_wrapper.model import (
     HelmFlags,
@@ -99,19 +99,21 @@
         return HelmDiff(self.config.helm_diff_config)
 
     @cached_property
     def dry_run_handler(self) -> DryRunHandler:
         helm_diff = HelmDiff(self.config.helm_diff_config)
         return DryRunHandler(self.helm, helm_diff, self.namespace)
 
+    @computed_field
     @property
     def helm_release_name(self) -> str:
         """The name for the Helm release."""
         return create_helm_release_name(self.full_name)
 
+    @computed_field
     @property
     def helm_name_override(self) -> str:
         """Helm chart name override."""
         return create_helm_name_override(self.full_name)
 
     @property
     def helm_chart(self) -> str:
```

### Comparing `kpops-5.0.1/kpops/components/base_components/kafka_app.py` & `kpops-5.1.0/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/kafka_connector.py` & `kpops-5.1.0/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/kubernetes_app.py` & `kpops-5.1.0/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/models/from_section.py` & `kpops-5.1.0/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/models/to_section.py` & `kpops-5.1.0/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/models/topic.py` & `kpops-5.1.0/kpops/components/base_components/models/topic.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/base_components/pipeline_component.py` & `kpops-5.1.0/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/streams_bootstrap/__init__.py` & `kpops-5.1.0/kpops/components/streams_bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/streams_bootstrap/producer/model.py` & `kpops-5.1.0/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-5.1.0/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/streams_bootstrap/streams/model.py` & `kpops-5.1.0/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-5.1.0/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/config.py` & `kpops-5.1.0/kpops/config.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/pipeline.py` & `kpops-5.1.0/kpops/pipeline.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/cli_commands.py` & `kpops-5.1.0/kpops/utils/cli_commands.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/dict_differ.py` & `kpops-5.1.0/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/dict_ops.py` & `kpops-5.1.0/kpops/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/docstring.py` & `kpops-5.1.0/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/environment.py` & `kpops-5.1.0/kpops/utils/environment.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/gen_schema.py` & `kpops-5.1.0/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/pydantic.py` & `kpops-5.1.0/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/kpops/utils/yaml.py` & `kpops-5.1.0/kpops/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `kpops-5.0.1/pyproject.toml` & `kpops-5.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "5.0.1"
+version = "5.1.0"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-5.0.1/PKG-INFO` & `kpops-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 5.0.1
+Version: 5.1.0
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<3.13
```

