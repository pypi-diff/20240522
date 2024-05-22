# Comparing `tmp/swh_deposit-2.2.1.tar.gz` & `tmp/swh_deposit-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_deposit-2.2.1.tar", last modified: Thu Apr 18 10:24:03 2024, max compression
+gzip compressed data, was "swh_deposit-2.2.2.tar", last modified: Wed May 22 16:19:45 2024, max compression
```

## Comparing `swh_deposit-2.2.1.tar` & `swh_deposit-2.2.2.tar`

### file list

```diff
@@ -1,341 +1,341 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      350 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      207 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1507 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      831 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/bin/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/Makefile
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      130 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/content.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      322 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      381 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit_atom.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      492 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/create_deposit_with_metadata.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/default-setup
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/download-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)       60 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/home.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      551 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/replace-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)       91 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/service-document.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      256 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/status.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      582 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/update-deposit-with-another-archive.sh
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      252 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/bin/update-status.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)      569 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.801169 swh_deposit-2.2.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3230 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/api-documentation.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8816 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/metadata.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1504 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/register-account.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8033 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/use-cases.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14875 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/api/user-manual.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      653 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      169 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/endpoints/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3371 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/collection.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1864 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/content.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2342 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/service-document.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3488 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/status.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      996 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/update-media.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      884 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/endpoints/update-metadata.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.805168 swh_deposit-2.2.1/docs/images/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-authentication-basic.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      977 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-authentication-keycloak.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      929 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-create-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1151 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-delete-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1460 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-update-chart.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1005 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-checking.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1208 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-loading.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1139 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/deposit-workflow-reception.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/images/status.uml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      372 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/index.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/docs/internals/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1646 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/authentication.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/dev-environment.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      299 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3534 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/loading-workflow.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4191 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/internals/prod-environment.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       60 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/metadata.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/spec-api.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/docs/specs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       59 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/blueprint.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1216 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/metadata_example.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13782 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/protocol-reference.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)    26123 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/spec-loading.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4118 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/specs/spec-meta-deposit.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/docs/user-manual.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1008 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2007 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      461 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-server.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      138 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-swh-server.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      155 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/requirements.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.785169 swh_deposit-2.2.1/resources/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.809168 swh_deposit-2.2.1/resources/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       46 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/resources/deposit/server.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-04-18 10:24:03.877168 swh_deposit-2.2.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.785169 swh_deposit-2.2.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.817168 swh_deposit-2.2.1/swh/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17249 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/checks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6094 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/collection.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45766 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/content.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1827 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5311 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/edit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3140 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/edit_media.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/api/private/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2624 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     9121 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_check.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7287 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8441 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_read.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3892 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/deposit_update_status.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2713 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/private/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1455 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/service_document.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1615 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/state.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/sword_edit.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1119 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/api/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/apps.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6082 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/auth.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1215 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8348 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    20150 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/cli/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    28542 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4025 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6080 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/errors.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1345 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/exception.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/fixtures/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/fixtures/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      194 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/fixtures/deposit_data.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/gunicorn_config.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.821168 swh_deposit-2.2.1/swh/deposit/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1397 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/checker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      657 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/loader/tasks.py
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1748 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/manage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/migrations/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5264 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0002_depositrequest_archive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0003_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      367 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0004_delete_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      908 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      518 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0006_depositclient_url.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      450 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0007_auto_20171129_1609.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      917 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0009_deposit_parent.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      883 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0012_deposit_status_detail.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      817 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1359 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      878 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      612 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12150 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0018_migrate_swhids.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      582 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      858 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1857 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      897 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/migrations/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8981 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/models.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/parsers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/py.typed
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/settings/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3446 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/development.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4677 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/production.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/settings/testing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/css/
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16840 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/css/bootstrap-responsive.min.css
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8833 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/css/style.css
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.829168 swh_deposit-2.2.1/swh/deposit/static/img/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      868 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/arrow-up-small.png
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.833168 swh_deposit-2.2.1/swh/deposit/static/img/icons/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1961 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16114 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17138 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    23808 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45250 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.png
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11585 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.svg
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/static/robots.txt
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.833168 swh_deposit-2.2.1/swh/deposit/templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      505 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/api.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.837168 swh_deposit-2.2.1/swh/deposit/templates/deposit/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      492 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/collection_list.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      840 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/content.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_info.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_receipt.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/error.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1357 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/service_document.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1501 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/deposit/state.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1571 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/homepage.html
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/layout.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.837168 swh_deposit-2.2.1/swh/deposit/templates/rest_framework/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/templates/rest_framework/api.html
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.841168 swh_deposit-2.2.1/swh/deposit/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.849168 swh_deposit-2.2.1/swh/deposit/tests/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2730 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      941 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_basic_auth.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    43592 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_checks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3499 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4256 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5083 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    26349 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_atom.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10039 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_binary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14940 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_multipart.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8201 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3860 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_converters.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4356 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_delete.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_check.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12960 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_list.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6169 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17497 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6857 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4175 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_schedule.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5193 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_state.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4695 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18690 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_atom.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13760 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_binary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1781 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_exception.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2435 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_get_file.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_keycloak_auth.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3586 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_parsers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3051 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/api/test_service_document.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.853168 swh_deposit-2.2.1/swh/deposit/tests/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10494 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/test_admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    38637 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/cli/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7496 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18049 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.789169 swh_deposit-2.2.1/swh/deposit/tests/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.853168 swh_deposit-2.2.1/swh/deposit/tests/data/archives/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/atom/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       73 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1349 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       74 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-empty-body.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      208 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-ko.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      111 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-minimal.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      501 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      639 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      413 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      463 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      630 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      484 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data0.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      253 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data1.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data2.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data3.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      695 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1021 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-only-create-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-update-in-place.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      346 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-cli.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      527 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/atom/metadata.xml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1209 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1164 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.861168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1240 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
--rw-r--r--   0 jenkins    (115) jenkins    (120)      792 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1218 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)      812 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1636 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.865168 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1217 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1634 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1635 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
--rw-r--r--   0 jenkins    (115) jenkins    (120)      750 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4190 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.789169 swh_deposit-2.2.1/swh/deposit/tests/loader/data/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       20 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/hello.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       13 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/http_example.org/hello_you
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2036 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
--rw-r--r--   0 jenkins    (115) jenkins    (120)   725946 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
--rw-r--r--   0 jenkins    (115) jenkins    (120)        5 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
--rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1233 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_checker.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7064 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2387 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/loader/test_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2466 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7253 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_client_module.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1050 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2031 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_gunicorn_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      762 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5134 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_migrations.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7679 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests/test_utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.869168 swh_deposit-2.2.1/swh/deposit/tests_migration/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/tests_migration/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1394 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/urls.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7713 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.873168 swh_deposit-2.2.1/swh/deposit/xsd/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3808 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/xsd/codemeta.xsd
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2699 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/swh/deposit/xsd/swh.xsd
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-04-18 10:24:03.873168 swh_deposit-2.2.1/swh.deposit.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7418 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11667 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      109 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      755 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-04-18 10:24:03.000000 swh_deposit-2.2.1/swh.deposit.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1289 2024-04-18 10:23:57.000000 swh_deposit-2.2.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.099334 swh_deposit-2.2.2/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      350 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      207 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1507 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      117 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      831 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7421 2024-05-22 16:19:45.099334 swh_deposit-2.2.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.015335 swh_deposit-2.2.2/bin/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      959 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/Makefile
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      130 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/content.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      322 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/create_deposit.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      381 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/create_deposit_atom.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      492 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/create_deposit_with_metadata.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       94 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/default-setup
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      109 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/download-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)       60 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/home.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      551 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/replace-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)       91 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/service-document.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      256 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/status.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      582 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/update-deposit-with-another-archive.sh
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      252 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/bin/update-status.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      569 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.019335 swh_deposit-2.2.2/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4279 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.019335 swh_deposit-2.2.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.019335 swh_deposit-2.2.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.019335 swh_deposit-2.2.2/docs/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3230 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/api-documentation.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      181 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8816 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/metadata.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1504 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/register-account.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8033 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/use-cases.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14875 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/api/user-manual.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      653 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      169 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.023335 swh_deposit-2.2.2/docs/endpoints/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3371 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/collection.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1864 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/content.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2342 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/service-document.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3488 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/status.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      996 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/update-media.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      884 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/endpoints/update-metadata.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.023335 swh_deposit-2.2.2/docs/images/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      687 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-authentication-basic.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      977 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-authentication-keycloak.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      929 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-create-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1151 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-delete-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1460 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-update-chart.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1005 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-workflow-checking.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1208 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-workflow-loading.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1139 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/deposit-workflow-reception.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      542 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/images/status.uml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      372 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/index.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.027335 swh_deposit-2.2.2/docs/internals/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1646 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/internals/authentication.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/internals/dev-environment.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      299 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/internals/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3534 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/internals/loading-workflow.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4191 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/internals/prod-environment.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       60 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/metadata.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/spec-api.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.027335 swh_deposit-2.2.2/docs/specs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       59 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/blueprint.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      179 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1216 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/metadata_example.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13782 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/protocol-reference.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    26123 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/spec-loading.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4118 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/specs/spec-meta-deposit.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/docs/user-manual.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1008 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2007 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      461 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements-server.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      139 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements-swh-server.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      169 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      225 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      155 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/requirements.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.003335 swh_deposit-2.2.2/resources/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.027335 swh_deposit-2.2.2/resources/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       46 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/resources/deposit/server.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-22 16:19:45.103334 swh_deposit-2.2.2/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.003335 swh_deposit-2.2.2/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.035334 swh_deposit-2.2.2/swh/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.039334 swh_deposit-2.2.2/swh/deposit/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17249 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/checks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6094 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/collection.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45758 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1362 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/content.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1827 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5311 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/edit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3140 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/edit_media.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.039334 swh_deposit-2.2.2/swh/deposit/api/private/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2624 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     9113 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/deposit_check.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7287 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/deposit_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8441 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/deposit_read.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3892 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/deposit_update_status.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2713 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/private/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1455 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/service_document.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1615 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/state.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3031 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/sword_edit.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2476 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1119 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/api/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/apps.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6082 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/auth.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.039334 swh_deposit-2.2.2/swh/deposit/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1215 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8348 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/cli/admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    20150 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/cli/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    28542 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4025 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6080 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/errors.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1345 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/exception.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.039334 swh_deposit-2.2.2/swh/deposit/fixtures/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/fixtures/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      194 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/fixtures/deposit_data.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      456 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/gunicorn_config.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.043334 swh_deposit-2.2.2/swh/deposit/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      245 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1397 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/loader/checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      657 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/loader/tasks.py
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1748 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/manage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.047334 swh_deposit-2.2.2/swh/deposit/migrations/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5264 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      551 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0002_depositrequest_archive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0003_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      367 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0004_delete_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      908 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0005_auto_20171019_1436.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      518 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0006_depositclient_url.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      450 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0007_auto_20171129_1609.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      917 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0008_auto_20171130_1513.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      609 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0009_deposit_parent.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0010_auto_20180110_0953.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      883 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0011_auto_20180115_1510.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      480 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0012_deposit_status_detail.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      462 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      817 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0014_auto_20180720_1221.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1359 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0015_depositrequest_typemigration.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      878 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0016_auto_20190507_1408.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      612 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0017_auto_20190925_0906.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12150 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0018_migrate_swhids.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      516 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0019_auto_20200519_1035.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      582 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0020_auto_20200929_0855.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      858 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1857 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0022_auto_20220223_1542.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      897 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/migrations/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8981 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/models.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/parsers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/py.typed
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.051334 swh_deposit-2.2.2/swh/deposit/settings/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/settings/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3446 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/settings/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1865 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/settings/development.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4677 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/settings/production.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/settings/testing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.051334 swh_deposit-2.2.2/swh/deposit/static/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.051334 swh_deposit-2.2.2/swh/deposit/static/css/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16840 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/css/bootstrap-responsive.min.css
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8833 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/css/style.css
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.051334 swh_deposit-2.2.2/swh/deposit/static/img/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      868 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/arrow-up-small.png
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.055334 swh_deposit-2.2.2/swh/deposit/static/img/icons/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1961 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-32x32.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16114 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17138 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    23808 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45250 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/swh-logo-deposit.png
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11585 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/img/swh-logo-deposit.svg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/static/robots.txt
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.055334 swh_deposit-2.2.2/swh/deposit/templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      505 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/api.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.059334 swh_deposit-2.2.2/swh/deposit/templates/deposit/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      492 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/collection_list.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      840 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/content.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      274 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/deposit_info.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1249 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/deposit_receipt.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      414 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/error.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1357 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/service_document.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1501 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/deposit/state.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1571 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/homepage.html
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3170 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/layout.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.059334 swh_deposit-2.2.2/swh/deposit/templates/rest_framework/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      168 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/templates/rest_framework/api.html
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.063334 swh_deposit-2.2.2/swh/deposit/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.071334 swh_deposit-2.2.2/swh/deposit/tests/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2730 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      941 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_basic_auth.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    43592 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_checks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3499 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4256 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_add_to_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5083 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    26349 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_atom.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10039 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_binary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14940 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_multipart.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8201 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_reuse_slug.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3860 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_converters.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4356 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_delete.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10240 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_check.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12960 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_list.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6169 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_read_archive.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17497 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_read_metadata.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6857 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_update_status.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4209 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_schedule.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5193 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_state.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4695 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18690 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update_atom.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13760 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update_binary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1781 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_exception.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2435 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_get_file.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_keycloak_auth.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3586 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_parsers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3051 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/api/test_service_document.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.071334 swh_deposit-2.2.2/swh/deposit/tests/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/cli/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10475 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/cli/test_admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    38637 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/cli/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7496 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18091 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.007335 swh_deposit-2.2.2/swh/deposit/tests/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.071334 swh_deposit-2.2.2/swh/deposit/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      102 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.079334 swh_deposit-2.2.2/swh/deposit/tests/data/atom/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3613 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/codemeta-sample.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       73 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1349 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       74 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-empty-body.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      220 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      208 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-ko.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      111 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-minimal.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      421 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      362 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      158 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      501 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      639 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      459 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      413 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      463 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      630 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      484 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data0.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      253 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data1.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data2.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data3.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      695 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1021 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      449 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-only-create-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      263 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-update-in-place.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      346 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/error-cli.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2060 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/error-with-decimal.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      527 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/atom/metadata.xml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.079334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.swh.test/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1209 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1164 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_test
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.083334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.list/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1469 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.083334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1214 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1240 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1196 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      792 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.083334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1218 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      812 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.083334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.status/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1212 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1636 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.087334 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1217 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1634 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1635 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      750 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.087334 swh_deposit-2.2.2/swh/deposit/tests/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4206 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      601 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.007335 swh_deposit-2.2.2/swh/deposit/tests/loader/data/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.087334 swh_deposit-2.2.2/swh/deposit/tests/loader/data/http_example.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       20 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/http_example.org/hello.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       13 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/http_example.org/hello_you
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.091334 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2036 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
+-rw-r--r--   0 jenkins    (115) jenkins    (120)   725946 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        5 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.091334 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_nowhere.org/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       23 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1233 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/test_checker.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7064 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/test_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2387 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/loader/test_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2466 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7253 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_client_module.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1050 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2042 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      762 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5134 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_migrations.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7679 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests/test_utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.091334 swh_deposit-2.2.2/swh/deposit/tests_migration/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/tests_migration/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1394 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/urls.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7713 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.091334 swh_deposit-2.2.2/swh/deposit/xsd/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3808 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/xsd/codemeta.xsd
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2699 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/swh/deposit/xsd/swh.xsd
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 16:19:45.091334 swh_deposit-2.2.2/swh.deposit.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7421 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11667 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      109 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      758 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-22 16:19:44.000000 swh_deposit-2.2.2/swh.deposit.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1289 2024-05-22 16:19:38.000000 swh_deposit-2.2.2/tox.ini
```

### Comparing `swh_deposit-2.2.1/.pre-commit-config.yaml` & `swh_deposit-2.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/CODE_OF_CONDUCT.md` & `swh_deposit-2.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/LICENSE` & `swh_deposit-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/Makefile.local` & `swh_deposit-2.2.2/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/PKG-INFO` & `swh_deposit-2.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 2.2.1
+Version: 2.2.2
 Summary: Software Heritage deposit server
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-deposit
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-deposit/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-deposit/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-deposit.git
@@ -18,35 +18,35 @@
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: iso8601
 Requires-Dist: requests
 Requires-Dist: sentry-sdk
 Requires-Dist: swh.core[http]>=3.0.0
-Requires-Dist: swh.model>=4.4.0
+Requires-Dist: swh.model>=6.13.0
 Provides-Extra: server
 Requires-Dist: django; extra == "server"
 Requires-Dist: djangorestframework; extra == "server"
 Requires-Dist: psycopg2; extra == "server"
 Requires-Dist: setuptools; extra == "server"
 Requires-Dist: xmlschema; extra == "server"
 Requires-Dist: pymemcache; extra == "server"
 Requires-Dist: swh.core[http]>=0.4; extra == "server"
 Requires-Dist: swh.loader.core>=0.0.71; extra == "server"
-Requires-Dist: swh.scheduler>=0.7.0; extra == "server"
-Requires-Dist: swh.model>=0.3.8; extra == "server"
+Requires-Dist: swh.scheduler>=2.3.0; extra == "server"
+Requires-Dist: swh.model>=6.13.0; extra == "server"
 Requires-Dist: swh.auth[django]>=0.5.3; extra == "server"
 Requires-Dist: swh.storage>=0.28.0; extra == "server"
 Provides-Extra: azure
 Requires-Dist: django-storages[azure]; extra == "azure"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-django; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
-Requires-Dist: swh.scheduler[testing]>=2.0.0; extra == "testing"
+Requires-Dist: swh.scheduler[testing]>=2.3.0; extra == "testing"
 Requires-Dist: swh.loader.core[testing]; extra == "testing"
 Requires-Dist: pytest-postgresql>=5; extra == "testing"
 Requires-Dist: requests_mock; extra == "testing"
 Requires-Dist: django-stubs; extra == "testing"
 Requires-Dist: djangorestframework-stubs>=1.4; extra == "testing"
 Requires-Dist: django-test-migrations; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
@@ -55,16 +55,16 @@
 Requires-Dist: djangorestframework; extra == "testing"
 Requires-Dist: psycopg2; extra == "testing"
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: xmlschema; extra == "testing"
 Requires-Dist: pymemcache; extra == "testing"
 Requires-Dist: swh.core[http]>=0.4; extra == "testing"
 Requires-Dist: swh.loader.core>=0.0.71; extra == "testing"
-Requires-Dist: swh.scheduler>=0.7.0; extra == "testing"
-Requires-Dist: swh.model>=0.3.8; extra == "testing"
+Requires-Dist: swh.scheduler>=2.3.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.auth[django]>=0.5.3; extra == "testing"
 Requires-Dist: swh.storage>=0.28.0; extra == "testing"
 Requires-Dist: django-storages[azure]; extra == "testing"
 
 Software Heritage - Deposit
 ===========================
```

### Comparing `swh_deposit-2.2.1/README.rst` & `swh_deposit-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/bin/Makefile` & `swh_deposit-2.2.2/bin/Makefile`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/bin/replace-deposit-archive.sh` & `swh_deposit-2.2.2/bin/replace-deposit-archive.sh`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/bin/update-deposit-with-another-archive.sh` & `swh_deposit-2.2.2/bin/update-deposit-with-another-archive.sh`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/conftest.py` & `swh_deposit-2.2.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/README.rst` & `swh_deposit-2.2.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/api/api-documentation.rst` & `swh_deposit-2.2.2/docs/api/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/api/metadata.rst` & `swh_deposit-2.2.2/docs/api/metadata.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/api/register-account.rst` & `swh_deposit-2.2.2/docs/api/register-account.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/api/use-cases.rst` & `swh_deposit-2.2.2/docs/api/use-cases.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/api/user-manual.rst` & `swh_deposit-2.2.2/docs/api/user-manual.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/cli.rst` & `swh_deposit-2.2.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/collection.rst` & `swh_deposit-2.2.2/docs/endpoints/collection.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/content.rst` & `swh_deposit-2.2.2/docs/endpoints/content.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/service-document.rst` & `swh_deposit-2.2.2/docs/endpoints/service-document.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/status.rst` & `swh_deposit-2.2.2/docs/endpoints/status.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/update-media.rst` & `swh_deposit-2.2.2/docs/endpoints/update-media.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/endpoints/update-metadata.rst` & `swh_deposit-2.2.2/docs/endpoints/update-metadata.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-authentication-basic.uml` & `swh_deposit-2.2.2/docs/images/deposit-authentication-basic.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-authentication-keycloak.uml` & `swh_deposit-2.2.2/docs/images/deposit-authentication-keycloak.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-create-chart.uml` & `swh_deposit-2.2.2/docs/images/deposit-create-chart.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-delete-chart.uml` & `swh_deposit-2.2.2/docs/images/deposit-delete-chart.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-update-chart.uml` & `swh_deposit-2.2.2/docs/images/deposit-update-chart.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-workflow-checking.uml` & `swh_deposit-2.2.2/docs/images/deposit-workflow-checking.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-workflow-loading.uml` & `swh_deposit-2.2.2/docs/images/deposit-workflow-loading.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/deposit-workflow-reception.uml` & `swh_deposit-2.2.2/docs/images/deposit-workflow-reception.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/images/status.uml` & `swh_deposit-2.2.2/docs/images/status.uml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/internals/authentication.rst` & `swh_deposit-2.2.2/docs/internals/authentication.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/internals/dev-environment.rst` & `swh_deposit-2.2.2/docs/internals/dev-environment.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/internals/loading-workflow.rst` & `swh_deposit-2.2.2/docs/internals/loading-workflow.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/internals/prod-environment.rst` & `swh_deposit-2.2.2/docs/internals/prod-environment.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/specs/metadata_example.xml` & `swh_deposit-2.2.2/docs/specs/metadata_example.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/specs/protocol-reference.rst` & `swh_deposit-2.2.2/docs/specs/protocol-reference.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/specs/spec-loading.rst` & `swh_deposit-2.2.2/docs/specs/spec-loading.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/docs/specs/spec-meta-deposit.rst` & `swh_deposit-2.2.2/docs/specs/spec-meta-deposit.rst`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/mypy.ini` & `swh_deposit-2.2.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/pyproject.toml` & `swh_deposit-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/checks.py` & `swh_deposit-2.2.2/swh/deposit/api/checks.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/collection.py` & `swh_deposit-2.2.2/swh/deposit/api/collection.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/common.py` & `swh_deposit-2.2.2/swh/deposit/api/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 )
 from swh.model.swhids import (
     ExtendedObjectType,
     ExtendedSWHID,
     QualifiedSWHID,
     ValidationError,
 )
-from swh.scheduler.utils import create_oneshot_task_dict
+from swh.scheduler.utils import create_oneshot_task
 
 ACCEPT_PACKAGINGS = ["http://purl.org/net/sword/package/SimpleZip"]
 ACCEPT_ARCHIVE_CONTENT_TYPES = ["application/zip", "application/x-tar"]
 
 
 @attr.s
 class ParsedRequestHeaders:
@@ -274,22 +274,22 @@
 
         if not deposit.origin_url:
             deposit.origin_url = guess_deposit_origin_url(deposit)
 
         if self.config["checks"]:
             scheduler = self.scheduler
             if deposit.status == DEPOSIT_STATUS_DEPOSITED and not deposit.check_task_id:
-                task = create_oneshot_task_dict(
+                task = create_oneshot_task(
                     "check-deposit",
                     collection=deposit.collection.name,
                     deposit_id=deposit.id,
                     retries_left=3,
                 )
-                check_task_id = scheduler.create_tasks([task])[0]["id"]
-                deposit.check_task_id = check_task_id
+                check_task_id = scheduler.create_tasks([task])[0].id
+                deposit.check_task_id = str(check_task_id)
 
         deposit.save()
 
     def _deposit_request_put(
         self,
         deposit: Deposit,
         deposit_request_data: Dict[str, Any],
```

### Comparing `swh_deposit-2.2.1/swh/deposit/api/content.py` & `swh_deposit-2.2.2/swh/deposit/api/content.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/converters.py` & `swh_deposit-2.2.2/swh/deposit/api/converters.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/edit.py` & `swh_deposit-2.2.2/swh/deposit/api/edit.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/edit_media.py` & `swh_deposit-2.2.2/swh/deposit/api/edit_media.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/__init__.py` & `swh_deposit-2.2.2/swh/deposit/api/private/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/deposit_check.py` & `swh_deposit-2.2.2/swh/deposit/api/private/deposit_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2017-2023  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from itertools import chain
 import os
 import re
@@ -20,15 +20,15 @@
 from swh.deposit.api.private import APIPrivateView, DepositReadMixin
 from swh.deposit.config import (
     ARCHIVE_TYPE,
     DEPOSIT_STATUS_REJECTED,
     DEPOSIT_STATUS_VERIFIED,
 )
 from swh.deposit.models import Deposit, DepositRequest
-from swh.scheduler.utils import create_oneshot_task_dict
+from swh.scheduler.utils import create_oneshot_task
 
 MANDATORY_ARCHIVE_UNREADABLE = (
     "At least one of its associated archives is not readable"  # noqa
 )
 MANDATORY_ARCHIVE_INVALID = (
     "Mandatory archive is invalid (i.e contains only one archive)"  # noqa
 )
@@ -209,19 +209,19 @@
         if details_dict:
             deposit.status_detail = details_dict
             response["details"] = details_dict
 
         # Deposit ok, then we schedule the deposit loading task (if not already done)
         if deposit_status_ok and not deposit.load_task_id and self.config["checks"]:
             url = deposit.origin_url
-            task = create_oneshot_task_dict(
+            task = create_oneshot_task(
                 "load-deposit", url=url, deposit_id=deposit.id, retries_left=3
             )
-            load_task_id = self.scheduler.create_tasks([task])[0]["id"]
-            deposit.load_task_id = load_task_id
+            load_task_id = self.scheduler.create_tasks([task])[0].id
+            deposit.load_task_id = str(load_task_id)
 
         deposit.save()
 
         return status.HTTP_200_OK, response, "application/json"
 
 
 def reset_content_settings_if_needed(archive) -> None:
```

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/deposit_list.py` & `swh_deposit-2.2.2/swh/deposit/api/private/deposit_list.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/deposit_read.py` & `swh_deposit-2.2.2/swh/deposit/api/private/deposit_read.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/deposit_update_status.py` & `swh_deposit-2.2.2/swh/deposit/api/private/deposit_update_status.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/private/urls.py` & `swh_deposit-2.2.2/swh/deposit/api/private/urls.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/service_document.py` & `swh_deposit-2.2.2/swh/deposit/api/service_document.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/state.py` & `swh_deposit-2.2.2/swh/deposit/api/state.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/sword_edit.py` & `swh_deposit-2.2.2/swh/deposit/api/sword_edit.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/urls.py` & `swh_deposit-2.2.2/swh/deposit/api/urls.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/api/utils.py` & `swh_deposit-2.2.2/swh/deposit/api/utils.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/auth.py` & `swh_deposit-2.2.2/swh/deposit/auth.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/cli/__init__.py` & `swh_deposit-2.2.2/swh/deposit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/cli/admin.py` & `swh_deposit-2.2.2/swh/deposit/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/cli/client.py` & `swh_deposit-2.2.2/swh/deposit/cli/client.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/client.py` & `swh_deposit-2.2.2/swh/deposit/client.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/config.py` & `swh_deposit-2.2.2/swh/deposit/config.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/errors.py` & `swh_deposit-2.2.2/swh/deposit/errors.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/exception.py` & `swh_deposit-2.2.2/swh/deposit/exception.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/loader/checker.py` & `swh_deposit-2.2.2/swh/deposit/loader/checker.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/loader/tasks.py` & `swh_deposit-2.2.2/swh/deposit/loader/tasks.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/manage.py` & `swh_deposit-2.2.2/swh/deposit/manage.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0001_initial.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0002_depositrequest_archive.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0002_depositrequest_archive.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0003_temporaryarchive.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0003_temporaryarchive.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0005_auto_20171019_1436.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0006_depositclient_url.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0006_depositclient_url.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0008_auto_20171130_1513.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0009_deposit_parent.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0009_deposit_parent.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0010_auto_20180110_0953.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0011_auto_20180115_1510.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0014_auto_20180720_1221.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0015_depositrequest_typemigration.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0016_auto_20190507_1408.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0017_auto_20190925_0906.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0018_migrate_swhids.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0018_migrate_swhids.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0019_auto_20200519_1035.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0020_auto_20200929_0855.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0022_auto_20220223_1542.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py` & `swh_deposit-2.2.2/swh/deposit/migrations/0023_alter_deposit_status_detail_alter_deposit_type_and_more.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/models.py` & `swh_deposit-2.2.2/swh/deposit/models.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/parsers.py` & `swh_deposit-2.2.2/swh/deposit/parsers.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/settings/common.py` & `swh_deposit-2.2.2/swh/deposit/settings/common.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/settings/development.py` & `swh_deposit-2.2.2/swh/deposit/settings/development.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/settings/production.py` & `swh_deposit-2.2.2/swh/deposit/settings/production.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/settings/testing.py` & `swh_deposit-2.2.2/swh/deposit/settings/testing.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/css/bootstrap-responsive.min.css` & `swh_deposit-2.2.2/swh/deposit/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/css/style.css` & `swh_deposit-2.2.2/swh/deposit/static/css/style.css`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/arrow-up-small.png` & `swh_deposit-2.2.2/swh/deposit/static/img/arrow-up-small.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png` & `swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png` & `swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png` & `swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png` & `swh_deposit-2.2.2/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.png` & `swh_deposit-2.2.2/swh/deposit/static/img/swh-logo-deposit.png`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/static/img/swh-logo-deposit.svg` & `swh_deposit-2.2.2/swh/deposit/static/img/swh-logo-deposit.svg`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/deposit/content.xml` & `swh_deposit-2.2.2/swh/deposit/templates/deposit/content.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/deposit/deposit_receipt.xml` & `swh_deposit-2.2.2/swh/deposit/templates/deposit/deposit_receipt.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/deposit/service_document.xml` & `swh_deposit-2.2.2/swh/deposit/templates/deposit/service_document.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/deposit/state.xml` & `swh_deposit-2.2.2/swh/deposit/templates/deposit/state.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/homepage.html` & `swh_deposit-2.2.2/swh/deposit/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/templates/layout.html` & `swh_deposit-2.2.2/swh/deposit/templates/layout.html`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/conftest.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_basic_auth.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_checks.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_checks.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_add_to_origin.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_list.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_list.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_atom.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_atom.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_binary.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_binary.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_post_multipart.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_post_multipart.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_collection_reuse_slug.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_converters.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_delete.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_delete.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_check.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_check.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_list.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_list.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_read_archive.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_read_metadata.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_private_update_status.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_schedule.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_schedule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2021  The Software Heritage developers
+# Copyright (C) 2020-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import copy
 import datetime
 
@@ -14,14 +14,15 @@
     COL_IRI,
     DEPOSIT_STATUS_DEPOSITED,
     DEPOSIT_STATUS_PARTIAL,
     SE_IRI,
 )
 from swh.deposit.parsers import parse_xml
 from swh.deposit.utils import NAMESPACES
+from swh.scheduler.model import TaskArguments
 
 
 @pytest.fixture()
 def deposit_config(deposit_config):
     """Overrides the `deposit_config` fixture define in swh/deposit/tests/conftest.py
     to re-enable the checks."""
     config_d = copy.deepcopy(deposit_config)
@@ -36,25 +37,25 @@
 def assert_task_for_deposit(
     swh_scheduler, deposit_id, timestamp_before_call, timestamp_after_call
 ):
     tasks = swh_scheduler.grab_ready_tasks("check-deposit")
     assert len(tasks) == 1
     task = tasks[0]
 
-    assert timestamp_before_call <= task.pop("next_run") <= timestamp_after_call
-    assert task["arguments"] == {
-        "args": [],
-        "kwargs": {
+    assert timestamp_before_call <= task.next_run <= timestamp_after_call
+    assert task.arguments == TaskArguments(
+        args=[],
+        kwargs={
             "collection": "test",
             "deposit_id": deposit_id,
         },
-    }
-    assert task["policy"] == "oneshot"
-    assert task["type"] == "check-deposit"
-    assert task["retries_left"] == 3
+    )
+    assert task.policy == "oneshot"
+    assert task.type == "check-deposit"
+    assert task.retries_left == 3
 
 
 def test_add_deposit_schedules_check(
     authenticated_client, deposit_collection, sample_archive, swh_scheduler
 ):
     """Posting deposit by POST Col-IRI creates a checker task"""
     tasks = swh_scheduler.grab_ready_tasks("check-deposit")
```

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_state.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_state.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_atom.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update_atom.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_deposit_update_binary.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_deposit_update_binary.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_exception.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_get_file.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_get_file.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_keycloak_auth.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_keycloak_auth.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_parsers.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_parsers.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/api/test_service_document.py` & `swh_deposit-2.2.2/swh/deposit/tests/api/test_service_document.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/cli/test_admin.py` & `swh_deposit-2.2.2/swh/deposit/tests/cli/test_admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# Copyright (C) 2019-2020 The Software Heritage developers
+# Copyright (C) 2019-2024 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
 
 from swh.deposit.cli.admin import admin as cli
 from swh.deposit.config import (
     DEPOSIT_STATUS_DEPOSITED,
     DEPOSIT_STATUS_PARTIAL,
     DEPOSIT_STATUS_VERIFIED,
 )
 from swh.deposit.models import DepositClient, DepositCollection
-from swh.scheduler.utils import create_oneshot_task_dict
+from swh.scheduler.utils import create_oneshot_task
 
 
 @pytest.fixture(autouse=True)
 def enable_db_access_for_all_tests(db):
     pass
 
 
@@ -316,24 +316,24 @@
 def test_cli_admin_reschedule_nominal(cli_runner, complete_deposit, swh_scheduler):
     """Rescheduling deposit with no load_task_id cannot work."""
     deposit = complete_deposit
 
     from swh.deposit.models import Deposit
 
     # create a task to keep a reference on it
-    task = create_oneshot_task_dict(
+    task = create_oneshot_task(
         "load-deposit", url=deposit.origin_url, deposit_id=deposit.id, retries_left=3
     )
     scheduled_task = swh_scheduler.create_tasks([task])[0]
     # disable it
-    swh_scheduler.set_status_tasks([scheduled_task["id"]], status="disabled")
+    swh_scheduler.set_status_tasks([scheduled_task.id], status="disabled")
 
     # Now update the deposit state with some swhid and relevant load_task_id
     deposit = complete_deposit
-    deposit.load_task_id = scheduled_task["id"]
+    deposit.load_task_id = scheduled_task.id
     deposit.swhid = "swh:1:dir:02ed6084fb0e8384ac58980e07548a547431cf74"
     deposit.swhid_context = f"{deposit.swhid};origin=https://url/external-id"
     deposit.save()
 
     # Reschedule it
     result = cli_runner.invoke(
         cli, ["deposit", "reschedule", "--deposit-id", deposit.id]
@@ -346,8 +346,8 @@
     # got reset to a state which allows rescheduling
     assert deposit.id
     assert deposit.swhid is None
     assert deposit.swhid_context is None
     assert deposit.status == DEPOSIT_STATUS_VERIFIED
 
     task = swh_scheduler.search_tasks(task_id=deposit.load_task_id)[0]
-    assert task["status"] == "next_run_not_scheduled"
+    assert task.status == "next_run_not_scheduled"
```

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/cli/test_client.py` & `swh_deposit-2.2.2/swh/deposit/tests/cli/test_client.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/common.py` & `swh_deposit-2.2.2/swh/deposit/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/conftest.py` & `swh_deposit-2.2.2/swh/deposit/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2023  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import base64
 from copy import deepcopy
 from functools import partial
@@ -170,29 +170,31 @@
 
 @pytest.fixture(autouse=True)
 def deposit_autoconfig(deposit_config_path):
     """Enforce config for deposit classes inherited from APIConfig."""
     cfg = read(deposit_config_path)
 
     if "scheduler" in cfg:
+        from swh.scheduler.model import TaskType
+
         # scheduler setup: require the check-deposit and load-deposit tasks
         scheduler = get_scheduler(**cfg["scheduler"])
         task_types = [
-            {
-                "type": "check-deposit",
-                "backend_name": "swh.deposit.loader.tasks.ChecksDepositTsk",
-                "description": "Check deposit metadata/archive before loading",
-                "num_retries": 3,
-            },
-            {
-                "type": "load-deposit",
-                "backend_name": "swh.loader.package.deposit.tasks.LoadDeposit",
-                "description": "Loading deposit archive into swh archive",
-                "num_retries": 3,
-            },
+            TaskType(
+                type="check-deposit",
+                backend_name="swh.deposit.loader.tasks.ChecksDepositTsk",
+                description="Check deposit metadata/archive before loading",
+                num_retries=3,
+            ),
+            TaskType(
+                type="load-deposit",
+                backend_name="swh.loader.package.deposit.tasks.LoadDeposit",
+                description="Loading deposit archive into swh archive",
+                num_retries=3,
+            ),
         ]
         for task_type in task_types:
             scheduler.create_task_type(task_type)
 
 
 @pytest.fixture(scope="session")
 def django_db_setup(request, django_db_blocker, postgresql_proc):
```

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/codemeta-sample.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data2.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data2.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-data3.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-data3.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/entry-list-deposits.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/error-with-decimal.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/atom/metadata.xml` & `swh_deposit-2.2.2/swh/deposit/tests/data/atom/metadata.xml`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_test`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status` & `swh_deposit-2.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/common.py` & `swh_deposit-2.2.2/swh/deposit/tests/loader/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 import json
 from typing import Dict, Optional
 
 from swh.deposit.client import PrivateApiDepositClient
 from swh.model.hashutil import hash_to_bytes, hash_to_hex
-from swh.model.model import SnapshotBranch, TargetType
+from swh.model.model import SnapshotBranch, SnapshotTargetType
 from swh.storage.algos.snapshot import snapshot_get_all_branches
 
 CLIENT_TEST_CONFIG = {
     "url": "http://nowhere:9000/",
     "auth": {},  # no authentication in test scenario
 }
 
@@ -88,15 +88,15 @@
 
 def decode_target(branch: Optional[SnapshotBranch]) -> Optional[Dict]:
     """Test helper to ease readability in test"""
     if not branch:
         return None
     target_type = branch.target_type
 
-    if target_type == TargetType.ALIAS:
+    if target_type == SnapshotTargetType.ALIAS:
         decoded_target = branch.target.decode("utf-8")
     else:
         decoded_target = hash_to_hex(branch.target)
 
     return {"target": decoded_target, "target_type": target_type}
```

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/conftest.py` & `swh_deposit-2.2.2/swh/deposit/tests/loader/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta` & `swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw` & `swh_deposit-2.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/test_checker.py` & `swh_deposit-2.2.2/swh/deposit/tests/loader/test_checker.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/test_client.py` & `swh_deposit-2.2.2/swh/deposit/tests/loader/test_client.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/loader/test_tasks.py` & `swh_deposit-2.2.2/swh/deposit/tests/loader/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_backend.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_client_module.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_client_module.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_common.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_config.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_gunicorn_config.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_gunicorn_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,72 @@
-# Copyright (C) 2019-2020  The Software Heritage developers
+# Copyright (C) 2019-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
-from unittest.mock import patch
 
 import swh.deposit.gunicorn_config as gunicorn_config
 
+django_integration = object()  # unique object to check for equality
 
-def test_post_fork_default():
-    with patch("sentry_sdk.init") as sentry_sdk_init:
-        gunicorn_config.post_fork(None, None)
 
-    sentry_sdk_init.assert_not_called()
+def test_post_fork_default(mocker):
+    mocker.patch(
+        "swh.deposit.gunicorn_config.DjangoIntegration", new=lambda: django_integration
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    gunicorn_config.post_fork(None, None)
+
+    sentry_sdk_init.assert_called_once_with(
+        dsn=None,
+        integrations=[django_integration],
+        environment=None,
+        debug=False,
+        release=None,
+    )
 
 
-def test_post_fork_with_dsn_env():
-    django_integration = object()  # unique object to check for equality
-    with patch(
+def test_post_fork_with_dsn_env(mocker):
+    mocker.patch(
         "swh.deposit.gunicorn_config.DjangoIntegration", new=lambda: django_integration
-    ):
-        with patch("sentry_sdk.init") as sentry_sdk_init:
-            with patch.dict(
-                os.environ,
-                {
-                    "SWH_SENTRY_DSN": "test_dsn",
-                    "SWH_SENTRY_ENVIRONMENT": "test",
-                },
-            ):
-                gunicorn_config.post_fork(None, None)
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(
+        os.environ,
+        {
+            "SWH_SENTRY_DSN": "test_dsn",
+            "SWH_SENTRY_ENVIRONMENT": "test",
+        },
+    )
+    gunicorn_config.post_fork(None, None)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[django_integration],
         environment="test",
         debug=False,
         release=None,
     )
 
 
-def test_post_fork_debug():
-    django_integration = object()  # unique object to check for equality
-    with patch(
+def test_post_fork_debug(mocker):
+    mocker.patch(
         "swh.deposit.gunicorn_config.DjangoIntegration", new=lambda: django_integration
-    ):
-        with patch("sentry_sdk.init") as sentry_sdk_init:
-            with patch.dict(
-                os.environ,
-                {
-                    "SWH_SENTRY_DSN": "test_dsn",
-                    "SWH_SENTRY_DEBUG": "1",
-                    "SWH_SENTRY_ENVIRONMENT": "test",
-                },
-            ):
-                gunicorn_config.post_fork(None, None)
+    )
+    sentry_sdk_init = mocker.patch("sentry_sdk.init")
+    mocker.patch.dict(
+        os.environ,
+        {
+            "SWH_SENTRY_DSN": "test_dsn",
+            "SWH_SENTRY_DEBUG": "1",
+            "SWH_SENTRY_ENVIRONMENT": "test",
+        },
+    )
+    gunicorn_config.post_fork(None, None)
 
     sentry_sdk_init.assert_called_once_with(
         dsn="test_dsn",
         integrations=[django_integration],
         environment="test",
         debug=True,
         release=None,
```

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_init.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_migrations.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/tests/test_utils.py` & `swh_deposit-2.2.2/swh/deposit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/urls.py` & `swh_deposit-2.2.2/swh/deposit/urls.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/utils.py` & `swh_deposit-2.2.2/swh/deposit/utils.py`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/xsd/codemeta.xsd` & `swh_deposit-2.2.2/swh/deposit/xsd/codemeta.xsd`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh/deposit/xsd/swh.xsd` & `swh_deposit-2.2.2/swh/deposit/xsd/swh.xsd`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh.deposit.egg-info/PKG-INFO` & `swh_deposit-2.2.2/swh.deposit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 2.2.1
+Version: 2.2.2
 Summary: Software Heritage deposit server
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-deposit
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-deposit/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-deposit/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-deposit.git
@@ -18,35 +18,35 @@
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: click
 Requires-Dist: iso8601
 Requires-Dist: requests
 Requires-Dist: sentry-sdk
 Requires-Dist: swh.core[http]>=3.0.0
-Requires-Dist: swh.model>=4.4.0
+Requires-Dist: swh.model>=6.13.0
 Provides-Extra: server
 Requires-Dist: django; extra == "server"
 Requires-Dist: djangorestframework; extra == "server"
 Requires-Dist: psycopg2; extra == "server"
 Requires-Dist: setuptools; extra == "server"
 Requires-Dist: xmlschema; extra == "server"
 Requires-Dist: pymemcache; extra == "server"
 Requires-Dist: swh.core[http]>=0.4; extra == "server"
 Requires-Dist: swh.loader.core>=0.0.71; extra == "server"
-Requires-Dist: swh.scheduler>=0.7.0; extra == "server"
-Requires-Dist: swh.model>=0.3.8; extra == "server"
+Requires-Dist: swh.scheduler>=2.3.0; extra == "server"
+Requires-Dist: swh.model>=6.13.0; extra == "server"
 Requires-Dist: swh.auth[django]>=0.5.3; extra == "server"
 Requires-Dist: swh.storage>=0.28.0; extra == "server"
 Provides-Extra: azure
 Requires-Dist: django-storages[azure]; extra == "azure"
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-django; extra == "testing"
 Requires-Dist: pytest-mock; extra == "testing"
-Requires-Dist: swh.scheduler[testing]>=2.0.0; extra == "testing"
+Requires-Dist: swh.scheduler[testing]>=2.3.0; extra == "testing"
 Requires-Dist: swh.loader.core[testing]; extra == "testing"
 Requires-Dist: pytest-postgresql>=5; extra == "testing"
 Requires-Dist: requests_mock; extra == "testing"
 Requires-Dist: django-stubs; extra == "testing"
 Requires-Dist: djangorestframework-stubs>=1.4; extra == "testing"
 Requires-Dist: django-test-migrations; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
@@ -55,16 +55,16 @@
 Requires-Dist: djangorestframework; extra == "testing"
 Requires-Dist: psycopg2; extra == "testing"
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: xmlschema; extra == "testing"
 Requires-Dist: pymemcache; extra == "testing"
 Requires-Dist: swh.core[http]>=0.4; extra == "testing"
 Requires-Dist: swh.loader.core>=0.0.71; extra == "testing"
-Requires-Dist: swh.scheduler>=0.7.0; extra == "testing"
-Requires-Dist: swh.model>=0.3.8; extra == "testing"
+Requires-Dist: swh.scheduler>=2.3.0; extra == "testing"
+Requires-Dist: swh.model>=6.13.0; extra == "testing"
 Requires-Dist: swh.auth[django]>=0.5.3; extra == "testing"
 Requires-Dist: swh.storage>=0.28.0; extra == "testing"
 Requires-Dist: django-storages[azure]; extra == "testing"
 
 Software Heritage - Deposit
 ===========================
```

### Comparing `swh_deposit-2.2.1/swh.deposit.egg-info/SOURCES.txt` & `swh_deposit-2.2.2/swh.deposit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_deposit-2.2.1/swh.deposit.egg-info/requires.txt` & `swh_deposit-2.2.2/swh.deposit.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 click
 iso8601
 requests
 sentry-sdk
 swh.core[http]>=3.0.0
-swh.model>=4.4.0
+swh.model>=6.13.0
 
 [azure]
 django-storages[azure]
 
 [server]
 django
 djangorestframework
 psycopg2
 setuptools
 xmlschema
 pymemcache
 swh.core[http]>=0.4
 swh.loader.core>=0.0.71
-swh.scheduler>=0.7.0
-swh.model>=0.3.8
+swh.scheduler>=2.3.0
+swh.model>=6.13.0
 swh.auth[django]>=0.5.3
 swh.storage>=0.28.0
 
 [testing]
 pytest
 pytest-django
 pytest-mock
-swh.scheduler[testing]>=2.0.0
+swh.scheduler[testing]>=2.3.0
 swh.loader.core[testing]
 pytest-postgresql>=5
 requests_mock
 django-stubs
 djangorestframework-stubs>=1.4
 django-test-migrations
 types-requests
@@ -39,12 +39,12 @@
 djangorestframework
 psycopg2
 setuptools
 xmlschema
 pymemcache
 swh.core[http]>=0.4
 swh.loader.core>=0.0.71
-swh.scheduler>=0.7.0
-swh.model>=0.3.8
+swh.scheduler>=2.3.0
+swh.model>=6.13.0
 swh.auth[django]>=0.5.3
 swh.storage>=0.28.0
 django-storages[azure]
```

### Comparing `swh_deposit-2.2.1/tox.ini` & `swh_deposit-2.2.2/tox.ini`

 * *Files identical despite different names*

