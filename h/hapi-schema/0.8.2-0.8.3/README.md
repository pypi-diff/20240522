# Comparing `tmp/hapi_schema-0.8.2.tar.gz` & `tmp/hapi_schema-0.8.3.tar.gz`

## Comparing `hapi_schema-0.8.2.tar` & `hapi_schema-0.8.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_currency.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_food_price.py
--rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0    13719 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_views_as_tables.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_wfp_commodity.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/db_wfp_market.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/hapi_views_code_generator.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_definitions.toml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/conftest.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_admin1.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_admin2.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_conflict_event.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_currency.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_dataset.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_food_price.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_food_security.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_funding.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_location.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_national_risk.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_operational_presence.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_org_type.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_patch.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_population.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_refugees.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_sector.py
--rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_views_as_tables.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_wfp_commodity.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/test_wfp_market.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_currency.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_food_price.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_wfp_commodity.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/tests/sample_data/data_wfp_market.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/conftest.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_admin1.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_admin2.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_dataset.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_food_price.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_food_security.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_funding.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_location.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_patch.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_population.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_sector.py
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/PKG-INFO
```

### Comparing `hapi_schema-0.8.2/changelog.md` & `hapi_schema-0.8.3/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.3
+
+### Changed
+- fixed WFP commodity enum
+- change FLOAT to DECIMAL in funding, national\_risk, and food\_security
+
 ## 0.8.2
 
 Miscellaneous fixes for pipelines
 
 ### Changed
 - added from\_cods column to location, admin1, and admin2
```

### Comparing `hapi_schema-0.8.2/contributing.md` & `hapi_schema-0.8.3/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/requirements.txt` & `hapi_schema-0.8.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/.config/pre-commit-config.yaml` & `hapi_schema-0.8.3/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/.github/workflows/publish.yaml` & `hapi_schema-0.8.3/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.3/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.3/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.3/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.3/src/hapi_schema/db_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_currency.py` & `hapi_schema-0.8.3/src/hapi_schema/db_currency.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.3/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_food_price.py` & `hapi_schema-0.8.3/src/hapi_schema/db_food_price.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """FoodPrice table and view."""
 
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     DateTime,
     Enum,
-    Float,
     ForeignKey,
     String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin2 import DBAdmin1, DBAdmin2, DBLocation
@@ -53,15 +53,15 @@
     unit: Mapped[str] = mapped_column(String(32), nullable=False)
     price_flag: Mapped[PriceFlag] = mapped_column(
         Enum(PriceFlag), primary_key=True
     )
     price_type: Mapped[PriceType] = mapped_column(
         Enum(PriceType), primary_key=True
     )
-    price: Mapped[float] = mapped_column(Float, nullable=False)
+    price: Mapped[Decimal] = mapped_column(nullable=False)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.3/src/hapi_schema/db_food_security.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Food security table and view."""
 
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     DateTime,
     Enum,
     Float,
     ForeignKey,
     Integer,
@@ -42,15 +43,15 @@
     ipc_phase: Mapped[IPCPhase] = mapped_column(
         Enum(IPCPhase), primary_key=True
     )
     ipc_type: Mapped[IPCType] = mapped_column(Enum(IPCType), primary_key=True)
     population_in_phase: Mapped[int] = mapped_column(
         Integer, nullable=False, index=True
     )
-    population_fraction_in_phase: Mapped[float] = mapped_column(
+    population_fraction_in_phase: Mapped[Decimal] = mapped_column(
         Float, nullable=False, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.3/src/hapi_schema/db_funding.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Funding subcategory table and view."""
 
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     CheckConstraint,
     DateTime,
     ForeignKey,
     String,
     select,
@@ -51,19 +52,21 @@
         primary_key=True,
     )
 
     appeal_name: Mapped[str] = mapped_column(String(256), nullable=False)
 
     appeal_type: Mapped[str] = mapped_column(String(32), nullable=False)
 
-    requirements_usd: Mapped[float] = mapped_column(nullable=False, index=True)
+    requirements_usd: Mapped[Decimal] = mapped_column(
+        nullable=False, index=True
+    )
 
-    funding_usd: Mapped[float] = mapped_column(nullable=False, index=True)
+    funding_usd: Mapped[Decimal] = mapped_column(nullable=False, index=True)
 
-    funding_pct: Mapped[float] = mapped_column(nullable=False, index=True)
+    funding_pct: Mapped[Decimal] = mapped_column(nullable=False, index=True)
 
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime,
         primary_key=True,
     )
 
     reference_period_end: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.8.3/src/hapi_schema/db_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_location.py` & `hapi_schema-0.8.3/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.3/src/hapi_schema/db_national_risk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """NationalRisk table and view."""
 
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     CheckConstraint,
     DateTime,
     Enum,
     Float,
     ForeignKey,
@@ -51,22 +52,26 @@
     location_ref: Mapped[int] = mapped_column(
         ForeignKey("location.id", onupdate="CASCADE"), primary_key=True
     )
     risk_class: Mapped[RiskClass] = mapped_column(
         Enum(RiskClass), nullable=False
     )
     global_rank: Mapped[int] = mapped_column(Integer, nullable=False)
-    overall_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    hazard_exposure_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    vulnerability_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    coping_capacity_risk: Mapped[float] = mapped_column(Float, nullable=False)
-    meta_missing_indicators_pct: Mapped[float] = mapped_column(
+    overall_risk: Mapped[Decimal] = mapped_column(Float, nullable=False)
+    hazard_exposure_risk: Mapped[Decimal] = mapped_column(
+        Float, nullable=False
+    )
+    vulnerability_risk: Mapped[Decimal] = mapped_column(Float, nullable=False)
+    coping_capacity_risk: Mapped[Decimal] = mapped_column(
+        Float, nullable=False
+    )
+    meta_missing_indicators_pct: Mapped[Decimal] = mapped_column(
         Float, nullable=True
     )
-    meta_avg_recentness_years: Mapped[float] = mapped_column(
+    meta_avg_recentness_years: Mapped[Decimal] = mapped_column(
         Float, nullable=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.8.3/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_org.py` & `hapi_schema-0.8.3/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.3/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.3/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_population.py` & `hapi_schema-0.8.3/src/hapi_schema/db_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.3/src/hapi_schema/db_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.3/src/hapi_schema/db_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_resource.py` & `hapi_schema-0.8.3/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.3/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_views_as_tables.py` & `hapi_schema-0.8.3/src/hapi_schema/db_views_as_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     Boolean,
     DateTime,
     Float,
     Integer,
     String,
@@ -63,15 +64,15 @@
 class DBFoodSecurityVAT(Base):
     __tablename__ = "food_security_vat"
     resource_hdx_id: Mapped[str] = mapped_column(String(36))
     admin2_ref: Mapped[int] = mapped_column(Integer, primary_key=True)
     ipc_phase: Mapped[str] = mapped_column(String(12), primary_key=True)
     ipc_type: Mapped[str] = mapped_column(String(17), primary_key=True)
     population_in_phase: Mapped[int] = mapped_column(Integer, index=True)
-    population_fraction_in_phase: Mapped[float] = mapped_column(
+    population_fraction_in_phase: Mapped[Decimal] = mapped_column(
         Float, index=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, index=True
@@ -91,17 +92,17 @@
 class DBFundingVAT(Base):
     __tablename__ = "funding_vat"
     resource_hdx_id: Mapped[str] = mapped_column(String(36))
     appeal_code: Mapped[str] = mapped_column(String(32), primary_key=True)
     location_ref: Mapped[int] = mapped_column(Integer, primary_key=True)
     appeal_name: Mapped[str] = mapped_column(String(256))
     appeal_type: Mapped[str] = mapped_column(String(32))
-    requirements_usd: Mapped[float] = mapped_column(Float, index=True)
-    funding_usd: Mapped[float] = mapped_column(Float, index=True)
-    funding_pct: Mapped[float] = mapped_column(Float, index=True)
+    requirements_usd: Mapped[Decimal] = mapped_column(Float, index=True)
+    funding_usd: Mapped[Decimal] = mapped_column(Float, index=True)
+    funding_pct: Mapped[Decimal] = mapped_column(Float, index=True)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, index=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=True
     )
     location_code: Mapped[str] = mapped_column(String(128), index=True)
@@ -158,22 +159,22 @@
 
 class DBNationalRiskVAT(Base):
     __tablename__ = "national_risk_vat"
     resource_hdx_id: Mapped[str] = mapped_column(String(36))
     location_ref: Mapped[int] = mapped_column(Integer, primary_key=True)
     risk_class: Mapped[str] = mapped_column(String(9))
     global_rank: Mapped[int] = mapped_column(Integer)
-    overall_risk: Mapped[float] = mapped_column(Float)
-    hazard_exposure_risk: Mapped[float] = mapped_column(Float)
-    vulnerability_risk: Mapped[float] = mapped_column(Float)
-    coping_capacity_risk: Mapped[float] = mapped_column(Float)
-    meta_missing_indicators_pct: Mapped[float] = mapped_column(
+    overall_risk: Mapped[Decimal] = mapped_column(Float)
+    hazard_exposure_risk: Mapped[Decimal] = mapped_column(Float)
+    vulnerability_risk: Mapped[Decimal] = mapped_column(Float)
+    coping_capacity_risk: Mapped[Decimal] = mapped_column(Float)
+    meta_missing_indicators_pct: Mapped[Decimal] = mapped_column(
         Float, nullable=True
     )
-    meta_avg_recentness_years: Mapped[float] = mapped_column(
+    meta_avg_recentness_years: Mapped[Decimal] = mapped_column(
         Float, nullable=True
     )
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, index=True
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_wfp_commodity.py` & `hapi_schema-0.8.3/src/hapi_schema/db_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/db_wfp_market.py` & `hapi_schema-0.8.3/src/hapi_schema/db_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/views.py` & `hapi_schema-0.8.3/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.3/src/hapi_schema/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.3/src/hapi_schema/utils/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 class Gender(str, enum.Enum):
     FEMALE = "f"
     MALE = "m"
     NONBINARY = "x"
     UNSPECIFIED = "u"
     OTHER = "o"
-    EUNUCH = "e"
     ALL = "*"
 
 
 class DisabledMarker(str, enum.Enum):
     YES = "y"
     NO = "n"
     ALL = "*"
@@ -91,15 +90,15 @@
     LOW = "2"
     MEDIUM = "3"
     HIGH = "4"
     VERY_HIGH = "5"
 
 
 class CommodityCategory(str, enum.Enum):
-    CEREALS_TUBORS = "cereals and tubors"
+    CEREALS_TUBERS = "cereals and tubers"
     MEAT_FISH_EGGS = "meat, fish and eggs"
     MILK_DAIRY = "milk and dairy"
     MISCELLANEOUS_FOOD = "miscellaneous food"
     NON_FOOD = "non-food"
-    OILS_FATS = "oils and fats"
+    OIL_FATS = "oil and fats"
     PULSES_NUTS = "pulses and nuts"
     VEGETABLES_FRUITS = "vegetables and fruits"
```

### Comparing `hapi_schema-0.8.2/src/hapi_schema/utils/hapi_views_code_generator.py` & `hapi_schema-0.8.3/src/hapi_schema/utils/hapi_views_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/src/hapi_schema/utils/view_as_table_definitions.toml` & `hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_definitions.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/conftest.py` & `hapi_schema-0.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_admin1.py` & `hapi_schema-0.8.3/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_admin2.py` & `hapi_schema-0.8.3/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_conflict_event.py` & `hapi_schema-0.8.3/tests/test_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_dataset.py` & `hapi_schema-0.8.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_food_price.py` & `hapi_schema-0.8.3/tests/test_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_food_security.py` & `hapi_schema-0.8.3/tests/test_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_funding.py` & `hapi_schema-0.8.3/tests/test_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.3/tests/test_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_location.py` & `hapi_schema-0.8.3/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_national_risk.py` & `hapi_schema-0.8.3/tests/test_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_operational_presence.py` & `hapi_schema-0.8.3/tests/test_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_patch.py` & `hapi_schema-0.8.3/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_population.py` & `hapi_schema-0.8.3/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_poverty_rate.py` & `hapi_schema-0.8.3/tests/test_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_refugees.py` & `hapi_schema-0.8.3/tests/test_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_views_as_tables.py` & `hapi_schema-0.8.3/tests/test_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_wfp_commodity.py` & `hapi_schema-0.8.3/tests/test_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/test_wfp_market.py` & `hapi_schema-0.8.3/tests/test_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.3/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.3/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_food_price.py` & `hapi_schema-0.8.3/tests/sample_data/data_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.3/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.8.3/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.3/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.3/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_patch.py` & `hapi_schema-0.8.3/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_population.py` & `hapi_schema-0.8.3/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.3/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/tests/sample_data/data_resource.py` & `hapi_schema-0.8.3/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/.gitignore` & `hapi_schema-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/LICENSE` & `hapi_schema-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/pyproject.toml` & `hapi_schema-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.2/PKG-INFO` & `hapi_schema-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.2
+Version: 0.8.3
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

