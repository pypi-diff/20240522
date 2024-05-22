# Comparing `tmp/kframe-0.4.3rc1.tar.gz` & `tmp/kframe-0.5.0rc1.tar.gz`

## Comparing `kframe-0.4.3rc1.tar` & `kframe-0.5.0rc1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.tool-versions
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/CHANGELOG.md
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_ci.yml
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_pre_release.yml
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.github/workflows/main_release.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/__init__.py
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/configattr.py
--rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/src/kframe/config/configentity.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/test_config.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/tests/test_secretattr.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/.gitignore
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/LICENSE.txt
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/pyproject.toml
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 kframe-0.4.3rc1/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.tool-versions
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.github/workflows/main_ci.yml
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.github/workflows/main_pre_release.yml
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.github/workflows/main_release.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/__about__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/api/__init__.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/api/apitools.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/config/__init__.py
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/config/configattr.py
+-rw-r--r--   0        0        0    14336 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/config/configentity.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/model/__init__.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/src/kframe/model/managedb.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4713 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/tests/test_config.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/tests/test_secretattr.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/.gitignore
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/LICENSE.txt
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/README.md
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 kframe-0.5.0rc1/PKG-INFO
```

### Comparing `kframe-0.4.3rc1/CHANGELOG.md` & `kframe-0.5.0rc1/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-## v0.4.3a1 (2024-05-01)
+## v0.5.0a1 (2024-05-22)
+
+### Feat
+
+- Update build_quality test command and environment in CI workflow
+- Add database model management tools
+- Add api management tools
+- Enforce config attributes type and allow async CLI execute methods
+
+## v0.4.3 (2024-05-01)
 
 ### Fix
 
 - Update CLI argument help message in ConfigAttr class to show required and env_var
 - Update .gitignore and pyproject.toml
 
 ### Refactor
```

### Comparing `kframe-0.4.3rc1/.github/workflows/main_ci.yml` & `kframe-0.5.0rc1/.github/workflows/main_ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Run static analysis
       run: hatch fmt --check
 
     - name: Run tests
-      run: hatch run cov
+      run: hatch run build_quality:test
 
   version_bump:
     name: "Version bump to alpha version"
     runs-on: "ubuntu-latest"
     needs: ci
     permissions:
       contents: write
```

### Comparing `kframe-0.4.3rc1/.github/workflows/main_pre_release.yml` & `kframe-0.5.0rc1/.github/workflows/main_pre_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.3rc1/.github/workflows/main_release.yml` & `kframe-0.5.0rc1/.github/workflows/main_release.yml`

 * *Files identical despite different names*

### Comparing `kframe-0.4.3rc1/src/kframe/config/configattr.py` & `kframe-0.5.0rc1/src/kframe/config/configattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Module for the ConfigAttr and Secret classes."""
+
 import weakref
 from typing import Any, Generic, TypeVar
 
 T = TypeVar("T")
 
 
 class Secret(Generic[T]):
@@ -174,14 +176,15 @@
 
     @property
     def attr_type(self):
         """Return the type of the attribute."""
         return self._attr_type
 
     def __repr__(self):
+        """Return a string representation of the ConfigAttr instance."""
         return (
             "<ConfigAttr ("
             f"name={self.name}, "
             f"default={self.default_value}, "
             f"required={self.required}, "
             f"env_var={self.env_var}, "
             f"cli_args={self._cli_args}, "
```

### Comparing `kframe-0.4.3rc1/src/kframe/config/configentity.py` & `kframe-0.5.0rc1/src/kframe/config/configentity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,87 +1,143 @@
+"""Configuration entity module."""
+
+from __future__ import annotations
+
+import asyncio
+import inspect
 import logging
 import os
 import sys
 from argparse import ArgumentError, ArgumentParser, ArgumentTypeError, Namespace
 from collections import ChainMap
 from enum import Enum
+from pathlib import Path
 
 from .configattr import ConfigAttr, Secret
 
 logger = logging.getLogger("kframe.config")
 
 
 class ConfigEntityType(Enum):
+    """Configuration entity type.
+
+    Attributes:
+        base (str): Base entity type.
+        module (str): Module entity type.
+        command (str): Command entity type.
+    """
+
     base = "base"
     module = "Module"
     command = "Command"
 
 
 class ConfigEntity(type):
+    """Metaclass for configuration entities.
+
+    Attributes:
+        _commands (set): Set of commands.
+        _submodules (set): Set of submodules.
+        _attribute_names (set): Set of attribute names.
+        _sources (ChainMap): ChainMap of sources.
+        show_config (ConfigAttr): Show configuration attribute.
+        attr (Namespace): Entity attributes namespace.
+        attrs (dict[str, ConfigAttr]): Entity attributes dictionary.
+        entity_type (ConfigEntityType): Entity type.
+        parent_module (ConfigEntity): Parent module.
+        root_module (ConfigEntity): Root module.
+    """
+
     _commands: set
     _submodules: set
     _attribute_names: set
     _sources: ChainMap
     show_config: ConfigAttr
     attr: Namespace
     attrs: dict[str, ConfigAttr]
     entity_type: ConfigEntityType
-    parent_module: "ConfigEntity"
-    root_module: "ConfigEntity"
+    parent_module: ConfigEntity
+    root_module: ConfigEntity
 
     def show(cls, file=sys.stdout):
-        """Prints entity configuration"""
+        """Prints entity configuration.
 
-    def __new__(cls, _name, bases, dct, name=None, parent_entity=None, description=None):
+        Args:
+            file (Any, optional): Output file. Defaults to sys.stdout.
+        """
+
+    def __new__(cls, _name, bases, dct, name=None, parent_entity=None, description=None) -> ConfigEntity:
+        """Create new class.
+
+        Args:
+            _name (str): Class name.
+            bases (tuple): Base classes.
+            dct (dict): Class namespace.
+            name (str, optional): Class name. Defaults to None.
+            parent_entity (ConfigEntity, optional): Parent entity. Defaults to None.
+            description (str, optional): Class description. Defaults to None.
+
+        Returns:
+            ConfigEntity: New class.
+        """
         sources = {}
 
         if len(bases) > 0:
             for k in bases[0]._attribute_names:
                 if k not in dct:
                     dct[k] = bases[0].__dict__[k]
 
         for k, v in dct.items():
             if isinstance(v, ConfigAttr) and k not in dct["_sources"]:
                 v._name = k
-                sources[k] = {"default": Secret[v.attr_type](v.default_value) if v.secret else v.default_value}
+                sources[k] = {"default": Secret(v.default_value) if v.secret else v.default_value}
                 v.__doc__ = v.description
 
                 if v.env_var is not None and v.env_var in os.environ:
-                    sources[k]["env"] = Secret[v.attr_type](v.env_var) if v.secret else os.environ[v.env_var]
+                    sources[k]["env"] = cls.cast_attr(v, os.environ[v.env_var])
 
                 if (
                     v.cli_args is None
                     and v.required
                     and v.default_value is None
                     and isinstance(v.env_var, str)
                     and os.getenv(v.env_var) is None
                 ):
-                    raise AttributeError(f"Required attribute {v} must have a default value or environment variable")
+                    logger.error(
+                        "ERROR: Required attribute %s must have a default value or environment variable",
+                        v.name,
+                    )
+                    sys.exit(1)
 
         dct["_sources"] = ChainMap(sources, dct["_sources"])
         dct["_commands"] = set()
         dct["_submodules"] = set()
 
         dct["_attribute_names"] = {k for k, v in dct.items() if isinstance(v, ConfigAttr)}
 
         attr = {k: dct[k] for k in dct["_attribute_names"]}
 
         def attrs(self) -> dict[str, ConfigAttr]:
-            """Entity attributes"""
+            """Entity attributes."""
             return attr
 
         dct["attr"] = property(lambda self: Namespace(**attr), doc="Entity attributes namespace")
         dct["attrs"] = property(attrs, doc="Entity attributes dictionary")
         dct["namespace"] = property(lambda self: ".".join(dct["_namespace"]), doc="Entity namespace")
 
         dct["parent_module"] = property(lambda self: parent_entity, doc=f"{dct['entity_type'].value} parent module ")
 
         def run(self):
-            """Execute command"""
-            self.execute()
+            """Execute command."""
+            if self.show_config:
+                self.show()
+            if inspect.iscoroutinefunction(self.execute):
+                asyncio.run(self.execute())
+            else:
+                self.execute()
 
         if dct["entity_type"] == ConfigEntityType.command:
             if "__call__" in dct:
                 raise AttributeError("Command class cannot have __call__ method")
             dct["__call__"] = run
 
         new_cls = super().__new__(cls, _name, bases, dct)
@@ -91,15 +147,26 @@
             if new_cls.entity_type == ConfigEntityType.command:
                 parent_entity._commands.add(new_cls)
         elif len(bases) > 0:
             bases[0].root_module = new_cls
 
         return new_cls
 
-    def __prepare__(cls, bases, name=None, parent_entity=None, description=None):  # noqa: PLW3201
+    def __prepare__(cls, bases, name=None, parent_entity=None, description=None):
+        """Prepare class namespace.
+
+        Args:
+            bases (tuple): Base classes.
+            name (str): Class name.
+            parent_entity (ConfigEntity): Parent entity.
+            description (str): Class description
+
+        Returns:
+            dict: Class namespace.
+        """
         match len(bases):
             case 0:
                 entity_type = ConfigEntityType.base
             case 1:
                 match bases[0].__name__:
                     case "AppModule":
                         entity_type = ConfigEntityType.module
@@ -131,48 +198,82 @@
         if parent_entity is not None:
             dct["_namespace"] = (parent_entity._namespace or []) + dct["_namespace"]
             for k in parent_entity._sources:
                 if k not in dct:
                     dct[k] = parent_entity.__dict__[k]
         return dct
 
+    @staticmethod
+    def cast_attr(attr: ConfigAttr, value: str) -> Secret | bool | int | str | None:
+        """Cast attribute value to the correct type.
+
+        Args:
+            attr (ConfigAttr): Configuration attribute.
+            value (str): Value to cast.
+
+        Returns:
+            Any: Casted value.
+        """
+        if attr.secret:
+            return Secret[attr.attr_type](value)  # type: ignore
+        if attr.attr_type is bool:
+            return value.lower().strip() in {"true", "yes", "1", "y"}
+        return attr.attr_type(value)
+
     def load(
         cls,
         get_command: bool = True,
         require_command: bool = False,
         show_parser_help: bool = True,
-    ):
+    ) -> ConfigEntity | None:
+        """Load configuration entity from environment variables and CLI arguments.
+
+        Args:
+            get_command (bool, optional): Get command entity. Defaults to True.
+            require_command (bool, optional): Require command entity. Defaults to False.
+            show_parser_help (bool, optional): Show parser help. Defaults to True.
+
+        Returns:
+            ConfigEntity: Configuration entity.
+        """
         logger.debug("Loading %s", cls.__name__)
 
         if cls.entity_type == ConfigEntityType.module:
             base = cls.root_module
         elif cls.entity_type == ConfigEntityType.command:
             base = cls().parent_module.root_module
         else:
             base = None
 
         if base is None:
             raise AttributeError("Entity must have a base module")
 
         arg_parser = build_parser(base)
+
+        if arg_parser is None:
+            logger.error("Error building parser")
+            return None
+
         try:
             args = vars(arg_parser.parse_known_args()[0])
         except (ArgumentError, ArgumentTypeError):
             logger.exception("Error parsing arguments")
             if show_parser_help:
                 arg_parser.print_help()
 
         current_cls = cls()
         while current_cls is not None:
-            logger.debug("Loading environment variables for %s: %s", current_cls.__name__, current_cls.attrs.keys())
+            logger.debug(
+                "Loading environment variables for %s: %s",
+                current_cls.__name__,
+                current_cls.attrs.keys(),
+            )
             for k, attr in current_cls.attrs.items():
                 if attr.cli_args is not None and attr.name in args and args[attr.name] is not None:
-                    current_cls._sources[k]["cli"] = (
-                        Secret[attr.attr_type](args[attr.name]) if attr.secret else args[attr.name]  # type: ignore
-                    )
+                    current_cls._sources[k]["cli"] = Secret(args[attr.name]) if attr.secret else args[attr.name]
             current_cls = current_cls.parent_module() if current_cls.parent_module is not None else None
 
         logger.debug("Sources for %s: %s", cls.__name__, cls._sources)
 
         if get_command or require_command:
             i = 0
             current_cls = base()
@@ -195,41 +296,55 @@
                 current_cls.__class__.load(get_command=False)
                 return current_cls
 
         return None
 
 
 class AppCommand(metaclass=ConfigEntity):
-    root_module: "AppModule"
+    """Base module for command type configuration entities."""
+
+    root_module: AppModule
 
     show_config = ConfigAttr(
         default=False,
         description="Show configuration",
         cli_args=["--show-config"],
         attr_type=bool,
     )
 
     def show(self, file=sys.stdout):
+        """Prints entity configuration.
+
+        Args:
+            file (Any, optional): Output file. Defaults to sys.stdout.
+        """
         file.write(f"\nCommand     : {self.__name__}")
         file.write(f"\nNamespace   : {self.namespace}")
         file.write(f"\nDescription : {self.__doc__}")
         file.write("\nAttributes")
         for f in self._attribute_names:
             if getattr(self.attr, f).required:
                 file.write("\n  * ")
             else:
                 file.write("\n  - ")
             file.write(f"{getattr(self.attr, f).name}: {getattr(self, f)}")
         file.write("\n\n")
 
 
 class AppModule(metaclass=ConfigEntity):
-    root_module: "AppModule"
+    """Base module for module type configuration entities."""
+
+    root_module: AppModule
 
     def show(self, file=sys.stdout):
+        """Prints entity configuration.
+
+        Args:
+            file (Any, optional): Output file. Defaults to sys.stdout.
+        """
         file.write(f"\nModule      : {self.__name__}")
         file.write(f"\nNamespace   : {self.namespace}")
         file.write(f"\nDescription : {self.__doc__}")
         file.write("\nAttributes:")
         for f in self._attribute_names:
             if getattr(self.attr, f).required:
                 file.write("\n  * ")
@@ -243,20 +358,30 @@
 
         file.write("\nSubmodules:")
         for f in self._submodules:
             file.write(f"\n  * {f.__name__}")
         file.write("\n\n")
 
 
-def build_parser(entity: ConfigEntity = AppModule, level=0, arg_parser=None):
+def build_parser(entity: ConfigEntity = AppModule, level=0, arg_parser=None) -> ArgumentParser | None:
+    """Build command line parser for the entity.
+
+    Args:
+        entity (ConfigEntity): Entity to build parser for.
+        level (int): Current level of the entity.
+        arg_parser (ArgumentParser): Argument parser.
+
+    Returns:
+        ArgumentParser: Argument parser.
+    """
     _entity = entity()
 
     if _entity.entity_type is ConfigEntityType.module and entity is entity.root_module:
         logger.debug("Building parser for %s", entity.__name__)
-        arg_parser = ArgumentParser(sys.argv[0], description=entity.__doc__)
+        arg_parser = ArgumentParser(Path(sys.argv[0]).name, description=entity.__doc__)
 
     logger.debug("Adding arguments for %s", entity.__name__)
 
     logger.debug(arg_parser)
     for attr in _entity._attribute_names:
         logger.debug("Adding argument %s to %s", attr, _entity.__name__)
         logger.debug(_entity.attr)
```

### Comparing `kframe-0.4.3rc1/tests/test_config.py` & `kframe-0.5.0rc1/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,22 @@
             a = ConfigAttr(env_var="A_VALUE", required=True, default="default_a", cli_args=["-a", "--a-value"])
 
         class Module1(AppModule, name="module_1", parent_entity=RootModule):
             b = ConfigAttr(env_var="B_VALUE", required=True, default="default_b", cli_args=["--b-value1"])
 
         class Command1(AppCommand, name="command_0", description="Command 0 extended help", parent_entity=Module1):
             x = ConfigAttr(env_var="X_VALUE", required=True, default="default_x", cli_args=["--x-value"])
-
+            bool_attr = ConfigAttr(default=False, description="Boolean attribute", cli_args=["--bool-attr"], attr_type=bool)
         assert Command1().x == "default_x"
         assert Command1().b == "default_b"
         assert Command1().a == "default_a"
         assert Command1().log_level == "ERROR"
-        assert set(Command1().attrs.keys()) == {"x", "a", "b", "log_level", "show_config"}
+        assert Command1().bool_attr == False
+        assert type(Command1().bool_attr) == bool
+        assert set(Command1().attrs.keys()) == {"x", "a", "b", "log_level", "show_config", "bool_attr"}
 
     def test_root_module_config(self):
         sys.argv = ["test.py", "module_1", "command_1", "-a", "cli_a", "-l", "DEBUG", "-b", "cli_b", "-x", "cli_x"]
         class RootModule(AppModule, name="root"):
             log_level = ConfigAttr(default="ERROR", description="Log level", cli_args=["-l", "--log-level"])
             a = ConfigAttr(env_var="A_VALUE", required=True, default="default_a", cli_args=["-a", "--a-value"])
```

### Comparing `kframe-0.4.3rc1/tests/test_secretattr.py` & `kframe-0.5.0rc1/tests/test_secretattr.py`

 * *Files identical despite different names*

### Comparing `kframe-0.4.3rc1/LICENSE.txt` & `kframe-0.5.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kframe-0.4.3rc1/README.md` & `kframe-0.5.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kframe-0.4.3rc1/pyproject.toml` & `kframe-0.5.0rc1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kframe"
-version = "0.4.3rc1"
+version = "0.5.0rc1"
 description = 'Kaeus development framework'
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MS-PL"
 keywords = []
 authors = [
   { name = "Sebastian Garcia", email = "sgarcia@kaeusanalytics.com" },
@@ -22,14 +22,27 @@
   "Environment :: Console",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
 ]
 dependencies = [
 ]
 
+[project.optional-dependencies]
+api = [
+  "fastapi==0.111.*",
+  "fastapi-health == 0.4.*",
+  "fastapi-pagination == 0.12.*",
+  "prometheus-fastapi-instrumentator == 6.1.*",
+  "uvicorn[standard] == 0.29.*",
+]
+db = [
+  "sqlalchemy==2.0.*",
+  "alembic==1.13.*",
+]
+
 [project.urls]
 # TODO: Update these URLs
 Documentation = "https://github.com/kaeus-sgarcia/kframe#readme"
 Issues = "https://github.com/kaeus-sgarcia/kframe/issues"
 Source = "https://github.com/kaeus-sgarcia/kframe"
 
 # Development environment
@@ -38,14 +51,16 @@
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "ruff",
   "pre-commit",
   "commitizen",
 ]
+features = ["api", "db"]
+
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
 ]
@@ -56,27 +71,41 @@
 
 
 [tool.hatch.envs.quality]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
 ]
+features = ["api", "db"]
 
 [[tool.hatch.envs.quality.matrix]]
 python = ["3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.quality.scripts]
 test = "pytest {args:tests}"
 
+[tool.hatch.envs.build_quality]
+dependencies = [
+  "coverage[toml]>=6.5",
+  "pytest",
+]
+features = ["api", "db"]
+
+[tool.hatch.envs.build_quality.scripts]
+test = "pytest {args:tests}"
+
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
+  "pytest",
 ]
+features = ["api", "db"]
+
 [tool.hatch.envs.types.scripts]
-check = "mypy --install-types --non-interactive {args:src/kframe tests}"
+check = "mypy --install-types  --ignore-missing-imports --non-interactive {args:src/kframe tests}"
 
 [tool.coverage.run]
 source_pkgs = ["kframe", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/kframe/__about__.py",
@@ -96,16 +125,20 @@
 [tool.ruff]
 exclude = [
   "tests/*",
   "*/__about__.py",
 ]
 
 [tool.ruff.lint]
-preview = true
-extend-ignore = ["TID252", "TRY003", "EM10", "SLF", "FBT", "ARG"]
+preview = false
+extend-select = ["D"]
+extend-ignore = ["TID252", "TRY003", "EM10", "SLF", "FBT", "ARG", "B019", "TCH010"]
+
+[tool.ruff.lint.pydocstyle]
+convention = "google"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 annoted_tag = true
```

### Comparing `kframe-0.4.3rc1/PKG-INFO` & `kframe-0.5.0rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kframe
-Version: 0.4.3rc1
+Version: 0.5.0rc1
 Summary: Kaeus development framework
 Project-URL: Documentation, https://github.com/kaeus-sgarcia/kframe#readme
 Project-URL: Issues, https://github.com/kaeus-sgarcia/kframe/issues
 Project-URL: Source, https://github.com/kaeus-sgarcia/kframe
 Author-email: Sebastian Garcia <sgarcia@kaeusanalytics.com>
 License-Expression: MS-PL
 License-File: LICENSE.txt
@@ -13,14 +13,23 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
+Provides-Extra: api
+Requires-Dist: fastapi-health==0.4.*; extra == 'api'
+Requires-Dist: fastapi-pagination==0.12.*; extra == 'api'
+Requires-Dist: fastapi==0.111.*; extra == 'api'
+Requires-Dist: prometheus-fastapi-instrumentator==6.1.*; extra == 'api'
+Requires-Dist: uvicorn[standard]==0.29.*; extra == 'api'
+Provides-Extra: db
+Requires-Dist: alembic==1.13.*; extra == 'db'
+Requires-Dist: sqlalchemy==2.0.*; extra == 'db'
 Description-Content-Type: text/markdown
 
 # Kaeus Development Framework
 
 [![PyPI - Version](https://img.shields.io/pypi/v/kframe.svg)](https://pypi.org/project/kframe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kframe.svg)](https://pypi.org/project/kframe)
 [![CI](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_ci.yml/badge.svg)](https://github.com/kaeus-sgarcia/kframe/actions/workflows/main_ci.yml)
```

