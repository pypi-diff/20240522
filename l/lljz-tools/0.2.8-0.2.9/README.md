# Comparing `tmp/lljz_tools-0.2.8.tar.gz` & `tmp/lljz_tools-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lljz_tools-0.2.8.tar", last modified: Tue Apr  2 13:25:44 2024, max compression
+gzip compressed data, was "lljz_tools-0.2.9.tar", last modified: Sun Apr  7 12:30:37 2024, max compression
```

## Comparing `lljz_tools-0.2.8.tar` & `lljz_tools-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 13:25:44.657611 lljz_tools-0.2.8/
--rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.8/LICENSE
--rw-rw-rw-   0        0        0     4188 2024-04-02 13:25:44.656611 lljz_tools-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 13:25:44.641610 lljz_tools-0.2.8/lljz_tools.egg-info/
--rw-rw-rw-   0        0        0     4188 2024-04-02 13:25:44.000000 lljz_tools-0.2.8/lljz_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-04-02 13:25:44.000000 lljz_tools-0.2.8/lljz_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 13:25:44.000000 lljz_tools-0.2.8/lljz_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-02 13:25:44.000000 lljz_tools-0.2.8/lljz_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 13:25:44.000000 lljz_tools-0.2.8/lljz_tools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-02 13:25:44.650611 lljz_tools-0.2.8/my_tools/
--rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.8/my_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:25:44.652611 lljz_tools-0.2.8/my_tools/attribute_dict/
--rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.8/my_tools/attribute_dict/__init__.py
--rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.8/my_tools/attribute_dict/model.py
--rw-rw-rw-   0        0        0     2931 2024-04-02 13:24:09.000000 lljz_tools-0.2.8/my_tools/c_random.py
-drwxrwxrwx   0        0        0        0 2024-04-02 13:25:44.655610 lljz_tools-0.2.8/my_tools/client/
--rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.8/my_tools/client/__init__.py
--rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.8/my_tools/client/db_client.py
--rw-rw-rw-   0        0        0      434 2024-04-02 11:32:23.000000 lljz_tools-0.2.8/my_tools/client/http_client.py
--rw-rw-rw-   0        0        0     1417 2024-04-02 09:57:01.000000 lljz_tools-0.2.8/my_tools/color.py
--rw-rw-rw-   0        0        0     2458 2024-04-02 12:02:46.000000 lljz_tools-0.2.8/my_tools/console_table.py
--rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.8/my_tools/decorators.py
--rw-rw-rw-   0        0        0     4543 2024-04-02 11:51:16.000000 lljz_tools-0.2.8/my_tools/excel.py
--rw-rw-rw-   0        0        0     5180 2024-04-02 10:36:48.000000 lljz_tools-0.2.8/my_tools/log_manager.py
--rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.8/my_tools/monkey.py
--rw-rw-rw-   0        0        0       85 2024-04-02 13:25:44.658610 lljz_tools-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      665 2024-04-02 13:25:42.000000 lljz_tools-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:30:37.333318 lljz_tools-0.2.9/
+-rw-rw-rw-   0        0        0     1073 2024-02-02 08:09:22.000000 lljz_tools-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0     4188 2024-04-07 12:30:37.332317 lljz_tools-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3755 2024-02-03 07:02:42.000000 lljz_tools-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 12:30:37.315318 lljz_tools-0.2.9/lljz_tools.egg-info/
+-rw-rw-rw-   0        0        0     4188 2024-04-07 12:30:37.000000 lljz_tools-0.2.9/lljz_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-04-07 12:30:37.000000 lljz_tools-0.2.9/lljz_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:30:37.000000 lljz_tools-0.2.9/lljz_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-07 12:30:37.000000 lljz_tools-0.2.9/lljz_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 12:30:37.000000 lljz_tools-0.2.9/lljz_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:30:37.324318 lljz_tools-0.2.9/my_tools/
+-rw-rw-rw-   0        0        0      179 2024-02-02 08:07:00.000000 lljz_tools-0.2.9/my_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:30:37.327319 lljz_tools-0.2.9/my_tools/attribute_dict/
+-rw-rw-rw-   0        0        0      261 2024-02-03 06:30:03.000000 lljz_tools-0.2.9/my_tools/attribute_dict/__init__.py
+-rw-rw-rw-   0        0        0     5886 2024-02-03 06:29:33.000000 lljz_tools-0.2.9/my_tools/attribute_dict/model.py
+-rw-rw-rw-   0        0        0     2972 2024-04-03 03:33:10.000000 lljz_tools-0.2.9/my_tools/c_random.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:30:37.330318 lljz_tools-0.2.9/my_tools/client/
+-rw-rw-rw-   0        0        0      179 2024-02-08 04:17:05.000000 lljz_tools-0.2.9/my_tools/client/__init__.py
+-rw-rw-rw-   0        0        0     5155 2024-02-28 03:49:18.000000 lljz_tools-0.2.9/my_tools/client/db_client.py
+-rw-rw-rw-   0        0        0      434 2024-04-02 11:32:23.000000 lljz_tools-0.2.9/my_tools/client/http_client.py
+-rw-rw-rw-   0        0        0     1462 2024-04-07 09:23:37.000000 lljz_tools-0.2.9/my_tools/color.py
+-rw-rw-rw-   0        0        0     3545 2024-04-07 12:28:31.000000 lljz_tools-0.2.9/my_tools/console_table.py
+-rw-rw-rw-   0        0        0     5328 2024-02-28 03:20:05.000000 lljz_tools-0.2.9/my_tools/decorators.py
+-rw-rw-rw-   0        0        0     4543 2024-04-02 11:51:16.000000 lljz_tools-0.2.9/my_tools/excel.py
+-rw-rw-rw-   0        0        0     6743 2024-04-07 08:57:15.000000 lljz_tools-0.2.9/my_tools/log_manager.py
+-rw-rw-rw-   0        0        0     1595 2024-02-22 09:50:16.000000 lljz_tools-0.2.9/my_tools/monkey.py
+-rw-rw-rw-   0        0        0       85 2024-04-07 12:30:37.334320 lljz_tools-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      665 2024-04-07 12:29:47.000000 lljz_tools-0.2.9/setup.py
```

### Comparing `lljz_tools-0.2.8/LICENSE` & `lljz_tools-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/PKG-INFO` & `lljz_tools-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz_tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.8/README.md` & `lljz_tools-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/lljz_tools.egg-info/PKG-INFO` & `lljz_tools-0.2.9/lljz_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lljz-tools
-Version: 0.2.8
+Version: 0.2.9
 Summary: 常用工具封装
 Home-page: 
 Author: liulangjuanzhou
 Author-email: liulangjuanzhou@gmail.com
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lljz_tools-0.2.8/lljz_tools.egg-info/SOURCES.txt` & `lljz_tools-0.2.9/lljz_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/my_tools/attribute_dict/model.py` & `lljz_tools-0.2.9/my_tools/attribute_dict/model.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/my_tools/c_random.py` & `lljz_tools-0.2.9/my_tools/c_random.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             charList.extend(list(chr(i) for i in range(ord('A'), ord('Z') + 1)))
         elif g == 'lettersUpper':
             charList.extend(list(chr(i) for i in range(ord('A'), ord('Z') + 1)))
         elif g == 'lettersLower':
             charList.extend(list(chr(i) for i in range(ord('a'), ord('z') + 1)))
         elif g == 'special':
             charList.extend(list('`~!@#$%^&*()_+-={}|:"?><,./;\'[]\\'))
-    random.shuffle(charList)
+    random.shuffle(list(set(charList)))
     result = ''.join(random.choice(charList) for _ in range(size))
     while result.startswith('0'):
         result = random_integer(size)
     return result
 
 
 def random_integer(size: int | list[int]):
@@ -74,8 +74,9 @@
     size = max(2, len(str(series)))
     return (f'{s}{i:0>{size}}' for i in range(1, series + 1))
 
 
 if __name__ == '__main__':
     print(random_string_series(3))
     print(random_integer(3))
+    print(random_string(20))
     pass
```

### Comparing `lljz_tools-0.2.8/my_tools/client/db_client.py` & `lljz_tools-0.2.9/my_tools/client/db_client.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/my_tools/color.py` & `lljz_tools-0.2.9/my_tools/color.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 @author : jiangmenggui@hosonsoft.com
 @data   : 2024/4/2
 """
 
 
 class _Color:
 
-    def __init__(self, s, start, end):
+    def __init__(self, s, start, end, name):
         self.raw = s
         self.s = start + s + end
         self.start = start
         self.end = end
+        self.name = name
 
     def __len__(self):
         return self.raw.__len__()
 
     def __str__(self):
         return self.s.__str__()
 
@@ -36,15 +37,15 @@
 
     def __init__(self, name, start, end='\033[0m'):
         self.name = name
         self.start = start
         self.end = end
 
     def __call__(self, s: str):
-        return _Color(s, self.start, self.end)
+        return _Color(s, self.start, self.end, self.name)
 
 
 class Color:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
     OKCYAN = '\033[96m'
     OKGREEN = '\033[92m'
@@ -57,8 +58,9 @@
     green = _ColorFactory('green', OKGREEN)
     yellow = _ColorFactory('yellow', WARNING)
     blue = _ColorFactory('blue', OKBLUE)
     cyan = _ColorFactory('cyan', OKCYAN)
 
 
 if __name__ == '__main__':
+
     pass
```

### Comparing `lljz_tools-0.2.8/my_tools/console_table.py` & `lljz_tools-0.2.9/my_tools/console_table.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,50 @@
 from my_tools.log_manager import LogManager
 
 logger = LogManager('ConsoleTable').get_logger()
 
 
 class ConsoleTable:
 
-    def __init__(self, data: Iterable[dict[str, Any]], max_width=100):
+    def __init__(self, data: Iterable[dict[str, Any]], max_width=100, use_rich_table=False):
         def init_value(val):
             if isinstance(val, str | _Color):
                 return val
             if val is None:
                 return ''
             return str(val)
 
         self.data = [{str(k): init_value(v) for k, v in row.items()} for row in data]
         self.header = list(self.data[0].keys()) if data else []
         self.max_width = max_width
-        self.col_width = self._get_widths()
-        self._table_str = self._make_table_str()
+        self.col_width = []
+        self._table_str = ""
+        self.use_rich_table = use_rich_table
+        if not self.use_rich_table:
+            self.col_width = self._get_widths()
+            self._table_str = self._make_table_str()
+
+    def _make_rich_table(self, title: str):
+        from rich.table import Table
+
+        def get_value(val):
+            if isinstance(val, _Color):
+                return f'[{val.name}]{val.raw}[/{val.name}]'
+            return val
+
+        tb = Table(
+            title=f'{title}' if title else None,
+            title_style='b yellow',
+            min_width=60)
+
+        for key in self.header:
+            tb.add_column(key, justify='center')
+        for row in self.data:
+            tb.add_row(*[get_value(row.get(key, '')) for key in self.header])
+        return tb
 
     @staticmethod
     def _get_string_width(val: str):
         w = 0
         for v in val:
             if u'\u4e00' <= v <= u'\u9fff' or v in '【】（）—…￥！·、？。，《》：；‘“':
                 w += 2
@@ -49,22 +72,31 @@
             left = (width - length) // 2
             right = (width - length) - left
             return f'{" " * left}{val}{" " * right}'
 
         header = ' | '.join(format_str(key, w) for w, key in zip(self.col_width, self.header))
         rows = [' | '.join(format_str(row.get(key, ""), w) for w, key in zip(self.col_width, self.header)) for row in
                 self.data]
-        return '\n'.join([header, '=' * len(header)] + rows)
+        return '\n'.join([header, '=' * (sum(self.col_width) + (len(self.col_width) - 1) * 3)] + rows)
 
     def __str__(self):
-        return self._table_str
+        if not self.use_rich_table:
+            return self._table_str
+        else:
+            return self.__str__()
 
     __repr__ = __str__
 
     def show(self, message=''):
-        logger.info(message + '\n' + str(self.__str__()))
+        if self.use_rich_table:
+            from rich import print as rprint
+            tb = self._make_rich_table(message)
+            if tb.columns:
+                rprint(tb)
+            else:
+                rprint(f'[i u yellow]🏃 {(message + " ") if message else ""}Table is Empty 🏃[/i u yellow]')
+        else:
+            logger.info(message + '\n' + str(self.__str__()))
 
 
 if __name__ == '__main__':
-    from my_tools.color import Color
-    table = ConsoleTable([{'name': Color.red("Tom"), 'b': 2}, {'name': Color.blue("Lucy"), 'b': 4}])
-    table.show()
+    pass
```

### Comparing `lljz_tools-0.2.8/my_tools/decorators.py` & `lljz_tools-0.2.9/my_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/my_tools/excel.py` & `lljz_tools-0.2.9/my_tools/excel.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/my_tools/log_manager.py` & `lljz_tools-0.2.9/my_tools/log_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,52 +8,66 @@
 import colorlog
 
 from my_tools.color import Color
 
 
 class LogManager:
 
-    def __init__(self, log_name, level=logging.DEBUG, formatter: str = None, to_console=True, console_colors=None,
-                 log_file: str =None,
-                 # log_file='/pythonlog/out.log',
-                 file_formatter: str = None, file_level=None,
-                 error_log_file: str = None, error_level=logging.ERROR
-                 ):
+    def __init__(
+            self,
+            log_name,
+            level=logging.DEBUG,  # 控制台中记录的日志等级
+            formatter: str = None,  # 日志格式
+            to_console=True,  # 是否打印到控制台
+            console_colors=None,  # 控制台颜色，为None则使用默认值
+            use_rich_handler=True,  # 是否启用rich.handler作为console的handler
+            log_file: str = None,  # 日志文件记录路径，为None则默认记录在PYTHONPATH下的logs目录
+            file_formatter: str = None,  # 日志文件中记录的格式
+            file_level=None,  # 日志文件中的日志等级，为None则保持和level参数相同
+            error_log_file: str = None,  # 错误日志文件记录路径
+            error_level=logging.ERROR  # 错误日志记录的记录等级
+    ):
         def _init_log_file_path(default_path):
             if 'PYTHONPATH' in os.environ:
                 python_path = os.environ['PYTHONPATH']
+                # 判断python_path是否为一个有效的路径
+                if not os.path.exists(python_path):
+                    print(Color.yellow(f'可能处于DEBUG模式或python控制台运行，无法正确识别到当前工作目录，使用默认路径：{default_path}'))
+                    return default_path
                 log_path = os.path.join(python_path, 'logs')
                 if not os.path.exists(log_path):
                     os.mkdir(path=log_path)
                 return log_path
-            print(Color.yellow(f'没有指定PYTHONPATH环境变量，使用默认路径：{default_path}'))
+            print(Color.yellow(f'未读取到PYTHONPATH环境变量，使用默认路径：{default_path}'))
             return default_path
 
         if not formatter:
             formatter = '%(asctime)s.%(msecs)03d - %(name)s - "%(pathname)s:%(lineno)d" - ' \
                         '%(levelname)s - %(funcName)s : %(message)s'
         if not file_formatter:
             file_formatter = formatter
+        self._use_rich_handler = use_rich_handler
         self._colors = console_colors or {}
         self.formatter = '%(log_color)s' + formatter
         self._file_formatter = file_formatter
         if not file_level:
             file_level = level
-        self._log_file = os.path.join(_init_log_file_path('/pythonlog'), 'out.log') if not log_file else log_file
-        self._error_log_file = os.path.join(_init_log_file_path('/pythonlog'), 'error.log') if not error_log_file else error_log_file
+        self._log_file = os.path.join(
+            _init_log_file_path('/pythonlog'), f'out.log') if not log_file else log_file
+        self._error_log_file = os.path.join(
+            _init_log_file_path('/pythonlog'), f'error.log') if not error_log_file else error_log_file
         self._file_level = file_level
         self._error_file_level = error_level
         logging.root.setLevel(logging.NOTSET)
         self._logger = logging.getLogger(log_name)
         self._logger.setLevel(level)
 
         self._to_console = to_console
         self._console = to_console
 
-
     @staticmethod
     def _make_dir(path):
         parent_dir = os.path.dirname(os.path.abspath(path))
         if not os.path.exists(parent_dir):
             os.makedirs(parent_dir)
 
     def get_logger(self):
@@ -70,19 +84,35 @@
             colors.update(self._colors)
             # 输出到控制台
             console_formatter = colorlog.ColoredFormatter(
                 fmt=self.formatter,
                 datefmt='%Y-%m-%d %H:%M:%S',
                 log_colors=colors,
             )
-            console_handler = logging.StreamHandler()
+            if self._use_rich_handler:
+                try:
+                    from rich.logging import RichHandler  # noqa
+                    console_handler = RichHandler(rich_tracebacks=True, show_path=True)
+                    console_handler.setLevel(logging.DEBUG)
+                    console_handler.setFormatter(
+                        logging.Formatter(
+                            fmt='%(message)s'
+                        ))
+                except ImportError:
+                    console_handler = logging.StreamHandler()
+                    console_handler.setFormatter(console_formatter)
+            else:
+                console_handler = logging.StreamHandler()
+                console_handler.setFormatter(console_formatter)
+
             console_handler.setLevel(logging.DEBUG)
-            console_handler.setFormatter(console_formatter)
+
             self._logger.addHandler(console_handler)
             console_handler.close()
+
         if self._log_file:
             # 输出到文件
             file_formatter = logging.Formatter(
                 fmt=self._file_formatter,
                 datefmt='%Y-%m-%d  %H:%M:%S'
             )
             self._make_dir(self._log_file)
@@ -120,15 +150,14 @@
             self._logger.addHandler(error_file_handler)
             error_file_handler.close()
 
         return self._logger
 
 
 if __name__ == '__main__':
-
     logger2 = LogManager("my log").get_logger()
 
     logger2.debug("Hello World")
     logger2.info("Hello World")
     logger2.warning("Hello World")
     logger2.error("Hello World")
     logger2.critical("Hello World")
```

### Comparing `lljz_tools-0.2.8/my_tools/monkey.py` & `lljz_tools-0.2.9/my_tools/monkey.py`

 * *Files identical despite different names*

### Comparing `lljz_tools-0.2.8/setup.py` & `lljz_tools-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lljz_tools",
-    version="0.2.8",
+    version="0.2.9",
     author="liulangjuanzhou",
     author_email="liulangjuanzhou@gmail.com",
     description="常用工具封装",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

