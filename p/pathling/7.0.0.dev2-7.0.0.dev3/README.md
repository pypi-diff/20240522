# Comparing `tmp/pathling-7.0.0.dev2.tar.gz` & `tmp/pathling-7.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathling-7.0.0.dev2.tar", last modified: Mon May 20 04:35:24 2024, max compression
+gzip compressed data, was "pathling-7.0.0.dev3.tar", last modified: Mon May 20 07:36:53 2024, max compression
```

## Comparing `pathling-7.0.0.dev2.tar` & `pathling-7.0.0.dev3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.902081 pathling-7.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-20 04:35:24.902081 pathling-7.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.894081 pathling-7.0.0.dev2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.894081 pathling-7.0.0.dev2/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.898081 pathling-7.0.0.dev2/examples/data/bundles/
--rw-r--r--   0 runner    (1001) docker     (127)    86431 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json
--rw-r--r--   0 runner    (1001) docker     (127)    66676 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.898081 pathling-7.0.0.dev2/examples/data/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/data/resources/Condition.ndjson
--rw-r--r--   0 runner    (1001) docker     (127)    29641 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/data/resources/Patient.ndjson
--rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/designation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/display.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/encode_bundles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/encode_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1606 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/member_of.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1358 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/member_of_old.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/property_of.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4537 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/query.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/subsumes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/subsumes_old.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1347 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/translate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1310 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/examples/translate_old.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.898081 pathling-7.0.0.dev2/pathling/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 04:35:20.000000 pathling-7.0.0.dev2/pathling/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/coding.py
--rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/datasink.py
--rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/fhir.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/pathling/udfs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.902081 pathling-7.0.0.dev2/pathling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-20 04:35:24.000000 pathling-7.0.0.dev2/pathling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 04:35:24.000000 pathling-7.0.0.dev2/pathling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 04:35:24.000000 pathling-7.0.0.dev2/pathling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 04:35:24.000000 pathling-7.0.0.dev2/pathling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 04:35:24.000000 pathling-7.0.0.dev2/pathling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 04:35:24.902081 pathling-7.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 04:35:24.902081 pathling-7.0.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/tests/test_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/tests/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-05-20 04:32:59.000000 pathling-7.0.0.dev2/tests/test_udfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.096365 pathling-7.0.0.dev3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-20 07:36:53.096365 pathling-7.0.0.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.088365 pathling-7.0.0.dev3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.088365 pathling-7.0.0.dev3/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.092365 pathling-7.0.0.dev3/examples/data/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)    86431 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json
+-rw-r--r--   0 runner    (1001) docker     (127)    66676 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.092365 pathling-7.0.0.dev3/examples/data/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/data/resources/Condition.ndjson
+-rw-r--r--   0 runner    (1001) docker     (127)    29641 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/data/resources/Patient.ndjson
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1263 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/designation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1111 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/display.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1300 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/encode_bundles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/encode_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1606 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/member_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1358 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/member_of_old.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1499 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/property_of.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4536 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/query.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1688 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/subsumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1755 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/subsumes_old.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1347 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/translate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1310 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/examples/translate_old.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.092365 pathling-7.0.0.dev3/pathling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 07:36:47.000000 pathling-7.0.0.dev3/pathling/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20655 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/datasink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/fhir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10302 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/pathling/udfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.096365 pathling-7.0.0.dev3/pathling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-20 07:36:53.000000 pathling-7.0.0.dev3/pathling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 07:36:53.000000 pathling-7.0.0.dev3/pathling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:36:53.000000 pathling-7.0.0.dev3/pathling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 07:36:53.000000 pathling-7.0.0.dev3/pathling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 07:36:53.000000 pathling-7.0.0.dev3/pathling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 07:36:53.096365 pathling-7.0.0.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:36:53.096365 pathling-7.0.0.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/tests/test_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/tests/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14214 2024-05-20 07:34:29.000000 pathling-7.0.0.dev3/tests/test_udfs.py
```

### Comparing `pathling-7.0.0.dev2/LICENSE` & `pathling-7.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/PKG-INFO` & `pathling-7.0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathling
-Version: 7.0.0.dev2
+Version: 7.0.0.dev3
 Summary: Python API for Pathling
 Home-page: https://github.com/aehrc/pathling
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache License, version 2.0
 Keywords: pathling,fhir,analytics,spark,standards,terminology
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pathling-7.0.0.dev2/README.md` & `pathling-7.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json` & `pathling-7.0.0.dev3/examples/data/bundles/Bennett146_Swaniawski813_704c9750-f6e6-473b-ee83-fbd48e07fe3f.json`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json` & `pathling-7.0.0.dev3/examples/data/bundles/Dino214_Parisian75_40d82b80-b682-cd8b-da6d-396809878641.json`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/data/resources/Condition.ndjson` & `pathling-7.0.0.dev3/examples/data/resources/Condition.ndjson`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/data/resources/Patient.ndjson` & `pathling-7.0.0.dev3/examples/data/resources/Patient.ndjson`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/designation.py` & `pathling-7.0.0.dev3/examples/designation.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/display.py` & `pathling-7.0.0.dev3/examples/display.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/encode_bundles.py` & `pathling-7.0.0.dev3/examples/encode_bundles.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/encode_resources.py` & `pathling-7.0.0.dev3/examples/encode_resources.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/member_of.py` & `pathling-7.0.0.dev3/examples/member_of.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/member_of_old.py` & `pathling-7.0.0.dev3/examples/member_of_old.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/property_of.py` & `pathling-7.0.0.dev3/examples/property_of.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/query.py` & `pathling-7.0.0.dev3/examples/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import os
-from tempfile import mkdtemp
-
 from pyspark.sql import DataFrame, SparkSession
+from tempfile import mkdtemp
 
 from pathling import PathlingContext, DataSource, Expression as exp
 from pathling._version import __java_version__
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 DATA_DIR = os.path.join(HERE, "data")
 BUNDLES_DIR = os.path.join(DATA_DIR, "bundles")
@@ -32,15 +31,15 @@
 WAREHOUSE_DIR = os.path.join(TEMP_DIR, "warehouse")
 NDJSON_DIR_2 = os.path.join(TEMP_DIR, "ndjson")
 
 # Configure Hive, so that we can test out the tables functionality.
 spark = (
     SparkSession.builder.config(
         "spark.jars.packages",
-        f"au.csiro.pathling:library-runtime:{__java_version__},io.delta:delta-spark_2.12:3.1.0",
+        f"au.csiro.pathling:library-runtime:{__java_version__},io.delta:delta-spark_2.12:3.2.0",
     )
     .config(
         "spark.sql.extensions",
         "io.delta.sql.DeltaSparkSessionExtension",
     )
     .config(
         "spark.sql.catalog.spark_catalog",
```

### Comparing `pathling-7.0.0.dev2/examples/subsumes.py` & `pathling-7.0.0.dev3/examples/subsumes.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/subsumes_old.py` & `pathling-7.0.0.dev3/examples/subsumes_old.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/translate.py` & `pathling-7.0.0.dev3/examples/translate.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/examples/translate_old.py` & `pathling-7.0.0.dev3/examples/translate_old.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/__init__.py` & `pathling-7.0.0.dev3/pathling/__init__.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/coding.py` & `pathling-7.0.0.dev3/pathling/coding.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/context.py` & `pathling-7.0.0.dev3/pathling/context.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/core.py` & `pathling-7.0.0.dev3/pathling/core.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/datasink.py` & `pathling-7.0.0.dev3/pathling/datasink.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,51 +24,82 @@
     Constants that represent the different import modes.
     """
 
     OVERWRITE: str = "overwrite"
     MERGE: str = "merge"
 
 
+class SaveMode:
+    """
+    Constants that represent the different save modes.
+
+    OVERWRITE: Overwrite any existing data.
+    APPEND: Append the new data to the existing data.
+    IGNORE: Only save the data if the file does not already exist.
+    ERROR: Raise an error if the file already exists.
+    """
+
+    OVERWRITE: str = "overwrite"
+    APPEND: str = "append"
+    IGNORE: str = "ignore"
+    ERROR: str = "error"
+
+
 class DataSinks(SparkConversionsMixin):
     """
     A class for writing FHIR data to a variety of different targets.
     """
 
     def __init__(self, datasource: DataSource):
         SparkConversionsMixin.__init__(self, datasource.spark)
         self._datasinks = (
             self.spark._jvm.au.csiro.pathling.library.io.sink.DataSinkBuilder(
                 datasource.pc._jpc, datasource._jds
             )
         )
 
-    def ndjson(self, path: str, file_name_mapper: Callable[[str], str] = None) -> None:
+    def ndjson(
+        self,
+        path: str,
+        save_mode: Optional[str] = SaveMode.ERROR,
+        file_name_mapper: Callable[[str], str] = None,
+    ) -> None:
         """
         Writes the data to a directory of NDJSON files. The files will be named using the resource
         type and the ".ndjson" extension.
 
         :param path: The URI of the directory to write the files to.
+        :param save_mode: The save mode to use when writing the data:
+            - "overwrite" will overwrite any existing data.
+            - "append" will append the new data to the existing data.
+            - "ignore" will only save the data if the file does not already exist.
+            - "error" will raise an error if the file already exists.
         :param file_name_mapper: An optional function that can be used to customise the mapping of
         the resource type to the file name.
         """
         if file_name_mapper:
             wrapped_mapper = StringMapper(
                 self.spark._jvm._gateway_client, file_name_mapper
             )
-            self._datasinks.ndjson(path, wrapped_mapper)
+            self._datasinks.ndjson(path, save_mode, wrapped_mapper)
         else:
-            self._datasinks.ndjson(path)
+            self._datasinks.ndjson(path, save_mode)
 
-    def parquet(self, path: str) -> None:
+    def parquet(self, path: str, save_mode: Optional[str] = SaveMode.ERROR) -> None:
         """
         Writes the data to a directory of Parquet files.
 
         :param path: The URI of the directory to write the files to.
+        :param save_mode: The save mode to use when writing the data:
+            - "overwrite" will overwrite any existing data.
+            - "append" will append the new data to the existing data.
+            - "ignore" will only save the data if the file does not already exist.
+            - "error" will raise an error if the file already exists.
         """
-        self._datasinks.parquet(path)
+        self._datasinks.parquet(path, save_mode)
 
     def delta(
         self, path: str, import_mode: Optional[str] = ImportMode.OVERWRITE
     ) -> None:
         """
         Writes the data to a directory of Delta files.
```

### Comparing `pathling-7.0.0.dev2/pathling/datasource.py` & `pathling-7.0.0.dev3/pathling/datasource.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/fhir.py` & `pathling-7.0.0.dev3/pathling/fhir.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/functions.py` & `pathling-7.0.0.dev3/pathling/functions.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/query.py` & `pathling-7.0.0.dev3/pathling/query.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling/udfs.py` & `pathling-7.0.0.dev3/pathling/udfs.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/pathling.egg-info/PKG-INFO` & `pathling-7.0.0.dev3/pathling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pathling
-Version: 7.0.0.dev2
+Version: 7.0.0.dev3
 Summary: Python API for Pathling
 Home-page: https://github.com/aehrc/pathling
 Author: Australian e-Health Research Centre, CSIRO
 Author-email: ontoserver-support@csiro.au
 License: Apache License, version 2.0
 Keywords: pathling,fhir,analytics,spark,standards,terminology
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pathling-7.0.0.dev2/pathling.egg-info/SOURCES.txt` & `pathling-7.0.0.dev3/pathling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/setup.py` & `pathling-7.0.0.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/tests/test_datasource.py` & `pathling-7.0.0.dev3/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/tests/test_encoders.py` & `pathling-7.0.0.dev3/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/tests/test_functions.py` & `pathling-7.0.0.dev3/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/tests/test_query.py` & `pathling-7.0.0.dev3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pathling-7.0.0.dev2/tests/test_udfs.py` & `pathling-7.0.0.dev3/tests/test_udfs.py`

 * *Files identical despite different names*

