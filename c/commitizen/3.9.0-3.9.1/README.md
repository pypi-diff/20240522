# Comparing `tmp/commitizen-3.9.0.tar.gz` & `tmp/commitizen-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.9.0.tar", max compression
+gzip compressed data, was "commitizen-3.9.1.tar", max compression
```

## Comparing `commitizen-3.9.0.tar` & `commitizen-3.9.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1065 2023-09-15 10:18:21.842960 commitizen-3.9.0/LICENSE
--rw-r--r--   0        0        0      609 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/__version__.py
--rw-r--r--   0        0        0     4770 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/bump.py
--rw-r--r--   0        0        0    12204 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/changelog.py
--rw-r--r--   0        0        0     3542 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    18426 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    14364 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/bump.py
--rw-r--r--   0        0        0     7340 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5266 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/check.py
--rw-r--r--   0        0        0     3724 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/info.py
--rw-r--r--   0        0        0    13205 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/commands/version.py
--rw-r--r--   0        0        0     1235 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/config/__init__.py
--rw-r--r--   0        0        0      948 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1616 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1758 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1479 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1213 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2983 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7113 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     3164 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2721 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      287 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3437 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/defaults.py
--rw-r--r--   0        0        0     4706 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/factory.py
--rw-r--r--   0        0        0     7385 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/hooks.py
--rw-r--r--   0        0        0      913 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/out.py
--rw-r--r--   0        0        0     1578 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/__init__.py
--rw-r--r--   0        0        0     2246 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/base_provider.py
--rw-r--r--   0        0        0      849 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/cargo_provider.py
--rw-r--r--   0        0        0      423 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/commitizen_provider.py
--rw-r--r--   0        0        0      232 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/composer_provider.py
--rw-r--r--   0        0        0     2611 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/npm_provider.py
--rw-r--r--   0        0        0      215 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/pep621_provider.py
--rw-r--r--   0        0        0      500 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/poetry_provider.py
--rw-r--r--   0        0        0     2422 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/providers/scm_provider.py
--rw-r--r--   0        0        0      405 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     9726 2023-09-15 10:18:21.842960 commitizen-3.9.0/commitizen/version_schemes.py
--rw-r--r--   0        0        0     5829 2023-09-15 10:18:21.842960 commitizen-3.9.0/docs/README.md
--rw-r--r--   0        0        0     4309 2023-09-15 10:18:21.854960 commitizen-3.9.0/pyproject.toml
--rw-r--r--   0        0        0     8369 1970-01-01 00:00:00.000000 commitizen-3.9.0/setup.py
--rw-r--r--   0        0        0     7662 1970-01-01 00:00:00.000000 commitizen-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-22 07:40:10.043755 commitizen-3.9.1/LICENSE
+-rw-r--r--   0        0        0      609 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/__version__.py
+-rw-r--r--   0        0        0     4770 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/bump.py
+-rw-r--r--   0        0        0    12204 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/changelog.py
+-rw-r--r--   0        0        0     3542 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    18426 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    14364 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     7340 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5266 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3724 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/info.py
+-rw-r--r--   0        0        0    13205 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1235 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      948 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1626 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1960 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1703 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1213 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     2983 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7113 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3164 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2721 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      287 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3437 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/defaults.py
+-rw-r--r--   0        0        0     4706 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/factory.py
+-rw-r--r--   0        0        0     7385 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/hooks.py
+-rw-r--r--   0        0        0      913 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/out.py
+-rw-r--r--   0        0        0     1578 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/__init__.py
+-rw-r--r--   0        0        0     2246 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/base_provider.py
+-rw-r--r--   0        0        0      849 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/cargo_provider.py
+-rw-r--r--   0        0        0      423 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/commitizen_provider.py
+-rw-r--r--   0        0        0      232 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/composer_provider.py
+-rw-r--r--   0        0        0     2611 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/npm_provider.py
+-rw-r--r--   0        0        0      215 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/pep621_provider.py
+-rw-r--r--   0        0        0      500 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/poetry_provider.py
+-rw-r--r--   0        0        0     2422 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/providers/scm_provider.py
+-rw-r--r--   0        0        0      405 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     9726 2023-09-22 07:40:10.043755 commitizen-3.9.1/commitizen/version_schemes.py
+-rw-r--r--   0        0        0     5829 2023-09-22 07:40:10.047755 commitizen-3.9.1/docs/README.md
+-rw-r--r--   0        0        0     4309 2023-09-22 07:40:10.059756 commitizen-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0     8369 1970-01-01 00:00:00.000000 commitizen-3.9.1/setup.py
+-rw-r--r--   0        0        0     7662 1970-01-01 00:00:00.000000 commitizen-3.9.1/PKG-INFO
```

### Comparing `commitizen-3.9.0/LICENSE` & `commitizen-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/__init__.py` & `commitizen-3.9.1/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/bump.py` & `commitizen-3.9.1/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/changelog.py` & `commitizen-3.9.1/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/changelog_parser.py` & `commitizen-3.9.1/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cli.py` & `commitizen-3.9.1/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cmd.py` & `commitizen-3.9.1/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/bump.py` & `commitizen-3.9.1/commitizen/commands/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/changelog.py` & `commitizen-3.9.1/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/check.py` & `commitizen-3.9.1/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/commit.py` & `commitizen-3.9.1/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/init.py` & `commitizen-3.9.1/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/commands/version.py` & `commitizen-3.9.1/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/config/__init__.py` & `commitizen-3.9.1/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/config/base_config.py` & `commitizen-3.9.1/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/config/json_config.py` & `commitizen-3.9.1/commitizen/config/json_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,14 @@
                 "name": "cz_conventional_commits"
             }
         }
         ```
         """
         try:
             doc = json.loads(data)
-        except json.JSONDecodeError:
-            raise InvalidConfigurationError(f"Failed to parse {self.path}")
+        except json.JSONDecodeError as e:
+            raise InvalidConfigurationError(f"Failed to parse {self.path}: {e}")
 
         try:
             self.settings.update(doc["commitizen"])
         except KeyError:
             self.is_empty_config = True
```

### Comparing `commitizen-3.9.0/commitizen/config/toml_config.py` & `commitizen-3.9.1/commitizen/config/toml_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 
 from tomlkit import exceptions, parse, table
 
+from commitizen.exceptions import InvalidConfigurationError
 from .base_config import BaseConfig
 
 
 class TomlConfig(BaseConfig):
     def __init__(self, *, data: bytes | str, path: Path | str):
         super(TomlConfig, self).__init__()
         self.is_empty_config = False
-        self._parse_setting(data)
         self.add_path(path)
+        self._parse_setting(data)
 
     def init_empty_config_content(self):
         if os.path.isfile(self.path):
             with open(self.path, "rb") as input_toml_file:
                 parser = parse(input_toml_file.read())
         else:
             parser = parse("")
@@ -46,12 +47,16 @@
         """We expect to have a section in pyproject looking like
 
         ```
         [tool.commitizen]
         name = "cz_conventional_commits"
         ```
         """
-        doc = parse(data)
+        try:
+            doc = parse(data)
+        except exceptions.ParseError as e:
+            raise InvalidConfigurationError(f"Failed to parse {self.path}: {e}")
+
         try:
             self.settings.update(doc["tool"]["commitizen"])  # type: ignore
         except exceptions.NonExistentKey:
             self.is_empty_config = True
```

### Comparing `commitizen-3.9.0/commitizen/config/yaml_config.py` & `commitizen-3.9.1/commitizen/config/yaml_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from __future__ import annotations
 
 from pathlib import Path
 
 import yaml
 
 from commitizen.git import smart_open
+from commitizen.exceptions import InvalidConfigurationError
 
 from .base_config import BaseConfig
 
 
 class YAMLConfig(BaseConfig):
     def __init__(self, *, data: bytes | str, path: Path | str):
         super(YAMLConfig, self).__init__()
         self.is_empty_config = False
-        self._parse_setting(data)
         self.add_path(path)
+        self._parse_setting(data)
 
     def init_empty_config_content(self):
         with smart_open(self.path, "a", encoding=self.encoding) as json_file:
             yaml.dump({"commitizen": {}}, json_file, explicit_start=True)
 
     def _parse_setting(self, data: bytes | str) -> None:
         """We expect to have a section in cz.yaml looking like
 
         ```
         commitizen:
           name: cz_conventional_commits
         ```
         """
-        doc = yaml.safe_load(data)
+        import yaml.scanner
+
+        try:
+            doc = yaml.safe_load(data)
+        except yaml.YAMLError as e:
+            raise InvalidConfigurationError(f"Failed to parse {self.path}: {e}")
+
         try:
             self.settings.update(doc["commitizen"])
         except (KeyError, TypeError):
             self.is_empty_config = True
 
     def set_key(self, key, value):
         """Set or update a key in the conf.
```

### Comparing `commitizen-3.9.0/commitizen/cz/__init__.py` & `commitizen-3.9.1/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/base.py` & `commitizen-3.9.1/commitizen/cz/base.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.9.1/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.9.1/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/customize/customize.py` & `commitizen-3.9.1/commitizen/cz/customize/customize.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/jira/jira.py` & `commitizen-3.9.1/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/cz/jira/jira_info.txt` & `commitizen-3.9.1/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/defaults.py` & `commitizen-3.9.1/commitizen/defaults.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/exceptions.py` & `commitizen-3.9.1/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/factory.py` & `commitizen-3.9.1/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/git.py` & `commitizen-3.9.1/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/hooks.py` & `commitizen-3.9.1/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/out.py` & `commitizen-3.9.1/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/providers/__init__.py` & `commitizen-3.9.1/commitizen/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/providers/base_provider.py` & `commitizen-3.9.1/commitizen/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/providers/cargo_provider.py` & `commitizen-3.9.1/commitizen/providers/cargo_provider.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/providers/npm_provider.py` & `commitizen-3.9.1/commitizen/providers/npm_provider.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/providers/scm_provider.py` & `commitizen-3.9.1/commitizen/providers/scm_provider.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/commitizen/version_schemes.py` & `commitizen-3.9.1/commitizen/version_schemes.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/docs/README.md` & `commitizen-3.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.9.0/pyproject.toml` & `commitizen-3.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.9.0"
+version = "3.9.1"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen",
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.9.0"
+version = "3.9.1"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
@@ -57,15 +57,15 @@
 pytest-mock = "^3.10"
 pytest-regressions = "^2.4.0"
 pytest-freezer = "^0.4.6"
 pytest-xdist = "^3.1.0"
 # code formatter
 black = "^22.10"
 # linter
-ruff = ">=0.0.275,<0.0.288"
+ruff = ">=0.0.275,<0.0.290"
 pre-commit = "^2.18.0"
 mypy = "^1.4"
 types-PyYAML = ">=5.4.3,<7.0.0"
 types-termcolor = "^0.1.1"
 # documentation
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.6"
```

### Comparing `commitizen-3.9.0/setup.py` & `commitizen-3.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
  'commitizen.scheme': ['pep440 = commitizen.version_schemes:Pep440',
                        'semver = commitizen.version_schemes:SemVer'],
  'console_scripts': ['cz = commitizen.cli:main',
                      'git-cz = commitizen.cli:main']}
 
 setup_kwargs = {
     'name': 'commitizen',
-    'version': '3.9.0',
+    'version': '3.9.1',
     'description': 'Python commitizen client tool',
     'long_description': '[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/commitizen-tools/commitizen/pythonpackage.yml?label=python%20package&logo=github&logoColor=white&style=flat-square)](https://github.com/commitizen-tools/commitizen/actions)\n[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat-square)](https://conventionalcommits.org)\n[![PyPI Package latest release](https://img.shields.io/pypi/v/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)\n[![PyPI Package download count (per month)](https://img.shields.io/pypi/dm/commitizen?style=flat-square)](https://pypi.org/project/commitizen/)\n[![Supported versions](https://img.shields.io/pypi/pyversions/commitizen.svg?style=flat-square)](https://pypi.org/project/commitizen/)\n[![homebrew](https://img.shields.io/homebrew/v/commitizen?color=teal&style=flat-square)](https://formulae.brew.sh/formula/commitizen)\n[![Codecov](https://img.shields.io/codecov/c/github/commitizen-tools/commitizen.svg?style=flat-square)](https://codecov.io/gh/commitizen-tools/commitizen)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?style=flat-square&logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n\n![Using commitizen cli](images/demo.gif)\n\n---\n\n**Documentation:** [https://commitizen-tools.github.io/commitizen/](https://commitizen-tools.github.io/commitizen/)\n\n---\n\n## About\n\nCommitizen is release management tool designed for teams.\n\nCommitizen assumes your team uses a standard way of committing rules\nand from that foundation, it can bump your project\'s version, create\nthe changelog, and update files.\n\nBy default, commitizen uses [conventional commits][conventional_commits], but you\ncan build your own set of rules, and publish them.\n\nUsing a standardized set of rules to write commits, makes commits easier to read, and enforces writing\ndescriptive commits.\n\n### Features\n\n- Command-line utility to create commits with your rules. Defaults: [Conventional commits][conventional_commits]\n- Bump version automatically using [semantic versioning][semver] based on the commits. [Read More](./bump.md)\n- Generate a changelog using [Keep a changelog][keepchangelog]\n- Update your project\'s version files automatically\n- Display information about your commit rules (commands: schema, example, info)\n- Create your own set of rules and publish them to pip. Read more on [Customization](./customization.md)\n\n## Requirements\n\n[Python](https://www.python.org/downloads/) `3.7+`\n\n[Git][gitscm] `1.8.5.2+`\n\n## Installation\n\nTo make commitizen available in your system\n\n```bash\npip install --user -U Commitizen\n```\n\n### Python project\n\nYou can add it to your local project using one of these:\n\n```bash\npip install -U commitizen\n```\n\nfor Poetry >= 1.2.0:\n\n```bash\npoetry add commitizen --group dev\n```\n\nfor Poetry < 1.2.0:\n\n```bash\npoetry add commitizen --dev\n```\n\n### macOS\n\nvia [homebrew](https://formulae.brew.sh/formula/commitizen):\n\n```bash\nbrew install commitizen\n```\n\n## Usage\n\nMost of the time this is the only command you\'ll run:\n\n```sh\ncz bump\n```\n\nOn top of that, you can use commitizen to assist you with the creation of commits:\n\n```sh\ncz commit\n```\n\nRead more in the section [Getting Started](./getting_started.md).\n\n### Help\n\n```sh\n$ cz --help\nusage: cz [-h] [--debug] [-n NAME] [-nr NO_RAISE] {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version} ...\n\nCommitizen is a cli tool to generate conventional commits.\nFor more information about the topic go to https://conventionalcommits.org/\n\noptional arguments:\n  -h, --help            show this help message and exit\n  --debug               use debug mode\n  -n NAME, --name NAME  use the given commitizen (default: cz_conventional_commits)\n  -nr NO_RAISE, --no-raise NO_RAISE\n                        comma separated error codes that won\'t rise error, e.g: cz -nr 1,2,3 bump. See codes at https://commitizen-\n                        tools.github.io/commitizen/exit_codes/\n\ncommands:\n  {init,commit,c,ls,example,info,schema,bump,changelog,ch,check,version}\n    init                init commitizen configuration\n    commit (c)          create new commit\n    ls                  show available commitizens\n    example             show commit example\n    info                show information about the cz\n    schema              show commit schema\n    bump                bump semantic version based on the git log\n    changelog (ch)      generate changelog (note that it will overwrite existing file)\n    check               validates that a commit message matches the commitizen schema\n    version             get the version of the installed commitizen or the current project (default: installed commitizen)\n```\n\n## Setting up bash completion\n\nWhen using bash as your shell (limited support for zsh, fish, and tcsh is available), Commitizen can use [argcomplete](https://kislyuk.github.io/argcomplete/) for auto-completion. For this argcomplete needs to be enabled.\n\nargcomplete is installed when you install Commitizen since it\'s a dependency.\n\nIf Commitizen is installed globally, global activation can be executed:\n\n```bash\nsudo activate-global-python-argcomplete\n```\n\nFor permanent (but not global) Commitizen activation, use:\n\n```bash\nregister-python-argcomplete cz >> ~/.bashrc\n```\n\nFor one-time activation of argcomplete for Commitizen only, use:\n\n```bash\neval "$(register-python-argcomplete cz)"\n```\n\nFor further information on activation, please visit the [argcomplete website](https://kislyuk.github.io/argcomplete/).\n\n## Sponsors\n\nThese are our cool sponsors!\n\n<!-- sponsors --><!-- sponsors -->\n\n[conventional_commits]: https://www.conventionalcommits.org\n[semver]: https://semver.org/\n[keepchangelog]: https://keepachangelog.com/\n[gitscm]: https://git-scm.com/downloads\n',
     'author': 'Santiago Fraire',
     'author_email': 'santiwilly@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/commitizen-tools/commitizen',
```

### Comparing `commitizen-3.9.0/PKG-INFO` & `commitizen-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

