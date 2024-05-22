# Comparing `tmp/conf_root-0.3.1.tar.gz` & `tmp/conf_root-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_root-0.3.1.tar", last modified: Tue May 14 13:16:29 2024, max compression
+gzip compressed data, was "conf_root-0.3.2.tar", last modified: Wed May 22 08:56:27 2024, max compression
```

## Comparing `conf_root-0.3.1.tar` & `conf_root-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 13:16:23.000000 conf_root-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-14 13:16:29.922479 conf_root-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-05-14 13:16:23.000000 conf_root-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.918479 conf_root-0.3.1/conf_root/
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/ConfRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.918479 conf_root-0.3.1/conf_root/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/BasicAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/JsonAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/SingleFileYamlAgent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-14 13:16:23.000000 conf_root-0.3.1/conf_root/agents/YamlAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/conf_root.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 13:16:29.000000 conf_root-0.3.1/conf_root.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:16:29.922479 conf_root-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-14 13:16:23.000000 conf_root-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:29.922479 conf_root-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_multi_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_nested_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_single_file_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-14 13:16:23.000000 conf_root-0.3.1/tests/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 08:56:23.000000 conf_root-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-22 08:56:27.499952 conf_root-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-22 08:56:23.000000 conf_root-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.495952 conf_root-0.3.2/conf_root/
+-rw-r--r--   0 runner    (1001) docker     (127)     4900 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/ConfRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/conf_root/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/BasicAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/JsonAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/SingleFileYamlAgent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-22 08:56:23.000000 conf_root-0.3.2/conf_root/agents/YamlAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/conf_root.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 08:56:27.000000 conf_root-0.3.2/conf_root.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:56:27.499952 conf_root-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-22 08:56:23.000000 conf_root-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:27.499952 conf_root-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_multi_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_nested_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_single_file_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-22 08:56:23.000000 conf_root-0.3.2/tests/test_wrap.py
```

### Comparing `conf_root-0.3.1/LICENSE` & `conf_root-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/PKG-INFO` & `conf_root-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conf_root
-Version: 0.3.1
+Version: 0.3.2
 Summary: 基于dataclass的符合逻辑的配置取用方式。
 Home-page: https://github.com/ciaranchen/conf_root
 Author: ciaranchen
 Author-email: ciaranchen@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -37,35 +37,33 @@
 @ConfRoot().wrap('config')
 @dataclass
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`) ，如果不存在则按照默认值新建文件。
+# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
+# 如不存在则按照默认值新建文件（或在文件中添加字段）。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
-# 对 app_config 内容改动后，可通过以下方式写入配置文件
-app_config.save()
-# 对 配置文件 内容改动后，可通过以下方式加载配置文件
-app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
 - name。该配置在path中的位置。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
```

### Comparing `conf_root-0.3.1/README.md` & `conf_root-0.3.2/conf_root.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: conf_root
+Version: 0.3.2
+Summary: 基于dataclass的符合逻辑的配置取用方式。
+Home-page: https://github.com/ciaranchen/conf_root
+Author: ciaranchen
+Author-email: ciaranchen@qq.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ruamel.yaml
+
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
 基于dataclass的符合逻辑的配置文件取用方式。主要功能如下：
 
 1. 封装dataclass到配置文件。
@@ -22,35 +37,33 @@
 @ConfRoot().wrap('config')
 @dataclass
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`) ，如果不存在则按照默认值新建文件。
+# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
+# 如不存在则按照默认值新建文件（或在文件中添加字段）。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
-# 对 app_config 内容改动后，可通过以下方式写入配置文件
-app_config.save()
-# 对 配置文件 内容改动后，可通过以下方式加载配置文件
-app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
 - name。该配置在path中的位置。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
```

### Comparing `conf_root-0.3.1/conf_root/ConfRoot.py` & `conf_root-0.3.2/conf_root/ConfRoot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 import argparse
-from dataclasses import make_dataclass, is_dataclass, MISSING
+from dataclasses import make_dataclass, is_dataclass, MISSING, dataclass
 from pathlib import Path
 from typing import Optional, Type
+import logging
 
 from conf_root.Configuration import Configuration
 from conf_root.agents.BasicAgent import BasicAgent
 from conf_root.agents.YamlAgent import YamlAgent
 
+logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s',
+                    datefmt='%m-%d %H:%M:%S')
+logger = logging.getLogger(__name__)
+
 
 class ConfRoot:
-    def __init__(self, path: str = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent):
+    def __init__(self, path: str = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False):
         self.path = Path(path) if path is not None else Path()
         self.agent_class = agent_class
         self.persist = (agent_class is not None)
         if self.persist:
             self.agent = self.agent_class(self.path)
+        self.dynamic = dynamic
 
     def wrap(self, *args, **kwargs):
         def decorator(cls, name: Optional[str] = None):
             if not is_dataclass(cls):
-                raise TypeError(f"Target class must be a dataclass, got {cls}")
+                logger.debug(f'decorate class {cls.__qualname__} to dataclass...')
+                cls = dataclass(cls)
             if name is None:
                 name = cls.__qualname__.replace('<locals>.', '')
 
             configuration = Configuration.from_wrapper(cls, name)
             setattr(cls, '__CONF_ROOT__', configuration)
 
             # 覆盖其 __init__ 函数
             origin_init = cls.__init__
 
             def decorated_init(_self, *args, **kwargs):
                 origin_init(_self, *args, **kwargs)
                 self.post_init(_self, configuration)
 
-            def save(_self):
-                return self.agent.save(configuration, _self)
-
-            def load(_self):
-                data = self.agent.load(configuration)
-                configuration.data2obj(_self, data)
-
             decorated_init.__name__ = '__init__'
             cls.__init__ = decorated_init
-            if self.persist:
+            if self.persist and self.dynamic:
+                def save(_self):
+                    return self.agent.save(configuration, _self)
+
+                def load(_self):
+                    data = self.agent.load(configuration)
+                    configuration.data2obj(_self, data)
+
                 cls.save = save
                 cls.load = load
             return cls
 
         if len(args) == 1 and isinstance(args[0], type):
             # 无参数情况下，相当于直接用类的定义调用decorator.
             # @wrap
```

### Comparing `conf_root-0.3.1/conf_root/Configuration.py` & `conf_root-0.3.2/conf_root/Configuration.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/conf_root/agents/BasicAgent.py` & `conf_root-0.3.2/conf_root/agents/BasicAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/conf_root/agents/JsonAgent.py` & `conf_root-0.3.2/conf_root/agents/JsonAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/conf_root/agents/SingleFileYamlAgent.py` & `conf_root-0.3.2/conf_root/agents/SingleFileYamlAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/conf_root/agents/YamlAgent.py` & `conf_root-0.3.2/conf_root/agents/YamlAgent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/conf_root.egg-info/PKG-INFO` & `conf_root-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: conf_root
-Version: 0.3.1
-Summary: 基于dataclass的符合逻辑的配置取用方式。
-Home-page: https://github.com/ciaranchen/conf_root
-Author: ciaranchen
-Author-email: ciaranchen@qq.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ruamel.yaml
-
 # Conf Root
 
 ![PyPI - Version](https://img.shields.io/pypi/v/conf_root)
 
 基于dataclass的符合逻辑的配置文件取用方式。主要功能如下：
 
 1. 封装dataclass到配置文件。
@@ -37,35 +22,33 @@
 @ConfRoot().wrap('config')
 @dataclass
 class AppConfig:
     database_host: str = 'localhost'
     database_port: int = 5432
 
 
-# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`) ，如果不存在则按照默认值新建文件。
+# 检测是否存在配置文件(文件名为name+后缀)(如果未传入name参数，文件名为 `{cls.__qual_name__}.yml`)。
+# 如不存在则按照默认值新建文件（或在文件中添加字段）。
 # 如存在配置文件，则加载文件中的配置。
 app_config = AppConfig()
-# 对 app_config 内容改动后，可通过以下方式写入配置文件
-app_config.save()
-# 对 配置文件 内容改动后，可通过以下方式加载配置文件
-app_config.load()
 ```
 
 > note: dataclass 中的字段需指定类型。如果不指定类型，将被视为类变量而不会被解析为dataclass中的字段。这个库在dataclass的基础上进行解析，将无法直接处理类变量。
 
 ### 参数解释
 
-#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent)`
+#### `ConfRoot(path = None, agent_class: Optional[Type[BasicAgent]] = YamlAgent, dynamic=False)`
 
 - path 为基本路径。当它为None时，将会设置为当前文件路径。
 - agent_class 为配置存储的形式。当前支持JsonAgent/YamlAgent/SingleFileYamlAgent。默认为YamlAgent。
     - 对于存储到多个文件的agent（JsonAgent、YamlAgent），path是配置存储的文件夹路径。
     - 对于存储到单个文件的agent（SingleFileYamlAgent），path是配置存储的文件路径。
     - 如果指定为None，可以不产生配置文件存储；同时也不会为类添加save与load方法。
     - 可以继承BasicAgent进行拓展以适配更多类型的序列化方式。
+- dynamic 为是否允许动态加载与变更配置文件。默认为False。如果设定为True，将会为类添加`save` 和 `load`方法来动态写入或读取配置文件。
 
 #### `ConfRoot.wrap`
 
 可以使用不同方式调用。详见上方示例。
 
 - name。该配置在path中的位置。
     - 对于多文件存储，name为文件名。指定时可以带上agent相应的后缀名。
```

### Comparing `conf_root-0.3.1/conf_root.egg-info/SOURCES.txt` & `conf_root-0.3.2/conf_root.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/setup.py` & `conf_root-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="conf_root",  # 包名
-    version="0.3.1",  # 版本号
+    version="0.3.2",  # 版本号
     install_requires=[
         "ruamel.yaml"
     ],
     author="ciaranchen",
     author_email="ciaranchen@qq.com",
     description="基于dataclass的符合逻辑的配置取用方式。",
     long_description=long_description,
```

### Comparing `conf_root-0.3.1/tests/test_argparse.py` & `conf_root-0.3.2/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/tests/test_multi_file_agent.py` & `conf_root-0.3.2/tests/test_multi_file_agent.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/tests/test_nested_dataclass.py` & `conf_root-0.3.2/tests/test_nested_dataclass.py`

 * *Files identical despite different names*

### Comparing `conf_root-0.3.1/tests/test_wrap.py` & `conf_root-0.3.2/tests/test_single_file_agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,80 @@
-import os.path
+import unittest
+
+import os
 import unittest
 from dataclasses import dataclass
 
 from conf_root import ConfRoot
-from conf_root.agents.JsonAgent import JsonAgent
+from conf_root.agents.SingleFileYamlAgent import SingleFileYamlAgent
+from tests.utils import replace_text
 
 
-class TestWrap(unittest.TestCase):
+class TestSingleFileYamlAgent(unittest.TestCase):
+    location = 'settings.yml'
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
-        self.yaml_location = 'config.yml'
-        self.json_location = 'config.json'
+        self.conf_root = ConfRoot(self.location, agent_class=SingleFileYamlAgent)
 
-    def tearDown(self):
-        # 使用os.remove删除在测试中创建的文件
-        try:
-            os.remove(self.yaml_location)
-        except FileNotFoundError:
-            pass
+        @self.conf_root.wrap
+        @dataclass
+        class AppConfig:
+            not_default: str
+            database_host: str = 'localhost'
+            database_port: int = 5432
 
-        try:
-            os.remove(self.json_location)
-        except FileNotFoundError:
-            pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
+        @self.conf_root.wrap
+        @dataclass
+        class AppConfig2:
+            one_thing: int = 42
+            another_thing: int = 1024
+
+        self.conf1 = AppConfig
+        self.conf2 = AppConfig2
+        self.section_name1 = self.conf1.__CONF_ROOT__.name
+        self.section_name2 = self.conf2.__CONF_ROOT__.name
 
-    def replace_text(self, filename, origin_text, replace_text):
+    @staticmethod
+    def replace_text(filename, origin_text, replace_text):
         with open(filename, 'r') as file:
             content = file.read()
         content = content.replace(origin_text, replace_text)
         with open(filename, 'w') as file:
             file.write(content)
 
-    def test_default_yaml_configuration(self):
-        # 测试直接使用configuration而不带参数的情况。
-        @ConfRoot().wrap('config')
-        @dataclass
-        class AppConfig:
-            something: int = 42
+    def tearDown(self):
+        # 使用os.remove删除在测试中创建的文件
+        try:
+            os.remove(self.location)
+        except FileNotFoundError:
+            pass  # 如果文件不存在，忽略错误（也可以根据需求抛出异常）
+
+    def test_create(self):
+        app_config = self.conf1('admin')
+        app_config2 = self.conf2()
 
-        app_config = AppConfig()
-        self.assertTrue(os.path.exists(self.yaml_location))
-        with open(self.yaml_location, 'r') as file:
+        self.assertTrue(os.path.exists(self.location))
+        with open(self.location, 'r') as file:
             content = file.read()
-        self.assertTrue('42' in content)
-        self.replace_text(self.yaml_location, '42', '43')
-        app_config2 = AppConfig()
-        self.assertEqual(app_config2.something, 43)
+        self.assertTrue(self.section_name1 in content)
+        self.assertTrue(self.section_name2 in content)
 
-    def test_default_json_configuration(self):
-        @ConfRoot(agent_class=JsonAgent).wrap('config')
-        @dataclass
-        class AppConfig:
-            something: int = 42
+    def test_save_and_load(self):
+        app_config = self.conf1('admin')
+        app_config2 = self.conf2()
+
+        app_config.database_port = 9527
+        app_config.save()
 
-        app_config = AppConfig()
-        self.assertTrue(os.path.exists(self.json_location))
-        with open(self.json_location, 'r') as file:
+        self.assertTrue(os.path.exists(self.location))
+        with open(self.location, 'r') as file:
             content = file.read()
-        self.assertTrue('42' in content)
-        self.replace_text(self.json_location, '42', '43')
-        app_config2 = AppConfig()
-        self.assertEqual(app_config2.something, 43)
+        self.assertTrue('9527' in content)
+        self.assertTrue(self.section_name2 in content)
+
+        replace_text(self.location, '42', '43')
+        conf2 = self.conf2()
+        self.assertEqual(conf2.one_thing, 43)
+        self.assertEqual(conf2.another_thing, 1024)
 
 
-if __name__ == '__main__':
-    unittest.main()
```

