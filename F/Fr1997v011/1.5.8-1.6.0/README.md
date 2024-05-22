# Comparing `tmp/Fr1997v011-1.5.8.tar.gz` & `tmp/Fr1997v011-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.5.8.tar", last modified: Tue May 21 11:21:26 2024, max compression
+gzip compressed data, was "Fr1997v011-1.6.0.tar", last modified: Wed May 22 03:53:05 2024, max compression
```

## Comparing `Fr1997v011-1.5.8.tar` & `Fr1997v011-1.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.392385 Fr1997v011-1.5.8/
-drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.384378 Fr1997v011-1.5.8/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-21 11:21:26.000000 Fr1997v011-1.5.8/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.5.8/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-21 11:21:26.391384 Fr1997v011-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-17 03:42:08.000000 Fr1997v011-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.386389 Fr1997v011-1.5.8/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.5.8/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.388385 Fr1997v011-1.5.8/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.5.8/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   161603 2024-05-21 11:21:23.000000 Fr1997v011-1.5.8/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:21:26.390387 Fr1997v011-1.5.8/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.5.8/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-21 11:21:26.393384 Fr1997v011-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-21 11:21:23.000000 Fr1997v011-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:05.182770 Fr1997v011-1.6.0/
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:05.176770 Fr1997v011-1.6.0/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-22 03:53:05.000000 Fr1997v011-1.6.0/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-22 03:53:05.000000 Fr1997v011-1.6.0/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:53:05.000000 Fr1997v011-1.6.0/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 03:48:53.000000 Fr1997v011-1.6.0/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-22 03:53:05.000000 Fr1997v011-1.6.0/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-22 03:53:05.181772 Fr1997v011-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-22 03:51:13.000000 Fr1997v011-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:05.177787 Fr1997v011-1.6.0/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.0/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:05.179771 Fr1997v011-1.6.0/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.0/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   161601 2024-05-22 01:12:48.000000 Fr1997v011-1.6.0/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:05.180770 Fr1997v011-1.6.0/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.0/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:53:05.182770 Fr1997v011-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-22 03:48:50.000000 Fr1997v011-1.6.0/setup.py
```

### Comparing `Fr1997v011-1.5.8/LICENSE` & `Fr1997v011-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.5.8/README.md` & `Fr1997v011-1.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.5.7.tar.gz
+pip install dist/Fr1997v011-1.6.0.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.5.8/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.6.0/fr1997_mode/mode_func/all_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -4087,8 +4087,7 @@
 mode_xhs = XhsJike()  # douyin配置
 mode_pros = ModeStatic()  # 其它函数
 mode_cos = Cos()  # cos
 mode_fr_cos = Cos(server_select='personal')  # cos 高阳
 mode_myself = MyGy()
 
 mode_pro = ModeFunc()  # main
-
```

