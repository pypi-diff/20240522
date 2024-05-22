# Comparing `tmp/tsc-cfg-0.5.tar.gz` & `tmp/tsc-cfg-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-cfg-0.5.tar", last modified: Wed May 22 12:08:27 2024, max compression
+gzip compressed data, was "tsc-cfg-0.6.tar", last modified: Wed May 22 13:10:51 2024, max compression
```

## Comparing `tsc-cfg-0.5.tar` & `tsc-cfg-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.509719 tsc-cfg-0.5/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.5/LICENSE
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 12:08:27.509719 tsc-cfg-0.5/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-22 12:08:27.510718 tsc-cfg-0.5/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1197 2024-05-21 08:10:27.000000 tsc-cfg-0.5/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.492718 tsc-cfg-0.5/tsc_cfg/
--rwxrwxrwx   0     1024 users      (100)      264 2024-05-21 08:11:33.000000 tsc-cfg-0.5/tsc_cfg/__init__.py
--rwxrwxrwx   0     1024 users      (100)     9999 2024-05-22 12:07:09.000000 tsc-cfg-0.5/tsc_cfg/cfg_utils.py
--rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.5/tsc_cfg/global_info.py
--rwxrwxrwx   0     1024 users      (100)    23842 2024-05-22 11:59:14.000000 tsc-cfg-0.5/tsc_cfg/py_static_cfg.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.506718 tsc-cfg-0.5/tsc_cfg.egg-info/
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      259 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)      135 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)        8 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.279150 tsc-cfg-0.6/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.6/LICENSE
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:10:51.278150 tsc-cfg-0.6/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-22 13:10:51.279150 tsc-cfg-0.6/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1197 2024-05-22 13:07:54.000000 tsc-cfg-0.6/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.262150 tsc-cfg-0.6/tsc_cfg/
+-rwxrwxrwx   0     1024 users      (100)      264 2024-05-21 08:11:33.000000 tsc-cfg-0.6/tsc_cfg/__init__.py
+-rwxrwxrwx   0     1024 users      (100)    10520 2024-05-22 13:10:08.000000 tsc-cfg-0.6/tsc_cfg/cfg_utils.py
+-rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.6/tsc_cfg/global_info.py
+-rwxrwxrwx   0     1024 users      (100)    23323 2024-05-22 13:07:44.000000 tsc-cfg-0.6/tsc_cfg/py_static_cfg.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 13:10:51.276150 tsc-cfg-0.6/tsc_cfg.egg-info/
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      259 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)      135 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)        8 2024-05-22 13:10:51.000000 tsc-cfg-0.6/tsc_cfg.egg-info/top_level.txt
```

### Comparing `tsc-cfg-0.5/LICENSE` & `tsc-cfg-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.5/PKG-INFO` & `tsc-cfg-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.5
+Version: 0.6
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tsc-cfg-0.5/setup.py` & `tsc-cfg-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = '教程: https://github.com/aitsc/tsc-cfg'
 
 setup(
     name='tsc-cfg',
-    version='0.5',
+    version='0.6',
     description="自定义的配置文件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='GPLv3',
     url='https://github.com/aitsc/tsc-cfg',
     keywords='tools',
```

### Comparing `tsc-cfg-0.5/tsc_cfg/cfg_utils.py` & `tsc-cfg-0.6/tsc_cfg/cfg_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler, FileSystemEvent, FileSystemMovedEvent
 import importlib
 import atexit
 import os
 import yaml
-from typing import Optional, Any, Dict, List
+from typing import Optional, Any, Dict, List, Union
 import threading
 import logging
 from types import ModuleType
+from copy import deepcopy
 from .py_static_cfg import Cfg
 
 
 class ReloadCfgHandler(FileSystemEventHandler):
     def __init__(
         self,
         module: ModuleType,
@@ -79,14 +80,15 @@
     ) -> 'ReloadCfgHandler':
         """添加监听的yaml文件夹或文件路径
 
         Args:
             *paths (str): 监听的yaml文件夹或文件路径
                 配置文件的文件名必须以 .yaml 结尾，不能以 . 开头
                 yaml 的 key 必须符合变量名的命名规范, 不能是任意的字符串, 否则转成普通对象或报错
+                重复的 key 后面更新的会覆盖前面
             delay (float, optional): 延迟处理时间, 单位秒
             logger (Optional[logging.Logger], optional): 日志记录器, 否则使用 print
 
         Returns:
             ReloadCfgHandler: 返回自身
         """
         for p in paths:
@@ -138,14 +140,15 @@
         """延迟处理文件变化事件，使用多线程实现延迟，不适合大量文件变化
 
         Args:
             module (ModuleType): 重新加载的模块, Cfg 类所在的模块
             path (str): 监听的yaml文件夹或文件路径
                 配置文件的文件名必须以 .yaml 结尾，不能以 . 开头
                 yaml 的 key 必须符合变量名的命名规范, 不能是任意的字符串, 否则转成普通对象或报错
+                重复的 key 后面更新的会覆盖前面
             delay (float, optional): 延迟处理时间, 单位秒
             logger (Optional[logging.Logger], optional): 日志记录器, 否则使用 print
             create_path (bool, optional): 是否创建不存在的路径, 防止文件不存在报错
                 后缀名为 .yaml 则创建文件，否则创建文件夹
             limit_value_type (bool, optional): 限制值的类型, 除 None 以外不允许 yaml 的 value 类型和配置类不同
         """
         if create_path and not os.path.exists(path):
@@ -175,19 +178,26 @@
         self._timers[path].start()
     
     @staticmethod
     def old_define(old: Any, new: Any) -> bool:
         if (  # 要求 old 和 new 都是 None 或者类型相同, 不然可能改变类型
             old is None or
             new is None or
-            type(old) == type(new)
+            type(old) == type(new) or
+            isinstance(old, (set, tuple)) and isinstance(new, list)
         ):
             return True
         raise TypeError(f"Cfg type mismatch: {type(old)} != {type(new)}, old={str(old)}, new={str(new)}")
     
+    @staticmethod
+    def direct_assign_func(key: Union[str, int], old: Any, new: Any) -> Any:
+        if isinstance(old, (set, tuple)) and isinstance(new, list):
+            return type(old)(new)
+        return deepcopy(new)
+    
     def load_all(self, opt: str = 'init'):
         if os.path.isdir(self.path):
             for root, dirs, files in os.walk(self.path):
                 for file in files:
                     if not self.yaml_check(file):
                         continue
                     path = os.path.join(root, file)
@@ -207,16 +217,17 @@
                     continue
                 vv = getattr(self.module, k)
                 if hasattr(vv, '_set_'):
                     vv: Cfg
                     vv._set_(
                         key=None,
                         value=v,
-                        cover_old=not self.limit_value_type,
+                        cover_old=self.limit_value_type,
                         old_define=self.old_define,
+                        direct_assign_func=self.direct_assign_func,
                     )
                 setattr(self.module, k, vv)
                 update_flag = True
             if update_flag and opt:
                 if self.logger:
                     self.logger.info(f"Reloaded cfg yaml ({opt}) {path}")
                 else:
```

### Comparing `tsc-cfg-0.5/tsc_cfg/global_info.py` & `tsc-cfg-0.6/tsc_cfg/global_info.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.5/tsc_cfg/py_static_cfg.py` & `tsc-cfg-0.6/tsc_cfg/py_static_cfg.py`

 * *Files 9% similar despite different names*

```diff
@@ -189,34 +189,40 @@
               value: Any,
               create_new: bool = True,
               cover_old: bool = True,
               old_define: Callable[[Any, Any], bool] = lambda old, new: True,
               ancestors_has_cfg: bool = False,
               raise_new: bool = True,
               new_bases: Optional[Tuple[type, ...]] = None,
+              direct_assign_func: Optional[Callable[[Union[str, int], Any, Any], Any]] = None,
               ):
         """设置静态变量中的内容
 
         Args:
             key (Union[str, int, None]): 针对哪个变量进行设置，如果为 None 则直接设置 cls 本身
             value (Any): 设置的值.
                 不允许普通变量（如dict/list）内再嵌套cfg类, 否则会导致 model_* 类方法都无法正常工作.
                 value 中空的 cfg 类永远不会覆盖, 但普通嵌套类型可能会覆盖.
                 新变量会尽量递归转换为配置类, 除非无法转换或者祖先中有配置类可以直接参考, 以及原始配置就不是配置类
             create_new (bool, optional): 是否允许创建新的变量
             cover_old (bool, optional): 是否允许覆盖旧的变量
                 普通list直接整体覆盖, 可以变成配置类的list按照int key编号覆盖
             old_define (Callable[[Any, Any], bool], optional): 输入 (old, new) 返回old是否是否旧值
-                只有 cover_old=False 才会调用
+                只有 cover_old=True 才会调用, 此时如果返回 True (即定义 old 是旧值) 才会覆盖
                 例如 lambda old, new: not old 可以表示旧值是 None 或 '' 等空值的时候才覆盖
             ancestors_has_cfg (bool, optional): value 递归中的祖先中是否有配置类, 主要用于递归
                 设置为 True 则尽量不将一般变量的 value 及其递归转换为配置类
             raise_new (bool, optional): 是否抛出构建了默认参数中没有的参数的异常, 前提是 create_new=False
             new_bases (Optional[Tuple[type, ...]], optional): 新建配置类的基类, 默认为 None 则继承自 (Cfg,)
                 也可以是 cls.__bases__ 继承自原来的基类，要求至少有个类是 Cfg 或其子类
+            direct_assign_func (Optional[Callable[[Union[str, int], Any, Any], Any]], optional): 非配置类的直接赋值函数
+                第一个参数是 key (可能是递归后的), 第二个参数是 old (key 对应的原来值), 第三个参数是 new (key 对应的新值), 返回修改后的实际 value
+                None 等价于: lambda key, this, value: deepcopy(value)
+                可以用于格式转换, 例如来自 json 的 list 转换为 str:
+                    lambda k, t, v: set(v) if isinstance(t, set) and isinstance(v, list) else deepcopy(v)
         """
         assert cls._is_config_class_(cls), 'model_deepcopy must be called on a config class'
         assert cls._is_config_value_(value), f'value {value} is not valid'
         if key is None:  # 设置 cls 本身
             iter_value = None
             if cls._is_config_class_(value):
                 iter_value = value._ikv_
@@ -224,15 +230,16 @@
                 iter_value = value.items()
             elif isinstance(value, list):
                 iter_value = enumerate(value)
             assert iter_value is not None, f'value {value} is not valid'
             for k, v in iter_value:
                 assert k is not None, f'k is not valid'
                 cls._set_(k, v, create_new=create_new, cover_old=cover_old, old_define=old_define,
-                          ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases)
+                          ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases,
+                          direct_assign_func=direct_assign_func)
             return
         try:
             key, this = cls._get_(key, return_kv=True)
         except:
             assert cls._is_config_key_(key) or isinstance(key, int) and key >= 0, f'key {key} is not valid'
             if not create_new:
                 assert not raise_new, f'key {key} is not in config'
@@ -252,51 +259,53 @@
             ):
                 this = type(key, new_bases or (Cfg,), {})
                 type.__setattr__(cls, key, this)
                 iter_value = value.items() if isinstance(value, dict) else enumerate(value)
                 for k, v in iter_value:
                     assert k is not None, f'k is not valid'
                     this._set_(k, v, create_new=create_new, cover_old=cover_old, old_define=old_define,
-                               ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases)
+                               ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases,
+                               direct_assign_func=direct_assign_func)
             else:  # 无法转换为配置类，直接复制
-                type.__setattr__(cls, key, deepcopy(value))
+                type.__setattr__(cls, key, direct_assign_func(key, KEY_NOT_FOUND, value) if direct_assign_func else deepcopy(value))
             return
         
         # 拥有正常的 key 和同一级别的 this 和 value
         if cls._is_config_class_(this):
             iter_value = None
             if cls._is_config_class_(value):  # 配置类直接复制
                 iter_value = value._ikv_
                 ancestors_has_cfg = True
             # 以贪心方式尽量将 value 转换为配置类
             elif not ancestors_has_cfg and value and (
                 isinstance(value, dict) and all(cls._is_config_key_(k) for k in value) or
                 isinstance(value, list) and any(isinstance(v, (dict, list)) for v in value)
             ):
                 iter_value = value.items() if isinstance(value, dict) else enumerate(value)
-            elif cover_old or old_define(this, value):  # 无法转换为配置类，直接复制
-                type.__setattr__(cls, key, deepcopy(value))
+            elif cover_old and old_define(this, value):  # 无法转换为配置类，直接复制
+                type.__setattr__(cls, key, direct_assign_func(key, this, value) if direct_assign_func else deepcopy(value))
             if iter_value is not None:  # 递归覆盖配置类
                 for k, v in iter_value:
                     assert k is not None, f'k is not valid'
                     this._set_(k, v, create_new=create_new, cover_old=cover_old, old_define=old_define,
-                               ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases)
+                               ancestors_has_cfg=ancestors_has_cfg, raise_new=raise_new, new_bases=new_bases,
+                               direct_assign_func=direct_assign_func)
         else:  # 原始配置不是配置类
             if cls._is_config_class_(value):  # this 不是类则不会再当类处理
                 value = value.model_dump(list_conversion=True)
             if isinstance(this, dict) and isinstance(value, dict):  # 递归覆盖普通值
                 ret = cover_dict(value, this, 
                                  allow_new=create_new, 
                                  cover_old=cover_old, 
                                  old_define=old_define,
                                  raise_new=raise_new,
                                  new_deepcopy=True)
                 type.__setattr__(cls, key, ret)
-            elif cover_old or old_define(this, value):  # 无法对齐，则直接覆盖
-                type.__setattr__(cls, key, deepcopy(value))
+            elif cover_old and old_define(this, value):  # 无法对齐，则直接覆盖
+                type.__setattr__(cls, key, direct_assign_func(key, this, value) if direct_assign_func else deepcopy(value))
     
     @classmethod
     def _pop_(cls, 
               key: Union[str, int], 
               return_kv: bool = False,
               t: T = None,
               ) -> Union[Any, Tuple[str, Any], T, Tuple[str, T]]:
@@ -483,66 +492,7 @@
         for k, v in new_class._ikv_:
             if cls._is_config_class_(v):
                 # 不用 setattr 为了防止Cfg配置子类的元类的 __setattr__ 被递归调用
                 type.__setattr__(new_class, k, v.model_deepcopy(k))
             else:
                 type.__setattr__(new_class, k, deepcopy(v))
         return new_class
-
-
-if __name__ == '__main__':
-    Cfg_ = Cfg
-    
-    class MyClass(Cfg_):
-        static_var: bool = False
-
-        class NestedClass(Cfg_, object):
-            nested_var: datetime = datetime.now()
-
-            class NestedClass(Cfg_):
-                nested_var = 10*2
-
-            class NestedClass2(Cfg_):
-                nested_var: Any = '20'
-
-        class Test(Cfg_):
-            ...
-        static_var1: Dict[str, Any] = {
-            'a': {},
-            'b': '2',
-            'c': (3,),
-        }
-
-    x = MyClass._get_('NestedClass', t=MyClass.NestedClass).nested_var
-    print(MyClass.model_dump_code(keep_class_newline=True))
-    # print(Cfg_.model_dump_code())
-    print(MyClass._len_)
-    print()
-
-    MyClass2 = MyClass.model_deepcopy('MyClass2')
-    MyClass.static_var1['a'][1] = 100
-    MyClass2.static_var1['a'][1] = 101
-    print(MyClass.static_var1)
-    print(MyClass2.static_var1)
-    print()
-    
-    print(create_unduplicated_key('a', {'a'}))
-    
-    MyClass2.NestedClass._set_('nested_var2', [{'a': [1, 2]}, 1], create_new=True)
-    MyClass2._set_(0, 1)
-    MyClass2._insert_(123, 2)
-    MyClass2._insert_([2, {'abc': {'test': 123}}, 4], 3, ['test', None, None])
-    print(MyClass2.model_dump_code())
-    print(MyClass._get_(1))
-    print()
-    
-    MyClass._set_(None, [1, 2, 3])
-    print(MyClass.model_dump_code())
-    print(MyClass._get_('a1234', allow_default=True))
-    
-    print('---------meta test---------')
-    # KEY_NOT_FOUND.use_raise = True
-    print(MyClass.abcdefg, MyClass[-1])
-    MyClass.abcdefg = MyClass['abcdefg'] = 1234
-    print(MyClass['abcdefg'])
-    print(MyClass['static_var1.a'])
-    print(KEY_NOT_FOUND.abc.asd)
```

### Comparing `tsc-cfg-0.5/tsc_cfg.egg-info/PKG-INFO` & `tsc-cfg-0.6/tsc_cfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.5
+Version: 0.6
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

