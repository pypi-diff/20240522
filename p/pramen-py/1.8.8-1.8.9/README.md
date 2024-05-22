# Comparing `tmp/pramen_py-1.8.8.tar.gz` & `tmp/pramen_py-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pramen_py-1.8.8.tar", max compression
+gzip compressed data, was "pramen_py-1.8.9.tar", max compression
```

## Comparing `pramen_py-1.8.8.tar` & `pramen_py-1.8.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1281 2024-05-16 06:42:42.133395 pramen_py-1.8.8/.env.example
--rw-r--r--   0        0        0     5111 2024-05-16 06:42:42.133395 pramen_py-1.8.8/README.md
--rw-r--r--   0        0        0     3763 2024-05-16 06:42:42.889402 pramen_py-1.8.8/pyproject.toml
--rw-r--r--   0        0        0      912 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/__init__.py
--rw-r--r--   0        0        0      790 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/app/__init__.py
--rw-r--r--   0        0        0     4290 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/app/cli.py
--rw-r--r--   0        0        0     1187 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/app/logger.py
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/metastore/__init__.py
--rw-r--r--   0        0        0    14366 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/metastore/reader.py
--rw-r--r--   0        0        0     4422 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/metastore/reader_base.py
--rw-r--r--   0        0        0     4610 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/metastore/writer.py
--rw-r--r--   0        0        0     1657 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/metastore/writer_base.py
--rw-r--r--   0        0        0     4688 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/models/__init__.py
--rw-r--r--   0        0        0     1387 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/models/utils.py
--rw-r--r--   0        0        0        0 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/py.typed
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/runner/__init__.py
--rw-r--r--   0        0        0     6408 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/runner/runner_base.py
--rw-r--r--   0        0        0     7431 2024-05-16 06:42:42.133395 pramen_py-1.8.8/src/pramen_py/runner/runner_transformation.py
--rw-r--r--   0        0        0     1098 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/test_utils/__init__.py
--rw-r--r--   0        0        0     3693 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/test_utils/fixtures.py
--rw-r--r--   0        0        0      684 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/test_utils/plugin.py
--rw-r--r--   0        0        0     4378 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/test_utils/spark_utils.py
--rw-r--r--   0        0        0    10788 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/test_utils/when.py
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/transformation/__init__.py
--rw-r--r--   0        0        0     1977 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/transformation/transformation_base.py
--rw-r--r--   0        0        0     7375 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/utils/__init__.py
--rw-r--r--   0        0        0     5320 2024-05-16 06:42:42.137395 pramen_py-1.8.8/src/pramen_py/utils/file_system.py
--rw-r--r--   0        0        0     1610 2024-05-16 06:42:42.137395 pramen_py-1.8.8/tests/resources/real_config.yaml
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/__init__.py
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/example_trasformation_one/__init__.py
--rw-r--r--   0        0        0     1371 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/example_trasformation_one/some_transformation.py
--rw-r--r--   0        0        0      592 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/example_trasformation_two/__init__.py
--rw-r--r--   0        0        0     1313 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/example_trasformation_two/some_transformation.py
--rw-r--r--   0        0        0     1534 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/identity_transformer/__init__.py
--rw-r--r--   0        0        0      612 2024-05-16 06:42:42.137395 pramen_py-1.8.8/transformations/identity_transformer/example_config.yaml
--rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 pramen_py-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1281 2024-05-22 07:32:50.025353 pramen_py-1.8.9/.env.example
+-rw-r--r--   0        0        0     5111 2024-05-22 07:32:50.025353 pramen_py-1.8.9/README.md
+-rw-r--r--   0        0        0     3763 2024-05-22 07:32:50.797351 pramen_py-1.8.9/pyproject.toml
+-rw-r--r--   0        0        0      912 2024-05-22 07:32:50.025353 pramen_py-1.8.9/src/pramen_py/__init__.py
+-rw-r--r--   0        0        0      790 2024-05-22 07:32:50.025353 pramen_py-1.8.9/src/pramen_py/app/__init__.py
+-rw-r--r--   0        0        0     4290 2024-05-22 07:32:50.025353 pramen_py-1.8.9/src/pramen_py/app/cli.py
+-rw-r--r--   0        0        0     1187 2024-05-22 07:32:50.025353 pramen_py-1.8.9/src/pramen_py/app/logger.py
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/metastore/__init__.py
+-rw-r--r--   0        0        0    14366 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/metastore/reader.py
+-rw-r--r--   0        0        0     4422 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/metastore/reader_base.py
+-rw-r--r--   0        0        0     4610 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/metastore/writer.py
+-rw-r--r--   0        0        0     1657 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/metastore/writer_base.py
+-rw-r--r--   0        0        0     4688 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/models/__init__.py
+-rw-r--r--   0        0        0     1387 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/models/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/py.typed
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/runner/__init__.py
+-rw-r--r--   0        0        0     6408 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/runner/runner_base.py
+-rw-r--r--   0        0        0     7431 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/runner/runner_transformation.py
+-rw-r--r--   0        0        0     1098 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/test_utils/__init__.py
+-rw-r--r--   0        0        0     3693 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/test_utils/fixtures.py
+-rw-r--r--   0        0        0      684 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/test_utils/plugin.py
+-rw-r--r--   0        0        0     4378 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/test_utils/spark_utils.py
+-rw-r--r--   0        0        0    10788 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/test_utils/when.py
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/transformation/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/transformation/transformation_base.py
+-rw-r--r--   0        0        0     7375 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/utils/__init__.py
+-rw-r--r--   0        0        0     5320 2024-05-22 07:32:50.029353 pramen_py-1.8.9/src/pramen_py/utils/file_system.py
+-rw-r--r--   0        0        0     1610 2024-05-22 07:32:50.029353 pramen_py-1.8.9/tests/resources/real_config.yaml
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/__init__.py
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/example_trasformation_one/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/example_trasformation_one/some_transformation.py
+-rw-r--r--   0        0        0      592 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/example_trasformation_two/__init__.py
+-rw-r--r--   0        0        0     1313 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/example_trasformation_two/some_transformation.py
+-rw-r--r--   0        0        0     1534 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/identity_transformer/__init__.py
+-rw-r--r--   0        0        0      612 2024-05-22 07:32:50.029353 pramen_py-1.8.9/transformations/identity_transformer/example_config.yaml
+-rw-r--r--   0        0        0     6719 1970-01-01 00:00:00.000000 pramen_py-1.8.9/PKG-INFO
```

### Comparing `pramen_py-1.8.8/.env.example` & `pramen_py-1.8.9/.env.example`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/README.md` & `pramen_py-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/pyproject.toml` & `pramen_py-1.8.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 [tool.pytest.ini_options]
 minversion = "6.0.0"
 addopts = "-vv -s --tb=native -n auto"
 testpaths = "tests/"
 
 [tool.poetry]
 name = "pramen-py"
-version = "1.8.8"
+version = "1.8.9"
 description = "Pramen transformations written in python"
 authors = [
     "Artem Zhukov <iam@zhukovgreen.pro>",
     "Valerii Khalimendik <Valerii.Khalimendik@absa.africa>",
     "Jiří Filip <Jiri.Filip@absa.africa>"
 ]
 maintainers = [
```

### Comparing `pramen_py-1.8.8/src/pramen_py/__init__.py` & `pramen_py-1.8.9/src/pramen_py/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/app/__init__.py` & `pramen_py-1.8.9/src/pramen_py/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/app/cli.py` & `pramen_py-1.8.9/src/pramen_py/app/cli.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/app/logger.py` & `pramen_py-1.8.9/src/pramen_py/app/logger.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/metastore/__init__.py` & `pramen_py-1.8.9/src/pramen_py/metastore/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/metastore/reader.py` & `pramen_py-1.8.9/src/pramen_py/metastore/reader.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/metastore/reader_base.py` & `pramen_py-1.8.9/src/pramen_py/metastore/reader_base.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/metastore/writer.py` & `pramen_py-1.8.9/src/pramen_py/metastore/writer.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/metastore/writer_base.py` & `pramen_py-1.8.9/src/pramen_py/metastore/writer_base.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/models/__init__.py` & `pramen_py-1.8.9/src/pramen_py/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/models/utils.py` & `pramen_py-1.8.9/src/pramen_py/models/utils.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/runner/__init__.py` & `pramen_py-1.8.9/src/pramen_py/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/runner/runner_base.py` & `pramen_py-1.8.9/src/pramen_py/runner/runner_base.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/runner/runner_transformation.py` & `pramen_py-1.8.9/src/pramen_py/runner/runner_transformation.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/test_utils/__init__.py` & `pramen_py-1.8.9/src/pramen_py/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/test_utils/fixtures.py` & `pramen_py-1.8.9/src/pramen_py/test_utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/test_utils/plugin.py` & `pramen_py-1.8.9/src/pramen_py/test_utils/plugin.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/test_utils/spark_utils.py` & `pramen_py-1.8.9/src/pramen_py/test_utils/spark_utils.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/test_utils/when.py` & `pramen_py-1.8.9/src/pramen_py/test_utils/when.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/transformation/__init__.py` & `pramen_py-1.8.9/src/pramen_py/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/transformation/transformation_base.py` & `pramen_py-1.8.9/src/pramen_py/transformation/transformation_base.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/utils/__init__.py` & `pramen_py-1.8.9/src/pramen_py/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/src/pramen_py/utils/file_system.py` & `pramen_py-1.8.9/src/pramen_py/utils/file_system.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/tests/resources/real_config.yaml` & `pramen_py-1.8.9/tests/resources/real_config.yaml`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/__init__.py` & `pramen_py-1.8.9/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/example_trasformation_one/__init__.py` & `pramen_py-1.8.9/transformations/example_trasformation_one/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/example_trasformation_one/some_transformation.py` & `pramen_py-1.8.9/transformations/example_trasformation_one/some_transformation.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/example_trasformation_two/__init__.py` & `pramen_py-1.8.9/transformations/example_trasformation_two/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/example_trasformation_two/some_transformation.py` & `pramen_py-1.8.9/transformations/example_trasformation_two/some_transformation.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/identity_transformer/__init__.py` & `pramen_py-1.8.9/transformations/identity_transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/transformations/identity_transformer/example_config.yaml` & `pramen_py-1.8.9/transformations/identity_transformer/example_config.yaml`

 * *Files identical despite different names*

### Comparing `pramen_py-1.8.8/PKG-INFO` & `pramen_py-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pramen-py
-Version: 1.8.8
+Version: 1.8.9
 Summary: Pramen transformations written in python
 Home-page: https://github.com/AbsaOSS/pramen
 Keywords: paramen,pyspark,transformations,metastore
 Author: Artem Zhukov
 Author-email: iam@zhukovgreen.pro
 Maintainer: Artem Zhukov
 Maintainer-email: iam@zhukovgreen.pro
```

