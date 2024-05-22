# Comparing `tmp/spice_rack-0.8.0.tar.gz` & `tmp/spice_rack-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spice_rack-0.8.0.tar", max compression
+gzip compressed data, was "spice_rack-0.9.0.tar", max compression
```

## Comparing `spice_rack-0.8.0.tar` & `spice_rack-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     2750 2024-04-10 14:00:46.489874 spice_rack-0.8.0/README.md
--rw-r--r--   0        0        0     3119 2024-04-10 14:01:07.170162 spice_rack-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      534 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/__init__.py
--rw-r--r--   0        0        0      104 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_api_helpers/__init__.py
--rw-r--r--   0        0        0     1757 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_api_helpers/_uvicorn_startup_config.py
--rw-r--r--   0        0        0      573 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/__init__.py
--rw-r--r--   0        0        0     5289 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_base_base.py
--rw-r--r--   0        0        0    12392 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_dispatchable.py
--rw-r--r--   0        0        0      294 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/_error_info.py
--rw-r--r--   0        0        0     6767 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/_exception_base.py
--rw-r--r--   0        0        0      778 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/_exception_exception.py
--rw-r--r--   0        0        0     1145 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/_external_wrapper.py
--rw-r--r--   0        0        0     5359 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_exception/_http.py
--rw-r--r--   0        0        0      157 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_mixins/__init__.py
--rw-r--r--   0        0        0      442 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_mixins/_guid_mixin.py
--rw-r--r--   0        0        0      628 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_mixins/_mixin_base.py
--rw-r--r--   0        0        0     1637 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_mixins/_timestamped.py
--rw-r--r--   0        0        0     4362 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_root.py
--rw-r--r--   0        0        0      108 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/__init__.py
--rw-r--r--   0        0        0     4414 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/_base.py
--rw-r--r--   0        0        0      126 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/__init__.py
--rw-r--r--   0        0        0      408 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/_base.py
--rw-r--r--   0        0        0     2067 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/_dot_env_ext.py
--rw-r--r--   0        0        0     2067 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py
--rw-r--r--   0        0        0     4874 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_special_str.py
--rw-r--r--   0        0        0      446 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_bases/_value_model.py
--rw-r--r--   0        0        0      316 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_common_validators/__init__.py
--rw-r--r--   0        0        0     5834 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_common_validators/_mutually_exclusive_fields.py
--rw-r--r--   0        0        0      114 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/__init__.py
--rw-r--r--   0        0        0    17738 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_base.py
--rw-r--r--   0        0        0      277 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/__init__.py
--rw-r--r--   0        0        0     1501 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_dupe_keys.py
--rw-r--r--   0        0        0     1835 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_item_ix_invalid.py
--rw-r--r--   0        0        0     1364 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_key_already_exists.py
--rw-r--r--   0        0        0     1510 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_missing_key.py
--rw-r--r--   0        0        0      327 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/__init__.py
--rw-r--r--   0        0        0     5557 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_exceptions.py
--rw-r--r--   0        0        0     3377 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_info.py
--rw-r--r--   0        0        0      464 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/__init__.py
--rw-r--r--   0        0        0    13876 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_base.py
--rw-r--r--   0        0        0      498 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_fs_inference.py
--rw-r--r--   0        0        0     3462 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py
--rw-r--r--   0        0        0      752 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_local.py
--rw-r--r--   0        0        0     6385 2024-04-10 14:00:46.493874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py
--rw-r--r--   0        0        0      438 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/__init__.py
--rw-r--r--   0        0        0     6564 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_base.py
--rw-r--r--   0        0        0     5108 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_constraints.py
--rw-r--r--   0        0        0     2936 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_deferred.py
--rw-r--r--   0        0        0     4569 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_dir.py
--rw-r--r--   0        0        0     9057 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_file.py
--rw-r--r--   0        0        0     1765 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_types.py
--rw-r--r--   0        0        0      650 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_helpers.py
--rw-r--r--   0        0        0      358 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_open_modes.py
--rw-r--r--   0        0        0     1003 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/__init__.py
--rw-r--r--   0        0        0     4666 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_abs.py
--rw-r--r--   0        0        0     1775 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_base.py
--rw-r--r--   0        0        0     1227 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py
--rw-r--r--   0        0        0     4484 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_rel.py
--rw-r--r--   0        0        0      190 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/__init__.py
--rw-r--r--   0        0        0      939 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_any_auth_strat.py
--rw-r--r--   0        0        0      311 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/__init__.py
--rw-r--r--   0        0        0      403 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_anon.py
--rw-r--r--   0        0        0      736 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py
--rw-r--r--   0        0        0     3184 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py
--rw-r--r--   0        0        0     2045 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py
--rw-r--r--   0        0        0      905 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_gcp_auth/_exceptions.py
--rw-r--r--   0        0        0      517 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_guid_service.py
--rw-r--r--   0        0        0      265 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/__init__.py
--rw-r--r--   0        0        0      113 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_log_aug/__init__.py
--rw-r--r--   0        0        0     2509 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_log_aug/_container.py
--rw-r--r--   0        0        0     1015 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py
--rw-r--r--   0        0        0     2395 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_log_level.py
--rw-r--r--   0        0        0    10107 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_logger.py
--rw-r--r--   0        0        0      437 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_logger_getter.py
--rw-r--r--   0        0        0     2997 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_setup.py
--rw-r--r--   0        0        0      197 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_sinks/__init__.py
--rw-r--r--   0        0        0     3843 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_base.py
--rw-r--r--   0        0        0     1200 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_file.py
--rw-r--r--   0        0        0      967 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_sys.py
--rw-r--r--   0        0        0       53 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_misc/__init__.py
--rw-r--r--   0        0        0      603 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_misc/_empty.py
--rw-r--r--   0        0        0      149 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/__init__.py
--rw-r--r--   0        0        0      123 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_services/__init__.py
--rw-r--r--   0        0        0     2531 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_services/_joiner.py
--rw-r--r--   0        0        0     2569 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_services/_json_dumper.py
--rw-r--r--   0        0        0        0 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_services/_misc.py
--rw-r--r--   0        0        0      234 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/__init__.py
--rw-r--r--   0        0        0     5167 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_collected_df.py
--rw-r--r--   0        0        0      789 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_dicts.py
--rw-r--r--   0        0        0     1046 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_discrim_helper.py
--rw-r--r--   0        0        0     5334 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_lazy_df.py
--rw-r--r--   0        0        0     1810 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_maybe_lazy.py
--rw-r--r--   0        0        0      189 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_ts_service/__init__.py
--rw-r--r--   0        0        0      623 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_ts_service/_fields.py
--rw-r--r--   0        0        0     6271 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_ts_service/_timestamp.py
--rw-r--r--   0        0        0     2643 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_ts_service/_tz_key.py
--rw-r--r--   0        0        0      251 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_ts_service/_utils.py
--rw-r--r--   0        0        0      145 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_utils/__init__.py
--rw-r--r--   0        0        0     1131 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_utils/_container_differ.py
--rw-r--r--   0        0        0     2511 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_utils/_dict_flattener.py
--rw-r--r--   0        0        0     1406 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_utils/_type_checkers.py
--rw-r--r--   0        0        0      152 2024-04-10 14:00:46.497874 spice_rack-0.8.0/src/spice_rack/_version_getter.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 spice_rack-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2750 2024-04-10 14:28:34.844706 spice_rack-0.9.0/README.md
+-rw-r--r--   0        0        0     3119 2024-04-10 14:28:55.992705 spice_rack-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      534 2024-04-10 14:28:34.844706 spice_rack-0.9.0/src/spice_rack/__init__.py
+-rw-r--r--   0        0        0      104 2024-04-10 14:28:34.844706 spice_rack-0.9.0/src/spice_rack/_api_helpers/__init__.py
+-rw-r--r--   0        0        0     1760 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_api_helpers/_uvicorn_startup_config.py
+-rw-r--r--   0        0        0      573 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/__init__.py
+-rw-r--r--   0        0        0     5289 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_base_base.py
+-rw-r--r--   0        0        0    12392 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_dispatchable.py
+-rw-r--r--   0        0        0      294 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/__init__.py
+-rw-r--r--   0        0        0     1318 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/_error_info.py
+-rw-r--r--   0        0        0     6767 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/_exception_base.py
+-rw-r--r--   0        0        0      778 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/_exception_exception.py
+-rw-r--r--   0        0        0     1145 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/_external_wrapper.py
+-rw-r--r--   0        0        0     5359 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_exception/_http.py
+-rw-r--r--   0        0        0      157 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_mixins/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_mixins/_guid_mixin.py
+-rw-r--r--   0        0        0      628 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_mixins/_mixin_base.py
+-rw-r--r--   0        0        0     1637 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_mixins/_timestamped.py
+-rw-r--r--   0        0        0     4362 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_root.py
+-rw-r--r--   0        0        0      108 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/__init__.py
+-rw-r--r--   0        0        0     4414 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/_base.py
+-rw-r--r--   0        0        0      126 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/__init__.py
+-rw-r--r--   0        0        0      408 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/_base.py
+-rw-r--r--   0        0        0     2067 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/_dot_env_ext.py
+-rw-r--r--   0        0        0     2067 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py
+-rw-r--r--   0        0        0     4874 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_special_str.py
+-rw-r--r--   0        0        0      446 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_bases/_value_model.py
+-rw-r--r--   0        0        0      316 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_common_validators/__init__.py
+-rw-r--r--   0        0        0     5834 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_common_validators/_mutually_exclusive_fields.py
+-rw-r--r--   0        0        0      114 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/__init__.py
+-rw-r--r--   0        0        0    17738 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_base.py
+-rw-r--r--   0        0        0      277 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/__init__.py
+-rw-r--r--   0        0        0     1501 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_dupe_keys.py
+-rw-r--r--   0        0        0     1835 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_item_ix_invalid.py
+-rw-r--r--   0        0        0     1364 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_key_already_exists.py
+-rw-r--r--   0        0        0     1510 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_missing_key.py
+-rw-r--r--   0        0        0      327 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/__init__.py
+-rw-r--r--   0        0        0     5557 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_exceptions.py
+-rw-r--r--   0        0        0     3377 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_info.py
+-rw-r--r--   0        0        0      464 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/__init__.py
+-rw-r--r--   0        0        0    13876 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_base.py
+-rw-r--r--   0        0        0      498 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_fs_inference.py
+-rw-r--r--   0        0        0     3462 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py
+-rw-r--r--   0        0        0      752 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_local.py
+-rw-r--r--   0        0        0     6385 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py
+-rw-r--r--   0        0        0      438 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/__init__.py
+-rw-r--r--   0        0        0     6564 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_base.py
+-rw-r--r--   0        0        0     5108 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_constraints.py
+-rw-r--r--   0        0        0     2936 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_deferred.py
+-rw-r--r--   0        0        0     4569 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_dir.py
+-rw-r--r--   0        0        0     9057 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_file.py
+-rw-r--r--   0        0        0     1765 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_types.py
+-rw-r--r--   0        0        0      650 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_helpers.py
+-rw-r--r--   0        0        0      358 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_open_modes.py
+-rw-r--r--   0        0        0     1003 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/__init__.py
+-rw-r--r--   0        0        0     4666 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_abs.py
+-rw-r--r--   0        0        0     1775 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_base.py
+-rw-r--r--   0        0        0     1227 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py
+-rw-r--r--   0        0        0     4484 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_rel.py
+-rw-r--r--   0        0        0      190 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/__init__.py
+-rw-r--r--   0        0        0      939 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_any_auth_strat.py
+-rw-r--r--   0        0        0      311 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_anon.py
+-rw-r--r--   0        0        0      736 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py
+-rw-r--r--   0        0        0     3184 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py
+-rw-r--r--   0        0        0     2045 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py
+-rw-r--r--   0        0        0      905 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_gcp_auth/_exceptions.py
+-rw-r--r--   0        0        0      517 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_guid_service.py
+-rw-r--r--   0        0        0      265 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/__init__.py
+-rw-r--r--   0        0        0      113 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_log_aug/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_log_aug/_container.py
+-rw-r--r--   0        0        0     1015 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py
+-rw-r--r--   0        0        0     2395 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_log_level.py
+-rw-r--r--   0        0        0    10107 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_logger.py
+-rw-r--r--   0        0        0      437 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_logger_getter.py
+-rw-r--r--   0        0        0     2997 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_setup.py
+-rw-r--r--   0        0        0      197 2024-04-10 14:28:34.848706 spice_rack-0.9.0/src/spice_rack/_logging/_sinks/__init__.py
+-rw-r--r--   0        0        0     3843 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_base.py
+-rw-r--r--   0        0        0     1200 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_file.py
+-rw-r--r--   0        0        0      967 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_sys.py
+-rw-r--r--   0        0        0       53 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_misc/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_misc/_empty.py
+-rw-r--r--   0        0        0      149 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/__init__.py
+-rw-r--r--   0        0        0      123 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_services/__init__.py
+-rw-r--r--   0        0        0     2531 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_services/_joiner.py
+-rw-r--r--   0        0        0     2569 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_services/_json_dumper.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_services/_misc.py
+-rw-r--r--   0        0        0      234 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/__init__.py
+-rw-r--r--   0        0        0     5167 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_collected_df.py
+-rw-r--r--   0        0        0      789 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_dicts.py
+-rw-r--r--   0        0        0     1046 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_discrim_helper.py
+-rw-r--r--   0        0        0     5334 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_lazy_df.py
+-rw-r--r--   0        0        0     1810 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_maybe_lazy.py
+-rw-r--r--   0        0        0      189 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_ts_service/__init__.py
+-rw-r--r--   0        0        0      623 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_ts_service/_fields.py
+-rw-r--r--   0        0        0     6271 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_ts_service/_timestamp.py
+-rw-r--r--   0        0        0     2643 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_ts_service/_tz_key.py
+-rw-r--r--   0        0        0      251 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_ts_service/_utils.py
+-rw-r--r--   0        0        0      145 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_utils/__init__.py
+-rw-r--r--   0        0        0     1131 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_utils/_container_differ.py
+-rw-r--r--   0        0        0     2511 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_utils/_dict_flattener.py
+-rw-r--r--   0        0        0     1406 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_utils/_type_checkers.py
+-rw-r--r--   0        0        0      152 2024-04-10 14:28:34.852706 spice_rack-0.9.0/src/spice_rack/_version_getter.py
+-rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 spice_rack-0.9.0/PKG-INFO
```

### Comparing `spice_rack-0.8.0/README.md` & `spice_rack-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/pyproject.toml` & `spice_rack-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spice_rack"
-version = "0.8.0"   # keep as 0.0.0 placeholder for poetry-dynamic-versioning
+version = "0.9.0"   # keep as 0.0.0 placeholder for poetry-dynamic-versioning
 description = "group of common things we use across different python packages"
 license = "Apache-2.0"
 authors = ["Tim Robin <timo.a.robin@gmail.com>",]
 readme = "README.md"
 
 packages = [
     {include = "spice_rack", from = "src"},
```

### Comparing `spice_rack-0.8.0/src/spice_rack/__init__.py` & `spice_rack-0.9.0/src/spice_rack/__init__.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_api_helpers/_uvicorn_startup_config.py` & `spice_rack-0.9.0/src/spice_rack/_api_helpers/_uvicorn_startup_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 import typing as t
 from pydantic import Field
-from spice_rack import bases
+from spice_rack import _bases
 
 
 __all__ = (
     "UvicornStartupConfig",
 )
 
 
-class _UvicornSslConfig(bases.ValueModelBase):
+class _UvicornSslConfig(_bases.ValueModelBase):
     """nested config for configuring ssl to uvicorn the server"""
     keyfile_path: str
     keyfile_password: str
     certfile_path: str
 
 
-class UvicornStartupConfig(bases.SettingsBase):
+class UvicornStartupConfig(_bases.SettingsBase):
     """
     config subsection for starting up an uvicorn process, useful for APIs such as litestar or fastapi.
 
     default env_prefix is 'uvicorn_startup__'
     """
     host: str = Field(default="localhost", description="host name of the app process")
     port: int = Field(default=8000, description="port the app is listening on")
```

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/__init__.py` & `spice_rack-0.9.0/src/spice_rack/_bases/__init__.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_base_base.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_base_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_dispatchable.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_dispatchable.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_exception/_error_info.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_exception/_error_info.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_exception/_exception_base.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_exception/_exception_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_exception/_exception_exception.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_exception/_exception_exception.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_exception/_external_wrapper.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_exception/_external_wrapper.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_exception/_http.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_exception/_http.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_mixins/_mixin_base.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_mixins/_mixin_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_mixins/_timestamped.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_mixins/_timestamped.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_root.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_root.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_settings/_base.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_settings/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/_dot_env_ext.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/_dot_env_ext.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_settings/_sources/_singleton_source.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_bases/_special_str.py` & `spice_rack-0.9.0/src/spice_rack/_bases/_special_str.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_common_validators/_mutually_exclusive_fields.py` & `spice_rack-0.9.0/src/spice_rack/_common_validators/_mutually_exclusive_fields.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_frozen_registry/_base.py` & `spice_rack-0.9.0/src/spice_rack/_frozen_registry/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_dupe_keys.py` & `spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_dupe_keys.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_item_ix_invalid.py` & `spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_item_ix_invalid.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_key_already_exists.py` & `spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_key_already_exists.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_frozen_registry/_exceptions/_missing_key.py` & `spice_rack-0.9.0/src/spice_rack/_frozen_registry/_exceptions/_missing_key.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_exceptions.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_exceptions.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_info.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_info.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_base.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_gcs.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_local.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_local.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_file_systems/_sftp.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_base.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_constraints.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_constraints.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_deferred.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_deferred.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_dir.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_dir.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_file.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_file.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_fs_models/_types.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_fs_models/_types.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_helpers.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_helpers.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/__init__.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/__init__.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_abs.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_abs.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_base.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_path_checkers.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_fs_ops/_path_strs/_rel.py` & `spice_rack-0.9.0/src/spice_rack/_fs_ops/_path_strs/_rel.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_gcp_auth/_any_auth_strat.py` & `spice_rack-0.9.0/src/spice_rack/_gcp_auth/_any_auth_strat.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py` & `spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py` & `spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_default.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py` & `spice_rack-0.9.0/src/spice_rack/_gcp_auth/_auth_strategies/_service_acct.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_gcp_auth/_exceptions.py` & `spice_rack-0.9.0/src/spice_rack/_gcp_auth/_exceptions.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_guid_service.py` & `spice_rack-0.9.0/src/spice_rack/_guid_service.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_log_aug/_container.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_log_aug/_container.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_log_aug/_loggable_mixin.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_log_level.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_log_level.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_logger.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_logger.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_setup.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_setup.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_base.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_base.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_file.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_file.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_logging/_sinks/_sys.py` & `spice_rack-0.9.0/src/spice_rack/_logging/_sinks/_sys.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_misc/_empty.py` & `spice_rack-0.9.0/src/spice_rack/_misc/_empty.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_services/_joiner.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_services/_joiner.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_services/_json_dumper.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_services/_json_dumper.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_collected_df.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_collected_df.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_dicts.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_dicts.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_discrim_helper.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_discrim_helper.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_lazy_df.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_lazy_df.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_polars_service/_types/_maybe_lazy.py` & `spice_rack-0.9.0/src/spice_rack/_polars_service/_types/_maybe_lazy.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_ts_service/_fields.py` & `spice_rack-0.9.0/src/spice_rack/_ts_service/_fields.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_ts_service/_timestamp.py` & `spice_rack-0.9.0/src/spice_rack/_ts_service/_timestamp.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_ts_service/_tz_key.py` & `spice_rack-0.9.0/src/spice_rack/_ts_service/_tz_key.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_utils/_container_differ.py` & `spice_rack-0.9.0/src/spice_rack/_utils/_container_differ.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_utils/_dict_flattener.py` & `spice_rack-0.9.0/src/spice_rack/_utils/_dict_flattener.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/src/spice_rack/_utils/_type_checkers.py` & `spice_rack-0.9.0/src/spice_rack/_utils/_type_checkers.py`

 * *Files identical despite different names*

### Comparing `spice_rack-0.8.0/PKG-INFO` & `spice_rack-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spice_rack
-Version: 0.8.0
+Version: 0.9.0
 Summary: group of common things we use across different python packages
 License: Apache-2.0
 Author: Tim Robin
 Author-email: timo.a.robin@gmail.com
 Requires-Python: >=3.9,<=3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

