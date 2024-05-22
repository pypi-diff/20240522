# Comparing `tmp/tsc-cfg-0.6.tar.gz` & `tmp/tsc-cfg-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-cfg-0.6.tar", last modified: Wed May 22 13:10:51 2024, max compression
+gzip compressed data, was "tsc-cfg-0.7.tar", last modified: Wed May 22 13:28:19 2024, max compression
```

## Comparing `tsc-cfg-0.6.tar` & `tsc-cfg-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.279150 tsc-cfg-0.6/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.6/LICENSE
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:10:51.278150 tsc-cfg-0.6/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-22 13:10:51.279150 tsc-cfg-0.6/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1197 2024-05-22 13:07:54.000000 tsc-cfg-0.6/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.262150 tsc-cfg-0.6/tsc_cfg/
--rwxrwxrwx   0     1024 users      (100)      264 2024-05-21 08:11:33.000000 tsc-cfg-0.6/tsc_cfg/__init__.py
--rwxrwxrwx   0     1024 users      (100)    10520 2024-05-22 13:10:08.000000 tsc-cfg-0.6/tsc_cfg/cfg_utils.py
--rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.6/tsc_cfg/global_info.py
--rwxrwxrwx   0     1024 users      (100)    23323 2024-05-22 13:07:44.000000 tsc-cfg-0.6/tsc_cfg/py_static_cfg.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.276150 tsc-cfg-0.6/tsc_cfg.egg-info/
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      259 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)      135 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)        8 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:28:19.254074 tsc-cfg-0.7/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.7/LICENSE
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:28:19.253075 tsc-cfg-0.7/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-22 13:28:19.255075 tsc-cfg-0.7/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1197 2024-05-22 13:26:54.000000 tsc-cfg-0.7/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:28:19.237074 tsc-cfg-0.7/tsc_cfg/
+-rwxrwxrwx   0     1024 users      (100)      299 2024-05-22 13:26:19.000000 tsc-cfg-0.7/tsc_cfg/__init__.py
+-rwxrwxrwx   0     1024 users      (100)    10865 2024-05-22 13:28:14.000000 tsc-cfg-0.7/tsc_cfg/cfg_utils.py
+-rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.7/tsc_cfg/global_info.py
+-rwxrwxrwx   0     1024 users      (100)    23323 2024-05-22 13:07:44.000000 tsc-cfg-0.7/tsc_cfg/py_static_cfg.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:28:19.251074 tsc-cfg-0.7/tsc_cfg.egg-info/
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:28:19.000000 tsc-cfg-0.7/tsc_cfg.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      259 2024-05-22 13:28:19.000000 tsc-cfg-0.7/tsc_cfg.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-22 13:28:19.000000 tsc-cfg-0.7/tsc_cfg.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)      135 2024-05-22 13:28:19.000000 tsc-cfg-0.7/tsc_cfg.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)        8 2024-05-22 13:28:19.000000 tsc-cfg-0.7/tsc_cfg.egg-info/top_level.txt
```

### Comparing `tsc-cfg-0.6/LICENSE` & `tsc-cfg-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.6/PKG-INFO` & `tsc-cfg-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.6
+Version: 0.7
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tsc-cfg-0.6/setup.py` & `tsc-cfg-0.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = '教程: https://github.com/aitsc/tsc-cfg'
 
 setup(
     name='tsc-cfg',
-    version='0.6',
+    version='0.7',
     description="自定义的配置文件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='GPLv3',
     url='https://github.com/aitsc/tsc-cfg',
     keywords='tools',
```

### Comparing `tsc-cfg-0.6/tsc_cfg/cfg_utils.py` & `tsc-cfg-0.7/tsc_cfg/cfg_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         self.delay = delay
         self.logger = logger
         self._timers: Dict[str, threading.Timer] = {}
         self._yaml_handlers: Dict[str, ReloadYamlHandler] = {}
         self._observer = Observer()
         self._observer.schedule(self, path=os.path.dirname(module.__file__), recursive=False)
         self._observer.start()
-        atexit.register(self._observer.stop)
+        atexit.register(self.stop)
 
     def reset_timer(self, path, opt):
         if path in self._timers:
             self._timers[path].cancel()  # 取消已存在的定时器
         self._timers[path] = threading.Timer(self.delay, self.process_event, [path, opt])
         self._timers[path].start()
 
@@ -69,15 +69,16 @@
             timer.cancel()
         self._timers.clear()
         for handler in self._yaml_handlers.values():
             handler.stop()
         self._yaml_handlers.clear()
     
     def add_yaml(
-        self, *paths: str,
+        self,
+        *paths: str,
         delay: Optional[float] = None,
         logger: Optional[logging.Logger] = None,
         **kwargs,
     ) -> 'ReloadCfgHandler':
         """添加监听的yaml文件夹或文件路径
 
         Args:
@@ -165,15 +166,15 @@
         self.delay = delay
         self.limit_value_type = limit_value_type
         self._timers: Dict[str, threading.Timer] = {}  # 用字典存储文件和对应的定时器
         self.load_all()
         self._observer = Observer()
         self._observer.schedule(self, path=self.path, recursive=True)
         self._observer.start()
-        atexit.register(self._observer.stop)
+        atexit.register(self.stop)
 
     def reset_timer(self, path, opt):
         if path in self._timers:
             self._timers[path].cancel()  # 取消已存在的定时器
         self._timers[path] = threading.Timer(self.delay, self.process_event, [path, opt])
         self._timers[path].start()
     
@@ -262,7 +263,19 @@
         return True
     
     def stop(self):
         self._observer.stop()
         for timer in self._timers.values():
             timer.cancel()
         self._timers.clear()
+
+
+ALL_CFG_HANDLERS: Dict[str, ReloadCfgHandler] = {}
+
+
+def get_cfg_handler(module: ModuleType, **kwargs) -> ReloadCfgHandler:
+    if module.__file__ in ALL_CFG_HANDLERS:
+        return ALL_CFG_HANDLERS[module.__file__]
+    else:
+        handler = ReloadCfgHandler(module, **kwargs)
+        ALL_CFG_HANDLERS[module.__file__] = handler
+        return handler
```

### Comparing `tsc-cfg-0.6/tsc_cfg/global_info.py` & `tsc-cfg-0.7/tsc_cfg/global_info.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.6/tsc_cfg/py_static_cfg.py` & `tsc-cfg-0.7/tsc_cfg/py_static_cfg.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.6/tsc_cfg.egg-info/PKG-INFO` & `tsc-cfg-0.7/tsc_cfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.6
+Version: 0.7
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

