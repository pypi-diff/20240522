# Comparing `tmp/aiokafkaengine-0.0.2.tar.gz` & `tmp/aiokafkaengine-0.0.3.tar.gz`

## Comparing `aiokafkaengine-0.0.2.tar` & `aiokafkaengine-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/dev_requirements.txt
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/docker-compose.yml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/notes.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/requirements.txt
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/.vscode/settings.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/kafka_setup/.dockerignore
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/kafka_setup/Dockerfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/kafka_setup/requirements.txt
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/kafka_setup/setup_kafka.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/kafka_setup/kafka_data/.gitkeep
--rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/src/AioKafkaEngine/AioKafkaEngine.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/src/AioKafkaEngine/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/tests/.gitkeep
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/tests/test_aio_kafka_engine.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/.gitignore
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/LICENSE
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/dev_requirements.txt
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/docker-compose.yml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/notes.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/.vscode/launch.json
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/.vscode/settings.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/kafka_setup/.dockerignore
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/kafka_setup/Dockerfile
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/kafka_setup/requirements.txt
+-rw-r--r--   0        0        0     2353 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/kafka_setup/setup_kafka.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/kafka_setup/kafka_data/.gitkeep
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/src/AioKafkaEngine/AioKafkaEngine.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/src/AioKafkaEngine/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/tests/.gitkeep
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/tests/pytest.ini
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/tests/test_aio_kafka_engine.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/LICENSE
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 aiokafkaengine-0.0.3/PKG-INFO
```

### Comparing `aiokafkaengine-0.0.2/docker-compose.yml` & `aiokafkaengine-0.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aiokafkaengine-0.0.2/.github/workflows/python-package.yml` & `aiokafkaengine-0.0.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `aiokafkaengine-0.0.2/.gitignore` & `aiokafkaengine-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aiokafkaengine-0.0.2/LICENSE` & `aiokafkaengine-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiokafkaengine-0.0.2/pyproject.toml` & `aiokafkaengine-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "AioKafkaEngine"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Extreme4all", email="author@example.com" },
 ]
 description = "Wrapper around aio-kafka to use and receive via a asyncio queue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aiokafkaengine-0.0.2/PKG-INFO` & `aiokafkaengine-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: AioKafkaEngine
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around aio-kafka to use and receive via a asyncio queue
 Project-URL: Homepage, https://github.com/Bot-detector/AioKafkaEngine
 Project-URL: Bug Tracker, https://github.com/Bot-detector/AioKafkaEngine/issues
 Author-email: Extreme4all <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

