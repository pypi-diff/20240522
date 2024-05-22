# Comparing `tmp/airbyte_source_coin_api-0.2.4.tar.gz` & `tmp/airbyte_source_coin_api-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_coin_api-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_coin_api-0.2.5.tar", max compression
```

## Comparing `airbyte_source_coin_api-0.2.4.tar` & `airbyte_source_coin_api-0.2.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4532 2024-05-01 18:33:56.658763 airbyte_source_coin_api-0.2.4/README.md
--rw-r--r--   0        0        0      755 2024-05-01 18:37:44.272873 airbyte_source_coin_api-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-01 18:33:56.662763 airbyte_source_coin_api-0.2.4/source_coin_api/__init__.py
--rw-r--r--   0        0        0     7223 2024-05-01 18:33:56.662763 airbyte_source_coin_api-0.2.4/source_coin_api/manifest.yaml
--rw-r--r--   0        0        0      234 2024-05-01 18:33:56.662763 airbyte_source_coin_api-0.2.4/source_coin_api/run.py
--rw-r--r--   0        0        0      476 2024-05-01 18:33:56.662763 airbyte_source_coin_api-0.2.4/source_coin_api/source.py
--rw-r--r--   0        0        0     1899 2024-05-01 18:33:56.662763 airbyte_source_coin_api-0.2.4/source_coin_api/spec.yaml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_coin_api-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-21 23:46:36.000000 airbyte_source_coin_api-0.2.5/README.md
+-rw-r--r--   0        0        0      755 2024-05-22 00:08:44.636999 airbyte_source_coin_api-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-21 23:46:36.000000 airbyte_source_coin_api-0.2.5/source_coin_api/__init__.py
+-rw-r--r--   0        0        0    10007 2024-05-21 23:46:36.000000 airbyte_source_coin_api-0.2.5/source_coin_api/manifest.yaml
+-rw-r--r--   0        0        0      234 2024-05-21 23:46:36.000000 airbyte_source_coin_api-0.2.5/source_coin_api/run.py
+-rw-r--r--   0        0        0      476 2024-05-21 23:46:36.000000 airbyte_source_coin_api-0.2.5/source_coin_api/source.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 airbyte_source_coin_api-0.2.5/PKG-INFO
```

### Comparing `airbyte_source_coin_api-0.2.4/README.md` & `airbyte_source_coin_api-0.2.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Coin-Api source connector
 
-
 This is the repository for the Coin-Api source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/coin-api).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/coin-api)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_coin_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-coin-api spec
 poetry run source-coin-api check --config secrets/config.json
 poetry run source-coin-api discover --config secrets/config.json
 poetry run source-coin-api read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-coin-api build
 ```
 
 An image will be available on your host with the tag `airbyte/source-coin-api:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-coin-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coin-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coin-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-coin-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-coin-api test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-coin-api test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/coin-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_coin_api-0.2.4/pyproject.toml` & `airbyte_source_coin_api-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.2.5"
 name = "airbyte-source-coin-api"
 description = "Source implementation for Coin Api."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_coin_api-0.2.4/PKG-INFO` & `airbyte_source_coin_api-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-coin-api
-Version: 0.2.4
+Version: 0.2.5
 Summary: Source implementation for Coin Api.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/coin-api
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Coin-Api source connector
 
-
 This is the repository for the Coin-Api source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/coin-api).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/coin-api)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_coin_api/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-coin-api spec
 poetry run source-coin-api check --config secrets/config.json
 poetry run source-coin-api discover --config secrets/config.json
 poetry run source-coin-api read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-coin-api build
 ```
 
 An image will be available on your host with the tag `airbyte/source-coin-api:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-coin-api:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coin-api:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-coin-api:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-coin-api:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-coin-api test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-coin-api test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/coin-api.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

