# Comparing `tmp/cxalio_studio_tools-0.2.7.tar.gz` & `tmp/cxalio_studio_tools-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxalio_studio_tools-0.2.7.tar", max compression
+gzip compressed data, was "cxalio_studio_tools-0.2.8.tar", max compression
```

## Comparing `cxalio_studio_tools-0.2.7.tar` & `cxalio_studio_tools-0.2.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.2.7/LICENSE
--rw-r--r--   0        0        0     1084 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2120 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.7/README.md
--rw-r--r--   0        0        0       21 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.7/src/cx_core/__init__.py
--rw-r--r--   0        0        0      108 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.7/src/cx_core/app/__init__.py
--rw-r--r--   0        0        0      139 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.7/src/cx_core/app/abstract_app.py
--rw-r--r--   0        0        0      839 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.7/src/cx_core/app/abstract_env.py
--rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.7/src/cx_core/app/app_logger.py
--rw-r--r--   0        0        0      489 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.7/src/cx_core/app/osinfo.py
--rw-r--r--   0        0        0       57 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.7/src/cx_core/filesystem/__init__.py
--rw-r--r--   0        0        0     7184 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.7/src/cx_core/filesystem/path_expander.py
--rw-r--r--   0        0        0     1011 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.7/src/cx_core/filesystem/path_utils.py
--rw-r--r--   0        0        0      106 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.7/src/cx_core/misc/__init__.py
--rw-r--r--   0        0        0     2252 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.7/src/cx_core/misc/datapackage.py
--rw-r--r--   0        0        0      185 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.7/src/cx_core/misc/misc_utils.py
--rw-r--r--   0        0        0     2991 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.7/src/cx_core/misc/timecode.py
--rw-r--r--   0        0        0     1640 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.7/src/cx_core/misc/timepoint.py
--rw-r--r--   0        0        0      111 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.7/src/cx_core/text/__init__.py
--rw-r--r--   0        0        0      490 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.7/src/cx_core/text/code_detecting.py
--rw-r--r--   0        0        0     1425 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.7/src/cx_core/text/tag_replacer.py
--rw-r--r--   0        0        0     1641 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.7/src/cx_core/text/text_utils.py
--rw-r--r--   0        0        0       29 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.7/src/cx_core/tui/__init__.py
--rw-r--r--   0        0        0      465 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.7/src/cx_core/tui/tui_elements.py
--rw-r--r--   0        0        0      102 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.7/src/cx_subtitle/__init__.py
--rw-r--r--   0        0        0     4872 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.7/src/cx_subtitle/loader.py
--rw-r--r--   0        0        0     5739 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.7/src/cx_subtitle/saver.py
--rw-r--r--   0        0        0      736 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.7/src/cx_subtitle/subtitle.py
--rw-r--r--   0        0        0     2854 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.7/src/cx_subtitle/subtitle_formatter.py
--rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.2.7/src/media_killer/__init__.py
--rw-r--r--   0        0        0     1554 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.7/src/media_killer/env.py
--rw-r--r--   0        0        0     3244 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.7/src/media_killer/example_project.toml
--rw-r--r--   0        0        0      783 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.7/src/media_killer/exceptions.py
--rw-r--r--   0        0        0     5453 2024-05-17 10:52:51.747736 cxalio_studio_tools-0.2.7/src/media_killer/help.md
--rw-r--r--   0        0        0     7390 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.7/src/media_killer/media_killer_app.py
--rw-r--r--   0        0        0     7205 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.7/src/media_killer/mission.py
--rw-r--r--   0        0        0     1324 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.7/src/media_killer/option_package.py
--rw-r--r--   0        0        0     3489 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.7/src/media_killer/profile_loader.py
--rw-r--r--   0        0        0     1772 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.7/src/media_killer/script_writer.py
--rw-r--r--   0        0        0     3075 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.7/src/media_killer/source_adapter.py
--rw-r--r--   0        0        0     4591 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.7/src/media_killer/task_inspector.py
--rw-r--r--   0        0        0     4246 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.7/src/media_killer/transcoder.py
--rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.2.7/src/sub_conv/__init__.py
--rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.7/src/sub_conv/env.py
--rw-r--r--   0        0        0      360 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.7/src/sub_conv/exceptions.py
--rw-r--r--   0        0        0     3548 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.7/src/sub_conv/help.md
--rw-r--r--   0        0        0     5503 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.7/src/sub_conv/subconv_app.py
--rw-r--r--   0        0        0     1857 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.7/src/sub_conv/subtitle_translator.py
--rw-r--r--   0        0        0     6762 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.7/src/sub_conv/worker.py
--rw-r--r--   0        0        0        0 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.7/src/systools/__init__.py
--rw-r--r--   0        0        0      282 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.7/src/systools/env.py
--rw-r--r--   0        0        0     3750 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.7/src/systools/update_githubhosts.py
--rw-r--r--   0        0        0     3031 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    35821 2023-12-06 11:01:10.654584 cxalio_studio_tools-0.2.8/LICENSE
+-rw-r--r--   0        0        0     1084 2024-05-22 12:52:36.684666 cxalio_studio_tools-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2193 2024-05-22 12:53:13.675715 cxalio_studio_tools-0.2.8/README.md
+-rw-r--r--   0        0        0       21 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_app.py
+-rw-r--r--   0        0        0      839 2024-05-17 10:52:51.740230 cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_env.py
+-rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/app/app_logger.py
+-rw-r--r--   0        0        0      489 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/app/osinfo.py
+-rw-r--r--   0        0        0       57 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/__init__.py
+-rw-r--r--   0        0        0     7200 2024-05-22 12:52:36.690771 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_expander.py
+-rw-r--r--   0        0        0     1011 2024-05-17 10:52:51.741230 cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_utils.py
+-rw-r--r--   0        0        0      106 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.8/src/cx_core/misc/__init__.py
+-rw-r--r--   0        0        0     2252 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/cx_core/misc/datapackage.py
+-rw-r--r--   0        0        0      185 2024-05-17 10:52:51.742230 cxalio_studio_tools-0.2.8/src/cx_core/misc/misc_utils.py
+-rw-r--r--   0        0        0     2991 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/misc/timecode.py
+-rw-r--r--   0        0        0     1640 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/misc/timepoint.py
+-rw-r--r--   0        0        0      111 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/text/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-17 10:52:51.743230 cxalio_studio_tools-0.2.8/src/cx_core/text/code_detecting.py
+-rw-r--r--   0        0        0     1425 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/cx_core/text/tag_replacer.py
+-rw-r--r--   0        0        0     1641 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.8/src/cx_core/text/text_utils.py
+-rw-r--r--   0        0        0       29 2024-05-17 10:52:51.744230 cxalio_studio_tools-0.2.8/src/cx_core/tui/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_core/tui/tui_elements.py
+-rw-r--r--   0        0        0      102 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/__init__.py
+-rw-r--r--   0        0        0     4872 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/loader.py
+-rw-r--r--   0        0        0     5739 2024-05-17 10:52:51.745230 cxalio_studio_tools-0.2.8/src/cx_subtitle/saver.py
+-rw-r--r--   0        0        0      736 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle.py
+-rw-r--r--   0        0        0     2854 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle_formatter.py
+-rw-r--r--   0        0        0       35 2024-01-27 12:52:22.618965 cxalio_studio_tools-0.2.8/src/media_killer/__init__.py
+-rw-r--r--   0        0        0     1554 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/media_killer/env.py
+-rw-r--r--   0        0        0     3244 2024-05-17 10:52:54.540884 cxalio_studio_tools-0.2.8/src/media_killer/example_project.toml
+-rw-r--r--   0        0        0      783 2024-05-17 10:52:51.746230 cxalio_studio_tools-0.2.8/src/media_killer/exceptions.py
+-rw-r--r--   0        0        0     5453 2024-05-17 10:52:51.747736 cxalio_studio_tools-0.2.8/src/media_killer/help.md
+-rw-r--r--   0        0        0     7390 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/media_killer_app.py
+-rw-r--r--   0        0        0     7205 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/mission.py
+-rw-r--r--   0        0        0     1324 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/option_package.py
+-rw-r--r--   0        0        0     3489 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/profile_loader.py
+-rw-r--r--   0        0        0     1772 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/script_writer.py
+-rw-r--r--   0        0        0     3075 2024-05-17 10:52:51.748742 cxalio_studio_tools-0.2.8/src/media_killer/source_adapter.py
+-rw-r--r--   0        0        0     4591 2024-05-17 10:52:54.542516 cxalio_studio_tools-0.2.8/src/media_killer/task_inspector.py
+-rw-r--r--   0        0        0     4246 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/media_killer/transcoder.py
+-rw-r--r--   0        0        0       30 2024-02-22 17:29:55.910721 cxalio_studio_tools-0.2.8/src/sub_conv/__init__.py
+-rw-r--r--   0        0        0     1286 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/sub_conv/env.py
+-rw-r--r--   0        0        0      360 2024-05-17 10:52:51.749742 cxalio_studio_tools-0.2.8/src/sub_conv/exceptions.py
+-rw-r--r--   0        0        0     3548 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/help.md
+-rw-r--r--   0        0        0     5503 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/subconv_app.py
+-rw-r--r--   0        0        0     1857 2024-05-17 10:52:51.750742 cxalio_studio_tools-0.2.8/src/sub_conv/subtitle_translator.py
+-rw-r--r--   0        0        0     6762 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.8/src/sub_conv/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 10:52:51.751742 cxalio_studio_tools-0.2.8/src/systools/__init__.py
+-rw-r--r--   0        0        0      282 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.8/src/systools/env.py
+-rw-r--r--   0        0        0     3750 2024-05-17 10:52:51.753851 cxalio_studio_tools-0.2.8/src/systools/update_githubhosts.py
+-rw-r--r--   0        0        0     3100 1970-01-01 00:00:00.000000 cxalio_studio_tools-0.2.8/PKG-INFO
```

### Comparing `cxalio_studio_tools-0.2.7/LICENSE` & `cxalio_studio_tools-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/pyproject.toml` & `cxalio_studio_tools-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cxalio-studio-tools"
-version = "0.2.7"
+version = "0.2.8"
 description = "Scripts for po studio made by cxalio"
 authors = ["xiii_1991 <xiii_1991@163.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cx_core", from = "src" },
     { include = "media_killer", from = "src" },
```

### Comparing `cxalio_studio_tools-0.2.7/README.md` & `cxalio_studio_tools-0.2.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.8
+
+- 强制扩展名按小写判断，不再区分大小写
+
 ### 0.2.7
 
 - 为 mediakiller 增加忽略默认白名单的功能
 - 为 mediakiller 增加自定义表引用的功能
 
 ### 0.2.6
```

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/app/abstract_env.py` & `cxalio_studio_tools-0.2.8/src/cx_core/app/abstract_env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/app/app_logger.py` & `cxalio_studio_tools-0.2.8/src/cx_core/app/app_logger.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/filesystem/path_expander.py` & `cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_expander.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,19 +145,19 @@
     简单的扩展名判断器，
     通过输入的扩展名判断路径是否合法。
     可以方便地插入到 PathExpander 中。
     """
 
     def __init__(self, acceptable_suffixes: Iterable):
         self._suffixes = {x if x.startswith('.') else '.' + x for x in
-                          [str(a).strip() for a in acceptable_suffixes]}
+                          [str(a).strip().lower() for a in acceptable_suffixes]}
 
     def __call__(self, entry: Path):
         entry = Path(entry)
-        return entry.suffix in self._suffixes
+        return entry.suffix.lower() in self._suffixes
 
 
 class BlackListValidator:
     """
     指定黑名单并进行验证，
     可以用于 global_validator
     """
```

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/filesystem/path_utils.py` & `cxalio_studio_tools-0.2.8/src/cx_core/filesystem/path_utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/misc/datapackage.py` & `cxalio_studio_tools-0.2.8/src/cx_core/misc/datapackage.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/misc/timecode.py` & `cxalio_studio_tools-0.2.8/src/cx_core/misc/timecode.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/misc/timepoint.py` & `cxalio_studio_tools-0.2.8/src/cx_core/misc/timepoint.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/text/tag_replacer.py` & `cxalio_studio_tools-0.2.8/src/cx_core/text/tag_replacer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_core/text/text_utils.py` & `cxalio_studio_tools-0.2.8/src/cx_core/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_subtitle/loader.py` & `cxalio_studio_tools-0.2.8/src/cx_subtitle/loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_subtitle/saver.py` & `cxalio_studio_tools-0.2.8/src/cx_subtitle/saver.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_subtitle/subtitle.py` & `cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/cx_subtitle/subtitle_formatter.py` & `cxalio_studio_tools-0.2.8/src/cx_subtitle/subtitle_formatter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/env.py` & `cxalio_studio_tools-0.2.8/src/media_killer/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/example_project.toml` & `cxalio_studio_tools-0.2.8/src/media_killer/example_project.toml`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/exceptions.py` & `cxalio_studio_tools-0.2.8/src/media_killer/exceptions.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/help.md` & `cxalio_studio_tools-0.2.8/src/media_killer/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/media_killer_app.py` & `cxalio_studio_tools-0.2.8/src/media_killer/media_killer_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/mission.py` & `cxalio_studio_tools-0.2.8/src/media_killer/mission.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/option_package.py` & `cxalio_studio_tools-0.2.8/src/media_killer/option_package.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/profile_loader.py` & `cxalio_studio_tools-0.2.8/src/media_killer/profile_loader.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/script_writer.py` & `cxalio_studio_tools-0.2.8/src/media_killer/script_writer.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/source_adapter.py` & `cxalio_studio_tools-0.2.8/src/media_killer/source_adapter.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/task_inspector.py` & `cxalio_studio_tools-0.2.8/src/media_killer/task_inspector.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/media_killer/transcoder.py` & `cxalio_studio_tools-0.2.8/src/media_killer/transcoder.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/sub_conv/env.py` & `cxalio_studio_tools-0.2.8/src/sub_conv/env.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/sub_conv/help.md` & `cxalio_studio_tools-0.2.8/src/sub_conv/help.md`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/sub_conv/subconv_app.py` & `cxalio_studio_tools-0.2.8/src/sub_conv/subconv_app.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/sub_conv/subtitle_translator.py` & `cxalio_studio_tools-0.2.8/src/sub_conv/subtitle_translator.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/sub_conv/worker.py` & `cxalio_studio_tools-0.2.8/src/sub_conv/worker.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/src/systools/update_githubhosts.py` & `cxalio_studio_tools-0.2.8/src/systools/update_githubhosts.py`

 * *Files identical despite different names*

### Comparing `cxalio_studio_tools-0.2.7/PKG-INFO` & `cxalio_studio_tools-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxalio-studio-tools
-Version: 0.2.7
+Version: 0.2.8
 Summary: Scripts for po studio made by cxalio
 Home-page: https://gitee.com/xiii_1991/cxalio-studio-tools
 License: GPL-3.0-or-later
 Keywords: ffmpeg,tool
 Author: xiii_1991
 Author-email: xiii_1991@163.com
 Requires-Python: >=3.11,<4.0
@@ -59,14 +59,18 @@
 
 ## To-do
 
 - media-inspector 解析媒体信息
 
 ## Change-log
 
+### 0.2.8
+
+- 强制扩展名按小写判断，不再区分大小写
+
 ### 0.2.7
 
 - 为 mediakiller 增加忽略默认白名单的功能
 - 为 mediakiller 增加自定义表引用的功能
 
 ### 0.2.6
```

