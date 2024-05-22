# Comparing `tmp/adotestplan_to_pytestbdd-0.1.4.tar.gz` & `tmp/adotestplan_to_pytestbdd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adotestplan_to_pytestbdd-0.1.4.tar", max compression
+gzip compressed data, was "adotestplan_to_pytestbdd-0.1.5.tar", max compression
```

## Comparing `adotestplan_to_pytestbdd-0.1.4.tar` & `adotestplan_to_pytestbdd-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1079 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/LICENSE
--rw-r--r--   0        0        0     4515 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/README.md
--rw-r--r--   0        0        0      339 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/adotestplan_to_pytestbdd/__init__.py
--rw-r--r--   0        0        0    52648 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/adotestplan_to_pytestbdd/ado_test_plan.py
--rw-r--r--   0        0        0      348 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/adotestplan_to_pytestbdd/exceptions.py
--rw-r--r--   0        0        0     2040 2024-05-08 13:59:50.765580 adotestplan_to_pytestbdd-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4515 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/README.md
+-rw-r--r--   0        0        0      339 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/adotestplan_to_pytestbdd/__init__.py
+-rw-r--r--   0        0        0    52662 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/adotestplan_to_pytestbdd/ado_test_plan.py
+-rw-r--r--   0        0        0      348 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/adotestplan_to_pytestbdd/exceptions.py
+-rw-r--r--   0        0        0     2040 2024-05-22 19:55:00.064568 adotestplan_to_pytestbdd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5967 1970-01-01 00:00:00.000000 adotestplan_to_pytestbdd-0.1.5/PKG-INFO
```

### Comparing `adotestplan_to_pytestbdd-0.1.4/LICENSE` & `adotestplan_to_pytestbdd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.4/README.md` & `adotestplan_to_pytestbdd-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `adotestplan_to_pytestbdd-0.1.4/adotestplan_to_pytestbdd/ado_test_plan.py` & `adotestplan_to_pytestbdd-0.1.5/adotestplan_to_pytestbdd/ado_test_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -762,15 +762,15 @@
                     ids.append(test_case.test_case.id)
 
             # next, with that array of IDs, we can get the more
             # generic ADO work items for those IDs, and then
             # loop through those work items, converting them to
             # BDD style "scenarios"
             scenario_work_items = self.witc.get_work_items(
-                ids=ids, project=self.project
+                ids=ids, project=self.project, expand="All"
             )
             for scenario_work_item in scenario_work_items:
                 scenario_work_item: WorkItem
 
                 # convert this ADO work item to a BDD Scenario.
 
                 # if it has shared parameters, that means we treat it as a
```

### Comparing `adotestplan_to_pytestbdd-0.1.4/pyproject.toml` & `adotestplan_to_pytestbdd-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adotestplan-to-pytestbdd"
-version = "0.1.4"
+version = "0.1.5"
 description = "Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners"
 authors = [
     "David VanKampen <david.vankampen@bissell.com>",
     "Tristan VanFossen <tristan.vanfossen@bissell.com>"
 ]
 readme = "README.md"
 repository = 'https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd'
```

### Comparing `adotestplan_to_pytestbdd-0.1.4/PKG-INFO` & `adotestplan_to_pytestbdd-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adotestplan-to-pytestbdd
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utility for translating AzureDevOps Test Plans to Gherkin Feature file and Pytest-BDD runners
 Home-page: https://github.com/bissell-homecare-inc/adotestplan-to-pytestbdd
 Keywords: ADO,AzureDevOps,BDD
 Author: David VanKampen
 Author-email: david.vankampen@bissell.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

