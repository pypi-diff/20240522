# Comparing `tmp/aioli_sdk-0.2.4.dev3.tar.gz` & `tmp/aioli_sdk-0.2.4.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4.dev3.tar", last modified: Thu May 16 10:38:47 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4.dev5.tar", last modified: Wed May 22 18:59:10 2024, max compression
```

## Comparing `aioli_sdk-0.2.4.dev3.tar` & `aioli_sdk-0.2.4.dev5.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.370155 aioli_sdk-0.2.4.dev3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29096 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 10:38:45.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/model_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 10:38:47.370155 aioli_sdk-0.2.4.dev3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.714497 aioli_sdk-0.2.4.dev5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-22 18:59:10.714497 aioli_sdk-0.2.4.dev5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.706497 aioli_sdk-0.2.4.dev5/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.706497 aioli_sdk-0.2.4.dev5/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.706497 aioli_sdk-0.2.4.dev5/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31029 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.706497 aioli_sdk-0.2.4.dev5/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.706497 aioli_sdk-0.2.4.dev5/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.714497 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-22 18:59:08.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-22 18:59:10.000000 aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.710497 aioli_sdk-0.2.4.dev5/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.710497 aioli_sdk-0.2.4.dev5/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:10.714497 aioli_sdk-0.2.4.dev5/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5468 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5294 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-22 18:59:06.000000 aioli_sdk-0.2.4.dev5/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-22 18:59:07.000000 aioli_sdk-0.2.4.dev5/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-22 18:59:10.714497 aioli_sdk-0.2.4.dev5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-22 18:53:47.000000 aioli_sdk-0.2.4.dev5/setup.py
```

### Comparing `aioli_sdk-0.2.4.dev3/PKG-INFO` & `aioli_sdk-0.2.4.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev3
+Version: 0.2.4.dev5
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/_util.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/cli.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/deployment.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/errors.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/model.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/registry.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/registry.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         r = TrainedModelRegistryRequest(
             name=args.name,
             accessKey=args.access_key,
             bucket=args.bucket,
             endpointUrl=args.endpoint_url,
             secretKey=args.secret_key,
             type=args.type,
+            insecureHttps=args.insecure_https,
         )
         api_instance.registries_post(r)
 
 
 def lookup_registry(name: str, api: aiolirest.RegistriesApi) -> TrainedModelRegistry:
     for r in api.registries_get():
         if r.name == name:
@@ -196,14 +197,19 @@
                     "contain letters, numbers, and hyphen",
                 ),
                 Arg("--type", help="The type of this model registry", required="true"),
                 Arg("--bucket", help="S3 Bucket name"),
                 Arg("--access-key", help="S3 access key/username"),
                 Arg("--secret-key", help="secret key/password", required="true"),
                 Arg("--endpoint-url", help="S3 endpoint URL"),
+                Arg(
+                    "--insecure-https",
+                    help="Allow insecure HTTPS connections to S3",
+                    action="store_true",  # prefer argparse.BooleanOptionalAction
+                ),
             ],
         ),
         # Show command.
         Cmd(
             "show",
             show_registry,
             "show a registry",
@@ -231,14 +237,19 @@
                     "contain letters, numbers, and hyphen",
                 ),
                 Arg("--type", help="The type of this model registry"),
                 Arg("--bucket", help="S3 Bucket name"),
                 Arg("--access-key", help="S3 access key/username"),
                 Arg("--secret-key", help="S3 secret key/password"),
                 Arg("--endpoint-url", help="S3 endpoint URL"),
+                Arg(
+                    "--insecure-https",
+                    help="Allow insecure HTTPS connections to S3",
+                    action="store_true",  # prefer argparse.BooleanOptionalAction
+                ),
             ],
         ),
         Cmd(
             "delete",
             delete_registry,
             "delete a registry",
             [
```

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/render.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/role.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/sso.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/test/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # © Copyright 2024 Hewlett Packard Enterprise Development LP
 import csv
 import os
 import subprocess
 
+import yaml
+
 
 class TestCli:
     testdir = os.path.dirname(os.path.realpath(__file__))
 
     def test_version(self, setup_login: None) -> None:
         version_file = self.testdir + "/../../../../VERSION"
         expected = None
@@ -29,14 +31,58 @@
         expected = (
             " Name   | Type   | Access Key   | Bucket   | Secret Key   | Endpoint URL"
             "\n--------+--------+--------------+----------+--------------+----------------\n"
         )
         actual = subprocess.check_output(["aioli", "registry", "list"]).decode("utf-8")
         assert actual == expected
 
+    def test_registry_create_and_update_insecure(self, setup_login: None) -> None:
+        # Create a registry with insecure-https and test for expected values
+        assert (
+            os.system(
+                "aioli registry create --type s3 --access-key minioadmin "
+                "--secret-key minioadmin --bucket demo-bento-registry "
+                "--endpoint-url http://10.30.89.14:30008 --insecure-https bento-registry-insecure"
+            )
+            == 0
+        )
+
+        # Newly created registry entry without id/modified as dict
+        expected = yaml.safe_load(
+            "accessKey: minioadmin\nbucket: demo-bento-registry\nendpointUrl: "
+            "http://10.30.89.14:30008\ninsecureHttps: true\n"
+            "name: bento-registry-insecure\nsecretKey: '**********'\ntype: s3\n\n"
+        )
+        actualstr = subprocess.check_output(
+            ["aioli", "registry", "show", "bento-registry-insecure"]
+        ).decode("utf-8")
+        actual = yaml.safe_load(actualstr)
+        del actual["id"]
+        del actual["modifiedAt"]
+        assert actual == expected
+
+        # Update to secure
+        if False:
+            # This is blocked until CI is at python 3.9 -- then update
+            # registry.py to use action=argparse.BoolOptionalAction
+            assert (
+                os.system("aioli registry update --no-insecure-https bento-registry-insecure") == 0
+            )
+            expected["insecureHttps"] = False
+            actual = subprocess.check_output(
+                ["aioli", "registry", "show", "bento-registry-insecure"]
+            ).decode("utf-8")
+            actual = yaml.safe_load(actual)
+            del actual["id"]
+            del actual["modifiedAt"]
+            assert actual == expected
+
+        # Cleanup test registry
+        assert os.system("aioli registry delete bento-registry-insecure") == 0
+
     def test_registry_create(self, setup_login: None) -> None:
         # Create a registry entry and test for success
         assert (
             os.system(
                 "aioli registry create --type s3 --access-key minioadmin "
                 "--secret-key minioadmin --bucket demo-bento-registry "
                 "--endpoint-url http://10.30.89.14:30008/ bento-registry"
@@ -129,14 +175,15 @@
     def test_registry_list_json(self, setup_login: None) -> None:
         expected = (
             '[\n'    # noqa: Q000
             '  {\n'  # noqa: Q000
             '    "accessKey": "minioadmin",\n'
             '    "bucket": "demo-bento-registry",\n'
             '    "endpointUrl": "http://10.30.89.14:30008/",\n'
+            '    "insecureHttps": false,\n'
             '    "name": "bento-registry",\n'
             '    "secretKey": "**********",\n'
             '    "type": "s3"\n'
             '  }\n'  # noqa: Q000
             ']\n'    # noqa: Q000
         )
         actual = subprocess.check_output(["aioli", "registry", "list", "--json"]).decode("utf-8")
```

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/user.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/cli/version.py` & `aioli_sdk-0.2.4.dev5/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4.dev5/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/api/certs.py` & `aioli_sdk-0.2.4.dev5/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/api/errors.py` & `aioli_sdk-0.2.4.dev5/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/api/request.py` & `aioli_sdk-0.2.4.dev5/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/check.py` & `aioli_sdk-0.2.4.dev5/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/constants.py` & `aioli_sdk-0.2.4.dev5/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4.dev5/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/requests.py` & `aioli_sdk-0.2.4.dev5/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/common/util.py` & `aioli_sdk-0.2.4.dev5/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli/util.py` & `aioli_sdk-0.2.4.dev5/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev3
+Version: 0.2.4.dev5
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4.dev5/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/__init__.py` & `aioli_sdk-0.2.4.dev5/aiolirest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/registries_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api_client.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/api_response.py` & `aioli_sdk-0.2.4.dev5/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/configuration.py` & `aioli_sdk-0.2.4.dev5/aiolirest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-dev3\n"\
+               "Version of the API: 0.2.4-dev5\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/exceptions.py` & `aioli_sdk-0.2.4.dev5/aiolirest/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/autoscaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/configuration_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/deployment_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/event_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/failure_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/login_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/model_auth_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/model_response.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/model_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/observability.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/observability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/packaged_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/packaged_model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/resource_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/resources_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/role.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/security.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/success_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/trained_model_registry_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModelRegistry(BaseModel):
+class TrainedModelRegistryRequest(BaseModel):
     """
     Provides the metadata that describes how to access a named model registry to enable download of a trained model for deployment.
     """ # noqa: E501
     access_key: Optional[StrictStr] = Field(default=None, description="The access key, username or team name for the registry. * `s3` - The access key/username. * `ngc` - The optional NGC team name.", alias="accessKey")
     bucket: Optional[StrictStr] = Field(default=None, description="The bucket or organization name.  * `s3` - The required S3 bucket name. * `ngc` - The required NGC org name.")
     endpoint_url: Optional[StrictStr] = Field(default=None, description="The registry endpoint (host): * `s3` - The S3 registry endpoint. Required. * `openllm` - The huggingface.co-compatible endpoint (default https://huggingface.co). * `ngc` - The NVIDIA NGC-compatible api endpoint (default https://api.ngc.nvidia.com).", alias="endpointUrl")
-    id: Optional[StrictStr] = Field(default=None, description="The ID of the model registry. This is a read-only field and is automatically assigned on creation.")
+    insecure_https: Optional[StrictBool] = Field(default=None, description="For https endpoints, the server certificate will be accepted without validation.", alias="insecureHttps")
     modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the registry. This is a read-only field and is automatically updated.", alias="modifiedAt")
     name: StrictStr = Field(description="The name of the registry.  Must begin with a letter, but may contain letters, numbers, and hyphen.")
-    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * `s3` - The secret key for the S3 bucket. * `openllm` -  The access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN` environment variable.bucket. * `ngc` - The NVIDIA NGC apikey.", alias="secretKey")
+    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * `s3` - The secret key for the S3 bucket. * `openllm` -  The access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN` environment variable.bucket. * `ngc` - The requied NVIDIA NGC apikey.", alias="secretKey")
     type: StrictStr = Field(description="The type of this model registry. Must be one of the values: (s3, http, openllm, ngc). * `s3` - Configuration to enable access to an s3 bucket. * `openllm` - Configuration to enable direct download of OpenLLM models from huggingface.co.   Provide your access token in the `secretKey` field. * `ngc` -  Configuration to enable direct download from the NVIDA NGC: AI Development Catalog. * `http` - Not yet supported.  Configuration to enable model download from a protected http endpoint that requires login.")
-    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "id", "modifiedAt", "name", "secretKey", "type"]
+    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "insecureHttps", "modifiedAt", "name", "secretKey", "type"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -54,15 +54,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModelRegistry from a JSON string"""
+        """Create an instance of TrainedModelRegistryRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,26 +77,26 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModelRegistry from a dict"""
+        """Create an instance of TrainedModelRegistryRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "accessKey": obj.get("accessKey"),
             "bucket": obj.get("bucket"),
             "endpointUrl": obj.get("endpointUrl"),
-            "id": obj.get("id"),
+            "insecureHttps": obj.get("insecureHttps"),
             "modifiedAt": obj.get("modifiedAt"),
             "name": obj.get("name"),
             "secretKey": obj.get("secretKey"),
             "type": obj.get("type")
         })
         return _obj
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/trained_model_registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, ClassVar, Dict, List, Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, StrictBool, StrictStr
 from pydantic import Field
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
-class TrainedModelRegistryRequest(BaseModel):
+class TrainedModelRegistry(BaseModel):
     """
     Provides the metadata that describes how to access a named model registry to enable download of a trained model for deployment.
     """ # noqa: E501
     access_key: Optional[StrictStr] = Field(default=None, description="The access key, username or team name for the registry. * `s3` - The access key/username. * `ngc` - The optional NGC team name.", alias="accessKey")
     bucket: Optional[StrictStr] = Field(default=None, description="The bucket or organization name.  * `s3` - The required S3 bucket name. * `ngc` - The required NGC org name.")
     endpoint_url: Optional[StrictStr] = Field(default=None, description="The registry endpoint (host): * `s3` - The S3 registry endpoint. Required. * `openllm` - The huggingface.co-compatible endpoint (default https://huggingface.co). * `ngc` - The NVIDIA NGC-compatible api endpoint (default https://api.ngc.nvidia.com).", alias="endpointUrl")
+    id: Optional[StrictStr] = Field(default=None, description="The ID of the model registry. This is a read-only field and is automatically assigned on creation.")
+    insecure_https: Optional[StrictBool] = Field(default=None, description="For https endpoints, the server certificate will be accepted without validation.", alias="insecureHttps")
     modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the registry. This is a read-only field and is automatically updated.", alias="modifiedAt")
     name: StrictStr = Field(description="The name of the registry.  Must begin with a letter, but may contain letters, numbers, and hyphen.")
-    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * `s3` - The secret key for the S3 bucket. * `openllm` -  The access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN` environment variable.bucket. * `ngc` - The requied NVIDIA NGC apikey.", alias="secretKey")
+    secret_key: StrictStr = Field(description="The secret key is the password, secret key, or access token for the registry.  * `s3` - The secret key for the S3 bucket. * `openllm` -  The access token for huggingface.co and is supplied to the launched container via the `HF_TOKEN` environment variable.bucket. * `ngc` - The NVIDIA NGC apikey.", alias="secretKey")
     type: StrictStr = Field(description="The type of this model registry. Must be one of the values: (s3, http, openllm, ngc). * `s3` - Configuration to enable access to an s3 bucket. * `openllm` - Configuration to enable direct download of OpenLLM models from huggingface.co.   Provide your access token in the `secretKey` field. * `ngc` -  Configuration to enable direct download from the NVIDA NGC: AI Development Catalog. * `http` - Not yet supported.  Configuration to enable model download from a protected http endpoint that requires login.")
-    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "modifiedAt", "name", "secretKey", "type"]
+    __properties: ClassVar[List[str]] = ["accessKey", "bucket", "endpointUrl", "id", "insecureHttps", "modifiedAt", "name", "secretKey", "type"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -53,15 +55,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TrainedModelRegistryRequest from a JSON string"""
+        """Create an instance of TrainedModelRegistry from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,25 +78,27 @@
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Dict) -> Self:
-        """Create an instance of TrainedModelRegistryRequest from a dict"""
+        """Create an instance of TrainedModelRegistry from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "accessKey": obj.get("accessKey"),
             "bucket": obj.get("bucket"),
             "endpointUrl": obj.get("endpointUrl"),
+            "id": obj.get("id"),
+            "insecureHttps": obj.get("insecureHttps"),
             "modifiedAt": obj.get("modifiedAt"),
             "name": obj.get("name"),
             "secretKey": obj.get("secretKey"),
             "type": obj.get("type")
         })
         return _obj
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/user.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/user_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4.dev5/aiolirest/models/user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/aiolirest/rest.py` & `aioli_sdk-0.2.4.dev5/aiolirest/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev3
+    The version of the OpenAPI document: 0.2.4-dev5
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev3/setup.py` & `aioli_sdk-0.2.4.dev5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-dev3",
+    version="0.2.4-dev5",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

