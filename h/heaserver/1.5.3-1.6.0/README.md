# Comparing `tmp/heaserver-1.5.3.tar.gz` & `tmp/heaserver-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.5.3.tar", last modified: Sun May  5 18:18:09 2024, max compression
+gzip compressed data, was "heaserver-1.6.0.tar", last modified: Tue May 21 23:07:24 2024, max compression
```

## Comparing `heaserver-1.5.3.tar` & `heaserver-1.6.0.tar`

### file list

```diff
@@ -1,299 +1,299 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.995705 heaserver-1.5.3/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.3/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.3/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.3/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7928 2024-05-05 18:18:08.993702 heaserver-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     5933 2024-05-05 17:45:18.000000 heaserver-1.5.3/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.3/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.281294 heaserver-1.5.3/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.281294 heaserver-1.5.3/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.320908 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.322529 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.282872 heaserver-1.5.3/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.283396 heaserver-1.5.3/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.326177 heaserver-1.5.3/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.340959 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.3/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.284957 heaserver-1.5.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.284957 heaserver-1.5.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.382415 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.433268 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     6107 2024-05-03 03:20:50.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500
--rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5775 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5544 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4749 2024-05-03 21:58:58.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.435901 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.3/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.3/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 18:18:08.995705 heaserver-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-05-05 18:17:14.000000 heaserver-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.287582 heaserver-1.5.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.288105 heaserver-1.5.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.532365 heaserver-1.5.3/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.3/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    24613 2024-05-03 22:10:30.000000 heaserver-1.5.3/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.551367 heaserver-1.5.3/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    28250 2024-05-05 18:15:37.000000 heaserver-1.5.3/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.3/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    31583 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.3/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.3/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.3/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.565363 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.592371 heaserver-1.5.3/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-05-02 20:04:27.000000 heaserver-1.5.3/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.3/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.3/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.3/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.636627 heaserver-1.5.3/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40481 2024-05-02 20:04:27.000000 heaserver-1.5.3/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    18431 2024-05-03 21:58:58.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.3/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.3/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.3/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.991711 heaserver-1.5.3/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     7928 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17709 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 18:18:08.000000 heaserver-1.5.3/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.290745 heaserver-1.5.3/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.291280 heaserver-1.5.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.751462 heaserver-1.5.3/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.815224 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.819219 heaserver-1.5.3/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.826212 heaserver-1.5.3/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.841295 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5571 2024-05-03 21:58:58.000000 heaserver-1.5.3/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5997 2024-05-03 21:58:58.000000 heaserver-1.5.3/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.877504 heaserver-1.5.3/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.983722 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:18:08.987709 heaserver-1.5.3/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.3/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.366009 heaserver-1.6.0/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.6.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.6.0/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8851 2024-05-21 23:07:24.363999 heaserver-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6856 2024-05-21 23:05:55.000000 heaserver-1.6.0/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.6.0/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.827937 heaserver-1.6.0/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.827937 heaserver-1.6.0/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.861159 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.863259 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.828937 heaserver-1.6.0/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.828937 heaserver-1.6.0/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.865862 heaserver-1.6.0/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.876101 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.6.0/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.830937 heaserver-1.6.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.830937 heaserver-1.6.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.904681 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.958681 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     6107 2024-05-03 03:20:50.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500
+-rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5994 2024-05-16 15:55:06.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     6084 2024-05-21 20:58:08.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5709 2024-05-07 19:13:00.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5524 2024-05-17 21:51:03.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4846 2024-05-17 00:33:46.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.960710 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16483 2024-05-21 20:53:53.000000 heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.6.0/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.6.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:07:24.366997 heaserver-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-05-21 23:06:48.000000 heaserver-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.832937 heaserver-1.6.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.832937 heaserver-1.6.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.022453 heaserver-1.6.0/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.6.0/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    20215 2024-05-07 19:13:00.000000 heaserver-1.6.0/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1527 2024-05-19 17:24:22.000000 heaserver-1.6.0/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    24632 2024-05-17 23:51:52.000000 heaserver-1.6.0/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.038114 heaserver-1.6.0/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.6.0/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    28035 2024-05-21 20:22:34.000000 heaserver-1.6.0/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.6.0/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31373 2024-05-20 15:23:52.000000 heaserver-1.6.0/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.6.0/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    32395 2024-05-19 17:18:08.000000 heaserver-1.6.0/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.6.0/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    28355 2024-05-20 17:32:54.000000 heaserver-1.6.0/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    17784 2024-05-20 15:17:06.000000 heaserver-1.6.0/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.048072 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.6.0/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.6.0/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.061161 heaserver-1.6.0/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-05-02 20:04:27.000000 heaserver-1.6.0/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.6.0/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.6.0/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.6.0/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.6.0/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.089207 heaserver-1.6.0/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    41015 2024-05-21 21:48:04.000000 heaserver-1.6.0/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.6.0/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.6.0/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    17879 2024-05-07 19:13:00.000000 heaserver-1.6.0/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.6.0/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11832 2024-05-19 17:17:26.000000 heaserver-1.6.0/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.6.0/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.361998 heaserver-1.6.0/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     8851 2024-05-21 23:07:23.000000 heaserver-1.6.0/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17709 2024-05-21 23:07:23.000000 heaserver-1.6.0/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:07:23.000000 heaserver-1.6.0/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-05-21 23:07:23.000000 heaserver-1.6.0/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 23:07:23.000000 heaserver-1.6.0/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.834936 heaserver-1.6.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:23.835937 heaserver-1.6.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.158657 heaserver-1.6.0/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.211663 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.213661 heaserver-1.6.0/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    17429 2024-05-21 21:21:05.000000 heaserver-1.6.0/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.217660 heaserver-1.6.0/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.228659 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5563 2024-05-07 19:13:00.000000 heaserver-1.6.0/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5931 2024-05-07 19:13:00.000000 heaserver-1.6.0/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.250659 heaserver-1.6.0/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.351996 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.6.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.6.0/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:07:24.359000 heaserver-1.6.0/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2024-05-21 21:19:06.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.6.0/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.5.3/LICENSE` & `heaserver-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/PKG-INFO` & `heaserver-1.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.3
+Version: 1.6.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.5.0
+Requires-Dist: heaobject~=1.6.0
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,26 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.0
+* Improved docstrings.
+* New heaobject dependency.
+* Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
+* New heaserver.service.util.now() function.
+* Removed file system-related parameters from heaserver.service.heaobjectsupport functions (type_to_resource_url, get_dict, get, get_all, get_component, get_resource_url).
+* heaserver.service.client: Made a type passed into type_or_obj not used to create the object instance; new get_all_list() function.
+* Use heaobject.util.now() instead of datetime.now() to get the current datetime with a timezone.
+* Don't allow creating a new desktop object in MongoDB if the current user and the owner of the object are not the same.
+* Set the created and modified attributes of desktop objects in heaserver.service.db.mongo.
+* Populate new AWSAccount attributes.
+
 ## Version 1.5.3
 * When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
 possibly resulting in a Content-Length header that is shorter than the request body.
 * Make heaserver.service.db.aws.get_credentials raise the right exception.
 
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
```

### Comparing `heaserver-1.5.3/README.md` & `heaserver-1.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.0
+* Improved docstrings.
+* New heaobject dependency.
+* Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
+* New heaserver.service.util.now() function.
+* Removed file system-related parameters from heaserver.service.heaobjectsupport functions (type_to_resource_url, get_dict, get, get_all, get_component, get_resource_url).
+* heaserver.service.client: Made a type passed into type_or_obj not used to create the object instance; new get_all_list() function.
+* Use heaobject.util.now() instead of datetime.now() to get the current datetime with a timezone.
+* Don't allow creating a new desktop object in MongoDB if the current user and the owner of the object are not the same.
+* Set the created and modified attributes of desktop objects in heaserver.service.db.mongo.
+* Populate new AWSAccount attributes.
+
 ## Version 1.5.3
 * When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
 possibly resulting in a Content-Length header that is shorter than the request body.
 * Make heaserver.service.db.aws.get_credentials raise the right exception.
 
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
```

### Comparing `heaserver-1.5.3/RELEASING.md` & `heaserver-1.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.6.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.6.0/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.29500`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 content = {
     service.MONGODB_COMPONENT_COLLECTION: {
         '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog'
     }
 }
 
-HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0a39'
+HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:latest'
 
 ClientTestCase = get_test_case_cls_default(package_name='heaserver-registry',
                                            coll=service.MONGODB_COMPONENT_COLLECTION, fixtures=fixtures,
                                               duplicate_action_name='component-duplicate-form',
                                               db_manager_cls=MockDockerMongoManager, wstl_package=service.__package__,
                                               content=content, content_type='text/plain', put_content_status=204,
                                               href='http://localhost:8080/components/',
```

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 from heaobject.volume import DEFAULT_FILE_SYSTEM
 from heaobject.user import ALL_USERS, NONE_USER
 from heaobject.root import Permission
 
 fixtures: Dict[str, List[Dict[str, Any]]] = {
     service.MONGODB_COMPONENT_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': ['foo', 'bar'],
         'description': 'Description of Reximus',
         'display_name': 'Reximus',
         'invites': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'reximus',
-        'owner': NONE_USER,
+        'owner': TEST_USER,
         'shares': [{
             'type': 'heaobject.root.ShareImpl',
             'invite': None,
             'user': ALL_USERS,
             'permissions': [Permission.COOWNER.name]
         }],
         'source': None,
@@ -44,21 +44,21 @@
                 'creator_users': [],
                 'default_shares': [],
                 'type_display_name': 'Resource'
             }]
     },
     {
         'id': '0123456789ab0123456789ab',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': ['oof', 'rab'],
         'description': 'Description of Luximus',
         'display_name': 'Luximus',
         'invites': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'luximus',
         'owner': TEST_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.registry.Component',
         'base_url': 'http://localhost/foo',
         'external_base_url': None,
```

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,20 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
-            'accounts': [],
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
@@ -65,21 +64,20 @@
                     'invite': None,
                     'user': TEST_USER,
                     'permissions': [Permission.VIEWER.name]
                 }
             ],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
-            'accounts': [],
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         }
     ]}
 
 content = {
```

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,24 +24,23 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'created': None,
-            'modified': None,
+            'modified': '2022-05-17T00:00:00+00:00',
             'admin_ids': [TEST_USER],
-            'accounts': [],
             'type_display_name': 'Organization',
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
@@ -56,24 +55,23 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'created': None,
-            'modified': None,
+            'modified': '2022-05-17T00:00:00+00:00',
             'admin_ids': [TEST_USER],
-            'accounts': [],
+            'account_ids': [],
             'type_display_name': 'Organization',
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         }
     ]}
```

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,18 @@
             'shares': [],
             'source': None,
             'source_detail': None,
             'type': 'heaobject.volume.Volume',
             'file_system_type': MongoDBFileSystem.get_type_name(),
             'file_system_name': DEFAULT_FILE_SYSTEM,
             'credential_id': '666f6f2d6261722d71757578',
+            'credential_type_name': 'heaobject.keychain.Credentials',
             'folder_id': None,
             'mime_type': 'application/x.volume',
-            'account': None,
+            'account_id': None,
             'type_display_name': 'Volume'
         }
     ],
     'credentials': [
         {
             'id': '666f6f2d6261722d71757578',
             'created': None,
@@ -49,15 +50,16 @@
             'shares': [],
             'source': None,
             'source_detail': None,
             'type': 'heaobject.keychain.Credentials',
             'where': None,
             'account': None,
             'password': None,
-            'type_display_name': 'Credentials'
+            'type_display_name': 'Credentials',
+            'role': None
         }
     ]
 }
 
 volume_microservice = MicroserviceContainerConfig(
     image='registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-volumes:1.0.0a17', port=8080,
     check_path='/volumes', db_manager_cls=DockerMongoManager,
@@ -76,27 +78,27 @@
 
 
 class KeychainTestCase(MicroserviceTestCase):
     def __init__(self, methodName='runTest'):
         super().__init__(coll='credentials', desktop_objects=fixtures, db_manager_cls=DockerMongoManager,
                          methodName=methodName,
                          registry_docker_image=RealRegistryContainerConfig(
-                             image='registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0a39'),
+                             image='registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:latest'),
                          other_docker_images=[volume_microservice, keychain_microservice])
 
     async def test_get_credential(self):
         volume = Volume()
         volume.from_dict(fixtures['volumes'][0])
         credential = await database._get_credentials(self.app, volume)
         self.assertEqual(fixtures['credentials'][0], credential.to_dict() if credential is not None else None)
 
 
 class VolumeTestCase(MicroserviceTestCase):
     def __init__(self, methodName='runTest'):
         super().__init__(coll='volumes', desktop_objects=fixtures, db_manager_cls=DockerMongoManager,
                          methodName=methodName, registry_docker_image=RealRegistryContainerConfig(
-                image='registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0a39'),
+                image='registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:latest'),
                          other_docker_images=[volume_microservice, keychain_microservice])
 
     async def test_get_volume(self):
         volume, _ = await database._get_volume(self.app, '666f6f2d6261722d71757578')
         self.assertEqual(fixtures['volumes'][0], volume.to_dict() if volume is not None else None)
```

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.6.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999909812409813%*

 * *Differences: {"'wstl'": "{'actions': {3: {'inputs': {9: {'readOnly': True}}}}}"}*

```diff
@@ -93,14 +93,15 @@
                                 "path": "/people/",
                                 "text": "display_name",
                                 "value": "name"
                             }
                         },
                         "name": "owner",
                         "prompt": "Owner",
+                        "readOnly": true,
                         "required": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "type": "datetime"
                         },
```

### Comparing `heaserver-1.5.3/setup.py` & `heaserver-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.5.3',
+      version='1.6.0',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=find_namespace_packages(where='src'),
       package_data={'heaserver.service': ['py.typed', 'jsonschemafiles/*']},
       install_requires=[
-          'heaobject~=1.5.0',
+          'heaobject~=1.6.0',
           'aiohttp[speedups]~=3.8.6',
           'hea-aiohttp-remotes~=1.2.1',  # replace with aiohttp-remotes if they incorporate our patch.
           'motor~=3.2.0',
           'motor-types~=1.0.0b2',
           'accept-types~=0.4.1',
           'mongoquery~=1.4.2',
           'jsonschema~=4.17.3',
```

### Comparing `heaserver-1.5.3/src/heaserver/service/__init__.py` & `heaserver-1.6.0/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/activity.py` & `heaserver-1.6.0/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/appfactory.py` & `heaserver-1.6.0/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/appproperty.py` & `heaserver-1.6.0/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/backgroundtasks.py` & `heaserver-1.6.0/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/caching.py` & `heaserver-1.6.0/src/heaserver/service/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import functools
+from .util import now as datetime_now
 
 
 DEFAULT_TTL = datetime.timedelta(hours=1)
 
 
 def ttl_cache(func=None, *, ttl: datetime.timedelta = DEFAULT_TTL):
     """
@@ -38,13 +39,13 @@
 
     time, value = None, None
 
     @functools.wraps(func)
     def wrapper(*args, **kw):
         nonlocal time
         nonlocal value
-        now = datetime.datetime.now()
+        now = datetime_now()
         if not time or now - time > ttl:
             value = func(*args, **kw)
             time = now
         return value
     return wrapper
```

### Comparing `heaserver-1.5.3/src/heaserver/service/client.py` & `heaserver-1.6.0/src/heaserver/service/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,15 +104,15 @@
               headers: dict[str, str] | MultiDict[str, str] | None = None,
               client_session: ClientSession | None = None) -> Optional[DesktopObjectTypeVar]:
     """
     Co-routine that gets a HEA desktop object from a HEA service. It retries when connection errors occur.
 
     :param app: the aiohttp application context (required).
     :param url: The URL (str or URL) of the resource (required).
-    :param type_or_obj: the HEA desktop object type to populate with the resource's content, or a desktop object instance. If a
+    :param type_or_obj: the expected HEA desktop object type, or a desktop object instance to populate with content. If a
     type, this function will attempt to create an instance using the type's no-arg constructor.
     :param query_params: optional Mapping, iterable of tuple of key/value pairs or string to be sent as parameters in the query string of the new request.
     :param headers: optional dict or MultiDict of headers. Attempts to set the Accept header will be ignored. The
     service will always receive Accepts: application/json.
     :param client_session: a client session. If None, the default session will be used.
     :return: the HEAObject populated with the resource's content, None if no such resource exists, or another HTTP
     status code if an error occurred.
@@ -120,15 +120,15 @@
     :raises aiohttp.client_exceptions.ClientConnectionError: if a connection to the service could not be established.
     """
     _logger = logging.getLogger(__name__)
     _logger.debug("about to make the GET client call ")
     if type_or_obj is None:
         obj_ = None
     elif isinstance(type_or_obj, type) and issubclass(type_or_obj, root.DesktopObject):
-        obj_ = type_or_obj()
+        obj_ = None
     elif isinstance(type_or_obj, root.DesktopObject):
         obj_ = type_or_obj
     else:
         raise TypeError('obj must be an HEAObject instance or an HEAObject type')
     headers_ = headers.copy() if headers is not None else {}
     headers_[hdrs.ACCEPT] = nvpjson.MIME_TYPE
 
@@ -201,15 +201,15 @@
 
 
 async def get_all(app: web.Application, url: Union[URL, str], type_: Type[DesktopObjectTypeVar],
                   query_params: Optional[Mapping[str, str]] = None,
                   headers: dict[str, str] | MultiDict[str, str] | None = None,
                   client_session: ClientSession | None = None) -> AsyncGenerator[DesktopObjectTypeVar, None]:
     """
-    Generator that returns the requested HEAObjects. It retries when connection errors occur.
+    Generator that returns the requested desktop objects. It retries when connection errors occur.
 
     :param app: the aiohttp application context (required).
     :param url: The URL (str or URL) of the resource (required).
     :param type_: the type to populate with the resource's content.
     :param query_params: optional Mapping, iterable of tuple of key/value pairs or string to be sent as parameters in the query string of the new request.
     :param headers: optional dict or MultiDict of headers. Attempts to set the Accept header will be ignored. The
     service will always receive Accepts: application/json.
@@ -235,14 +235,37 @@
         _logger.debug('Client returning %s', result)
         for r in result:
             obj__ = obj___()
             obj__.from_dict(r)
             yield obj__
 
 
+async def get_all_list(app: web.Application, url: Union[URL, str], type_: Type[DesktopObjectTypeVar],
+                       query_params: Optional[Mapping[str, str]] = None,
+                       headers: dict[str, str] | MultiDict[str, str] | None = None,
+                       client_session: ClientSession | None = None) -> list[DesktopObjectTypeVar]:
+    """
+    Returns the requested desktop objects in a list. It retries when connection errors occur.
+
+    :param app: the aiohttp application context (required).
+    :param url: The URL (str or URL) of the resource (required).
+    :param type_: the type to populate with the resource's content.
+    :param query_params: optional Mapping, iterable of tuple of key/value pairs or string to be sent as parameters in the query string of the new request.
+    :param headers: optional dict or MultiDict of headers. Attempts to set the Accept header will be ignored. The
+    service will always receive Accepts: application/json.
+    :param client_session: a client session. If None, the default session will be used.
+    :return: a list of desktop objects with the provided type_.
+    :raises ClientResponseError: if the response's status code was unexpected.
+    :raises ClientConnectionError: if a connection to the service could not be established.
+    """
+    result: list[DesktopObjectTypeVar] = []
+    async for obj in get_all(app, url, type_, query_params, headers, client_session):
+        result.append(obj)
+    return result
+
 async def post(app: web.Application, url: Union[URL, str], data: root.DesktopObject | root.DesktopObjectDict,
                headers: dict[str, str] | MultiDict[str, str] | None = None,
                client_session: ClientSession | None = None) -> str:  # type: ignore[return]
     """
     Coroutine that posts a HEAObject to a HEA service.
 
     :param app: the aiohttp application context (required).
@@ -321,67 +344,54 @@
     :return: a Component instance or None (if not found).
     """
     return await get(app, URL(app[appproperty.HEA_REGISTRY]) / 'components' / 'byname' / name, Component,
                      client_session=client_session)
 
 
 async def get_component(app: web.Application, type_or_type_name: Union[str, Type[root.DesktopObject]],
-                        file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-                        file_system_name: str = DEFAULT_FILE_SYSTEM,
                         client_session: ClientSession | None = None) -> Component | None:
     """
     Gets the component corresponding to the HEA object type from the HEA registry service. It retries when connection
     errors occur.
 
     :param app: the aiohttp app.
     :param type_or_type_name: the desktop object type or type name of the resource.
-    :param file_system_type_or_type_name: optional file system type or type name. The default is heaobject.volume.DefaultFileSystem.
-    :param file_system_name: optional file system name. The default is heaobject.volume.FileSystem.DEFAULT_FILE_SYSTEM.
     :param client_session: a client session. If None, the default session will be used.
     :return: the Component, or None if not found.
     :raises aiohttp.client_exceptions.ClientResponseError: if the response's status code was unexpected.
     :raises aiohttp.client_exceptions.ClientConnectionError: if a connection to the service could not be established.
     """
-    from .heaobjectsupport import desktop_object_type_or_type_name_to_type, type_or_type_name_to_type
-    file_system_name_ = DEFAULT_FILE_SYSTEM if file_system_name is None else file_system_name
-    file_system_type_ = desktop_object_type_or_type_name_to_type(file_system_type_or_type_name,
-                                                                 default_type=MongoDBFileSystem)
+    from .heaobjectsupport import type_or_type_name_to_type
     type_name_ = type_or_type_name_to_type(type_or_type_name).get_type_name()
-    url = URL(app[appproperty.HEA_REGISTRY]) / 'components' / 'bytype' / type_name_ / 'byfilesystemtype' / file_system_type_.get_type_name() / 'byfilesystemname' / file_system_name_
+    url = URL(app[appproperty.HEA_REGISTRY]) / 'components' / 'bytype' / type_name_
     return await get(app, url, Component, client_session=client_session)
 
 
 async def get_resource_url(app: web.Application, type_or_type_name: Union[str, Type[root.HEAObject]],
-                           file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-                           file_system_name: str = DEFAULT_FILE_SYSTEM,
                            client_session: ClientSession | None = None,
                            parameters: Optional[dict[str, Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]]] = None,
                            **kwargs: Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]) -> str | None:
     """
     Gets the resource URL corresponding to the HEA object type from the HEA registry service. The URL is constructed by
     joining the component's base URL and the resource base path. It retries when connection errors occur.
 
     :param app: the aiohttp app.
     :param type_or_type_name: the HEAObject type or type name of the resource.
-    :param file_system_type_or_type_name: optional file system type or type name. The default is
-    heaobject.volume.DefaultFileSystem.
-    :param file_system_name: optional file system name. The default is heaobject.volume.FileSystem.DEFAULT_FILE_SYSTEM.
     :param client_session: a client session. If None, the default session will be used.
     :param parameters: for resource URLs with a URI template, the template parameters.
     :param kwargs: alternative way to provide template parameters.
     :return: a URL string or None if no such resource is found in the registry service.
     :raises ValueError: if there was a problem accessing the registry service.
     """
     from .heaobjectsupport import type_or_type_name_to_type
     logger = logging.getLogger(__name__)
-    component = await get_component(app, type_or_type_name, file_system_type_or_type_name, file_system_name, client_session=client_session)
+    component = await get_component(app, type_or_type_name, client_session=client_session)
     logger.debug('Got component %s from registry', component)
-    file_system_name_ = DEFAULT_FILE_SYSTEM if file_system_name is None else file_system_name
     type_name_ = type_or_type_name_to_type(type_or_type_name).get_type_name()
-    return component.get_resource_url(type_name_, file_system_name=file_system_name_, parameters=parameters, kwargs=kwargs) if component is not None else None
+    return component.get_resource_url(type_name_, parameters=parameters, kwargs=kwargs) if component is not None else None
 
 async def get_collection(type_or_type_name: Union[str, Type[root.HEAObject]]):
     pass
 
 
 async def get_property(app: web.Application, name: str,
                        client_session: ClientSession | None = None) -> Property | None:
```

### Comparing `heaserver-1.5.3/src/heaserver/service/config.py` & `heaserver-1.6.0/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/db/aws.py` & `heaserver-1.6.0/src/heaserver/service/db/aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 from ..oidcclaimhdrs import SUB
 from ..sources import AWS as AWS_SOURCE
 
 from heaobject.account import AWSAccount
 from heaobject.keychain import AWSCredentials, Credentials
 from heaobject.registry import Property
 from heaobject.volume import AWSFileSystem
-from heaobject.user import NONE_USER, AWS_USER
-from heaobject.person import Role, encode_role
+from heaobject.user import AWS_USER, CREDENTIALS_MANAGER_USER
 from ..heaobjectsupport import type_to_resource_url
 from .. import client
 from yarl import URL
-from typing import Optional, Any, TypeVar, cast, overload, Literal
+from typing import Optional, TypeVar, cast, overload, Literal
 from configparser import ConfigParser
 import asyncio
 from threading import Lock
 from contextlib import closing
 from collections import defaultdict
 from collections.abc import Callable, Sequence, AsyncGenerator
+from datetime import datetime
 import logging
 
 _boto3_client_lock = Lock()
 _boto3_resource_lock = Lock()
 _boto3_client_config = botocore.config.Config(max_pool_connections=25)
 
 
@@ -63,27 +63,27 @@
 
     @property
     def file_system_type(self) -> type[AWSFileSystem]:
         return AWSFileSystem
 
     async def update_credentials(self, request: Request, credentials: AWSCredentials) -> None:
         """
-        This is a wrapper function to be extended by tests
-        It obtains credential's url from the registry and that makes PUT
+        Obtains the keychain microservice's url from the registry and executes a PUT call to update the credentials
+        object. It executes the PUT call as the system|awscredentialsmanager user.
 
-        :param request:
-        :param credentials:
-        :returns: None if it succeeds otherwise it will raise ValueError or HTTPError
+        :param request: the HTTP request (required).
+        :param credentials: the AWS credentials to update (required).
         :raises ValueError: if there was a problem accessing the registry service or the credentials service was not
         found.
+        :raises ClientResponseError: if there was a problem making the PUT request.
         """
         if credentials.id is None:
             raise ValueError(f'credentials must have a non-None id attribute')
         resource_url = await type_to_resource_url(request, Credentials)
-        headers = {SUB: request.headers.get(SUB, NONE_USER)}
+        headers = {SUB: CREDENTIALS_MANAGER_USER}
         try:
             await client.put(app=request.app, url=URL(resource_url) / credentials.id, data=credentials,
                             headers=headers)
         except ClientResponseError as e:
             raise ValueError(f'Updating credentials failed: {str(e)}') from e
 
     async def get_property(self, app: web.Application, name: str) -> Optional[Property]:
@@ -242,14 +242,17 @@
         account = AWSAccount()
         account.id = aid
         account.name = aid
         account.display_name = aid
         account.owner = AWS_USER
         account.source = AWS_SOURCE
         account.source_detail = AWS_SOURCE
+        account.type_display_name
+        account.file_system_type = AWSFileSystem.get_type_name()
+        account.credential_type_name = AWSCredentials.get_type_name()
         return account
 
     async def _get_account(self, request: Request, volume_id: str) -> AWSAccount:
         logger = logging.getLogger(__name__)
         loop = asyncio.get_running_loop()
         credentials = await self.get_credentials_from_volume(request, volume_id)
         logger.debug('Got credentials %s for volume %s', credentials, volume_id)
@@ -330,44 +333,43 @@
                                                             aws_access_key_id=credentials.account,
                                                             aws_secret_access_key=credentials.password))
 
 
     async def __get_temporary_credentials(self, request: web.Request, credentials: AWSCredentials,
                                           creator: Callable[
                                               [str, str | None, str | None, str | None, str | None], _S3Service],
-                                          service_name: str) -> Any:
+                                          service_name: str) -> _S3Service:
         """
             Gets temporary credentials and returns the authorized client. In order to do that it
-            gets the previous credential's role_arn and then assumes it.
+            gets the previous credential's role and then assumes it.
 
             :param request: the aiohttp request
             :param credentials: the aws credentials last saved
             :param aws_source: must be either boto3.client or boto3.resource.
             :param service_name: The type of client to return
             :return: the boto3 client provided with credentials
             :raise ValueError if no previously saved credentials it raises ValueError
         """
         logger = logging.getLogger(__name__)
-        assert credentials.role_arn is not None, 'credentials must have a non-None role_arn attribute'
+        assert credentials.role is not None, 'credentials must have a non-None role attribute'
         loop = asyncio.get_running_loop()
 
         async with self.__locks[credentials.id]:
             if credentials.has_expired(S3.EXPIRATION_LIMIT):
                 logger.debug("credentials need to be refreshed")
-                cloud_creds = await self.generate_cloud_credentials(request, credentials.role_arn)
+                cloud_creds = await self.generate_cloud_credentials(request, credentials.role)
                 if not cloud_creds:
-                    raise ValueError(f'Could not generate cloud credentials with these params {credentials.role_arn}')
-                if logger.getEffectiveLevel() == logging.DEBUG:
-                    logger.debug("credentials successfully obtained from cloud: %s", cloud_creds.to_dict())
+                    raise ValueError(f'Could not generate cloud credentials with role {credentials.role}')
+                logger.debug("Credentials successfully obtained from cloud: %r", cloud_creds)
                 credentials.account = cloud_creds.account
                 credentials.password = cloud_creds.password
                 credentials.session_token = cloud_creds.session_token
                 credentials.expiration = cloud_creds.expiration
                 await self.update_credentials(request=request, credentials=credentials)
-                logger.debug("credentials updated in the database")
+                logger.debug("Credentials updated in the database")
             return await loop.run_in_executor(None, partial(creator,
                                                             service_name,
                                                             region_name=credentials.where,
                                                             aws_access_key_id=credentials.account,
                                                             aws_secret_access_key=credentials.password,
                                                             aws_session_token=credentials.session_token))
 
@@ -539,30 +541,24 @@
         raise ValueError('Cannot get credentials arn which is required')
     auth = request.headers.get(hdrs.AUTHORIZATION, '')
     auth_token = auth.split(' ')
 
     if len(auth_token) != 2:
         raise ValueError("Bearer Token is required in header")
     logger.debug('Getting credentials for user %s with role %s...', sub, arn)
-    roles_url = await type_to_resource_url(request, Role)
     try:
-        if await client.has(request.app, URL(roles_url) / 'byname' / encode_role(arn),
-                        headers={hdrs.AUTHORIZATION: auth, SUB: sub}):
-            logger.debug('User %s has role %s', sub, arn)
-            loop = asyncio.get_running_loop()
-            sts_client_call = partial(boto3.client, 'sts', config=_boto3_client_config)
-            with closing(await loop.run_in_executor(None, sts_client_call)) as sts_client:
-                assumed_role_object = await loop.run_in_executor(None, partial(sts_client.assume_role_with_web_identity,
-                                                                                WebIdentityToken=auth_token[1],
-                                                                                RoleArn=arn,
-                                                                                RoleSessionName=sub,
-                                                                                DurationSeconds=S3.MAX_DURATION_SECONDS))
-        else:
-            logger.debug('User does not have role %s, so temporary credentials could not be generated', arn)
-            return None
+        logger.debug('User %s has role %s', sub, arn)
+        loop = asyncio.get_running_loop()
+        sts_client_call = partial(boto3.client, 'sts', config=_boto3_client_config)
+        with closing(await loop.run_in_executor(None, sts_client_call)) as sts_client:
+            assumed_role_object = await loop.run_in_executor(None, partial(sts_client.assume_role_with_web_identity,
+                                                                            WebIdentityToken=auth_token[1],
+                                                                            RoleArn=arn,
+                                                                            RoleSessionName=sub,
+                                                                            DurationSeconds=S3.MAX_DURATION_SECONDS))
     except ClientError:
         logger.exception('User %s does not have role %s', sub, arn)
         return None
     creds_dict = assumed_role_object.get('Credentials')
     if not creds_dict:
         return None
     creds = AWSCredentials()
```

### Comparing `heaserver-1.5.3/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.6.0/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/db/database.py` & `heaserver-1.6.0/src/heaserver/service/db/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,44 +91,43 @@
         :param volume_id: the volume id (required).
         :return a Credentials object, or None if no credentials were found.
         :raises ValueError: if no volume with that id exists.
         """
         return await get_credentials_from_volume(request, volume_id)
 
     async def get_volumes(self, request: Request, file_system_type_or_type_name: str | type[FileSystem],
-                          account_ids: Sequence[str] | None = None,
-                          account_type_names: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
+                          account_ids: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
         """
         An async generator of volumes of a given file system type. This implementation is identical to the module-level
         get_volumes() function.
 
         :param request: the HTTP request (required).
         :param file_system_type_or_type_name: the file system type or type name string (required).
         :raises ValueError: if no volume microservice is registered.
         :raises TypeError: if file_system_type_or_type_name is a type but not a FileSystem.
         """
-        async for volume in get_volumes(request, file_system_type_or_type_name, account_ids=account_ids,
-                                        account_type_names=account_type_names):
+        async for volume in get_volumes(request, file_system_type_or_type_name, account_ids=account_ids):
             yield volume
 
     async def is_creator(self, request: Request, for_type_or_type_name: str | type[DesktopObject]) -> bool:
         """
         Returns whether the current user may create new desktop objects of the given type. This method consults the
         registry service metadata to determine the user's create permissions.
 
         :param request: the HTTP request (required).
         :param for_type_or_type_name: the desktop object type or type name.
         :return: True or False.
-        :raises ValueError: if an error occurred checking the registry service.
+        :raises ValueError: if an error occurred checking the registry service, or if the provided type is not
+        registered in the heaserver-registry service.
         """
         type_ = for_type_or_type_name.get_type_name() if issubclass(for_type_or_type_name, DesktopObject) else str(for_type_or_type_name)
         component = await client.get_component(request.app, type_)
         if component is None:
             raise ValueError(f'Could not find component for type {type_}')
-        resource = component.get_resource(type_.get_type_name())
+        resource = component.get_resource(type_)
         if resource is None:
             raise ValueError(f'No resource found for type {type_}')
         return resource.is_creator_user(request.headers.get(SUB, NONE_USER))
 
     def close(self):
         """
         Closes the database connection. This method may be called multiple times.
@@ -309,16 +308,15 @@
             return response.status_not_found()
         return response.status_ok()
     else:
         return response.status_not_found()
 
 
 async def get_volumes(request: Request, file_system_type_or_type_name: Union[str, type[FileSystem]],
-                      account_ids: Sequence[str] | None = None,
-                      account_type_names: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
+                      account_ids: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
     """
     Gets the volumes accessible to the current user that have the provided filesystem type.
 
     :param request: the aiohttp request (required).
     :param file_system_type_or_type_name: the filesystem type or type name.
     :return: an async generator of Volume objects.
     :raises ValueError: if no volume microservice is registered.
@@ -327,16 +325,15 @@
     headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
     volume_url = await type_to_resource_url(request, Volume)
     file_system_type_ = desktop_object_type_or_type_name_to_type(file_system_type_or_type_name)
     if not issubclass(file_system_type_, FileSystem):
         raise TypeError(f'Provided file_system_type_or_type_name is a {file_system_type_} not a FileSystem')
     get_volumes_url = URL(volume_url) / 'byfilesystemtype' / file_system_type_.get_type_name()
     if account_ids:
-        query = ([('account_id', account_id) for account_id in account_ids] +
-                 [('account_type_name', account_type_name) for account_type_name in account_type_names])
+        query = [('account_id', account_id) for account_id in account_ids]
     else:
         query = None
     async for volume in client.get_all(request.app, get_volumes_url.with_query(query) if query else get_volumes_url, Volume, headers=headers):
         yield volume
 
 
 async def get_options(request: Request, methods: list[str]):
@@ -646,16 +643,18 @@
     """
 
     def __init__(self, request: Request, volume_id: str | None = None, credentials: CredentialTypeVar | None = None) -> None:
         """
         Create the context manager.
 
         :param request: the HTTP request (required).
-        :param volume_id: optional volume id. You must either provide a volume id or a credentials object.
-        :param credentials: optional credentials object. You must either provide a volume id or a credentials object.
+        :param volume_id: optional volume id. Subclasses may require that you either provide a volume id or a
+        credentials object.
+        :param credentials: optional credentials object. Subclasses may require that you provide a volume id or a
+        credentials object.
         """
         if request is None:
             raise ValueError('Request cannot be None')
         if not isinstance(request, Request):
             raise ValueError(f'request {request} must be a Request')
         self.__request = request
         self.__volume_id = str(volume_id) if volume_id is not None else None
```

### Comparing `heaserver-1.5.3/src/heaserver/service/db/dbapi2.py` & `heaserver-1.6.0/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/db/mongo.py` & `heaserver-1.6.0/src/heaserver/service/db/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from yarl import URL
 from motor.motor_asyncio import AsyncIOMotorGridFSBucket
 from ..response import SupportsAsyncRead
 from gridfs.errors import NoFile
 from bson import ObjectId
 from heaserver.service.appproperty import HEA_DB
 from typing import cast
+from ..util import now
 
 _codec_options = CodecOptions(tz_aware=True)
 
 
 class Mongo(Database):
     """
     Connectivity to a MongoDB database for HEA resources.
@@ -288,14 +289,15 @@
         :param request: the HTTP request (required).
         :param obj: the desktop object instance to put.
         :param collection: the MongoDB collection containing the requested object (required).
         :param sub: the user to filter by. Defaults to None.
         :return: an instance of pymongo.results.UpdateResult.
         """
         coll = self._get_collection(collection)
+        obj.modified = now()
         try:
             extra_ = sub_filter_expr(sub or user.NONE_USER,
                                      permissions=[perm.name for perm in RESTPermissionGroup.PUTTER_PERMS._perms_internal])
             mongo_expr_ = Mongo.__replace_object_ids(mongo_expr(request, 'id', extra=extra_))
             return await coll.replace_one(mongo_expr_, replace_id_with_object_id(obj.to_dict()))
         except bson.errors.InvalidId:
             return None
@@ -327,14 +329,15 @@
             except Exception as e:
                 if failed:
                     try:
                         fileobj.close()
                     except:
                         pass
                 raise e
+            await self.put(request, desktop_obj, collection, sub)
             return True
         except NoFile:
             # Delete orphaned chunks from gridfs if an error occurred
             return False
 
     async def delete(self, request: web.Request, collection: str, var_parts=None, mongoattributes=None,
                      sub: Optional[str] = None) -> Optional[DeleteResult]:
@@ -442,14 +445,15 @@
         logger = logging.getLogger(__name__)
         if obj is None:
             return None
         if isinstance(obj, root.DesktopObject):
             obj_ = obj.to_dict()
         else:
             obj_ = obj
+        obj_['created'] = now()
         coll = self._get_collection(collection)
         try:
             result = await coll.insert_one(document=obj_)
             if result and default_content is not None:
                 fs = self.__new_gridfs_bucket(collection)
                 await fs.upload_from_stream_with_id(ObjectId(result.inserted_id), obj_['display_name'], default_content)
             return str(result.inserted_id)
@@ -470,14 +474,15 @@
         logger = logging.getLogger(__name__)
         if obj is None:
             return None
         if isinstance(obj, root.DesktopObject):
             obj_ = obj.to_dict()
         else:
             obj_ = obj
+        obj_['modified'] = now()
         coll = self._get_collection(collection)
         try:
             result = await coll.replace_one({'_id': ObjectId(obj_['id'])}, obj_)
             if result and default_content is not None:
                 fs = self.__new_gridfs_bucket(collection)
                 await fs.upload_from_stream_with_id(ObjectId(obj_['id']), obj_['display_name'], default_content)
             return result
@@ -623,15 +628,17 @@
     @classmethod
     def database_types(self) -> list[str]:
         return ['system|mongo']
 
 
 class MongoContext(DatabaseContextManager[Mongo]): # Go into db package?
     """
-    Provides a Mongo object.
+    Provides a Mongo database connection object. If neither a volume nor a credentials object is passed into the
+    constructor, the connection string in the microservice's configuration file will be used, otherwise it will use
+    the default localhost connection string.
     """
 
     async def connection(self) -> Mongo:
         return cast(Mongo, await _get_mongo(self.request, self.volume_id))
 
 
 async def _get_mongo(request: web.Request, volume_id: Optional[str]) -> Mongo:
```

### Comparing `heaserver-1.5.3/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.6.0/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.6.0/src/heaserver/service/db/mongoservicelib.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from aiohttp.web import Request, StreamResponse, Response, HTTPError
 from typing import Any, AsyncGenerator, Literal, IO
 from heaobject.root import DesktopObject, DesktopObjectDict, desktop_object_from_dict, Permission
 from heaobject.user import NONE_USER
 from heaserver.service.oidcclaimhdrs import SUB
 from pymongo.errors import WriteError
 from collections.abc import Sequence, Mapping
+import logging
 
 
 async def get_dict(request: Request, collection: str,
                            volume_id: str | None = None) -> DesktopObjectDict | None:
     """
     Gets the requested desktop object as a desktop object dict.
 
@@ -252,55 +253,84 @@
             else:
                 return response.status_not_found()
 
 
 
 async def post(request: Request, collection: str, type_: type[DesktopObject], default_content: IO | None = None, volume_id: str | None = None) -> Response:
     """
-    Posts the provided HEA object.
+    Posts the desktop object from a request body.
 
-    :param request: the HTTP request.
+    :param request: the HTTP request containing the desktop object. The object's owner and the request's OIDC_CLAIM_sub
+    header must match.
     :param collection: the Mongo collection name. Required.
-    :param type_: The HEA object type. Required.
+    :param type_: The HEA object type. Required. The type of the object in the request body is compared to this type
+    for whether the object is an instance of the given type, and a response with a 400 status code is returned if it is
+    not.
     :param default_content: an optional blank document or other default content as a file-like object. This must be not-None
     for any microservices that manage content.
     :param volume_id: the id string of the volume containing the requested HEA object. If None, the root volume is
     assumed.
     :return: a Response object with a status of Created and the object's URI in the
     """
+    logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, NONE_USER)
-    if not await request.app[HEA_DB].is_creator(request, type_):
-        return response.status_forbidden(f'Permission denied creating objects of type {type_.get_type_name()}')
     try:
         obj = await new_heaobject_from_type(request, type_)
     except DeserializeException as e:
         return response.status_bad_request(str(e))
-    if obj.owner is None:
-        obj.owner = request.headers.get(SUB, None)
+    if not await request.app[HEA_DB].is_creator(request, type(obj)):
+        logger.debug('Permission denied to %s creating object %s', sub, obj)
+        return response.status_forbidden(f'Permission denied creating object of type {type_.get_type_name()}')
+    if obj.owner != sub:
+        logger.debug('Permission denied to %s creating object with owner %s', sub, obj.owner)
+        return response.status_forbidden(f'Permission denied creating object of type {type_.get_type_name()}')
     async with MongoContext(request, volume_id) as mongo:
         result = await mongo.post(request, obj, collection, default_content)
         to_delete = []
         for cache_key in request.app[HEA_CACHE]:
             if cache_key[1] == collection and cache_key[2] is None:
                 to_delete.append(cache_key)
         for cache_key in to_delete:
             request.app[HEA_CACHE].pop(cache_key, None)
         return await response.post(request, result, collection)
 
-async def post_dict_return_id(request: Request, obj_dict: DesktopObjectDict, collection: str, type_: type[DesktopObject], default_content: IO | None = None, volume_id: str | None = None) -> str | None:
+async def post_dict_return_id(request: Request, obj_dict: DesktopObjectDict, collection: str,
+                              type_: type[DesktopObject], default_content: IO | None = None,
+                              volume_id: str | None = None) -> str | None:
+    logger = logging.getLogger(__name__)
+    sub = request.headers.get(SUB, NONE_USER)
+    owner = obj_dict.get('owner')
+    if sub != owner:
+        logger.debug('Permission denied to %s creating object %s', sub, obj)
+        return response.status_forbidden(f'Permission denied creating object with owner {owner}')
     try:
         obj = desktop_object_from_dict(obj_dict)
     except (DeserializeException, ValueError, TypeError) as e:
         raise response.status_bad_request(str(e))
-    if obj.owner is None:
-        obj.owner = request.headers.get(SUB, None)
     async with MongoContext(request, volume_id) as mongo:
         return await mongo.post(request, obj, collection, default_content)
 
-async def post_dict(request: Request, obj_dict: DesktopObjectDict, collection: str, type_: type[DesktopObject], default_content: IO | None = None, volume_id: str | None = None) -> Response:
+async def post_dict(request: Request, obj_dict: DesktopObjectDict, collection: str, type_: type[DesktopObject],
+                    default_content: IO | None = None, volume_id: str | None = None) -> Response:
+    """
+    Posts a desktop object dict.
+
+    :param request: the HTTP request (required). The owner property in the obj_dict parameter and the request's
+    OIDC_CLAIM_sub header must match.
+    :param obj_dict: a desktop object dict (required).
+    :param collection: the Mongo collection name (required).
+    :param type_: The HEA object type. Required. The type of the object in the request body is compared to this type
+    for whether the object is an instance of the given type, and a response with a 400 status code is returned if it is
+    not.
+    :param default_content: an optional blank document or other default content as a file-like object. This must be not-None
+    for any microservices that manage content.
+    :param volume_id: the id string of the volume containing the requested HEA object. If None, the root volume is
+    assumed.
+    :return: a Response object with a status of Created and the object's URI in the
+    """
     try:
         result = await post_dict_return_id(request, obj_dict, collection, type_, default_content, volume_id)
         return await response.post(request, result, collection)
     except HTTPError as e:
         return e
 
 async def put(request: Request, collection: str, type_: type[DesktopObject], volume_id: str | None = None) -> Response:
```

### Comparing `heaserver-1.5.3/src/heaserver/service/expression.py` & `heaserver-1.6.0/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/functional.py` & `heaserver-1.6.0/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.6.0/src/heaserver/service/heaobjectsupport.py`

 * *Files 10% similar despite different names*

```diff
@@ -181,105 +181,80 @@
         raise DeserializeException from e
     except Exception as e:
         _logger.exception('Got exception %s', e)
         raise DeserializeException from e
 
 
 async def type_to_resource_url(request: web.Request, type_or_type_name: Union[str, Type[DesktopObject]],
-                               file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-                               file_system_name: str = DEFAULT_FILE_SYSTEM,
                                parameters: Optional[dict[str, Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]]] = None,
                                **kwargs: Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]) -> str:
     """
     Use the HEA registry service to get the resource URL for accessing HEA objects of the given type.
 
     :param request: the HTTP request. Required.
     :param type_or_type_name: the type or type name of HEA desktop object. Required.
-    :param file_system_type_or_type_name: the type of file system. The default is the default file system type.
-    :param file_system_name: the name of a file system. The default is filesystems.DEFAULT.
+    :param parameters: for resource URLs with a URI template, the template parameters.
     :return: the URL string.
     :raises ValueError: if no resource URL was found in the registry or there was a problem accesing the registry
     service.
     """
-    result = await client.get_resource_url(request.app, type_or_type_name, file_system_type_or_type_name,
-                                         file_system_name, parameters=parameters, kwargs=kwargs)
+    result = await client.get_resource_url(request.app, type_or_type_name, parameters=parameters, kwargs=kwargs)
     if result is None:
-        raise ValueError(f'No resource in the registry for type {type_or_type_name}, file system type {file_system_type_or_type_name}, and file system name {file_system_name}')
+        raise ValueError(f'No resource in the registry for type {type_or_type_name}')
     return result
 
 
 async def get_dict(request: web.Request, id_: str, type_or_type_name: Union[str, Type[DesktopObject]],
-                   file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-                   file_system_name: str = DEFAULT_FILE_SYSTEM,
                    headers: Optional[dict[str, str]] = None) -> Optional[DesktopObjectDict]:
     """
     Gets the HEA desktop object dict with the provided id from the service for the given type, file system type,
     and file system name.
 
     :param request: the aiohttp request (required).
     :param id_: the id of the HEA desktop object of interest.
     :param type_or_type_name: the desktop object type or type name.
-    :param file_system_type_or_type_name: the file system type or type name. The
-    default is the default file system type for HEA.
-    :param file_system_name: the file system name.
     :param headers: optional HTTP headers to use.
     :return: the requested HEA desktop object dict, or None if not found.
     :raises ValueError: if no appropriate service was found or there was a problem accessing the registry service.
     """
-    url = await type_to_resource_url(request, type_or_type_name=type_or_type_name,
-                                     file_system_type_or_type_name=file_system_type_or_type_name,
-                                     file_system_name=file_system_name)
+    url = await type_to_resource_url(request, type_or_type_name=type_or_type_name)
     return await client.get_dict(request.app, URL(url) / id_, headers)
 
 
 async def get(request: web.Request, id_: str, type_: Type[DesktopObjectTypeVar],
-              file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-              file_system_name: str = DEFAULT_FILE_SYSTEM,
               headers: Optional[dict[str, str]] = None) -> Optional[DesktopObjectTypeVar]:
     """
     Gets the HEA desktop object with the provided id from the service for the given type, file system type, and file
     system name.
 
     :param request: the aiohttp request (required).
     :param id_: the id of the HEA desktop object of interest.
     :param type_: the desktop object type.
-    :param file_system_type_or_type_name: the file system type or type name. The
-    default is the default file system type for HEA.
-    :param file_system_name: the file system name.
     :param headers: optional HTTP headers to use.
     :return: the requested HEA desktop object, or None if not found.
     :raises ValueError: if no appropriate service was found or there was a problem accessing the registry service.
     """
-    url = await type_to_resource_url(request, type_or_type_name=type_,
-                                     file_system_type_or_type_name=file_system_type_or_type_name,
-                                     file_system_name=file_system_name)
+    url = await type_to_resource_url(request, type_or_type_name=type_)
 
     return await client.get(request.app, URL(url) / id_, type_, headers)
 
 
 async def get_all(request: web.Request, type_: Type[DesktopObjectTypeVar],
-                  file_system_type_or_type_name: Union[str, Type[FileSystem]] = MongoDBFileSystem,
-                  file_system_name: str = DEFAULT_FILE_SYSTEM,
                   headers: Optional[dict[str, str]] = None) -> AsyncGenerator[DesktopObjectTypeVar, None]:
     """
     Async generator for all HEA desktop objects from the service for the given type, file system type, and file system
     name.
 
     :param request: the aiohttp request (required).
     :param type_: the desktop object type.
-    :param file_system_type_or_type_name: the file system type or type name. The
-    default is the default file system type for HEA.
-    :param file_system_name: the file system name.
     :param headers: optional HTTP headers to use.
     :return: an async generator with the requested desktop objects.
     :raises ValueError: if no appropriate service was found or there was a problem accessing the registry service.
     """
-    url = await type_to_resource_url(request, type_or_type_name=type_,
-                                     file_system_type_or_type_name=file_system_type_or_type_name,
-                                     file_system_name=file_system_name)
+    url = await type_to_resource_url(request, type_or_type_name=type_)
 
     return client.get_all(request.app, url, type_, headers)
 
 
 def has_permissions(obj: DesktopObject, sub: str | None, permissions: Sequence[Permission] | PermissionGroup) -> bool:
     """
     Return whether the provided user subject has any of the provided permissions to the object.
```

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschema.py` & `heaserver-1.6.0/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.6.0/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.6.0/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.6.0/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.6.0/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.6.0/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/messagebroker.py` & `heaserver-1.6.0/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/mimetypes.py` & `heaserver-1.6.0/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.6.0/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/openapi.py` & `heaserver-1.6.0/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/__init__.py` & `heaserver-1.6.0/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/cj.py` & `heaserver-1.6.0/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/factory.py` & `heaserver-1.6.0/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.6.0/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/representor.py` & `heaserver-1.6.0/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/wstljson.py` & `heaserver-1.6.0/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.6.0/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/response.py` & `heaserver-1.6.0/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/runner.py` & `heaserver-1.6.0/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.6.0/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.6.0/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.6.0/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/collection.py` & `heaserver-1.6.0/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/docker.py` & `heaserver-1.6.0/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.6.0/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.6.0/src/heaserver/service/testcase/expectedvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -656,20 +656,35 @@
 
 def _section_prompt_key_value(i):
     epv = wstl.get_extended_property_value('sectionPrompt', i)
     return {'sectionPrompt': epv} if epv is not None else {}
 
 
 def _new_template_data_item(i: dict[str, Any], value: Any, sub: str) -> dict[str, Any]:
+    """
+    Generates a template data item.
+
+    Assumptions:
+    The modified and created properties must always be readOnly. They are set by the server.
+    The owner property must have a non-None value unless the document has more than one item, in which case it must be
+    None.
+    The owner property must be readOnly if its non-None value is different from the current user.
+    """
+    readOnly = i.get('readOnly', None)
+    if readOnly is None:
+        if (i['name'] in ('modified', 'created')) or (i['name'] == 'owner' and value and value != sub):
+            readOnly = True
+        else:
+            readOnly = False
     rtn = {'name': i['name'],
            'value': _value_append(value),
            'prompt': i.get('prompt', i['name']),
            'required': i.get('required', False),
            'pattern': i.get('pattern'),
-           'readOnly': i.get('readOnly', True if i['name'] in ('modified', 'created') or (i['name'] == 'owner' and i.get('value', NONE_USER) != sub) else False)}
+           'readOnly': i.get('readOnly', readOnly)}
     add_extended_property_values(i, rtn)
     return rtn
 
 
 def _set_collection_template(action, collection_doc, fixture, len_fixtures, rel, sub):
     """
     Adds a template object to the provided Collection+JSON document.
```

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.6.0/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/mixin.py` & `heaserver-1.6.0/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.6.0/src/heaserver/service/testcase/mockaws.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,42 +166,32 @@
             creds.password = self.__aws_secret_access_key
             creds.expiration = self.__expiration
         else:
             creds = self._get_credential_by_volume(volume_id=volume_id)
         return creds
 
     async def get_volumes(self, request: Request, file_system_type_or_type_name: str | type[FileSystem],
-                          account_ids: Sequence[str] | None = None,
-                          account_type_names: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
+                          account_ids: Sequence[str] | None = None) -> AsyncGenerator[Volume, None]:
         """
         An asynchronous generator of the volumes to which the user has access, retrieved from the mock mongo in-memory
         database.
 
         :param request: the HTTP request (required).
         :param file_system_type_or_type_name: filter by a file system type or type name (required).
         :return: an asynchronous generator of Volume objects.
         """
-        if account_ids:
-            account_assocs: list[AccountAssociation] | None = []
-            for account_id, account_type_name in zip(account_ids, account_type_names):
-                account_assoc = AccountAssociation()
-                account_assoc.actual_object_id = account_id
-                account_assoc.actual_object_type_name = account_type_name
-                account_assocs.append(account_assoc)
-        else:
-            account_assocs = None
         for volume_dict in self.get_desktop_objects_by_collection('volumes'):
             if issubclass(file_system_type_or_type_name, DesktopObject):
                 file_system_type_name_ = file_system_type_or_type_name.get_type_name()
             else:
                 file_system_type_name_ = str(file_system_type_or_type_name)
             if volume_dict.get('file_system_type', AWSFileSystem.get_type_name()) == file_system_type_name_:
                 volume = Volume()
                 volume.from_dict(volume_dict)
-                if not account_assocs or volume.account in account_assocs:
+                if not account_ids or volume.account_id in account_ids:
                     yield volume
 
     async def get_property(self, app: web.Application, name: str) -> Property | None:
         """
         Gets the value of the requested property from the mock mongo in-memory database.
 
         :param app: the aiohttp web.Application object (required).
```

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.6.0/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.6.0/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.6.0/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.6.0/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/testenv.py` & `heaserver-1.6.0/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/testcase/util.py` & `heaserver-1.6.0/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/uritemplate.py` & `heaserver-1.6.0/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver/service/util.py` & `heaserver-1.6.0/src/heaserver/service/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections.abc import AsyncGenerator, Awaitable, Coroutine, Callable, Generator, Iterable
 import requests
 from contextlib import contextmanager
 import asyncio
 import time
 import os
 from dataclasses import dataclass
+from datetime import datetime, timezone
 import inspect
 
 RT = TypeVar('RT')  # return type
 
 def async_retry(*exceptions: Type[Exception], retries: int = 3, cooldown: Optional[int] = 1,
                 verbose: bool = True) -> Callable[[Coroutine[Any, Any, RT]], Coroutine[Any, Any, RT]]:
     """
@@ -297,7 +298,16 @@
 
 
 async def yield_control():
     """
     Yields control from the current async task to another task.
     """
     await asyncio.sleep(0.1)
+
+
+def now() -> datetime:
+    """
+    Returns the current datetime in UTC.
+
+    :return: a datetime.
+    """
+    return datetime.now(timezone.utc)
```

### Comparing `heaserver-1.5.3/src/heaserver/service/wstl.py` & `heaserver-1.6.0/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.6.0/src/heaserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.3
+Version: 1.6.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.5.0
+Requires-Dist: heaobject~=1.6.0
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,26 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.6.0
+* Improved docstrings.
+* New heaobject dependency.
+* Removed account_type_names parameters from heaserver.service.db.database.get_volumes and heaserver.service.db.database.Database.get_volumes.
+* New heaserver.service.util.now() function.
+* Removed file system-related parameters from heaserver.service.heaobjectsupport functions (type_to_resource_url, get_dict, get, get_all, get_component, get_resource_url).
+* heaserver.service.client: Made a type passed into type_or_obj not used to create the object instance; new get_all_list() function.
+* Use heaobject.util.now() instead of datetime.now() to get the current datetime with a timezone.
+* Don't allow creating a new desktop object in MongoDB if the current user and the owner of the object are not the same.
+* Set the created and modified attributes of desktop objects in heaserver.service.db.mongo.
+* Populate new AWSAccount attributes.
+
 ## Version 1.5.3
 * When updating AWS temporary credentials, generate new headers rather than pass the headers from the HTTP request,
 possibly resulting in a Content-Length header that is shorter than the request body.
 * Make heaserver.service.db.aws.get_credentials raise the right exception.
 
 ## Version 1.5.2
 * Fixed TypeError regression in the heaserver.service.client module.
```

### Comparing `heaserver-1.5.3/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.6.0/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.6.0/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.6.0/tests/heaserver/servicetest/componenttestcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         'derived_by': None,
         'derived_from': ['foo', 'bar'],
         'description': None,
         'display_name': 'Reximus',
         'invites': [],
         'modified': datetime(2021, 12, 2, 17, 31, 15, 630000, tzinfo=timezone.utc),
         'name': 'reximus',
-        'owner': NONE_USER,
+        'owner': TEST_USER,
         'shares': [{
             'type': 'heaobject.root.ShareImpl',
             'invite': None,
             'user': ALL_USERS,
             'permissions': [Permission.COOWNER.name]
         }],
         'source': None,
```

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.6.0/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.6.0/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.6.0/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
             'admin_group_ids': [],
             'manager_group_ids': [],
@@ -63,15 +63,15 @@
                     'invite': None,
                     'user': TEST_USER,
                     'permissions': [Permission.VIEWER.name]
                 }
             ],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
             'admin_group_ids': [],
             'manager_group_ids': [],
```

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.6.0/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,21 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'admin_ids': [TEST_USER],
-            'accounts': [],
             'type_display_name': 'Organization',
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
@@ -58,22 +57,21 @@
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
+            "account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
             'admin_ids': [TEST_USER],
-            'accounts': [],
             'type_display_name': 'Organization',
             'admin_group_ids': [],
             'manager_group_ids': [],
             'member_group_ids': []
         }
     ]}
```

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.6.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/service.py` & `heaserver-1.6.0/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_client.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_response.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_util.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.6.0/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.3/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.6.0/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

