# Comparing `tmp/edx-django-utils-5.8.0.tar.gz` & `tmp/edx-django-utils-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-django-utils-5.8.0.tar", last modified: Fri Nov  3 18:00:29 2023, max compression
+gzip compressed data, was "edx-django-utils-5.9.0.tar", last modified: Mon Nov 27 12:02:41 2023, max compression
```

## Comparing `edx-django-utils-5.8.0.tar` & `edx-django-utils-5.9.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.744710 edx-django-utils-5.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    13826 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21569 2023-11-03 18:00:29.744710 edx-django-utils-5.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/admin/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/admin/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/admin/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/admin/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/admin/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/cache/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12886 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/cache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils/db/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/db/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/tests/test_queryset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/db/tests/test_read_replica.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/ip/
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/ip/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/ip/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/ip/internal/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/ip/internal/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/ip/internal/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13591 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/ip/internal/tests/test_ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/logging/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/internal/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/internal/log_sensitive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/logging/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/tests/test_log_sensitive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/logging/tests/test_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22556 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/monitoring/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)    13423 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/scripts/new_relic_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.736710 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    13563 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/monitoring/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/pluggable_override.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_contexts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.728710 edx-django-utils-5.8.0/edx_django_utils/security/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/security/csp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/security/csp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5753 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/security/csp/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/security/csp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/security/csp/tests/test_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/tests/test_pluggable_override.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/user/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/user/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/user/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/commands/manage_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/commands/manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/user/management/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/tests/test_manage_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7796 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/management/tests/test_manage_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/edx_django_utils/user/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/edx_django_utils/user/tests/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.732710 edx-django-utils-5.8.0/edx_django_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21569 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-03 18:00:29.000000 edx-django-utils-5.8.0/edx_django_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-03 18:00:29.744710 edx-django-utils-5.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-03 18:00:29.740710 edx-django-utils-5.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-03 18:00:22.000000 edx-django-utils-5.8.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.643113 edx-django-utils-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    13988 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20877 2023-11-27 12:02:41.643113 edx-django-utils-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.627114 edx-django-utils-5.9.0/edx_django_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/admin/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/admin/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/admin/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/admin/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/admin/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/cache/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12520 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10864 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/cache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/db/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/tests/test_queryset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/db/tests/test_read_replica.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/ip/
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/ip/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/ip/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/ip/internal/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/ip/internal/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/ip/internal/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/ip/internal/tests/test_ip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/logging/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/internal/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/internal/log_sensitive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/logging/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/tests/test_log_sensitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/logging/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22556 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2621 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)    13423 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/scripts/new_relic_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8178 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.635114 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/mock_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/monitoring/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/pluggable_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/plugins/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.627114 edx-django-utils-5.9.0/edx_django_utils/security/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/security/csp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/security/csp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/security/csp/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/security/csp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/security/csp/tests/test_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/tests/test_pluggable_override.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/user/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/user/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/commands/manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/commands/manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/user/management/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/tests/test_manage_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7796 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/management/tests/test_manage_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/edx_django_utils/user/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/edx_django_utils/user/tests/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.631114 edx-django-utils-5.9.0/edx_django_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20877 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-11-27 12:02:41.000000 edx-django-utils-5.9.0/edx_django_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.639114 edx-django-utils-5.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-27 12:02:41.643113 edx-django-utils-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:02:41.643113 edx-django-utils-5.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-27 12:02:38.000000 edx-django-utils-5.9.0/tests/test_models.py
```

### Comparing `edx-django-utils-5.8.0/CHANGELOG.rst` & `edx-django-utils-5.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,21 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[5.9.0] - 2023-11-27
+--------------------
+
+Removed
+~~~~~~~
+* Removed ``edx_django_utils.cache.disable_forced_cache_miss_for_none`` which was added in ``5.7.0``.
+
 [5.8.0] - 2023-11-03
 --------------------
 
 Changed
 ~~~~~~~
 * Adjusted ``get_plugin_apps`` to log at info level rather than debug and with more detail, though with a comment that this may not actually end up logging.
```

### Comparing `edx-django-utils-5.8.0/LICENSE.txt` & `edx-django-utils-5.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/PKG-INFO` & `edx-django-utils-5.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-django-utils
-Version: 5.8.0
+Version: 5.9.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
@@ -73,64 +73,18 @@
 .. _Security Utilities: edx_django_utils/security/README.rst
 
 Documentation
 -------------
 
 The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
 
-Getting Started
----------------
+Getting Started with Development
+--------------------------------
 
-One Time Setup
-~~~~~~~~~~~~~~
-.. code-block::
-
-  # clone the repo
-  git clone git@github.com:edx/edx-django-utils.git
-  cd edx-django-utils
-
-  # setup a virtualenv using virtualenvwrapper with the same name as the repo and activate it.
-  # $(basename $(pwd)) will give you the name of the current working directory, in this case ``edx-django-utils``
-  mkvirtualenv -p python3 $(basename $(pwd))
-
-
-Every time you develop something in this repo
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-.. code-block::
-
-  # Activate the virtualenv.
-  workon edx-django-utils
-
-  # Grab the latest code.
-  git checkout master
-  git pull
-
-  # Install the dev requirements
-  make requirements
-
-  # Run the tests
-  make test
-
-  # Make a new branch for your changes
-  git checkout -b <your_github_username>/<short_description>
-
-  # Using your favorite editor, edit the code to make your change.
-  vim …
-
-  # Run your new tests
-  pytest ./path/to/new/tests
-
-  # Run all the test
-  make test
-
-  # Commit all your changes
-  git commit …
-  git push
-
-  # Open a PR and ask for review.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
 Design Pattern followed by packages
 -----------------------------------
 
 All tools in edx_django_utils should expose their public api in their __init__.py files. This entails adding to __init__.py all functions/classes/constants/objects that are intended to be used by users of library.
 
 Getting Help
@@ -236,14 +190,21 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[5.9.0] - 2023-11-27
+--------------------
+
+Removed
+~~~~~~~
+* Removed ``edx_django_utils.cache.disable_forced_cache_miss_for_none`` which was added in ``5.7.0``.
+
 [5.8.0] - 2023-11-03
 --------------------
 
 Changed
 ~~~~~~~
 * Adjusted ``get_plugin_apps`` to log at info level rather than debug and with more detail, though with a comment that this may not actually end up logging.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edx-django-utils-5.8.0/README.rst` & `edx-django-utils-5.9.0/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -45,64 +45,18 @@
 .. _Security Utilities: edx_django_utils/security/README.rst
 
 Documentation
 -------------
 
 The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
 
-Getting Started
----------------
+Getting Started with Development
+--------------------------------
 
-One Time Setup
-~~~~~~~~~~~~~~
-.. code-block::
-
-  # clone the repo
-  git clone git@github.com:edx/edx-django-utils.git
-  cd edx-django-utils
-
-  # setup a virtualenv using virtualenvwrapper with the same name as the repo and activate it.
-  # $(basename $(pwd)) will give you the name of the current working directory, in this case ``edx-django-utils``
-  mkvirtualenv -p python3 $(basename $(pwd))
-
-
-Every time you develop something in this repo
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-.. code-block::
-
-  # Activate the virtualenv.
-  workon edx-django-utils
-
-  # Grab the latest code.
-  git checkout master
-  git pull
-
-  # Install the dev requirements
-  make requirements
-
-  # Run the tests
-  make test
-
-  # Make a new branch for your changes
-  git checkout -b <your_github_username>/<short_description>
-
-  # Using your favorite editor, edit the code to make your change.
-  vim …
-
-  # Run your new tests
-  pytest ./path/to/new/tests
-
-  # Run all the test
-  make test
-
-  # Commit all your changes
-  git commit …
-  git push
-
-  # Open a PR and ask for review.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
 Design Pattern followed by packages
 -----------------------------------
 
 All tools in edx_django_utils should expose their public api in their __init__.py files. This entails adding to __init__.py all functions/classes/constants/objects that are intended to be used by users of library.
 
 Getting Help
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edx-django-utils-5.8.0/edx_django_utils/admin/mixins.py` & `edx-django-utils-5.9.0/edx_django_utils/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/admin/tests/test_mixins.py` & `edx-django-utils-5.9.0/edx_django_utils/admin/tests/test_mixins.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/cache/middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/cache/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/cache/tests/test_middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/cache/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/cache/tests/test_utils.py` & `edx-django-utils-5.9.0/edx_django_utils/cache/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 """
 
 from threading import Thread
 from unittest import TestCase, mock
 
 import ddt
 from django.test import TestCase as DjangoTestCase
-from waffle.testutils import override_switch
 
 from edx_django_utils.cache.utils import (
     DEFAULT_REQUEST_CACHE_NAMESPACE,
     SHOULD_FORCE_CACHE_MISS_KEY,
     CachedResponse,
     CachedResponseError,
     RequestCache,
@@ -166,65 +165,14 @@
         cached_response = TieredCache.get_cached_response(TEST_KEY)
         self.assertTrue(cached_response.is_found)
         self.assertEqual(cached_response.value, EXPECTED_VALUE)
 
         cached_response = self.request_cache.get_cached_response(TEST_KEY)
         self.assertTrue(cached_response.is_found, 'Django cache hit should cache value in request cache.')
 
-    @mock.patch('edx_django_utils.monitoring.internal.utils.set_custom_attribute')
-    @override_switch('edx_django_utils.cache.disable_forced_cache_miss_for_none', True)
-    def test_get_cached_response_hit_with_cached_none(self, mock_set_custom_attribute):
-        """
-        Tests cache hit when caching a None.
-
-        For rollout, this test relies on ``disable_forced_cache_miss_for_none`` switch to be on, because
-        by default we are temporarily forcing cache misses for backward compatibility.
-        """
-        TieredCache.set_all_tiers(TEST_KEY, None)
-        # Test retrieval from tier 1: RequestCache
-        cached_response = TieredCache.get_cached_response(TEST_KEY)
-        self.assertTrue(cached_response.is_found)
-        self.assertEqual(cached_response.value, None)
-
-        self.request_cache.clear()
-        # Test retrieval from tier 2: Django Cache
-        cached_response = TieredCache.get_cached_response(TEST_KEY)
-        self.assertTrue(cached_response.is_found)
-        self.assertEqual(cached_response.value, None)
-
-        expected_calls = [
-            mock.call('retrieved_cached_none', True)
-        ]
-        mock_set_custom_attribute.assert_has_calls(expected_calls)
-
-    @mock.patch('edx_django_utils.monitoring.internal.utils.set_custom_attribute')
-    def test_get_cached_response_miss_with_cached_none(self, mock_set_custom_attribute):
-        """
-        Temporary tests for cache miss when caching a None.
-
-        Temporarily we are forcing cache misses by default when caching None for
-        backward compatibility purposes. See ``disable_forced_cache_miss_for_none``
-        switch for more details.
-        """
-        TieredCache.set_all_tiers(TEST_KEY, None)
-        # Test retrieval from tier 1: RequestCache
-        cached_response = TieredCache.get_cached_response(TEST_KEY)
-        self.assertTrue(cached_response.is_found)
-        self.assertEqual(cached_response.value, None)
-
-        self.request_cache.clear()
-        # Test retrieval from tier 2: Django Cache
-        cached_response = TieredCache.get_cached_response(TEST_KEY)
-        self.assertFalse(cached_response.is_found)
-
-        expected_calls = [
-            mock.call('retrieved_cached_none', True)
-        ]
-        mock_set_custom_attribute.assert_has_calls(expected_calls)
-
     @mock.patch('django.core.cache.cache.get')
     def test_get_cached_response_force_cache_miss(self, mock_cache_get):
         self.request_cache.set(SHOULD_FORCE_CACHE_MISS_KEY, True)
         mock_cache_get.return_value = EXPECTED_VALUE
         cached_response = TieredCache.get_cached_response(TEST_KEY)
         self.assertFalse(cached_response.is_found)
```

### Comparing `edx-django-utils-5.8.0/edx_django_utils/cache/utils.py` & `edx-django-utils-5.9.0/edx_django_utils/cache/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """
 Cache utilities.
 """
 import hashlib
 import threading
 
-import waffle  # pylint: disable=invalid-django-waffle-import
 from django.core.cache import cache as django_cache
 from django.core.cache.backends.base import DEFAULT_TIMEOUT
 from django.utils.encoding import force_str
 
 FORCE_CACHE_MISS_PARAM = 'force_cache_miss'
 DEFAULT_NAMESPACE = 'edx_django_utils.cache'
 DEFAULT_REQUEST_CACHE_NAMESPACE = f'{DEFAULT_NAMESPACE}.default'
 SHOULD_FORCE_CACHE_MISS_KEY = 'edx_django_utils.cache.should_force_cache_miss'
 
 _CACHE_MISS = object()
-_CACHED_NONE = 'CACHED_NONE'
 
 
 def get_cache_key(**kwargs):
     """
     Get MD5 encoded cache key for given arguments.
 
     **Note:** We convert keyword arguments to their string form to build the cache key. So do not pass
@@ -208,18 +206,15 @@
             django_cache_timeout (int): (Optional) Timeout used to determine
                 if and for how long to cache in the django cache. A timeout of
                 0 will skip the django cache. If timeout is provided, use that
                 timeout for the key; otherwise use the default cache timeout.
 
         """
         DEFAULT_REQUEST_CACHE.set(key, value)
-        cached_value = value
-        if value is None:
-            cached_value = _CACHED_NONE
-        django_cache.set(key, cached_value, django_cache_timeout)
+        django_cache.set(key, value, django_cache_timeout)
 
     @staticmethod
     def delete_all_tiers(key):
         """
         Deletes the cached value for the provided key in both the request cache and the
         django cache.
 
@@ -260,29 +255,14 @@
             A CachedResponse with is_found status and value.
 
         """
         if TieredCache._should_force_django_cache_miss():
             return CachedResponse(is_found=False, key=key, value=None)
 
         cached_value = django_cache.get(key, _CACHE_MISS)
-
-        if cached_value == _CACHED_NONE:
-            # Avoiding circular import
-            from edx_django_utils.monitoring.internal.utils import \
-                set_custom_attribute  # isort:skip, pylint: disable=cyclic-import, import-outside-toplevel
-
-            # .. custom_attribute_name: retrieved_cached_none
-            # .. custom_attribute_description: Temporary attribute to see when a None would
-            #      have been retrieved, so we know what will be affected by the toggle.
-            set_custom_attribute('retrieved_cached_none', True)
-            if TieredCache._is_forced_cache_miss_for_none_disabled():
-                cached_value = None
-            else:
-                cached_value = _CACHE_MISS
-
         is_found = cached_value is not _CACHE_MISS
         return CachedResponse(is_found, key, cached_value)
 
     @staticmethod
     def _set_request_cache_if_django_cache_hit(key, django_cached_response):
         """
         Sets the value in the request cache if the django cached response was a hit.
@@ -319,33 +299,14 @@
         Returns True if the tiered cache should force a cache miss for the
         django cache, and False otherwise.
 
         """
         cached_response = DEFAULT_REQUEST_CACHE.get_cached_response(SHOULD_FORCE_CACHE_MISS_KEY)
         return False if not cached_response.is_found else cached_response.value
 
-    @staticmethod
-    def _is_forced_cache_miss_for_none_disabled():
-        """
-        Returns True if disable_forced_cache_miss_for_none is on, and False otherwise.
-        """
-        # .. toggle_name: edx_django_utils.cache.disable_forced_cache_miss_for_none
-        # .. toggle_implementation: WaffleSwitch
-        # .. toggle_default: False
-        # .. toggle_description: By default, this toggle will replicate an existing bug by forcing
-        #      cache misses when setting None. Set the toggle to True to disable this behavior,
-        #      which fixes the bug and returns None when None was cached. This toggle is
-        #      being used for backward compatibility during rollout, until the toggle and old
-        #      broken behavior can be removed.
-        # .. toggle_use_cases: temporary
-        # .. toggle_creation_date: 2023-08-02
-        # .. toggle_target_removal_date: 2023-09-01
-        # .. toggle_tickets: https://github.com/openedx/edx-django-utils/issues/333
-        return waffle.switch_is_active('edx_django_utils.cache.disable_forced_cache_miss_for_none')
-
 
 class CachedResponseError(Exception):
     """
     Error used when CachedResponse is misused.
     """
     USAGE_MESSAGE = 'CachedResponse was misused. Try the attributes is_found, value or key.'
```

### Comparing `edx-django-utils-5.8.0/edx_django_utils/db/queryset_utils.py` & `edx-django-utils-5.9.0/edx_django_utils/db/queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/db/read_replica.py` & `edx-django-utils-5.9.0/edx_django_utils/db/read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/db/tests/test_queryset_utils.py` & `edx-django-utils-5.9.0/edx_django_utils/db/tests/test_queryset_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/db/tests/test_read_replica.py` & `edx-django-utils-5.9.0/edx_django_utils/db/tests/test_read_replica.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/ip/__init__.py` & `edx-django-utils-5.9.0/edx_django_utils/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/ip/internal/ip.py` & `edx-django-utils-5.9.0/edx_django_utils/ip/internal/ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/ip/internal/tests/test_ip.py` & `edx-django-utils-5.9.0/edx_django_utils/ip/internal/tests/test_ip.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/logging/internal/filters.py` & `edx-django-utils-5.9.0/edx_django_utils/logging/internal/filters.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/logging/internal/log_sensitive.py` & `edx-django-utils-5.9.0/edx_django_utils/logging/internal/log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/logging/tests/test_log_sensitive.py` & `edx-django-utils-5.9.0/edx_django_utils/logging/tests/test_log_sensitive.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/logging/tests/test_logging.py` & `edx-django-utils-5.9.0/edx_django_utils/logging/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/__init__.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/code_owner/utils.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/code_owner/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/transactions.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/transactions.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/internal/utils.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/internal/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/scripts/new_relic_search.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/scripts/new_relic_search.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/scripts/process_cookie_monitoring_logs.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/code_owner/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_custom_monitoring.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/tests/test_utils.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/monitoring/utils.py` & `edx-django-utils-5.9.0/edx_django_utils/monitoring/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/__init__.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/constants.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/constants.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/pluggable_override.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_apps.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_apps.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_contexts.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_contexts.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_manager.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_settings.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_signals.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_signals.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/plugin_urls.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/plugin_urls.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/plugins/utils.py` & `edx-django-utils-5.9.0/edx_django_utils/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/security/csp/middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/security/csp/middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/security/csp/tests/test_middleware.py` & `edx-django-utils-5.9.0/edx_django_utils/security/csp/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/tests/test_pluggable_override.py` & `edx-django-utils-5.9.0/edx_django_utils/tests/test_pluggable_override.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/__init__.py` & `edx-django-utils-5.9.0/edx_django_utils/user/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/management/commands/manage_group.py` & `edx-django-utils-5.9.0/edx_django_utils/user/management/commands/manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/management/commands/manage_user.py` & `edx-django-utils-5.9.0/edx_django_utils/user/management/commands/manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/management/tests/test_manage_group.py` & `edx-django-utils-5.9.0/edx_django_utils/user/management/tests/test_manage_group.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/management/tests/test_manage_user.py` & `edx-django-utils-5.9.0/edx_django_utils/user/management/tests/test_manage_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils/user/tests/test_user.py` & `edx-django-utils-5.9.0/edx_django_utils/user/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/edx_django_utils.egg-info/PKG-INFO` & `edx-django-utils-5.9.0/edx_django_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-django-utils
-Version: 5.8.0
+Version: 5.9.0
 Summary: EdX utilities for Django Application development.
 Home-page: https://github.com/openedx/edx-django-utils
 Author: edX
 Author-email: oscm@edx.org
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
@@ -73,64 +73,18 @@
 .. _Security Utilities: edx_django_utils/security/README.rst
 
 Documentation
 -------------
 
 The full documentation is in the docs directory, and is published to https://edx-django-utils.readthedocs.org.
 
-Getting Started
----------------
+Getting Started with Development
+--------------------------------
 
-One Time Setup
-~~~~~~~~~~~~~~
-.. code-block::
-
-  # clone the repo
-  git clone git@github.com:edx/edx-django-utils.git
-  cd edx-django-utils
-
-  # setup a virtualenv using virtualenvwrapper with the same name as the repo and activate it.
-  # $(basename $(pwd)) will give you the name of the current working directory, in this case ``edx-django-utils``
-  mkvirtualenv -p python3 $(basename $(pwd))
-
-
-Every time you develop something in this repo
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-.. code-block::
-
-  # Activate the virtualenv.
-  workon edx-django-utils
-
-  # Grab the latest code.
-  git checkout master
-  git pull
-
-  # Install the dev requirements
-  make requirements
-
-  # Run the tests
-  make test
-
-  # Make a new branch for your changes
-  git checkout -b <your_github_username>/<short_description>
-
-  # Using your favorite editor, edit the code to make your change.
-  vim …
-
-  # Run your new tests
-  pytest ./path/to/new/tests
-
-  # Run all the test
-  make test
-
-  # Commit all your changes
-  git commit …
-  git push
-
-  # Open a PR and ask for review.
+Please see the Open edX documentation for `guidance on Python development <https://docs.openedx.org/en/latest/developers/how-tos/get-ready-for-python-dev.html>`_ in this repo.
 
 Design Pattern followed by packages
 -----------------------------------
 
 All tools in edx_django_utils should expose their public api in their __init__.py files. This entails adding to __init__.py all functions/classes/constants/objects that are intended to be used by users of library.
 
 Getting Help
@@ -236,14 +190,21 @@
    but in reStructuredText instead of Markdown (for ease of incorporation into
    Sphinx documentation and the PyPI description).
 
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
+[5.9.0] - 2023-11-27
+--------------------
+
+Removed
+~~~~~~~
+* Removed ``edx_django_utils.cache.disable_forced_cache_miss_for_none`` which was added in ``5.7.0``.
+
 [5.8.0] - 2023-11-03
 --------------------
 
 Changed
 ~~~~~~~
 * Adjusted ``get_plugin_apps`` to log at info level rather than debug and with more detail, though with a comment that this may not actually end up logging.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `edx-django-utils-5.8.0/edx_django_utils.egg-info/SOURCES.txt` & `edx-django-utils-5.9.0/edx_django_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/requirements/base.in` & `edx-django-utils-5.9.0/requirements/base.in`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/requirements/constraints.txt` & `edx-django-utils-5.9.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-django-utils-5.8.0/setup.py` & `edx-django-utils-5.9.0/setup.py`

 * *Files identical despite different names*

