# Comparing `tmp/pysigma_validators_sigmahq-0.5.2.tar.gz` & `tmp/pysigma_validators_sigmahq-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_validators_sigmahq-0.5.2.tar", max compression
+gzip compressed data, was "pysigma_validators_sigmahq-0.6.0.tar", max compression
```

## Comparing `pysigma_validators_sigmahq-0.5.2.tar` & `pysigma_validators_sigmahq-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    26526 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/LICENSE
--rw-r--r--   0        0        0     3292 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/README.md
--rw-r--r--   0        0        0      644 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      830 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/__init__.py
--rw-r--r--   0        0        0    53521 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/config.py
--rw-r--r--   0        0        0     7066 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/field.py
--rw-r--r--   0        0        0     2772 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/filename.py
--rw-r--r--   0        0        0     1516 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/logsource.py
--rw-r--r--   0        0        0     7349 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/metadata.py
--rw-r--r--   0        0        0     2914 2024-05-07 04:51:56.111775 pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/title.py
--rw-r--r--   0        0        0     4085 1970-01-01 00:00:00.000000 pysigma_validators_sigmahq-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-05-22 17:03:55.660574 pysigma_validators_sigmahq-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3742 2024-05-22 17:03:55.660574 pysigma_validators_sigmahq-0.6.0/README.md
+-rw-r--r--   0        0        0      643 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/__init__.py
+-rw-r--r--   0        0        0     3967 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/condition.py
+-rw-r--r--   0        0        0    53521 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/config.py
+-rw-r--r--   0        0        0     8529 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/field.py
+-rw-r--r--   0        0        0     2772 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/filename.py
+-rw-r--r--   0        0        0     1516 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/logsource.py
+-rw-r--r--   0        0        0     7349 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/metadata.py
+-rw-r--r--   0        0        0     2914 2024-05-22 17:03:55.664574 pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/title.py
+-rw-r--r--   0        0        0     4533 1970-01-01 00:00:00.000000 pysigma_validators_sigmahq-0.6.0/PKG-INFO
```

### Comparing `pysigma_validators_sigmahq-0.5.2/LICENSE` & `pysigma_validators_sigmahq-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/README.md` & `pysigma_validators_sigmahq-0.6.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,39 +7,44 @@
 
 Create all validators specific to the requirements of the SigmaHQ rules repository
 
 # Validators
 
 | Name | Description|
 | --- | ---|
-| sigmahq_date_existence                | Checks if rule has a data.                                   |
-| sigmahq_description_existence         | Checks if rule has a description.                            |
-| sigmahq_description_length            | Checks if rule has a description.                            |
-| sigmahq_falsepositives_banned_word    | Checks if rule falsepositive start with a banned word.       |
-| sigmahq_falsepositives_capital        | Checks if rule falsepositive start with a capital.           |
-| sigmahq_falsepositives_typo_word      | Checks if rule falsepositive start with a common typo error. |
-| sigmahq_field_duplicate_value         | Check uniques value in field list.                           |
-| sigmahq_fieldname_cast                | Check field name have a cast error.                          |
-| sigmahq_filename                      | Check rule filename match SigmaHQ standard.                  |
-| sigmahq_filename_prefix               | Check rule filename match SigmaHQ prefix standard.           |
-| sigmahq_invalid_all_modifier          | Check All modifier used with a single value.                 |
-| sigmahq_invalid_field_source          | Check field Source use with Eventlog.                        |
-| sigmahq_invalid_fieldname             | Check field name do not exist in the logsource.              |
-| sigmahq_level_existence               | Checks if rule has a level.                                  |
-| sigmahq_link_description              | Checks if rule description use a link instead of references. |
-| sigmahq_logsource_coherent            | Checks if rule has Coherent logsource.                       |
-| sigmahq_logsource_known               | Checks if rule has known logsource.                          |
-| sigmahq_space_fieldname               | Check field name have a space.                               |
-| sigmahq_status_deprecated             | Checks if rule has a status DEPRECATED.                      |
-| sigmahq_status_existence              | Checks if rule has a status.                                 |
-| sigmahq_status_unsupported            | Checks if rule has a status UNSUPPORTED.                     |
-| sigmahq_title_case                    | Checks if rule title use capitalization.                     |
-| sigmahq_title_end                     | Checks if rule title end with a dot(.).                      |
-| sigmahq_title_length                  | Checks if rule has a title too long.                         |
-| sigmahq_title_start                   | Checks if rule title start with Detects.                     |
+| sigmahq_date_existence                 | Checks if rule has a data.                                   |
+| sigmahq_description_existence          | Checks if rule has a description.                            |
+| sigmahq_description_length             | Checks if rule has a description.                            |
+| sigmahq_falsepositives_banned_word     | Checks if rule falsepositive start with a banned word.       |
+| sigmahq_falsepositives_capital         | Checks if rule falsepositive start with a capital.           |
+| sigmahq_falsepositives_typo_word       | Checks if rule falsepositive start with a common typo error. |
+| sigmahq_field_duplicate_value          | Check uniques value in field list.                           |
+| sigmahq_field_with_space               | Check field do not have a space.                             |
+| sigmahq_fieldname_cast                 | Check field name have a cast error.                          |
+| sigmahq_filename                       | Check rule filename match SigmaHQ standard.                  |
+| sigmahq_filename_prefix                | Check rule filename match SigmaHQ prefix standard.           |
+| sigmahq_invalid_all_modifier           | Check All modifier used with a single value.                 |
+| sigmahq_invalid_field_source           | Check field Source use with Eventlog.                        |
+| sigmahq_invalid_fieldname              | Check field name do not exist in the logsource.              |
+| sigmahq_level_existence                | Checks if rule has a level.                                  |
+| sigmahq_link_description               | Checks if rule description use a link instead of references. |
+| sigmahq_logsource_coherent             | Checks if rule has Coherent logsource.                       |
+| sigmahq_logsource_known                | Checks if rule has known logsource.                          |
+| sigmahq_noasterixofselection_condition | Check use '1/all of ' without asterix                        |
+| sigmahq_ofselection_condition          | Check use 'all/X of ' with only one selection                |
+| sigmahq_ofthem_condition               | Check use ' of them' with only one selection                 |
+| sigmahq_space_fieldname                | Check field name have a space.                               |
+| sigmahq_status_deprecated              | Checks if rule has a status DEPRECATED.                      |
+| sigmahq_status_existence               | Checks if rule has a status.                                 |
+| sigmahq_status_unsupported             | Checks if rule has a status UNSUPPORTED.                     |
+| sigmahq_title_case                     | Checks if rule title use capitalization.                     |
+| sigmahq_title_end                      | Checks if rule title end with a dot(.).                      |
+| sigmahq_title_length                   | Checks if rule has a title too long.                         |
+| sigmahq_title_start                    | Checks if rule title start with Detects.                     |
+
 
 # Data
 
 All the data value are in the config.py
 
 # Maintainer
```

### Comparing `pysigma_validators_sigmahq-0.5.2/pyproject.toml` & `pysigma_validators_sigmahq-0.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "pySigma-validators-sigmahq"
-version = "0.5.2"
+version = "0.6.0"
 description = "pySigma SigmaHQ validators"
 authors = ["François Hubaut <frack113@users.noreply.github.com>"]
 license = "LGPL-2.1-only"
 readme = "README.md"
-repository = "https://github.com/frack113/pySigma_validators_sigmaHQ"
+repository = "https://github.com/SigmaHQ/pySigma_validators_sigmaHQ"
 packages = [
     { include = "sigma" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pysigma = "^0.11"
```

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/__init__.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/__init__.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/config.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/config.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/field.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/field.py`

 * *Files 8% similar despite different names*

```diff
@@ -192,7 +192,49 @@
                         SigmahqFieldDuplicateValueIssue(
                             self.rule, detection_item.field, str(v)
                         )
                     ]
                 else:
                     value_see.append(str(v).lower())
             return []
+
+
+@dataclass
+class SigmahqInvalidAllModifierIssue(SigmaValidationIssue):
+    description: ClassVar[str] = "All modifier without a list of value"
+    severity: ClassVar[SigmaValidationIssueSeverity] = SigmaValidationIssueSeverity.HIGH
+    field: str
+
+
+class SigmahqInvalidAllModifierValidator(SigmaDetectionItemValidator):
+    """Check All modifier used with a single value."""
+
+    def validate_detection_item(
+        self, detection_item: SigmaDetectionItem
+    ) -> List[SigmaValidationIssue]:
+        if (
+            SigmaAllModifier in detection_item.modifiers
+            and len(detection_item.value) < 2
+        ):
+            return [SigmahqInvalidAllModifierIssue(self.rule, detection_item.field)]
+        else:
+            return []
+
+
+@dataclass
+class SigmahqFieldWithSpaceIssue(SigmaValidationIssue):
+    description: ClassVar[str] = "Field has a space instead of an underscore"
+    severity: ClassVar[SigmaValidationIssueSeverity] = SigmaValidationIssueSeverity.HIGH
+    field: str
+
+
+class SigmahqFieldWithSpaceValidator(SigmaDetectionItemValidator):
+    """Check field do not have a space."""
+
+    def validate_detection_item(
+        self, detection_item: SigmaDetectionItem
+    ) -> List[SigmaValidationIssue]:
+        # Special case where value is case sensitive
+        if detection_item.field and " " in detection_item.field:
+            return [SigmahqFieldWithSpaceIssue(self.rule, detection_item.field)]
+        else:
+            return []
```

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/filename.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/filename.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/logsource.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/logsource.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/metadata.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/metadata.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/sigma/validators/sigmahq/title.py` & `pysigma_validators_sigmahq-0.6.0/sigma/validators/sigmahq/title.py`

 * *Files identical despite different names*

### Comparing `pysigma_validators_sigmahq-0.5.2/PKG-INFO` & `pysigma_validators_sigmahq-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pySigma-validators-sigmahq
-Version: 0.5.2
+Version: 0.6.0
 Summary: pySigma SigmaHQ validators
-Home-page: https://github.com/frack113/pySigma_validators_sigmaHQ
+Home-page: https://github.com/SigmaHQ/pySigma_validators_sigmaHQ
 License: LGPL-2.1-only
 Author: François Hubaut
 Author-email: frack113@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pysigma (>=0.11,<0.12)
-Project-URL: Repository, https://github.com/frack113/pySigma_validators_sigmaHQ
+Project-URL: Repository, https://github.com/SigmaHQ/pySigma_validators_sigmaHQ
 Description-Content-Type: text/markdown
 
 # pySigma_validators_sigmaHQ
 ![Tests](https://github.com/SigmaHQ/pySigma-validators-sigmaHQ/actions/workflows/test.yml/badge.svg)
 ![Coverage Badge](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/frack113/b27ee1cbe964fb1a299cc20c3403f8c8/raw/pySigma-validators-sigmaHQ.json)
 ![Status](https://img.shields.io/badge/Status-pre--release-orange)
 
@@ -27,39 +27,44 @@
 
 Create all validators specific to the requirements of the SigmaHQ rules repository
 
 # Validators
 
 | Name | Description|
 | --- | ---|
-| sigmahq_date_existence                | Checks if rule has a data.                                   |
-| sigmahq_description_existence         | Checks if rule has a description.                            |
-| sigmahq_description_length            | Checks if rule has a description.                            |
-| sigmahq_falsepositives_banned_word    | Checks if rule falsepositive start with a banned word.       |
-| sigmahq_falsepositives_capital        | Checks if rule falsepositive start with a capital.           |
-| sigmahq_falsepositives_typo_word      | Checks if rule falsepositive start with a common typo error. |
-| sigmahq_field_duplicate_value         | Check uniques value in field list.                           |
-| sigmahq_fieldname_cast                | Check field name have a cast error.                          |
-| sigmahq_filename                      | Check rule filename match SigmaHQ standard.                  |
-| sigmahq_filename_prefix               | Check rule filename match SigmaHQ prefix standard.           |
-| sigmahq_invalid_all_modifier          | Check All modifier used with a single value.                 |
-| sigmahq_invalid_field_source          | Check field Source use with Eventlog.                        |
-| sigmahq_invalid_fieldname             | Check field name do not exist in the logsource.              |
-| sigmahq_level_existence               | Checks if rule has a level.                                  |
-| sigmahq_link_description              | Checks if rule description use a link instead of references. |
-| sigmahq_logsource_coherent            | Checks if rule has Coherent logsource.                       |
-| sigmahq_logsource_known               | Checks if rule has known logsource.                          |
-| sigmahq_space_fieldname               | Check field name have a space.                               |
-| sigmahq_status_deprecated             | Checks if rule has a status DEPRECATED.                      |
-| sigmahq_status_existence              | Checks if rule has a status.                                 |
-| sigmahq_status_unsupported            | Checks if rule has a status UNSUPPORTED.                     |
-| sigmahq_title_case                    | Checks if rule title use capitalization.                     |
-| sigmahq_title_end                     | Checks if rule title end with a dot(.).                      |
-| sigmahq_title_length                  | Checks if rule has a title too long.                         |
-| sigmahq_title_start                   | Checks if rule title start with Detects.                     |
+| sigmahq_date_existence                 | Checks if rule has a data.                                   |
+| sigmahq_description_existence          | Checks if rule has a description.                            |
+| sigmahq_description_length             | Checks if rule has a description.                            |
+| sigmahq_falsepositives_banned_word     | Checks if rule falsepositive start with a banned word.       |
+| sigmahq_falsepositives_capital         | Checks if rule falsepositive start with a capital.           |
+| sigmahq_falsepositives_typo_word       | Checks if rule falsepositive start with a common typo error. |
+| sigmahq_field_duplicate_value          | Check uniques value in field list.                           |
+| sigmahq_field_with_space               | Check field do not have a space.                             |
+| sigmahq_fieldname_cast                 | Check field name have a cast error.                          |
+| sigmahq_filename                       | Check rule filename match SigmaHQ standard.                  |
+| sigmahq_filename_prefix                | Check rule filename match SigmaHQ prefix standard.           |
+| sigmahq_invalid_all_modifier           | Check All modifier used with a single value.                 |
+| sigmahq_invalid_field_source           | Check field Source use with Eventlog.                        |
+| sigmahq_invalid_fieldname              | Check field name do not exist in the logsource.              |
+| sigmahq_level_existence                | Checks if rule has a level.                                  |
+| sigmahq_link_description               | Checks if rule description use a link instead of references. |
+| sigmahq_logsource_coherent             | Checks if rule has Coherent logsource.                       |
+| sigmahq_logsource_known                | Checks if rule has known logsource.                          |
+| sigmahq_noasterixofselection_condition | Check use '1/all of ' without asterix                        |
+| sigmahq_ofselection_condition          | Check use 'all/X of ' with only one selection                |
+| sigmahq_ofthem_condition               | Check use ' of them' with only one selection                 |
+| sigmahq_space_fieldname                | Check field name have a space.                               |
+| sigmahq_status_deprecated              | Checks if rule has a status DEPRECATED.                      |
+| sigmahq_status_existence               | Checks if rule has a status.                                 |
+| sigmahq_status_unsupported             | Checks if rule has a status UNSUPPORTED.                     |
+| sigmahq_title_case                     | Checks if rule title use capitalization.                     |
+| sigmahq_title_end                      | Checks if rule title end with a dot(.).                      |
+| sigmahq_title_length                   | Checks if rule has a title too long.                         |
+| sigmahq_title_start                    | Checks if rule title start with Detects.                     |
+
 
 # Data
 
 All the data value are in the config.py
 
 # Maintainer
```

