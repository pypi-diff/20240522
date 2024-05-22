# Comparing `tmp/tsc-cfg-0.4.tar.gz` & `tmp/tsc-cfg-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsc-cfg-0.4.tar", last modified: Thu May 16 10:41:21 2024, max compression
+gzip compressed data, was "tsc-cfg-0.5.tar", last modified: Wed May 22 12:08:27 2024, max compression
```

## Comparing `tsc-cfg-0.4.tar` & `tsc-cfg-0.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-16 10:41:21.073135 tsc-cfg-0.4/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.4/LICENSE
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-16 10:41:21.072135 tsc-cfg-0.4/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-16 10:41:21.074134 tsc-cfg-0.4/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1150 2024-05-16 10:40:55.000000 tsc-cfg-0.4/setup.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-16 10:41:21.056134 tsc-cfg-0.4/tsc_cfg/
--rwxrwxrwx   0     1024 users      (100)      245 2024-01-16 05:41:54.000000 tsc-cfg-0.4/tsc_cfg/__init__.py
--rwxrwxrwx   0     1024 users      (100)      948 2024-01-09 06:00:22.000000 tsc-cfg-0.4/tsc_cfg/cfg_utils.py
--rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.4/tsc_cfg/global_info.py
--rwxrwxrwx   0     1024 users      (100)    23741 2024-02-29 07:51:56.000000 tsc-cfg-0.4/tsc_cfg/py_static_cfg.py
--rwxrwxrwx   0     1024 users      (100)     4239 2024-05-16 10:40:57.000000 tsc-cfg-0.4/tsc_cfg/test_global_info.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-16 10:41:21.069135 tsc-cfg-0.4/tsc_cfg.egg-info/
--rwxrwxrwx   0     1024 users      (100)      966 2024-05-16 10:41:21.000000 tsc-cfg-0.4/tsc_cfg.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      287 2024-05-16 10:41:21.000000 tsc-cfg-0.4/tsc_cfg.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-16 10:41:21.000000 tsc-cfg-0.4/tsc_cfg.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)      114 2024-05-16 10:41:21.000000 tsc-cfg-0.4/tsc_cfg.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)        8 2024-05-16 10:41:21.000000 tsc-cfg-0.4/tsc_cfg.egg-info/top_level.txt
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.509719 tsc-cfg-0.5/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-01-09 07:05:44.000000 tsc-cfg-0.5/LICENSE
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 12:08:27.509719 tsc-cfg-0.5/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-22 12:08:27.510718 tsc-cfg-0.5/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1197 2024-05-21 08:10:27.000000 tsc-cfg-0.5/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.492718 tsc-cfg-0.5/tsc_cfg/
+-rwxrwxrwx   0     1024 users      (100)      264 2024-05-21 08:11:33.000000 tsc-cfg-0.5/tsc_cfg/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     9999 2024-05-22 12:07:09.000000 tsc-cfg-0.5/tsc_cfg/cfg_utils.py
+-rwxrwxrwx   0     1024 users      (100)    16476 2024-05-16 10:40:22.000000 tsc-cfg-0.5/tsc_cfg/global_info.py
+-rwxrwxrwx   0     1024 users      (100)    23842 2024-05-22 11:59:14.000000 tsc-cfg-0.5/tsc_cfg/py_static_cfg.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-22 12:08:27.506718 tsc-cfg-0.5/tsc_cfg.egg-info/
+-rwxrwxrwx   0     1024 users      (100)      966 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      259 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)      135 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)        8 2024-05-22 12:08:27.000000 tsc-cfg-0.5/tsc_cfg.egg-info/top_level.txt
```

### Comparing `tsc-cfg-0.4/LICENSE` & `tsc-cfg-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.4/PKG-INFO` & `tsc-cfg-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.4
+Version: 0.5
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tsc-cfg-0.4/setup.py` & `tsc-cfg-0.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = '教程: https://github.com/aitsc/tsc-cfg'
 
 setup(
     name='tsc-cfg',
-    version='0.4',
+    version='0.5',
     description="自定义的配置文件",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='aitsc',
     license='GPLv3',
     url='https://github.com/aitsc/tsc-cfg',
     keywords='tools',
@@ -26,17 +26,19 @@
     ],
     python_requires='>=3.7',
     install_requires=[
         'tsc-base',
         'watchdog',
         'redis',
         'jsonpath-ng',
+        'PyYAML',
     ],
     extras_require={
         'recommended': [
             'tsc-base==0.42',
             'watchdog==3.0.0',
             'redis==5.0.1',
             'jsonpath-ng==1.6.0',
+            'PyYAML==6.0.1',
         ]
     }
 )
```

### Comparing `tsc-cfg-0.4/tsc_cfg/global_info.py` & `tsc-cfg-0.5/tsc_cfg/global_info.py`

 * *Files identical despite different names*

### Comparing `tsc-cfg-0.4/tsc_cfg/py_static_cfg.py` & `tsc-cfg-0.5/tsc_cfg/py_static_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,16 +200,17 @@
             key (Union[str, int, None]): 针对哪个变量进行设置，如果为 None 则直接设置 cls 本身
             value (Any): 设置的值.
                 不允许普通变量（如dict/list）内再嵌套cfg类, 否则会导致 model_* 类方法都无法正常工作.
                 value 中空的 cfg 类永远不会覆盖, 但普通嵌套类型可能会覆盖.
                 新变量会尽量递归转换为配置类, 除非无法转换或者祖先中有配置类可以直接参考, 以及原始配置就不是配置类
             create_new (bool, optional): 是否允许创建新的变量
             cover_old (bool, optional): 是否允许覆盖旧的变量
+                普通list直接整体覆盖, 可以变成配置类的list按照int key编号覆盖
             old_define (Callable[[Any, Any], bool], optional): 输入 (old, new) 返回old是否是否旧值
-                只有 cover_old=True 才会调用
+                只有 cover_old=False 才会调用
                 例如 lambda old, new: not old 可以表示旧值是 None 或 '' 等空值的时候才覆盖
             ancestors_has_cfg (bool, optional): value 递归中的祖先中是否有配置类, 主要用于递归
                 设置为 True 则尽量不将一般变量的 value 及其递归转换为配置类
             raise_new (bool, optional): 是否抛出构建了默认参数中没有的参数的异常, 前提是 create_new=False
             new_bases (Optional[Tuple[type, ...]], optional): 新建配置类的基类, 默认为 None 则继承自 (Cfg,)
                 也可以是 cls.__bases__ 继承自原来的基类，要求至少有个类是 Cfg 或其子类
         """
```

### Comparing `tsc-cfg-0.4/tsc_cfg.egg-info/PKG-INFO` & `tsc-cfg-0.5/tsc_cfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsc-cfg
-Version: 0.4
+Version: 0.5
 Summary: 自定义的配置文件
 Home-page: https://github.com/aitsc/tsc-cfg
 Author: aitsc
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

