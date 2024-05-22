# Comparing `tmp/zcbot-shop-parser-1.0.7.tar.gz` & `tmp/zcbot-shop-parser-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zcbot-shop-parser-1.0.7.tar", last modified: Mon Mar 18 08:23:21 2024, max compression
+gzip compressed data, was "zcbot-shop-parser-1.0.8.tar", last modified: Mon Mar 18 10:25:10 2024, max compression
```

## Comparing `zcbot-shop-parser-1.0.7.tar` & `zcbot-shop-parser-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.021398 zcbot-shop-parser-1.0.7/
--rw-rw-rw-   0        0        0        0 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2024-03-18 08:23:21.021398 zcbot-shop-parser-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      140 2023-10-27 02:13:50.000000 zcbot-shop-parser-1.0.7/README.rst
--rw-rw-rw-   0        0        0       42 2024-03-18 08:23:21.022398 zcbot-shop-parser-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      586 2024-03-18 08:23:04.000000 zcbot-shop-parser-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.008398 zcbot-shop-parser-1.0.7/zcbot_shop_parser/
--rw-rw-rw-   0        0        0       40 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.015398 zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/
--rw-rw-rw-   0        0        0        0 2023-11-01 03:03:33.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/__init__.py
--rw-rw-rw-   0        0        0     1237 2023-11-28 08:49:30.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/model.py
--rw-rw-rw-   0        0        0     3832 2024-03-18 08:21:48.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/parser.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.017398 zcbot-shop-parser-1.0.7/zcbot_shop_parser/core/
--rw-rw-rw-   0        0        0        0 2023-11-01 03:06:05.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/core/__init__.py
--rw-rw-rw-   0        0        0      407 2023-11-01 03:08:57.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/core/model.py
--rw-rw-rw-   0        0        0     2406 2023-10-27 02:07:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/model.py
--rw-rw-rw-   0        0        0     1140 2023-11-01 07:44:05.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/parser.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.020398 zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/
--rw-rw-rw-   0        0        0        0 2023-11-01 03:03:17.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/__init__.py
--rw-rw-rw-   0        0        0     2010 2023-11-01 03:16:29.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/model.py
--rw-rw-rw-   0        0        0     3707 2023-11-01 07:36:07.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/parser.py
--rw-rw-rw-   0        0        0      618 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-18 08:23:21.012397 zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/
--rw-rw-rw-   0        0        0      390 2024-03-18 08:23:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      589 2024-03-18 08:23:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 08:23:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-03-18 08:23:20.000000 zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.161981 zcbot-shop-parser-1.0.8/
+-rw-rw-rw-   0        0        0        0 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2024-03-18 10:25:10.160981 zcbot-shop-parser-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-10-27 02:13:50.000000 zcbot-shop-parser-1.0.8/README.rst
+-rw-rw-rw-   0        0        0       42 2024-03-18 10:25:10.161981 zcbot-shop-parser-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      586 2024-03-18 10:24:51.000000 zcbot-shop-parser-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.146981 zcbot-shop-parser-1.0.8/zcbot_shop_parser/
+-rw-rw-rw-   0        0        0       40 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.154981 zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/
+-rw-rw-rw-   0        0        0        0 2023-11-01 03:03:33.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/__init__.py
+-rw-rw-rw-   0        0        0     1237 2023-11-28 08:49:30.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/model.py
+-rw-rw-rw-   0        0        0     3832 2024-03-18 10:24:29.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/parser.py
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.156981 zcbot-shop-parser-1.0.8/zcbot_shop_parser/core/
+-rw-rw-rw-   0        0        0        0 2023-11-01 03:06:05.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/core/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-11-01 03:08:57.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/core/model.py
+-rw-rw-rw-   0        0        0     2406 2023-10-27 02:07:20.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/model.py
+-rw-rw-rw-   0        0        0     1140 2023-11-01 07:44:05.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/parser.py
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.159981 zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/
+-rw-rw-rw-   0        0        0        0 2023-11-01 03:03:17.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/__init__.py
+-rw-rw-rw-   0        0        0     2010 2023-11-01 03:16:29.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/model.py
+-rw-rw-rw-   0        0        0     3707 2023-11-01 07:36:07.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/parser.py
+-rw-rw-rw-   0        0        0      618 2023-10-26 09:04:20.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-18 10:25:10.150981 zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/
+-rw-rw-rw-   0        0        0      390 2024-03-18 10:25:10.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2024-03-18 10:25:10.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 10:25:10.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-03-18 10:25:10.000000 zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/top_level.txt
```

### Comparing `zcbot-shop-parser-1.0.7/setup.py` & `zcbot-shop-parser-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(name='zcbot-shop-parser',
-      version='1.0.7',
+      version='1.0.8',
       description='zcbot shop parser for zsodata',
       long_description=long_description,
       author='zsodata',
       author_email='team@zso.io',
       url='http://www.zsodata.com',
       install_requires=[],
       python_requires='>=3.7',
```

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/model.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/common/parser.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/common/parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,24 +25,25 @@
                 if "自营" in shop_name and "企业购" in shop_name:
                     _shop_type = "自营企业购"
                 elif "旗舰店" in shop_name and "自营" not in shop_name:
                     _shop_type = "非自营旗舰店"
                 elif "专营店" in shop_name:
                     _shop_type = "专营店"
 
-                elif not brand_name:
-                    _shop_type = "其他"
-
                 elif "自营" in shop_name:
                     if brand_name and brand_name in shop_name:
                         _shop_type = "自营品牌旗舰店"
                     elif "旗舰" in shop_name:
                         _shop_type = "自营旗舰店"
                     else:
                         _shop_type = "自营非旗舰店"
+
+                elif not brand_name:
+                    _shop_type = "其他"
+
                 shop_model = self.build_model(plat_code=plat_code, shop_name=shop_name, shop_type=_shop_type)
         elif plat_code == "tmall":
             if shop_name in ["天猫超市"]:
                 _shop_type = "自营"
                 _is_self = "是"
             else:
                 _shop_type = "非自营"
@@ -94,8 +95,7 @@
                 shop_model.shop_type_name = ShopTypeSeven.TYPE_8.value
 
             elif is_self == "否":
                 shop_model.shop_type_code = ShopTypeSeven.TYPE_9.name
                 shop_model.shop_type_name = ShopTypeSeven.TYPE_9.value
 
             return shop_model
-
```

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/model.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/parser.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/parser.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/model.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/model.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/staples/parser.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/staples/parser.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser/utils.py` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser/utils.py`

 * *Files identical despite different names*

### Comparing `zcbot-shop-parser-1.0.7/zcbot_shop_parser.egg-info/SOURCES.txt` & `zcbot-shop-parser-1.0.8/zcbot_shop_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

