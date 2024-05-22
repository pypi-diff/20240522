# Comparing `tmp/aurum_hikari-0.1.5.1.tar.gz` & `tmp/aurum_hikari-0.1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurum_hikari-0.1.5.1.tar", max compression
+gzip compressed data, was "aurum_hikari-0.1.5.2.tar", max compression
```

## Comparing `aurum_hikari-0.1.5.1.tar` & `aurum_hikari-0.1.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1080 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/LICENSE
--rw-r--r--   0        0        0     3510 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/README.md
--rw-r--r--   0        0        0      598 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/__init__.py
--rw-r--r--   0        0        0      430 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/_about.py
--rw-r--r--   0        0        0      183 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/__init__.py
--rw-r--r--   0        0        0     9241 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/client.py
--rw-r--r--   0        0        0      309 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/client/integration.py
--rw-r--r--   0        0        0      366 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/__init__.py
--rw-r--r--   0        0        0      198 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/decorators/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/decorators/sub_command.py
--rw-r--r--   0        0        0     2324 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/message_command.py
--rw-r--r--   0        0        0     5767 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/slash_command.py
--rw-r--r--   0        0        0     2720 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/sub_command.py
--rw-r--r--   0        0        0     2402 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/commands/user_command.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/enum/__init__.py
--rw-r--r--   0        0        0      423 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/enum/sync_commands.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/__init__.py
--rw-r--r--   0        0        0      312 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/__init__.py
--rw-r--r--   0        0        0     4226 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin.py
--rw-r--r--   0        0        0     1720 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_integration.py
--rw-r--r--   0        0        0     3457 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_manager.py
--rw-r--r--   0        0        0      292 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/includable.py
--rw-r--r--   0        0        0      220 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/interactions/__init__.py
--rw-r--r--   0        0        0     8344 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/interactions/interaction_context.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/__init__.py
--rw-r--r--   0        0        0      332 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/__init__.py
--rw-r--r--   0        0        0     3035 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/app_command.py
--rw-r--r--   0        0        0     5565 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/command_handler.py
--rw-r--r--   0        0        0     1937 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/commands/context_menu_command.py
--rw-r--r--   0        0        0       75 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/consts.py
--rw-r--r--   0        0        0      290 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/__init__.py
--rw-r--r--   0        0        0       67 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/base_exception.py
--rw-r--r--   0        0        0      456 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/exceptions/commands_exceptions.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/internal/utils/commands.py
--rw-r--r--   0        0        0      401 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/localization_provider_interface.py
--rw-r--r--   0        0        0      255 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/localized.py
--rw-r--r--   0        0        0      479 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/pass_localization_provider.py
--rw-r--r--   0        0        0      207 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/l10n/types.py
--rw-r--r--   0        0        0      219 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/__init__.py
--rw-r--r--   0        0        0      299 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/choice.py
--rw-r--r--   0        0        0     1715 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/options/option.py
--rw-r--r--   0        0        0        0 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/py.typed
--rw-r--r--   0        0        0      147 2024-05-21 12:03:56.437685 aurum_hikari-0.1.5.1/aurum/types.py
--rw-r--r--   0        0        0     2047 2024-05-21 12:04:06.217797 aurum_hikari-0.1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/LICENSE
+-rw-r--r--   0        0        0     3510 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/README.md
+-rw-r--r--   0        0        0      598 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/__init__.py
+-rw-r--r--   0        0        0      430 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/_about.py
+-rw-r--r--   0        0        0      183 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/client/__init__.py
+-rw-r--r--   0        0        0     9241 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/client/client.py
+-rw-r--r--   0        0        0      309 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/client/integration.py
+-rw-r--r--   0        0        0      366 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/decorators/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/decorators/sub_command.py
+-rw-r--r--   0        0        0     2324 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/message_command.py
+-rw-r--r--   0        0        0     5767 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/slash_command.py
+-rw-r--r--   0        0        0     2720 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/sub_command.py
+-rw-r--r--   0        0        0     2402 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/commands/user_command.py
+-rw-r--r--   0        0        0        0 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/enum/__init__.py
+-rw-r--r--   0        0        0      423 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/enum/sync_commands.py
+-rw-r--r--   0        0        0        0 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/ext/__init__.py
+-rw-r--r--   0        0        0      312 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/ext/plugins/__init__.py
+-rw-r--r--   0        0        0     4226 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin.py
+-rw-r--r--   0        0        0     1720 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin_integration.py
+-rw-r--r--   0        0        0     3457 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin_manager.py
+-rw-r--r--   0        0        0      292 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/includable.py
+-rw-r--r--   0        0        0      220 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/interactions/__init__.py
+-rw-r--r--   0        0        0     8344 2024-05-21 13:46:17.628382 aurum_hikari-0.1.5.2/aurum/interactions/interaction_context.py
+-rw-r--r--   0        0        0        0 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/__init__.py
+-rw-r--r--   0        0        0      332 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/commands/__init__.py
+-rw-r--r--   0        0        0     3035 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/commands/app_command.py
+-rw-r--r--   0        0        0     5565 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/commands/command_handler.py
+-rw-r--r--   0        0        0     1937 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/commands/context_menu_command.py
+-rw-r--r--   0        0        0       75 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/consts.py
+-rw-r--r--   0        0        0      290 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/exceptions/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/exceptions/base_exception.py
+-rw-r--r--   0        0        0      456 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/exceptions/commands_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/internal/utils/commands.py
+-rw-r--r--   0        0        0      374 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/l10n/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/l10n/localization_provider_interface.py
+-rw-r--r--   0        0        0      255 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/l10n/localized.py
+-rw-r--r--   0        0        0      479 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/l10n/pass_localization_provider.py
+-rw-r--r--   0        0        0      207 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/l10n/types.py
+-rw-r--r--   0        0        0      219 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/options/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/options/choice.py
+-rw-r--r--   0        0        0     1715 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/options/option.py
+-rw-r--r--   0        0        0        0 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/py.typed
+-rw-r--r--   0        0        0      147 2024-05-21 13:46:17.632382 aurum_hikari-0.1.5.2/aurum/types.py
+-rw-r--r--   0        0        0     2047 2024-05-21 13:46:26.884338 aurum_hikari-0.1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4869 1970-01-01 00:00:00.000000 aurum_hikari-0.1.5.2/PKG-INFO
```

### Comparing `aurum_hikari-0.1.5.1/LICENSE` & `aurum_hikari-0.1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/README.md` & `aurum_hikari-0.1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/__init__.py` & `aurum_hikari-0.1.5.2/aurum/__init__.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/client/client.py` & `aurum_hikari-0.1.5.2/aurum/client/client.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/commands/decorators/sub_command.py` & `aurum_hikari-0.1.5.2/aurum/commands/decorators/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/commands/message_command.py` & `aurum_hikari-0.1.5.2/aurum/commands/message_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/commands/slash_command.py` & `aurum_hikari-0.1.5.2/aurum/commands/slash_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/commands/sub_command.py` & `aurum_hikari-0.1.5.2/aurum/commands/sub_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/commands/user_command.py` & `aurum_hikari-0.1.5.2/aurum/commands/user_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin.py` & `aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_integration.py` & `aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin_integration.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/ext/plugins/plugin_manager.py` & `aurum_hikari-0.1.5.2/aurum/ext/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/interactions/interaction_context.py` & `aurum_hikari-0.1.5.2/aurum/interactions/interaction_context.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/internal/commands/app_command.py` & `aurum_hikari-0.1.5.2/aurum/internal/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/internal/commands/command_handler.py` & `aurum_hikari-0.1.5.2/aurum/internal/commands/command_handler.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/internal/commands/context_menu_command.py` & `aurum_hikari-0.1.5.2/aurum/internal/commands/context_menu_command.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/internal/utils/commands.py` & `aurum_hikari-0.1.5.2/aurum/internal/utils/commands.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/l10n/localization_provider_interface.py` & `aurum_hikari-0.1.5.2/aurum/l10n/localization_provider_interface.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/aurum/options/option.py` & `aurum_hikari-0.1.5.2/aurum/options/option.py`

 * *Files identical despite different names*

### Comparing `aurum_hikari-0.1.5.1/pyproject.toml` & `aurum_hikari-0.1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 build-backend = "poetry.core.masonry.api"
 
 
 # Package information
 [tool.poetry]
 packages = [{ include = "aurum" }]
 name = "aurum-hikari"
-version = "v0.1.5.1"
+version = "v0.1.5.2"
 license = "MIT"
 authors = ["stefanlight <64615032+stefanlight8@users.noreply.github.com>"]
 description = "A flexible framework for handling commands and components with integrations."
 keywords = [
     "discord",
     "hikari",
     "commands",
```

### Comparing `aurum_hikari-0.1.5.1/PKG-INFO` & `aurum_hikari-0.1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurum-hikari
-Version: 0.1.5.1
+Version: 0.1.5.2
 Summary: A flexible framework for handling commands and components with integrations.
 License: MIT
 Keywords: discord,hikari,commands,components,command-handler,component-handler,integrations
 Author: stefanlight
 Author-email: 64615032+stefanlight8@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 3 - Alpha
```

