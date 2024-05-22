# Comparing `tmp/zfx-1.0.8.tar.gz` & `tmp/zfx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfx-1.0.8.tar", last modified: Tue Apr 30 08:36:07 2024, max compression
+gzip compressed data, was "zfx-1.0.9.tar", last modified: Tue Apr 30 09:50:04 2024, max compression
```

## Comparing `zfx-1.0.8.tar` & `zfx-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 08:36:07.442983 zfx-1.0.8/
--rw-rw-rw-   0        0        0      233 2024-04-30 08:36:07.439489 zfx-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-30 08:36:07.443322 zfx-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      511 2024-04-30 08:36:03.000000 zfx-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:36:07.428543 zfx-1.0.8/zfx/
--rw-rw-rw-   0        0        0     3416 2024-04-30 08:35:24.000000 zfx-1.0.8/zfx/__init__.py
--rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.8/zfx/g2g_account_list.py
--rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.8/zfx/g2g_account_list_s.py
--rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.8/zfx/zmodule_240414A.py
--rw-rw-rw-   0        0        0      905 2024-04-30 07:38:51.000000 zfx-1.0.8/zfx/zprint.py
--rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.8/zfx/目录_创建.py
--rw-rw-rw-   0        0        0      245 2024-04-30 08:17:43.000000 zfx-1.0.8/zfx/算数_保留小数点后指定位数.py
--rw-rw-rw-   0        0        0      239 2024-04-30 07:53:10.000000 zfx-1.0.8/zfx/算数_取绝对值.py
--rw-rw-rw-   0        0        0      191 2024-04-30 08:11:28.000000 zfx-1.0.8/zfx/算数_向上取整.py
--rw-rw-rw-   0        0        0      210 2024-04-30 08:14:48.000000 zfx-1.0.8/zfx/算数_向下取整.py
--rw-rw-rw-   0        0        0      504 2024-04-30 07:56:31.000000 zfx-1.0.8/zfx/算数_四舍五入.py
--rw-rw-rw-   0        0        0      547 2024-04-30 08:32:05.000000 zfx-1.0.8/zfx/算数_求余弦.py
--rw-rw-rw-   0        0        0      201 2024-04-30 08:01:08.000000 zfx-1.0.8/zfx/算数_求余数.py
--rw-rw-rw-   0        0        0      580 2024-04-30 08:35:24.000000 zfx-1.0.8/zfx/算数_求反正切.py
--rw-rw-rw-   0        0        0      370 2024-04-30 08:23:32.000000 zfx-1.0.8/zfx/算数_求平方根.py
--rw-rw-rw-   0        0        0      437 2024-04-30 08:20:33.000000 zfx-1.0.8/zfx/算数_求次方.py
--rw-rw-rw-   0        0        0      547 2024-04-30 08:33:35.000000 zfx-1.0.8/zfx/算数_求正切.py
--rw-rw-rw-   0        0        0      540 2024-04-30 08:29:45.000000 zfx-1.0.8/zfx/算数_求正弦.py
--rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.8/zfx/系统_取CPU型号.py
--rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.8/zfx/系统_取剪辑版内容.py
--rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.8/zfx/系统_取操作系统类别.py
--rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.8/zfx/系统_取时区.py
--rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.8/zfx/系统_取用户名.py
--rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.8/zfx/系统_取硬盘特征字.py
--rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.8/zfx/系统_取系统现行时间.py
--rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.8/zfx/系统_强制关机.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.8/zfx/系统_强制注销.py
--rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.8/zfx/系统_强制重启.py
--rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.8/zfx/系统_是否为管理员.py
--rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.8/zfx/系统_是否已联网.py
--rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.8/zfx/系统_清空回收站.py
--rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.8/zfx/系统_置剪辑版内容.py
--rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.8/zfx/系统任务计划_创建.py
--rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.8/zfx/系统任务计划_删除.py
--rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.8/zfx/系统任务计划_遍历名称.py
--rw-rw-rw-   0        0        0      384 2024-04-30 06:40:31.000000 zfx-1.0.8/zfx/编码_十六进制文本到字符串.py
--rw-rw-rw-   0        0        0      375 2024-04-30 06:40:31.000000 zfx-1.0.8/zfx/编码_字符串到十六进制文本.py
--rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.8/zfx/进程_名取ID.py
-drwxrwxrwx   0        0        0        0 2024-04-30 08:36:07.438491 zfx-1.0.8/zfx.egg-info/
--rw-rw-rw-   0        0        0      233 2024-04-30 08:36:07.000000 zfx-1.0.8/zfx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2024-04-30 08:36:07.000000 zfx-1.0.8/zfx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 08:36:07.000000 zfx-1.0.8/zfx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-04-30 08:36:07.000000 zfx-1.0.8/zfx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-30 08:36:07.000000 zfx-1.0.8/zfx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 09:50:04.970443 zfx-1.0.9/
+-rw-rw-rw-   0        0        0      233 2024-04-30 09:50:04.967466 zfx-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-30 09:50:04.970443 zfx-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      511 2024-04-30 09:50:01.000000 zfx-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:50:04.956468 zfx-1.0.9/zfx/
+-rw-rw-rw-   0        0        0     3677 2024-04-30 09:49:14.000000 zfx-1.0.9/zfx/__init__.py
+-rw-rw-rw-   0        0        0     1711 2024-04-30 03:32:01.000000 zfx-1.0.9/zfx/g2g_account_list.py
+-rw-rw-rw-   0        0        0     2105 2024-04-30 03:32:10.000000 zfx-1.0.9/zfx/g2g_account_list_s.py
+-rw-rw-rw-   0        0        0    10990 2024-04-23 06:27:52.000000 zfx-1.0.9/zfx/zmodule_240414A.py
+-rw-rw-rw-   0        0        0      905 2024-04-30 07:38:51.000000 zfx-1.0.9/zfx/zprint.py
+-rw-rw-rw-   0        0        0      980 2024-04-30 09:49:14.000000 zfx-1.0.9/zfx/文本文件_写入文件内容.py
+-rw-rw-rw-   0        0        0      565 2024-04-30 09:49:14.000000 zfx-1.0.9/zfx/文本文件_取指定文件文本行数.py
+-rw-rw-rw-   0        0        0      923 2024-04-30 09:46:31.000000 zfx-1.0.9/zfx/文本文件_读入全部内容.py
+-rw-rw-rw-   0        0        0      364 2024-04-30 05:26:52.000000 zfx-1.0.9/zfx/目录_创建.py
+-rw-rw-rw-   0        0        0      245 2024-04-30 08:17:43.000000 zfx-1.0.9/zfx/算数_保留小数点后指定位数.py
+-rw-rw-rw-   0        0        0      239 2024-04-30 07:53:10.000000 zfx-1.0.9/zfx/算数_取绝对值.py
+-rw-rw-rw-   0        0        0      191 2024-04-30 08:11:28.000000 zfx-1.0.9/zfx/算数_向上取整.py
+-rw-rw-rw-   0        0        0      210 2024-04-30 08:14:48.000000 zfx-1.0.9/zfx/算数_向下取整.py
+-rw-rw-rw-   0        0        0      504 2024-04-30 07:56:31.000000 zfx-1.0.9/zfx/算数_四舍五入.py
+-rw-rw-rw-   0        0        0      547 2024-04-30 08:32:05.000000 zfx-1.0.9/zfx/算数_求余弦.py
+-rw-rw-rw-   0        0        0      201 2024-04-30 08:01:08.000000 zfx-1.0.9/zfx/算数_求余数.py
+-rw-rw-rw-   0        0        0      580 2024-04-30 08:35:24.000000 zfx-1.0.9/zfx/算数_求反正切.py
+-rw-rw-rw-   0        0        0      370 2024-04-30 08:23:32.000000 zfx-1.0.9/zfx/算数_求平方根.py
+-rw-rw-rw-   0        0        0      437 2024-04-30 08:20:33.000000 zfx-1.0.9/zfx/算数_求次方.py
+-rw-rw-rw-   0        0        0      547 2024-04-30 08:33:35.000000 zfx-1.0.9/zfx/算数_求正切.py
+-rw-rw-rw-   0        0        0      540 2024-04-30 08:29:45.000000 zfx-1.0.9/zfx/算数_求正弦.py
+-rw-rw-rw-   0        0        0      273 2024-04-30 03:09:39.000000 zfx-1.0.9/zfx/系统_取CPU型号.py
+-rw-rw-rw-   0        0        0      225 2024-04-30 03:04:34.000000 zfx-1.0.9/zfx/系统_取剪辑版内容.py
+-rw-rw-rw-   0        0        0     1316 2024-04-30 04:11:09.000000 zfx-1.0.9/zfx/系统_取操作系统类别.py
+-rw-rw-rw-   0        0        0      588 2024-04-30 04:17:38.000000 zfx-1.0.9/zfx/系统_取时区.py
+-rw-rw-rw-   0        0        0      433 2024-04-30 04:34:35.000000 zfx-1.0.9/zfx/系统_取用户名.py
+-rw-rw-rw-   0        0        0      787 2024-04-30 04:25:33.000000 zfx-1.0.9/zfx/系统_取硬盘特征字.py
+-rw-rw-rw-   0        0        0      263 2024-04-30 03:13:42.000000 zfx-1.0.9/zfx/系统_取系统现行时间.py
+-rw-rw-rw-   0        0        0      154 2024-04-30 03:44:02.000000 zfx-1.0.9/zfx/系统_强制关机.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:48:40.000000 zfx-1.0.9/zfx/系统_强制注销.py
+-rw-rw-rw-   0        0        0      240 2024-04-30 03:47:12.000000 zfx-1.0.9/zfx/系统_强制重启.py
+-rw-rw-rw-   0        0        0      454 2024-04-30 04:38:22.000000 zfx-1.0.9/zfx/系统_是否为管理员.py
+-rw-rw-rw-   0        0        0      697 2024-04-30 04:43:28.000000 zfx-1.0.9/zfx/系统_是否已联网.py
+-rw-rw-rw-   0        0        0      487 2024-04-30 04:04:45.000000 zfx-1.0.9/zfx/系统_清空回收站.py
+-rw-rw-rw-   0        0        0      175 2024-04-30 03:04:01.000000 zfx-1.0.9/zfx/系统_置剪辑版内容.py
+-rw-rw-rw-   0        0        0     3299 2024-04-25 02:56:01.000000 zfx-1.0.9/zfx/系统任务计划_创建.py
+-rw-rw-rw-   0        0        0      267 2024-04-25 02:26:25.000000 zfx-1.0.9/zfx/系统任务计划_删除.py
+-rw-rw-rw-   0        0        0      665 2024-04-25 02:26:25.000000 zfx-1.0.9/zfx/系统任务计划_遍历名称.py
+-rw-rw-rw-   0        0        0      384 2024-04-30 06:40:31.000000 zfx-1.0.9/zfx/编码_十六进制文本到字符串.py
+-rw-rw-rw-   0        0        0      375 2024-04-30 06:40:31.000000 zfx-1.0.9/zfx/编码_字符串到十六进制文本.py
+-rw-rw-rw-   0        0        0      494 2024-04-30 05:31:14.000000 zfx-1.0.9/zfx/进程_名取ID.py
+drwxrwxrwx   0        0        0        0 2024-04-30 09:50:04.966451 zfx-1.0.9/zfx.egg-info/
+-rw-rw-rw-   0        0        0      233 2024-04-30 09:50:04.000000 zfx-1.0.9/zfx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1360 2024-04-30 09:50:04.000000 zfx-1.0.9/zfx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 09:50:04.000000 zfx-1.0.9/zfx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-30 09:50:04.000000 zfx-1.0.9/zfx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-30 09:50:04.000000 zfx-1.0.9/zfx.egg-info/top_level.txt
```

### Comparing `zfx-1.0.8/zfx/__init__.py` & `zfx-1.0.9/zfx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 from zfx.zmodule_240414A import 文本_取长度
 from zfx.zmodule_240414A import 文本_取指定变量文本行
 from zfx.zmodule_240414A import 文本_取左边
 from zfx.zmodule_240414A import 文本_替换行内容
 from zfx.zmodule_240414A import 文本区分_只取符号
 from zfx.zmodule_240414A import 文本区分_只取汉字
 from zfx.zmodule_240414A import 文本区分_只取数字
+from zfx.文本文件_读入全部内容 import 文本文件_读入全部内容
+from zfx.文本文件_取指定文件文本行数 import 文本文件_取指定文件文本行数
+from zfx.文本文件_写入文件内容 import 文本文件_写入文件内容
 from zfx.目录_创建 import 目录_创建
 from zfx.算数_保留小数点后指定位数 import 算数_保留小数点后指定位数
 from zfx.算数_取绝对值 import 算数_取绝对值
 from zfx.算数_向上取整 import 算数_向上取整
 from zfx.算数_向下取整 import 算数_向下取整
 from zfx.算数_四舍五入 import 算数_四舍五入
 from zfx.算数_求余弦 import 算数_求余弦
```

### Comparing `zfx-1.0.8/zfx/g2g_account_list.py` & `zfx-1.0.9/zfx/g2g_account_list.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/g2g_account_list_s.py` & `zfx-1.0.9/zfx/g2g_account_list_s.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/zmodule_240414A.py` & `zfx-1.0.9/zfx/zmodule_240414A.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/zprint.py` & `zfx-1.0.9/zfx/zprint.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/算数_求余弦.py` & `zfx-1.0.9/zfx/算数_求余弦.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/算数_求反正切.py` & `zfx-1.0.9/zfx/算数_求反正切.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/算数_求正切.py` & `zfx-1.0.9/zfx/算数_求正切.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/算数_求正弦.py` & `zfx-1.0.9/zfx/算数_求正弦.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统_取操作系统类别.py` & `zfx-1.0.9/zfx/系统_取操作系统类别.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统_取时区.py` & `zfx-1.0.9/zfx/系统_取时区.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统_取硬盘特征字.py` & `zfx-1.0.9/zfx/系统_取硬盘特征字.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统_是否已联网.py` & `zfx-1.0.9/zfx/系统_是否已联网.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统任务计划_创建.py` & `zfx-1.0.9/zfx/系统任务计划_创建.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx/系统任务计划_遍历名称.py` & `zfx-1.0.9/zfx/系统任务计划_遍历名称.py`

 * *Files identical despite different names*

### Comparing `zfx-1.0.8/zfx.egg-info/SOURCES.txt` & `zfx-1.0.9/zfx.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 setup.py
 zfx/__init__.py
 zfx/g2g_account_list.py
 zfx/g2g_account_list_s.py
 zfx/zmodule_240414A.py
 zfx/zprint.py
+zfx/文本文件_写入文件内容.py
+zfx/文本文件_取指定文件文本行数.py
+zfx/文本文件_读入全部内容.py
 zfx/目录_创建.py
 zfx/算数_保留小数点后指定位数.py
 zfx/算数_取绝对值.py
 zfx/算数_向上取整.py
 zfx/算数_向下取整.py
 zfx/算数_四舍五入.py
 zfx/算数_求余弦.py
```

