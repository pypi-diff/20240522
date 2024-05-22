# Comparing `tmp/invenio-records-resources-5.7.0.tar.gz` & `tmp/invenio-records-resources-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-records-resources-5.7.0.tar", last modified: Mon May  6 18:04:17 2024, max compression
+gzip compressed data, was "dist/invenio-records-resources-5.8.0.tar", last modified: Tue May 21 09:20:43 2024, max compression
```

## Comparing `invenio-records-resources-5.7.0.tar` & `invenio-records-resources-5.8.0.tar`

### file list

```diff
@@ -1,475 +1,475 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/tests-feature.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/babel.ini
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/constraints-pypi.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/factories/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/dumpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/calculated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/entity_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/field.py
--rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid_statuscheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/grants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/references/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/files/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/resources/records/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/files/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/links.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/querystr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/sort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/suggest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/results.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/records/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/references/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/services/uow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/invenio_records_resources.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/requirements-feature.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/factories/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/jsonschemas/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/records/
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_modelpid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/records/test_systemfield_pidstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_files_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_faceting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_preference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resource_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/resources/test_resources_etag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_base_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_boolean_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_date_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_number_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_schema_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_text_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/custom_fields/test_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:04:17.000000 invenio-records-resources-5.7.0/tests/services/files/
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/files_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_file_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_file_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_files_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/test_files_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/files/testimage.png
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_results_expand.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_facets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_queryparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_relation_propagation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_revision_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_service_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/services/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/test_invenio_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-06 18:04:12.000000 invenio-records-resources-5.7.0/tests/test_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.github/workflows/tests-feature.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/babel.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/constraints-pypi.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7874 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/factories/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/dumpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/calculated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/entity_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17053 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8455 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/pid_statuscheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/grants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/references/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/files/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/files/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/resources/records/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8263 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/files/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/links.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/querystr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/sort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/suggest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18663 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/records/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/references/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/services/uow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16581 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/invenio_records_resources.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/requirements-feature.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1277 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/factories/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/factories/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/factories/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v1/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v2/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/v7/records/
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/jsonschemas/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/jsonschemas/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v1/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v2/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/v7/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/v7/grants/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/records/
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_systemfield_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_systemfield_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_systemfield_modelpid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_systemfield_pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/records/test_systemfield_pidstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_files_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resource_faceting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resource_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resource_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resource_preference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resource_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/resources/test_resources_etag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_base_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_boolean_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_date_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_number_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_schema_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_text_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/custom_fields/test_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:20:43.000000 invenio-records-resources-5.8.0/tests/services/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/files_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/test_file_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15803 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/test_file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/test_files_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/test_files_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20358 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/files/testimage.png
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9701 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_results_expand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_queryparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6286 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_relation_propagation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_revision_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_service_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/services/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/test_invenio_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 09:20:35.000000 invenio-records-resources-5.8.0/tests/test_tasks.py
```

### Comparing `invenio-records-resources-5.7.0/.editorconfig` & `invenio-records-resources-5.8.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/.github/workflows/pypi-publish.yml` & `invenio-records-resources-5.8.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/.github/workflows/tests-feature.yml` & `invenio-records-resources-5.8.0/.github/workflows/tests-feature.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/.github/workflows/tests.yml` & `invenio-records-resources-5.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/.tx/config` & `invenio-records-resources-5.8.0/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/CHANGES.rst` & `invenio-records-resources-5.8.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
     Invenio-Records-Resources is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 5.8.0 (released 2024-05-21)
+
+- processors: optionally use PyVIPS for image metadata
+
 Version 5.7.0 (released 2024-05-06)
 
 - files-schema: hide `uri` from serialization
 - records: added access field to files
 
 Version 5.6.0 (released 2024-04-23)
```

### Comparing `invenio-records-resources-5.7.0/CONTRIBUTING.rst` & `invenio-records-resources-5.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/LICENSE` & `invenio-records-resources-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/MANIFEST.in` & `invenio-records-resources-5.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/PKG-INFO` & `invenio-records-resources-5.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-resources
-Version: 5.7.0
+Version: 5.8.0
 Summary: Invenio resources module to create REST APIs.
 Home-page: https://github.com/inveniosoftware/invenio-records-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -45,14 +45,18 @@
             Invenio-Records-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 5.8.0 (released 2024-05-21)
+        
+        - processors: optionally use PyVIPS for image metadata
+        
         Version 5.7.0 (released 2024-05-06)
         
         - files-schema: hide `uri` from serialization
         - records: added access field to files
         
         Version 5.6.0 (released 2024-04-23)
```

### Comparing `invenio-records-resources-5.7.0/README.rst` & `invenio-records-resources-5.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/docs/Makefile` & `invenio-records-resources-5.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/docs/conf.py` & `invenio-records-resources-5.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/docs/index.rst` & `invenio-records-resources-5.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/docs/make.bat` & `invenio-records-resources-5.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/errors.py` & `invenio-records-resources-5.8.0/invenio_records_resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/ext.py` & `invenio-records-resources-5.8.0/invenio_records_resources/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/factories/factory.py` & `invenio-records-resources-5.8.0/invenio_records_resources/factories/factory.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/pagination.py` & `invenio-records-resources-5.8.0/invenio_records_resources/pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/proxies.py` & `invenio-records-resources-5.8.0/invenio_records_resources/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/api.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/dumpers.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json` & `invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/definitions-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json` & `invenio-records-resources-5.8.0/invenio_records_resources/records/jsonschemas/definitions-v2.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/models.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/providers.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/resolver.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/calculated.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/calculated.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/entity_reference.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/entity_reference.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/field.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/field.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/files/manager.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/files/manager.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/index.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/index.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/pid_statuscheck.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/pid_statuscheck.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/records/systemfields/relations.py` & `invenio-records-resources-5.8.0/invenio_records_resources/records/systemfields/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/records.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/entity_resolvers/results.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/entity_resolvers/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/grants.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/grants.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/references/registry.py` & `invenio-records-resources-5.8.0/invenio_records_resources/references/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/registry.py` & `invenio-records-resources-5.8.0/invenio_records_resources/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/errors.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/files/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/parser.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/files/parser.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/files/resource.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/files/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/args.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/args.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/headers.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/headers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/resource.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/resources/records/utils.py` & `invenio-records-resources-5.8.0/invenio_records_resources/resources/records/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/components.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/components.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/links.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/results.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/service.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/base/utils.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/base/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/boolean.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/boolean.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/date.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/date.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/errors.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/mappings.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/mappings.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/number.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/number.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/schema.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/text.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/text.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/custom_fields/validate.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/custom_fields/validate.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/errors.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/content.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/content.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/metadata.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/components/processor.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/components/processor.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/generators.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/generators.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/links.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 CERN.
+# Copyright (C) 2021-2024 CERN.
 #
 # Invenio-Records-Resources is free software; you can redistribute it and/or
 # modify it under the terms of the MIT License; see LICENSE file for more
 # details.
 
 """Files processing engine."""
 
-
 import os
 
 
 class ProcessorRunner:
     """Runner for file processors."""
 
     def __init__(self, processors):
```

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/processors/image.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/processors/image.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,40 +21,80 @@
 except pkg_resources.DistributionNotFound:
     # Python module not installed
     HAS_IMAGEMAGICK = False
 except ImportError:
     # ImageMagick notinstalled
     HAS_IMAGEMAGICK = False
 
+try:
+    import pyvips
+
+    HAS_VIPS = True
+except ModuleNotFoundError:
+    # Python module pyvips not installed
+    HAS_VIPS = False
+except OSError:
+    # Underlying library libvips not installed
+    HAS_VIPS = False
+
 
 class ImageMetadataExtractor(FileProcessor):
     """Basic image metadata extractor."""
 
     def can_process(self, file_record):
         """Images can be processed."""
-        if HAS_IMAGEMAGICK:
+        if HAS_IMAGEMAGICK or HAS_VIPS:
             ext = self.file_extension(file_record).lower()
             return ext in current_app.config["RECORDS_RESOURCES_IMAGE_FORMATS"]
         return False
 
-    def process(self, file_record):
-        """Process the file record.
+    def _process_wand(self, file_record):
+        """Process the file record using Wand.
+
+        Warning: Wand (and ImageMagick) actually reads the entire file in memory to
+        extract the image metadata.
 
         Security: Do not execute ImageMagick inside an HTTP request. Always
         execute via e.g. a Celery task. See
         https://docs.wand-py.org/en/0.6.6/guide/security.html
         """
-        # TODO: gracefully deal with errors.
-        # TODO: security
-        width = -1
-        height = -1
-
-        ext = self.file_extension(file_record)[1:]
-
+        width = height = -1
         with file_record.open_stream("rb") as fp:
-            with Image.ping(file=fp, format=ext) as img:
+            with Image.ping(file=fp) as img:
                 # Get image or first frame of sequence
                 img_or_seq = img if not len(img.sequence) else img.sequence[0]
                 width = img_or_seq.width
                 height = img_or_seq.height
+        return width, height
+
+    def _process_vips(self, file_record):
+        """Process the file record using pyvips."""
+        width = height = -1
+        with file_record.open_stream("rb") as fp:
+
+            def _seek_handler(offset, whence):
+                fp.seek(offset, whence)
+                return fp.tell()
+
+            source = pyvips.SourceCustom()
+            source.on_read(fp.read)
+            source.on_seek(_seek_handler)
+
+            image = pyvips.Image.new_from_source(source, "", access="sequential")
+            width = image.width
+            height = image.height
+        return width, height
+
+    def process(self, file_record):
+        """Process the file record."""
+        width = height = -1
+
+        # Prefer VIPS if available
+        if HAS_VIPS:
+            width, height = self._process_vips(file_record)
+        elif HAS_IMAGEMAGICK:
+            width, height = self._process_wand(file_record)
+
         if width > 0 and height > 0:
-            file_record.metadata.update({"width": width, "height": height})
+            metadata = file_record.metadata or {}
+            metadata.update({"width": width, "height": height})
+            file_record.metadata = metadata
```

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/results.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/schema.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/service.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/tasks.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/files/transfer.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/files/transfer.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/data.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/data.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/files.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/files.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/metadata.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/metadata.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/components/relations.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/components/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/config.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/facets.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/labels.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/labels.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/facets/response.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/facets/response.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/links.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/base.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/base.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/facets.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/filter.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/filter.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/pagination.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/querystr.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/querystr.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/params/sort.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/params/sort.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/__init__.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/query.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/query.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/suggest.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/suggest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/queryparser/transformer.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/queryparser/transformer.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/results.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/schema.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/records/service.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/records/service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/references/schema.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/references/schema.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/services/uow.py` & `invenio-records-resources-5.8.0/invenio_records_resources/services/uow.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/tasks.py` & `invenio-records-resources-5.8.0/invenio_records_resources/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-records-resources-5.8.0/invenio_records_resources/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/PKG-INFO` & `invenio-records-resources-5.8.0/invenio_records_resources.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-resources
-Version: 5.7.0
+Version: 5.8.0
 Summary: Invenio resources module to create REST APIs.
 Home-page: https://github.com/inveniosoftware/invenio-records-resources
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -45,14 +45,18 @@
             Invenio-Records-Resources is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 5.8.0 (released 2024-05-21)
+        
+        - processors: optionally use PyVIPS for image metadata
+        
         Version 5.7.0 (released 2024-05-06)
         
         - files-schema: hide `uri` from serialization
         - records: added access field to files
         
         Version 5.6.0 (released 2024-04-23)
```

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/SOURCES.txt` & `invenio-records-resources-5.8.0/invenio_records_resources.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/entry_points.txt` & `invenio-records-resources-5.8.0/invenio_records_resources.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/invenio_records_resources.egg-info/requires.txt` & `invenio-records-resources-5.8.0/invenio_records_resources.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/run-tests.sh` & `invenio-records-resources-5.8.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/setup.cfg` & `invenio-records-resources-5.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/conftest.py` & `invenio-records-resources-5.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/factories/conftest.py` & `invenio-records-resources-5.8.0/tests/factories/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/factories/test_factory.py` & `invenio-records-resources-5.8.0/tests/factories/test_factory.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/factories/test_service.py` & `invenio-records-resources-5.8.0/tests/factories/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/api.py` & `invenio-records-resources-5.8.0/tests/mock_module/api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/config.py` & `invenio-records-resources-5.8.0/tests/mock_module/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/records/record-nofiles-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module/jsonschemas/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v1/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module/mappings/os-v2/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module/mappings/v7/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/models.py` & `invenio-records-resources-5.8.0/tests/mock_module/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/permissions.py` & `invenio-records-resources-5.8.0/tests/mock_module/permissions.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/resource.py` & `invenio-records-resources-5.8.0/tests/mock_module/resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module/schemas.py` & `invenio-records-resources-5.8.0/tests/mock_module/schemas.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v1/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/os-v2/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json` & `invenio-records-resources-5.8.0/tests/mock_module_factory/mappings/v7/grants/grant-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/conftest.py` & `invenio-records-resources-5.8.0/tests/records/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_api.py` & `invenio-records-resources-5.8.0/tests/records/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_dumpers.py` & `invenio-records-resources-5.8.0/tests/records/test_dumpers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_systemfield_files.py` & `invenio-records-resources-5.8.0/tests/records/test_systemfield_files.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_systemfield_index.py` & `invenio-records-resources-5.8.0/tests/records/test_systemfield_index.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_systemfield_modelpid.py` & `invenio-records-resources-5.8.0/tests/records/test_systemfield_modelpid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_systemfield_pid.py` & `invenio-records-resources-5.8.0/tests/records/test_systemfield_pid.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/records/test_systemfield_pidstatus.py` & `invenio-records-resources-5.8.0/tests/records/test_systemfield_pidstatus.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/conftest.py` & `invenio-records-resources-5.8.0/tests/resources/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_files_resource.py` & `invenio-records-resources-5.8.0/tests/resources/test_files_resource.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resource_faceting.py` & `invenio-records-resources-5.8.0/tests/resources/test_resource_faceting.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resource_links.py` & `invenio-records-resources-5.8.0/tests/resources/test_resource_links.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resource_pagination.py` & `invenio-records-resources-5.8.0/tests/resources/test_resource_pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resource_preference.py` & `invenio-records-resources-5.8.0/tests/resources/test_resource_preference.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resource_sorting.py` & `invenio-records-resources-5.8.0/tests/resources/test_resource_sorting.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resources.py` & `invenio-records-resources-5.8.0/tests/resources/test_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/resources/test_resources_etag.py` & `invenio-records-resources-5.8.0/tests/resources/test_resources_etag.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/conftest.py` & `invenio-records-resources-5.8.0/tests/services/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_boolean_cf.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_boolean_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_date_cf.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_date_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_number_cf.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_number_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_schema_cf.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_schema_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_text_cf.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_text_cf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/custom_fields/test_validate.py` & `invenio-records-resources-5.8.0/tests/services/custom_fields/test_validate.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/conftest.py` & `invenio-records-resources-5.8.0/tests/services/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/files_utils.py` & `invenio-records-resources-5.8.0/tests/services/files/files_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/test_file_results.py` & `invenio-records-resources-5.8.0/tests/services/files/test_file_results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/test_file_service.py` & `invenio-records-resources-5.8.0/tests/services/files/test_file_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/test_files_options.py` & `invenio-records-resources-5.8.0/tests/services/files/test_files_options.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/test_files_processing.py` & `invenio-records-resources-5.8.0/tests/services/files/test_files_processing.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/files/testimage.png` & `invenio-records-resources-5.8.0/tests/services/files/testimage.png`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_results.py` & `invenio-records-resources-5.8.0/tests/services/test_results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_results_expand.py` & `invenio-records-resources-5.8.0/tests/services/test_results_expand.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service.py` & `invenio-records-resources-5.8.0/tests/services/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_create.py` & `invenio-records-resources-5.8.0/tests/services/test_service_create.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_facets.py` & `invenio-records-resources-5.8.0/tests/services/test_service_facets.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_pagination.py` & `invenio-records-resources-5.8.0/tests/services/test_service_pagination.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_queryparser.py` & `invenio-records-resources-5.8.0/tests/services/test_service_queryparser.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_relation_propagation.py` & `invenio-records-resources-5.8.0/tests/services/test_service_relation_propagation.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_revision_id.py` & `invenio-records-resources-5.8.0/tests/services/test_service_revision_id.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_service_sort.py` & `invenio-records-resources-5.8.0/tests/services/test_service_sort.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/services/test_utils.py` & `invenio-records-resources-5.8.0/tests/services/test_utils.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/test_invenio_resources.py` & `invenio-records-resources-5.8.0/tests/test_invenio_resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-resources-5.7.0/tests/test_tasks.py` & `invenio-records-resources-5.8.0/tests/test_tasks.py`

 * *Files identical despite different names*

