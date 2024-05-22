# Comparing `tmp/hdx_python_country-3.7.0.tar.gz` & `tmp/hdx_python_country-3.7.1.tar.gz`

## Comparing `hdx_python_country-3.7.0.tar` & `hdx_python_country-3.7.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/CONTRIBUTING.md
--rwxr-xr-x   0        0        0     3812 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.config/coveragerc
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.config/pytest.ini
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.config/ruff.toml
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/documentation/.readthedocs.yaml
--rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/documentation/main.md
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/documentation/pydoc-markdown.yaml
--rw-r--r--   0        0        0    76222 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
--rwxr-xr-x   0        0        0      419 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/_version.py
--rwxr-xr-x   0        0        0    26849 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/adminlevel.py
--rwxr-xr-x   0        0        0    32557 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/country.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/currency.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/names.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/phonetics.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/src/hdx/location/wfp_exchangerates.py
--rwxr-xr-x   0        0        0    22256 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/fixtures/adminlevel.yaml
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/fixtures/global_pcode_lengths.csv
--rw-r--r--   0        0        0  1439447 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/fixtures/global_pcodes_adm_1_2.csv
--rw-r--r--   0        0        0   603829 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/fixtures/secondary_historic_rates.csv
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/fixtures/secondary_rates.json
--rw-r--r--   0        0        0    75934 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/Countries_UZB_Deleted.csv
--rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/__init__.py
--rwxr-xr-x   0        0        0    19361 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/test_adminlevel.py
--rwxr-xr-x   0        0        0    31834 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/test_country.py
--rwxr-xr-x   0        0        0    21314 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/test_currency.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/tests/hdx/location/test_wfp_exchangerates.py
--rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/.gitignore
--rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/LICENSE
--rwxr-xr-x   0        0        0     2264 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/README.md
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hdx_python_country-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0     3885 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.config/coveragerc
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.config/pytest.ini
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.config/ruff.toml
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/documentation/.readthedocs.yaml
+-rw-r--r--   0        0        0    10623 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/documentation/main.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/documentation/pydoc-markdown.yaml
+-rw-r--r--   0        0        0    76222 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv
+-rwxr-xr-x   0        0        0      419 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/_version.py
+-rwxr-xr-x   0        0        0    27247 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/adminlevel.py
+-rwxr-xr-x   0        0        0    32557 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/country.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/currency.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/names.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/phonetics.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/src/hdx/location/wfp_exchangerates.py
+-rwxr-xr-x   0        0        0    22256 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/fixtures/adminlevel.yaml
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/fixtures/global_pcode_lengths.csv
+-rw-r--r--   0        0        0  1439447 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/fixtures/global_pcodes_adm_1_2.csv
+-rw-r--r--   0        0        0   603829 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/fixtures/secondary_historic_rates.csv
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/fixtures/secondary_rates.json
+-rw-r--r--   0        0        0    75934 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/Countries_UZB_Deleted.csv
+-rwxr-xr-x   0        0        0      177 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/__init__.py
+-rwxr-xr-x   0        0        0    19629 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/test_adminlevel.py
+-rwxr-xr-x   0        0        0    31834 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/test_country.py
+-rwxr-xr-x   0        0        0    21314 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/test_currency.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/tests/hdx/location/test_wfp_exchangerates.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/.gitignore
+-rwxr-xr-x   0        0        0     1307 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/LICENSE
+-rwxr-xr-x   0        0        0     2264 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/README.md
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 hdx_python_country-3.7.1/PKG-INFO
```

### Comparing `hdx_python_country-3.7.0/CONTRIBUTING.md` & `hdx_python_country-3.7.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/requirements.txt` & `hdx_python_country-3.7.1/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,63 @@
-#
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
-#
-#    pip-compile --all-extras --output-file=requirements.txt pyproject.toml
-#
-annotated-types==0.6.0
+# This file was autogenerated by uv via the following command:
+#    uv pip compile pyproject.toml --resolver=backtracking --all-extras -o requirements.txt
+annotated-types==0.7.0
     # via pydantic
 attrs==23.2.0
     # via
     #   frictionless
     #   jsonlines
     #   jsonschema
+    #   referencing
 certifi==2024.2.2
     # via requests
 cfgv==3.4.0
     # via pre-commit
 chardet==5.2.0
     # via frictionless
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via typer
-colorama==0.4.6
-    # via typer
-coverage[toml]==7.4.4
+coverage==7.5.1
     # via pytest-cov
 distlib==0.3.8
     # via virtualenv
 et-xmlfile==1.1.0
     # via openpyxl
-filelock==3.13.3
+filelock==3.14.0
     # via virtualenv
-frictionless==5.16.1
+frictionless==5.17.0
     # via hdx-python-utilities
-hdx-python-utilities==3.6.7
+hdx-python-utilities==3.6.8
     # via hdx-python-country (pyproject.toml)
 humanize==4.9.0
     # via frictionless
-identify==2.5.35
+identify==2.5.36
     # via pre-commit
-idna==3.6
+idna==3.7
     # via requests
 ijson==3.2.3
     # via hdx-python-utilities
 iniconfig==2.0.0
     # via pytest
 isodate==0.6.1
     # via frictionless
-jinja2==3.1.3
+jinja2==3.1.4
     # via frictionless
 jsonlines==4.0.0
     # via hdx-python-utilities
 jsonpath-ng==1.6.1
     # via libhxl
-jsonschema==4.17.3
+jsonschema==4.22.0
     # via
     #   frictionless
     #   tableschema-to-template
+jsonschema-specifications==2023.12.1
+    # via jsonschema
 libhxl==5.2.1
     # via hdx-python-country (pyproject.toml)
 loguru==0.7.2
     # via hdx-python-utilities
 markdown-it-py==3.0.0
     # via rich
 marko==2.0.3
@@ -73,35 +70,33 @@
     # via pre-commit
 openpyxl==3.1.2
     # via hdx-python-utilities
 packaging==24.0
     # via pytest
 petl==1.7.15
     # via frictionless
-platformdirs==4.2.0
+platformdirs==4.2.2
     # via virtualenv
-pluggy==1.4.0
+pluggy==1.5.0
     # via pytest
 ply==3.11
     # via
     #   jsonpath-ng
     #   libhxl
-pre-commit==3.7.0
+pre-commit==3.7.1
     # via hdx-python-country (pyproject.toml)
-pydantic==2.6.4
+pydantic==2.7.1
     # via frictionless
-pydantic-core==2.16.3
+pydantic-core==2.18.2
     # via pydantic
-pygments==2.17.2
+pygments==2.18.0
     # via rich
 pyphonetics==0.5.3
     # via hdx-python-country (pyproject.toml)
-pyrsistent==0.20.0
-    # via jsonschema
-pytest==8.1.1
+pytest==8.2.1
     # via
     #   hdx-python-country (pyproject.toml)
     #   pytest-cov
 pytest-cov==5.0.0
     # via hdx-python-country (pyproject.toml)
 python-dateutil==2.8.2
     # via
@@ -115,29 +110,39 @@
 pyyaml==6.0.1
     # via
     #   frictionless
     #   pre-commit
     #   tableschema-to-template
 ratelimit==2.2.1
     # via hdx-python-utilities
-requests==2.31.0
+referencing==0.35.1
+    # via
+    #   jsonschema
+    #   jsonschema-specifications
+requests==2.32.2
     # via
     #   frictionless
     #   libhxl
     #   requests-file
-requests-file==2.0.0
+requests-file==2.1.0
     # via hdx-python-utilities
 rfc3986==2.0.0
     # via frictionless
 rich==13.7.1
     # via typer
+rpds-py==0.18.1
+    # via
+    #   jsonschema
+    #   referencing
 ruamel-yaml==0.18.6
     # via hdx-python-utilities
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
+setuptools==70.0.0
+    # via nodeenv
 shellingham==1.5.4
     # via typer
 simpleeval==0.9.13
     # via frictionless
 six==1.16.0
     # via
     #   isodate
@@ -148,40 +153,37 @@
     # via libhxl
 tableschema-to-template==0.0.13
     # via hdx-python-utilities
 tabulate==0.9.0
     # via frictionless
 text-unidecode==1.3
     # via python-slugify
-typer[all]==0.10.0
+typer==0.12.3
     # via frictionless
-typing-extensions==4.10.0
+typing-extensions==4.11.0
     # via
     #   frictionless
     #   pydantic
     #   pydantic-core
     #   typer
 unidecode==1.3.8
     # via
     #   libhxl
     #   pyphonetics
 urllib3==2.2.1
     # via
     #   libhxl
     #   requests
-validators==0.24.0
+validators==0.28.1
     # via frictionless
-virtualenv==20.25.1
+virtualenv==20.26.2
     # via pre-commit
 wheel==0.43.0
     # via libhxl
 xlrd==2.0.1
     # via hdx-python-utilities
 xlrd3==1.1.0
     # via libhxl
 xlsxwriter==3.2.0
     # via tableschema-to-template
 xlwt==1.3.0
     # via hdx-python-utilities
-
-# The following packages are considered to be unsafe in a requirements file:
-# setuptools
```

### Comparing `hdx_python_country-3.7.0/.github/workflows/publish.yaml` & `hdx_python_country-3.7.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/.github/workflows/run-python-tests.yaml` & `hdx_python_country-3.7.1/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/documentation/main.md` & `hdx_python_country-3.7.1/documentation/main.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/documentation/pydoc-markdown.yaml` & `hdx_python_country-3.7.1/documentation/pydoc-markdown.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
     packages:
       - hdx.location
 renderer:
   type: mkdocs
   output_directory: docs
   mkdocs_config:
     site_name: HDX Python Country
-    theme: mkdocs
+    theme: material
     repo_url: "https://github.com/OCHA-DAP/hdx-python-country"
   markdown:
     source_linker:
       type: github
       repo: OCHA-DAP/hdx-python-country
   pages:
     - title: Home
       name: index
       source: main.md
     - title: API Documentation
       children:
       - title: Countries
         contents:
           - hdx.location.country.*
-      - title: Administration level one
+      - title: Administration Level
         contents:
-          - hdx.location.adminone.*
+          - hdx.location.adminlevel.*
       - title: Currencies
         contents:
           - hdx.location.currency.*
```

### Comparing `hdx_python_country-3.7.0/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv` & `hdx_python_country-3.7.1/src/hdx/location/Countries & Territories Taxonomy MVP - C&T Taxonomy with HXL Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/src/hdx/location/adminlevel.py` & `hdx_python_country-3.7.1/src/hdx/location/adminlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,7 +739,20 @@
             if len(error) == 2:
                 line = f"{error[0]} - Could not find {error[1]} in map names!"
             else:
                 line = f"{error[0]} - {error[1]}: Could not find {error[2]} in map names!"
             logger.error(line)
             output.append(line)
         return output
+
+    def output_admin_name_mappings(self) -> List[str]:
+        """Output log of name mappings
+
+        Returns:
+            List[str]: List of mappings
+        """
+        output = []
+        for name, pcode in self.admin_name_mappings.items():
+            line = f"{name}: {self.pcode_to_name[pcode]} ({pcode})"
+            logger.info(line)
+            output.append(line)
+        return output
```

### Comparing `hdx_python_country-3.7.0/src/hdx/location/country.py` & `hdx_python_country-3.7.1/src/hdx/location/country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/src/hdx/location/currency.py` & `hdx_python_country-3.7.1/src/hdx/location/currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/src/hdx/location/names.py` & `hdx_python_country-3.7.1/src/hdx/location/names.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/src/hdx/location/phonetics.py` & `hdx_python_country-3.7.1/src/hdx/location/phonetics.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/src/hdx/location/wfp_exchangerates.py` & `hdx_python_country-3.7.1/src/hdx/location/wfp_exchangerates.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/fixtures/adminlevel.yaml` & `hdx_python_country-3.7.1/tests/fixtures/adminlevel.yaml`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/fixtures/global_pcode_lengths.csv` & `hdx_python_country-3.7.1/tests/fixtures/global_pcode_lengths.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/fixtures/global_pcodes_adm_1_2.csv` & `hdx_python_country-3.7.1/tests/fixtures/global_pcodes_adm_1_2.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/fixtures/secondary_historic_rates.csv` & `hdx_python_country-3.7.1/tests/fixtures/secondary_historic_rates.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/fixtures/secondary_rates.json` & `hdx_python_country-3.7.1/tests/fixtures/secondary_rates.json`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/hdx/location/Countries_UZB_Deleted.csv` & `hdx_python_country-3.7.1/tests/hdx/location/Countries_UZB_Deleted.csv`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/hdx/location/test_adminlevel.py` & `hdx_python_country-3.7.1/tests/hdx/location/test_adminlevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,19 @@
             "test - Ignored ZWE!",
         ]
         output = adminone.output_errors()
         assert output == [
             "test - Could not find ABC in map names!",
             "test - NER: Could not find ABCDEFGH in map names!",
         ]
+        output = adminone.output_admin_name_mappings()
+        assert len(output) == 62
+        assert output[0] == "Nord-Ouest: North West (HT09)"
+        assert output[31] == "Juba Dhexe: Middle Juba (SO27)"
+        assert output[61] == "CU Niamey: Niamey (NER008)"
 
     def test_adminlevel_fuzzy(self, config):
         adminone = AdminLevel(config)
         adminone.setup_from_admin_info(config["admin_info"])
         assert adminone.get_pcode("YEM", "Al Dali", logname="test") == (
             "YE30",
             False,
@@ -227,15 +232,15 @@
         AdminLevel.set_default_admin_url(url)
         assert AdminLevel._admin_url == url
         adminone.setup_from_url(countryiso3s=("YEM",))
         assert len(adminone.get_pcode_list()) == 22
         adminone = AdminLevel(config)
         adminone.setup_from_url()
         assert adminone.get_admin_level("YEM") == 1
-        assert len(adminone.get_pcode_list()) == 2506
+        assert len(adminone.get_pcode_list()) == 2509
         assert adminone.get_pcode_length("YEM") == 4
         assert adminone.get_pcode("YEM", "YE30", logname="test") == (
             "YE30",
             True,
         )
         assert adminone.get_pcode(
             "YEM", "YE30", parent="YEM", logname="test"
```

### Comparing `hdx_python_country-3.7.0/tests/hdx/location/test_country.py` & `hdx_python_country-3.7.1/tests/hdx/location/test_country.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/hdx/location/test_currency.py` & `hdx_python_country-3.7.1/tests/hdx/location/test_currency.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/tests/hdx/location/test_wfp_exchangerates.py` & `hdx_python_country-3.7.1/tests/hdx/location/test_wfp_exchangerates.py`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/.gitignore` & `hdx_python_country-3.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/LICENSE` & `hdx_python_country-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/README.md` & `hdx_python_country-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hdx_python_country-3.7.0/pyproject.toml` & `hdx_python_country-3.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Operating System :: Unix",
     "Operating System :: MacOS",
     "Operating System :: Microsoft :: Windows",
 ]
 requires-python = ">=3.8"
 
 dependencies = [
-    "hdx-python-utilities>=3.6.7",
+    "hdx-python-utilities>=3.6.8",
     "libhxl>=5.2.1",
     "pyphonetics",
 ]
 dynamic = ["version"]
 
 [project.readme]
 file = "README.md"
```

### Comparing `hdx_python_country-3.7.0/PKG-INFO` & `hdx_python_country-3.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hdx-python-country
-Version: 3.7.0
+Version: 3.7.1
 Summary: HDX Python country code and exchange rate (fx) utilities
 Project-URL: Homepage, https://github.com/OCHA-DAP/hdx-python-country
 Author: Michael Rans
 License: MIT
 License-File: LICENSE
 Keywords: HDX,country,country code,currencies,currency,exchange rate,foreign exchange,fx,iso 3166,iso2,iso3,location,region
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
-Requires-Dist: hdx-python-utilities>=3.6.7
+Requires-Dist: hdx-python-utilities>=3.6.8
 Requires-Dist: libhxl>=5.2.1
 Requires-Dist: pyphonetics
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
```

