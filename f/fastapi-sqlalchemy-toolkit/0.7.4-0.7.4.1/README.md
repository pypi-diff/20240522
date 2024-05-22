# Comparing `tmp/fastapi_sqlalchemy_toolkit-0.7.4.tar.gz` & `tmp/fastapi_sqlalchemy_toolkit-0.7.4.1.tar.gz`

## Comparing `fastapi_sqlalchemy_toolkit-0.7.4.tar` & `fastapi_sqlalchemy_toolkit-0.7.4.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/.flake8
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/.pylintrc
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/Makefile
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/mkdocs.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/.github/workflows/docker-test.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/benefits.md
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/db_validation.md
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/extension.md
--rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/filtering.md
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/index.md
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/sorting.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/transactions.md
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/usage.md
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/utils.md
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/benefits.md
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/db_validation.md
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/extension.md
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/filtering.md
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/index.md
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/sorting.md
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/transactions.md
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/usage.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/utils.md
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/.env
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/__init__.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/config.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/db.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/main.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/managers.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/models.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/api.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/deps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/endpoints/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/endpoints/child.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/filters.py
--rw-r--r--   0        0        0    41723 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/model_manager.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/ordering.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/utils.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/requirements/base.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/requirements/docs.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/requirements/lint.txt
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/requirements/test.txt
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/Dockerfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/__init__.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/conftest.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/db.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/docker-compose.yml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/models.py
--rw-r--r--   0        0        0    27409 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/tests/test_public_methods.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/AUTHORS
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/LICENSE
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/README.md
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/.flake8
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/.pylintrc
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/Makefile
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/mkdocs.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/.github/workflows/docker-test.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/benefits.md
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/db_validation.md
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/extension.md
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/filtering.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/index.md
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/sorting.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/transactions.md
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/usage.md
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/utils.md
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/benefits.md
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/db_validation.md
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/extension.md
+-rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/filtering.md
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/index.md
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/sorting.md
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/transactions.md
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/usage.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/utils.md
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/.env
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/__init__.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/config.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/db.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/main.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/managers.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/models.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/api.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/deps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/endpoints/child.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/filters.py
+-rw-r--r--   0        0        0    41723 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/model_manager.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/ordering.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/requirements/base.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/requirements/docs.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/requirements/lint.txt
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/requirements/test.txt
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/Dockerfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/db.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/docker-compose.yml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/models.py
+-rw-r--r--   0        0        0    27409 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/tests/test_public_methods.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/AUTHORS
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/LICENSE
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/README.md
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 fastapi_sqlalchemy_toolkit-0.7.4.1/PKG-INFO
```

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/mkdocs.yml` & `fastapi_sqlalchemy_toolkit-0.7.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/.github/workflows/docker-test.yml` & `fastapi_sqlalchemy_toolkit-0.7.4.1/.github/workflows/docker-test.yml`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/.github/workflows/python-publish.yml` & `fastapi_sqlalchemy_toolkit-0.7.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/benefits.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/benefits.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/db_validation.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/db_validation.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/extension.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/extension.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/filtering.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/filtering.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/index.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/sorting.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/sorting.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/transactions.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/transactions.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/usage.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/usage.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/utils.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/utils.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/benefits.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/benefits.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/db_validation.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/db_validation.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/extension.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/extension.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/filtering.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/filtering.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/index.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/index.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/sorting.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/sorting.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/transactions.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/transactions.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/usage.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/usage.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/docs/ru/utils.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/docs/ru/utils.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/examples/app/config.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/examples/app/main.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/main.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/examples/app/models.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/examples/app/schemas.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/examples/app/api/endpoints/child.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/examples/app/api/endpoints/child.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/model_manager.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/model_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/ordering.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/ordering.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/fastapi_sqlalchemy_toolkit/utils.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/fastapi_sqlalchemy_toolkit/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from copy import deepcopy
 from typing import Annotated, Any, Optional, TypeVar
 
 import pydantic
+import pydantic_core
 from fastapi import Query
 
 BaseModelT = TypeVar("BaseModelT", bound=pydantic.BaseModel)
 
 
 def _make_field_optional(
     field: pydantic.fields.FieldInfo,
 ) -> tuple[Any, pydantic.fields.FieldInfo]:
     new = deepcopy(field)
     new.default = (
-        None
-        if field.default == pydantic.pydantic_core.PydanticUndefined
-        else field.default
+        None if field.default == pydantic_core.PydanticUndefined else field.default
     )
     new.annotation = Optional[field.annotation]  # type: ignore  # noqa: UP007
     return (new.annotation, new)
 
 
 def make_partial_model(model: type[BaseModelT]) -> type[BaseModelT]:
     """
```

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/tests/conftest.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/tests/db.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/tests/db.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/tests/models.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/tests/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/tests/test_public_methods.py` & `fastapi_sqlalchemy_toolkit-0.7.4.1/tests/test_public_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/LICENSE` & `fastapi_sqlalchemy_toolkit-0.7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/README.md` & `fastapi_sqlalchemy_toolkit-0.7.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/pyproject.toml` & `fastapi_sqlalchemy_toolkit-0.7.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_sqlalchemy_toolkit"
-version = "0.7.4"
+version = "0.7.4.1"
 authors = [
   { name="Egor Kondrashov", email="e.kondr01@gmail.com" },
 ]
 description = "FastAPI SQLAlchemy Toolkit"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_sqlalchemy_toolkit-0.7.4/PKG-INFO` & `fastapi_sqlalchemy_toolkit-0.7.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_sqlalchemy_toolkit
-Version: 0.7.4
+Version: 0.7.4.1
 Summary: FastAPI SQLAlchemy Toolkit
 Project-URL: Homepage, https://github.com/e-kondr01/fastapi-sqlalchemy-toolkit
 Author-email: Egor Kondrashov <e.kondr01@gmail.com>
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

