# Comparing `tmp/airbyte-source-exchange-rates-1.3.0.tar.gz` & `tmp/airbyte_source_exchange_rates-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-exchange-rates-1.3.0.tar", last modified: Tue Jan 30 15:11:48 2024, max compression
+gzip compressed data, was "airbyte_source_exchange_rates-1.3.1.tar", max compression
```

## Comparing `airbyte-source-exchange-rates-1.3.0.tar` & `airbyte_source_exchange_rates-1.3.1.tar`

### file list

```diff
@@ -1,28 +1,8 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/
--rw-r--r--   0 root         (0) root         (0)     4260 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4123 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4260 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      814 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       57 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-01-30 15:11:48.000000 airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 15:11:48.312623 airbyte-source-exchange-rates-1.3.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)       55 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)    15820 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       86 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       89 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       55 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4170 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      917 2024-01-30 15:11:46.000000 airbyte-source-exchange-rates-1.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1314 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      252 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 15:11:48.316624 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/schemas/
--rw-r--r--   0 root         (0) root         (0)    11406 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/schemas/exchange_rates.json
--rw-r--r--   0 root         (0) root         (0)      482 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/source.py
--rw-r--r--   0 root         (0) root         (0)     1215 2024-01-30 15:06:43.000000 airbyte-source-exchange-rates-1.3.0/source_exchange_rates/spec.yaml
+-rw-r--r--   0        0        0     4661 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/README.md
+-rw-r--r--   0        0        0      142 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/main.py
+-rw-r--r--   0        0        0      803 2024-05-22 21:03:19.440080 airbyte_source_exchange_rates-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/source_exchange_rates/__init__.py
+-rw-r--r--   0        0        0    16786 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/source_exchange_rates/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/source_exchange_rates/run.py
+-rw-r--r--   0        0        0      482 2024-05-22 20:58:32.989494 airbyte_source_exchange_rates-1.3.1/source_exchange_rates/source.py
+-rw-r--r--   0        0        0     5387 1970-01-01 00:00:00.000000 airbyte_source_exchange_rates-1.3.1/PKG-INFO
```

### Comparing `airbyte-source-exchange-rates-1.3.0/PKG-INFO` & `airbyte_source_exchange_rates-1.3.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,103 @@
-Metadata-Version: 2.1
-Name: airbyte-source-exchange-rates
-Version: 1.3.0
-Summary: Source implementation for Exchange Rates.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-
 # Exchange Rates Source
 
 This is the repository for the Exchange Rates configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/exchange-rates).
 
+## Local development
+
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/exchange-rates)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_exchange_rates/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `src/source_exchange_rates/mnifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source exchange-rates test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-exchange-rates spec
+poetry run source-exchange-rates check --config secrets/config.json
+poetry run source-exchange-rates discover --config secrets/config.json
+poetry run source-exchange-rates read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-exchange-rates build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-exchange-rates:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-exchange-rates:dev .
+airbyte-ci connectors --name=source-exchange-rates build
 ```
 
+An image will be available on your host with the tag `airbyte/source-exchange-rates:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-exchange-rates:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-exchange-rates:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-exchange-rates:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-exchange-rates:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-exchange-rates test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-exchange-rates test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/exchange-rates.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/exchange-rates.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-exchange-rates-1.3.0/airbyte_source_exchange_rates.egg-info/PKG-INFO` & `airbyte_source_exchange_rates-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,122 @@
 Metadata-Version: 2.1
 Name: airbyte-source-exchange-rates
-Version: 1.3.0
-Summary: Source implementation for Exchange Rates.
+Version: 1.3.1
+Summary: Source implementation for exchange-rates.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/exchange-rates
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
 # Exchange Rates Source
 
 This is the repository for the Exchange Rates configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/exchange-rates).
 
+## Local development
+
+### Prerequisites
+
+* Python (`^3.9`)
+* Poetry (`^1.7`) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+
+### Installing the connector
+
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/exchange-rates)
-to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_exchange_rates/spec.yaml` file.
+to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `spec` inside `src/source_exchange_rates/mnifest.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source exchange-rates test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
 
+```
+poetry run source-exchange-rates spec
+poetry run source-exchange-rates check --config secrets/config.json
+poetry run source-exchange-rates discover --config secrets/config.json
+poetry run source-exchange-rates read --config secrets/config.json --catalog integration_tests/configured_catalog.json
+```
+
+### Running tests
+
+To run tests locally, from the connector directory run:
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
-```bash
-airbyte-ci connectors --name=source-exchange-rates build
+```
+poetry run pytest tests
 ```
 
-An image will be built with the tag `airbyte/source-exchange-rates:dev`.
+### Building the docker image
 
-**Via `docker build`:**
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
-docker build -t airbyte/source-exchange-rates:dev .
+airbyte-ci connectors --name=source-exchange-rates build
 ```
 
+An image will be available on your host with the tag `airbyte/source-exchange-rates:dev`.
+
+
+### Running as a docker container
+
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-exchange-rates:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-exchange-rates:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-exchange-rates:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-exchange-rates:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-exchange-rates test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
+
+## Publishing a new version of the connector
 
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-exchange-rates test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/exchange-rates.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/exchange-rates.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

