# Comparing `tmp/hc_log_tools-1.2.5.tar.gz` & `tmp/hc_log_tools-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hc_log_tools-1.2.5.tar", last modified: Sat May 11 06:36:50 2024, max compression
+gzip compressed data, was "hc_log_tools-1.2.6.tar", last modified: Wed May 22 08:35:24 2024, max compression
```

## Comparing `hc_log_tools-1.2.5.tar` & `hc_log_tools-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:36:50.192451 hc_log_tools-1.2.5/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-11 06:36:50.192451 hc_log_tools-1.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1272 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:36:50.192451 hc_log_tools-1.2.5/hc_log_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-11 06:36:50.000000 hc_log_tools-1.2.5/hc_log_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2024-05-11 06:36:50.000000 hc_log_tools-1.2.5/hc_log_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 06:36:50.000000 hc_log_tools-1.2.5/hc_log_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       94 2024-05-11 06:36:50.000000 hc_log_tools-1.2.5/hc_log_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-11 06:36:50.000000 hc_log_tools-1.2.5/hc_log_tools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-05-11 06:36:42.000000 hc_log_tools-1.2.5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 06:36:50.192451 hc_log_tools-1.2.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      749 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:36:50.188451 hc_log_tools-1.2.5/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 06:35:58.000000 hc_log_tools-1.2.5/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/src/entry.py
--rw-rw-rw-   0 root         (0) root         (0)    18729 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/src/log_utility.py
--rw-rw-rw-   0 root         (0) root         (0)     6125 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/src/pack_log.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/src/public.py
--rw-rw-rw-   0 root         (0) root         (0)     3986 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/src/v_t_chart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 06:36:50.192451 hc_log_tools-1.2.5/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-11 06:35:58.000000 hc_log_tools-1.2.5/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_log_download.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_log_file_name_match.py
--rw-rw-rw-   0 root         (0) root         (0)     1946 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_log_utility.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_read_pick_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2601 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_read_sort_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-11 04:32:33.000000 hc_log_tools-1.2.5/test/test_tiem_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/hc_log_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-22 08:35:24.000000 hc_log_tools-1.2.6/hc_log_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2024-05-22 08:35:24.000000 hc_log_tools-1.2.6/hc_log_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 08:35:24.000000 hc_log_tools-1.2.6/hc_log_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2024-05-22 08:35:24.000000 hc_log_tools-1.2.6/hc_log_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 08:35:24.000000 hc_log_tools-1.2.6/hc_log_tools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-05-22 08:35:16.000000 hc_log_tools-1.2.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-05-22 08:14:12.000000 hc_log_tools-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:34:40.000000 hc_log_tools-1.2.6/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2024-05-22 08:14:12.000000 hc_log_tools-1.2.6/src/entry.py
+-rw-rw-rw-   0 root         (0) root         (0)    20487 2024-05-22 08:14:12.000000 hc_log_tools-1.2.6/src/log_utility.py
+-rw-r--r--   0 root         (0) root         (0)     6125 2024-05-22 05:30:52.000000 hc_log_tools-1.2.6/src/pack_log.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/src/public.py
+-rw-rw-rw-   0 root         (0) root         (0)     3986 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/src/v_t_chart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 08:35:24.491318 hc_log_tools-1.2.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 08:34:40.000000 hc_log_tools-1.2.6/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3537 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_log_download.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_log_file_name_match.py
+-rw-rw-rw-   0 root         (0) root         (0)     1946 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_log_utility.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_read_pick_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2601 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_read_sort_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-05-11 04:32:33.000000 hc_log_tools-1.2.6/test/test_tiem_range.py
```

### Comparing `hc_log_tools-1.2.5/LICENSE` & `hc_log_tools-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/PKG-INFO` & `hc_log_tools-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.5
+Version: 1.2.6
 Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_tools-1.2.5/README.md` & `hc_log_tools-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/hc_log_tools.egg-info/PKG-INFO` & `hc_log_tools-1.2.6/hc_log_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hc_log_tools
-Version: 1.2.5
+Version: 1.2.6
 Author-email: "xukai.shi" <xukai.shi@hcrobots.com>, "xukai.shi" <xukai.shi@hcrobots.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: alive_progress==2.4.1
 Requires-Dist: matplotlib==3.5.3
 Requires-Dist: pip>=20.0.2
```

### Comparing `hc_log_tools-1.2.5/hc_log_tools.egg-info/SOURCES.txt` & `hc_log_tools-1.2.6/hc_log_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/src/entry.py` & `hc_log_tools-1.2.6/src/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,40 +7,34 @@
     # only can run one process at a time
     lock_file = open("/tmp/log-tool-lock", "w")
     try:
         fcntl.flock(lock_file, fcntl.LOCK_EX | fcntl.LOCK_NB)
     except IOError:
         print("another process is running, exit")
         sys.exit(-1)
-    
 
     parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.set_defaults(func=lambda args: parser.print_help())
 
     subparsers = parser.add_subparsers(title='subcommands', dest='command', help='sub-command help')
 
     subparsers_pack = subparsers.add_parser("pack", help='pack help')
     src.pack_log.init_input_args(subparsers_pack)
     subparsers_pack.set_defaults(func=src.pack_log.pack_log)
 
     subparsers_chart = subparsers.add_parser("chart", help='chart help')
     src.v_t_chart.init_input_args(subparsers_chart)
     subparsers_chart.set_defaults(func=src.v_t_chart.generate_chart)
-    
 
     # parse the args and call whatever function was selected
-    
-    
     args = parser.parse_args()
     args.func(args)
 
     # pack_log(args)
 
     # if args.up_to_cloud:
     #     pass
     # else:
     #     print(f'output_file_path: {Public.output_file_path}')
 
 if __name__=="__main__":
     sys.exit(entry())
-       
-
```

### Comparing `hc_log_tools-1.2.5/src/log_utility.py` & `hc_log_tools-1.2.6/src/log_utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,38 +20,76 @@
         delta_mins (int, optional): 期望的时间窗口，前后N分钟
         date_selected (_type_, optional): 日志查询窗口的中心时间戳
 
     Returns:
         _type_: _description_
     """
     try:
-        mt = os.path.getmtime(file_path)
-        ct = os.path.getctime(file_path)
+        # 打印当前正在检查的文件路径，帮助调试
+        print(f"{file_path} is checking ...")
 
-        time_range_start_timestamp = (date_selected - timedelta(minutes=delta_mins)).timestamp()
-        time_range_end_timestamp = (date_selected + timedelta(minutes=delta_mins)).timestamp()
+        # 检查文件是否位于特定子目录
+        if "/video" in file_path:
+            print("File is in /video directory, applying video-specific checks.")
+            return check_video_filename(file_path, date_selected)
+        else:
+            mt = os.path.getmtime(file_path)
+            time_range_start_timestamp = (date_selected - timedelta(minutes=delta_mins)).timestamp()
+            time_range_end_timestamp = (date_selected + timedelta(minutes=delta_mins)).timestamp()
 
         # 最后编辑时间小于范围开始时间
         if mt < time_range_start_timestamp:
             print(f"{file_path} not in time range")
             return False
-
+        
+        
         if file_path.endswith("gz"):
             print(f"{file_path} is checking ...")
             with gzip.open(os.path.join(file_path), mode="rt") as f:
                 return check_line_in_a_file(f, delta_mins, date_selected)
         else:
             print(f"{file_path} is checking ...")
             with open(os.path.join(file_path), mode="r", encoding="utf-8") as f:
                 return check_line_in_a_file(f, delta_mins, date_selected)
 
+
     except FileNotFoundError as file_not_find_error:
         print(str(file_not_find_error))
 
 
+
+def check_video_filename(file_path, target_datetime):
+    filename = os.path.basename(file_path)
+    print(f"Debug: Checking filename {filename}")
+
+    # 修改正则表达式以匹配实际的时间格式 "YYYY-MM-DD-HH:MM:SS~YYYY-MM-DD-HH:MM:SS.zip"
+    regex_pattern = r'(\d{4}-\d{2}-\d{2}-\d{2}:\d{2}:\d{2})~(\d{4}-\d{2}-\d{2}-\d{2}:\d{2}:\d{2})\.zip'
+    # print(f"Debug: Using regex pattern {regex_pattern}")
+    match = re.match(regex_pattern, filename)
+
+    if match:
+        start_time_str, end_time_str = match.groups()
+        start_datetime = datetime.strptime(start_time_str, "%Y-%m-%d-%H:%M:%S")
+        end_datetime = datetime.strptime(end_time_str, "%Y-%m-%d-%H:%M:%S")
+
+        # 在这里添加额外的调试输出来显示日期和时间
+        print(f"Debug: Start datetime: {start_datetime}, End datetime: {end_datetime}, Target datetime: {target_datetime}")
+
+        # 检查 target_datetime 是否在 start_datetime 和 end_datetime 之间
+        if start_datetime <= target_datetime <= end_datetime:
+            print(f"The target datetime {target_datetime} is within the range of the file {filename}.")
+            return True
+        else:
+            print(f"The target datetime {target_datetime} is not within the range of the file {filename}.")
+            return False
+    else:
+        print(f"No valid timestamps found in the filename {filename}.")
+        return False
+
+    
 def check_line_in_a_file(f, delta_mins, date_selected=datetime.now()):
     """检测数据是否符合时间预期
 
     Args:
         f (_type_): 已经打开的文件
         delta_mins (int, optional): 期望的时间窗口，前后N分钟
         date_selected (_type_, optional): 日志查询窗口的中心时间戳
```

### Comparing `hc_log_tools-1.2.5/src/pack_log.py` & `hc_log_tools-1.2.6/src/pack_log.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/src/v_t_chart.py` & `hc_log_tools-1.2.6/src/v_t_chart.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_log_download.py` & `hc_log_tools-1.2.6/test/test_log_download.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_log_file_name_match.py` & `hc_log_tools-1.2.6/test/test_log_file_name_match.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_log_utility.py` & `hc_log_tools-1.2.6/test/test_log_utility.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_read_pick_data.py` & `hc_log_tools-1.2.6/test/test_read_pick_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_read_sort_data.py` & `hc_log_tools-1.2.6/test/test_read_sort_data.py`

 * *Files identical despite different names*

### Comparing `hc_log_tools-1.2.5/test/test_tiem_range.py` & `hc_log_tools-1.2.6/test/test_tiem_range.py`

 * *Files identical despite different names*

