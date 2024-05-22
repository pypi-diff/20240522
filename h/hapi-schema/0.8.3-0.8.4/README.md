# Comparing `tmp/hapi_schema-0.8.3.tar.gz` & `tmp/hapi_schema-0.8.4.tar.gz`

## Comparing `hapi_schema-0.8.3.tar` & `hapi_schema-0.8.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_currency.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_food_price.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_views_as_tables.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_wfp_commodity.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/db_wfp_market.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/hapi_views_code_generator.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_definitions.toml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/conftest.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_admin1.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_admin2.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_conflict_event.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_currency.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_dataset.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_food_price.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_food_security.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_funding.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_location.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_national_risk.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_operational_presence.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_org_type.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_patch.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_population.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_refugees.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_sector.py
--rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_views_as_tables.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_wfp_commodity.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/test_wfp_market.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_currency.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_food_price.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_wfp_commodity.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/tests/sample_data/data_wfp_market.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    13767 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6718 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/conftest.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_admin1.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_admin2.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_dataset.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_food_price.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_food_security.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_funding.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_location.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_patch.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_population.py
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_sector.py
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.4/PKG-INFO
```

### Comparing `hapi_schema-0.8.3/changelog.md` & `hapi_schema-0.8.4/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.4
+
+### Added
+
+- New constraints: rate\_constraint
+
+### Changed
+
+- remove ALL ("*") from PovertyClassification enum
+- refactor DBPovertyRate to track rates rather than population, and link to location (with admin1\_name as a text field)
+
 ## 0.8.3
 
 ### Changed
 - fixed WFP commodity enum
 - change FLOAT to DECIMAL in funding, national\_risk, and food\_security
 
 ## 0.8.2
```

### Comparing `hapi_schema-0.8.3/contributing.md` & `hapi_schema-0.8.4/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/requirements.txt` & `hapi_schema-0.8.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/.config/pre-commit-config.yaml` & `hapi_schema-0.8.4/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/.github/workflows/publish.yaml` & `hapi_schema-0.8.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.4/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.4/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.4/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.4/src/hapi_schema/db_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_currency.py` & `hapi_schema-0.8.4/src/hapi_schema/db_currency.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.4/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_food_price.py` & `hapi_schema-0.8.4/src/hapi_schema/db_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.4/src/hapi_schema/db_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.4/src/hapi_schema/db_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.8.4/src/hapi_schema/db_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_location.py` & `hapi_schema-0.8.4/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.4/src/hapi_schema/db_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.8.4/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_org.py` & `hapi_schema-0.8.4/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.4/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.4/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_population.py` & `hapi_schema-0.8.4/src/hapi_schema/db_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.4/src/hapi_schema/db_poverty_rate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,76 @@
 """PovertyRate table and view."""
 
 from datetime import datetime
+from decimal import Decimal
 
 from sqlalchemy import (
     DateTime,
     Enum,
     ForeignKey,
-    Integer,
+    String,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
-from hapi_schema.db_admin1 import DBAdmin1
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_resource import DBResource
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
-    population_constraint,
+    rate_constraint,
     reference_period_constraint,
 )
 from hapi_schema.utils.enums import PovertyClassification
 from hapi_schema.utils.view_params import ViewParams
 
 
 # normalised table
 class DBPovertyRate(Base):
     __tablename__ = "poverty_rate"
     __table_args__ = (
-        population_constraint(),
+        rate_constraint(),
         reference_period_constraint(),
     )
 
     resource_hdx_id: Mapped[str] = mapped_column(
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
-    admin1_ref: Mapped[int] = mapped_column(
-        ForeignKey("admin1.id", onupdate="CASCADE"),
+    location_ref: Mapped[int] = mapped_column(
+        ForeignKey("location.id", onupdate="CASCADE"),
         nullable=False,
         primary_key=True,
     )
+    admin1_name: Mapped[str] = mapped_column(
+        String(512), nullable=False, index=True, primary_key=True
+    )
     classification: Mapped[PovertyClassification] = mapped_column(
         Enum(PovertyClassification), nullable=False, primary_key=True
     )
-    population: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
+    rate: Mapped[Decimal] = mapped_column(nullable=True, index=False)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
         DateTime, nullable=False, index=True
     )
 
     resource = relationship(DBResource)
-    admin1 = relationship(DBAdmin1)
+    location = relationship(DBLocation)
 
 
 # view
 view_params_poverty_rate = ViewParams(
     name="poverty_rate_view",
     metadata=Base.metadata,
     selectable=select(
         *DBPovertyRate.__table__.columns,
         DBLocation.code.label("location_code"),
         DBLocation.name.label("location_name"),
-        DBAdmin1.code.label("admin1_code"),
-        DBAdmin1.name.label("admin1_name"),
-        DBAdmin1.is_unspecified.label("admin1_is_unspecified"),
-        DBAdmin1.location_ref.label("location_ref"),
     ).select_from(
         DBPovertyRate.__table__.join(
-            DBAdmin1.__table__,
-            DBPovertyRate.admin1_ref == DBAdmin1.id,
-            isouter=True,
-        ).join(
             DBLocation.__table__,
-            DBAdmin1.location_ref == DBLocation.id,
+            DBPovertyRate.location_ref == DBLocation.id,
             isouter=True,
         )
     ),
 )
```

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.4/src/hapi_schema/db_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_resource.py` & `hapi_schema-0.8.4/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.4/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_views_as_tables.py` & `hapi_schema-0.8.4/src/hapi_schema/db_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_wfp_commodity.py` & `hapi_schema-0.8.4/src/hapi_schema/db_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/db_wfp_market.py` & `hapi_schema-0.8.4/src/hapi_schema/db_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/views.py` & `hapi_schema-0.8.4/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.4/src/hapi_schema/utils/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,22 @@
     var_name: str,
 ) -> CheckConstraint:
     """Require a column to be non-negative."""
     sqltext = f"{var_name} >= 0"
     return CheckConstraint(sqltext=sqltext, name=f"{var_name}")
 
 
+def rate_constraint(
+    var_name: str = "rate",
+) -> CheckConstraint:
+    """Require a column to be between 0.0 and 1.0."""
+    sqltext = f"{var_name} >= 0 AND {var_name} <= 1.0"
+    return CheckConstraint(sqltext=sqltext, name=f"{var_name}")
+
+
 def reference_period_constraint() -> CheckConstraint:
     """reference_period_end should be greater than reference_period_start"""
     sqltext = "reference_period_end >= reference_period_start "
     return CheckConstraint(sqltext=sqltext, name="reference_period")
 
 
 def general_risk_constraint(risk_name: str) -> CheckConstraint:
```

### Comparing `hapi_schema-0.8.3/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.4/src/hapi_schema/utils/enums.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     WHOLESALE = "Wholesale"
 
 
 class PovertyClassification(str, enum.Enum):
     POOR = "poor"
     VULNERABLE = "vulnerable"
     EXTREMELY_POOR = "extremely_poor"
-    ALL = "*"
 
 
 class IPCPhase(str, enum.Enum):
     PHASE_1 = "1"
     PHASE_2 = "2"
     PHASE_3 = "3"
     PHASE_4 = "4"
```

### Comparing `hapi_schema-0.8.3/src/hapi_schema/utils/hapi_views_code_generator.py` & `hapi_schema-0.8.4/src/hapi_schema/utils/hapi_views_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.4/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/src/hapi_schema/utils/view_as_table_definitions.toml` & `hapi_schema-0.8.4/src/hapi_schema/utils/view_as_table_definitions.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/conftest.py` & `hapi_schema-0.8.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_admin1.py` & `hapi_schema-0.8.4/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_admin2.py` & `hapi_schema-0.8.4/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_conflict_event.py` & `hapi_schema-0.8.4/tests/test_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_dataset.py` & `hapi_schema-0.8.4/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_food_price.py` & `hapi_schema-0.8.4/tests/test_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_food_security.py` & `hapi_schema-0.8.4/tests/test_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_funding.py` & `hapi_schema-0.8.4/tests/test_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.4/tests/test_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_location.py` & `hapi_schema-0.8.4/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_national_risk.py` & `hapi_schema-0.8.4/tests/test_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_operational_presence.py` & `hapi_schema-0.8.4/tests/test_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_patch.py` & `hapi_schema-0.8.4/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_population.py` & `hapi_schema-0.8.4/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_poverty_rate.py` & `hapi_schema-0.8.4/tests/test_poverty_rate.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,28 @@
     run_view_test(
         view=view_poverty_rate,
         whereclause=(
             view_poverty_rate.c.resource_hdx_id
             == "90deb235-1bf5-4bae-b231-3393222c2d01",
             view_poverty_rate.c.location_name == "Foolandia",
             view_poverty_rate.c.admin1_name == "Province 01",
+            view_poverty_rate.c.rate == 0.75,
         ),
     )
 
 
-def test_population_constraint(run_constraints_test):
-    """Check that population cannot be negative"""
+def test_rate_constraint(run_constraints_test):
+    """Check that rate is between 0.0 and 1.0"""
     data = _sample_data()
-    data["population"] = -1
+    data["rate"] = 1.1
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="population",
+        expected_constraint="rate",
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["reference_period_start"] = datetime(2025, 1, 1)
@@ -51,13 +52,14 @@
 # Util functions
 
 
 def _sample_data():
     # return the whole record, then tests can change as needed
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
-        admin1_ref=1,
+        location_ref=1,
+        admin1_name="Province 01",
         classification="vulnerable",
-        population=1000000,
+        rate=0.75,
         reference_period_start=datetime(2024, 1, 1),
         reference_period_end=datetime(2024, 12, 31),
     )
```

### Comparing `hapi_schema-0.8.3/tests/test_refugees.py` & `hapi_schema-0.8.4/tests/test_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_views_as_tables.py` & `hapi_schema-0.8.4/tests/test_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_wfp_commodity.py` & `hapi_schema-0.8.4/tests/test_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/test_wfp_market.py` & `hapi_schema-0.8.4/tests/test_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.4/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.4/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_food_price.py` & `hapi_schema-0.8.4/tests/sample_data/data_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.4/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.8.4/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.4/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.4/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_patch.py` & `hapi_schema-0.8.4/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_population.py` & `hapi_schema-0.8.4/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.4/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/tests/sample_data/data_resource.py` & `hapi_schema-0.8.4/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/.gitignore` & `hapi_schema-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/LICENSE` & `hapi_schema-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/pyproject.toml` & `hapi_schema-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.3/PKG-INFO` & `hapi_schema-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.3
+Version: 0.8.4
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

