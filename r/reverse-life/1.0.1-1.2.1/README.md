# Comparing `tmp/reverse_life-1.0.1.tar.gz` & `tmp/reverse_life-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_life-1.0.1.tar", last modified: Mon May 20 01:39:50 2024, max compression
+gzip compressed data, was "reverse_life-1.2.1.tar", last modified: Wed May 22 02:17:08 2024, max compression
```

## Comparing `reverse_life-1.0.1.tar` & `reverse_life-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 01:39:50.369070 reverse_life-1.0.1/
--rw-rw-rw-   0        0        0     1085 2024-05-20 01:10:24.000000 reverse_life-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2914 2024-05-20 01:39:50.368283 reverse_life-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2024-05-20 01:37:16.000000 reverse_life-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 01:39:50.362670 reverse_life-1.0.1/reverse_life/
--rw-rw-rw-   0        0        0      128 2024-02-22 12:39:42.000000 reverse_life-1.0.1/reverse_life/__init__.py
--rw-rw-rw-   0        0        0     1679 2024-04-16 22:11:54.000000 reverse_life-1.0.1/reverse_life/reverse_oklink.py
--rw-rw-rw-   0        0        0     3648 2024-04-16 22:12:36.000000 reverse_life-1.0.1/reverse_life/reverse_sxfae.py
-drwxrwxrwx   0        0        0        0 2024-05-20 01:39:50.367770 reverse_life-1.0.1/reverse_life.egg-info/
--rw-rw-rw-   0        0        0     2914 2024-05-20 01:39:50.000000 reverse_life-1.0.1/reverse_life.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-20 01:39:50.000000 reverse_life-1.0.1/reverse_life.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 01:39:50.000000 reverse_life-1.0.1/reverse_life.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-20 01:39:50.000000 reverse_life-1.0.1/reverse_life.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 01:39:50.000000 reverse_life-1.0.1/reverse_life.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 01:39:50.369572 reverse_life-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1674 2024-05-20 01:39:10.000000 reverse_life-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:17:08.385651 reverse_life-1.2.1/
+-rw-rw-rw-   0        0        0     1085 2024-05-22 02:02:06.000000 reverse_life-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3620 2024-05-22 02:17:08.385651 reverse_life-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1891 2024-05-22 02:09:21.000000 reverse_life-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 02:17:08.380853 reverse_life-1.2.1/reverse-life/
+-rw-rw-rw-   0        0        0      128 2024-02-22 12:39:42.000000 reverse_life-1.2.1/reverse-life/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:17:08.382526 reverse_life-1.2.1/reverse-life/pjstealth/
+-rw-rw-rw-   0        0        0      108 2024-02-04 06:11:10.000000 reverse_life-1.2.1/reverse-life/pjstealth/__init__.py
+-rw-rw-rw-   0        0        0     7777 2024-02-04 06:11:10.000000 reverse_life-1.2.1/reverse-life/pjstealth/env_data.py
+-rw-rw-rw-   0        0        0     1347 2024-02-04 06:11:10.000000 reverse_life-1.2.1/reverse-life/pjstealth/pjstealth.py
+-rw-rw-rw-   0        0        0    16138 2024-02-04 06:11:10.000000 reverse_life-1.2.1/reverse-life/pjstealth/stealth.py
+-rw-rw-rw-   0        0        0     1679 2024-04-16 22:11:54.000000 reverse_life-1.2.1/reverse-life/reverse_oklink.py
+-rw-rw-rw-   0        0        0     3648 2024-04-16 22:12:36.000000 reverse_life-1.2.1/reverse-life/reverse_sxfae.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:17:08.385148 reverse_life-1.2.1/reverse_life.egg-info/
+-rw-rw-rw-   0        0        0     3620 2024-05-22 02:17:08.000000 reverse_life-1.2.1/reverse_life.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2024-05-22 02:17:08.000000 reverse_life-1.2.1/reverse_life.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 02:17:08.000000 reverse_life-1.2.1/reverse_life.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      325 2024-05-22 02:17:08.000000 reverse_life-1.2.1/reverse_life.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 02:17:08.000000 reverse_life-1.2.1/reverse_life.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 02:17:08.385651 reverse_life-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     2222 2024-05-22 02:16:39.000000 reverse_life-1.2.1/setup.py
```

### Comparing `reverse_life-1.0.1/LICENSE` & `reverse_life-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reverse_life-1.0.1/PKG-INFO` & `reverse_life-1.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: reverse_life
-Version: 1.0.1
-Summary: This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
-Home-page: https://github.com/yanjlee/reverse_life
-Author: yanjlee
-Author-email: yanjlee@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: faker
-Requires-Dist: execjs
-Requires-Dist: loguru
-Requires-Dist: base64
-Requires-Dist: hashlib
-Requires-Dist: Crypto
-
 
 # Web Reverse Engineering Project
 
 ## Introduction
 
 This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.
 
@@ -33,15 +13,15 @@
 
 ## Installation
 
 To use the resources of this project, you need to set up your development environment first. Below are the basic installation instructions:
 
 ```bash
 # Clone the repository
-git clone https://github.com/yanjlee/reverse_life.git
+git clone https://github.com/yanjlee/reverse-life.git
 
 # Enter the project directory
 cd your-repository-name
 
 # Install dependencies (if any)
 pip install -r requirements.txt
 ```
```

### Comparing `reverse_life-1.0.1/reverse_life/reverse_oklink.py` & `reverse_life-1.2.1/reverse-life/reverse_oklink.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.0.1/reverse_life/reverse_sxfae.py` & `reverse_life-1.2.1/reverse-life/reverse_sxfae.py`

 * *Files identical despite different names*

### Comparing `reverse_life-1.0.1/setup.py` & `reverse_life-1.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-# @Time    : 2024/4/17 01:12
 # @Name    : setup.py
 # @Author  : yanlee
 
-
-
 import setuptools
 import shutil
 
 # 删除dist/目录
 shutil.rmtree('dist', ignore_errors=True)
 
 setuptools.setup(
-    name="reverse_life",
-    version="1.0.1",
+    name="reverse-life",
+    version="1.2.1",
     author="yanjlee",
-    author_email="yanjlee@163.com",  # 作者邮箱
+    author_email="yanjlee@163.com", 
     description="This project is dedicated to sharing and teaching the fundamentals and techniques of web reverse engineering. Web reverse engineering involves analyzing how websites and web applications work, and cracking or modifying existing code to achieve specific objectives. This project includes a series of tutorials, practical tools, and case studies aimed at helping developers, security researchers, and enthusiasts understand how to effectively reverse engineer web technologies.",  # 模块简介
     install_requires=[
         'requests',
         'faker',
         'execjs',
         'loguru',
         'base64',
         'hashlib',
         'Crypto',
+        'pandas',
+        'fuzzywuzzy',
+        'httpx',
+        'Pillow',
+        'playwright',
+        'PyExecJS',
+        'redis',
+        'fastapi',
+        'uvicorn',
+        'APScheduler',
+        'beautifulsoup4',
+        'bs4',
+        'certifi',
+        'clickhouse-driver',
+        'curl-cffi',
+        'DrissionPage',
+        'fake-useragent',
+        'Flask',
+        'Flask-APScheduler',
+        'Flask-Cors',
+        'frida',
+        'gevent',
+        'httpx',
+        'Jinja2',
+        'langchain',
+        'langchain-community',
+        'langchain-core'
     ],
     long_description=open(r'readme.md', encoding='utf-8').read(),  # 读取readme自述文件
     long_description_content_type="text/markdown",
-    url="https://github.com/yanjlee/reverse_life",  # 模块github地址
+    url="https://github.com/yanjlee/reverse-life",  # 模块github地址
     packages=setuptools.find_packages(),     # 自动列出项目下的包
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",   # 开源许可证
         "Operating System :: OS Independent",      # 这里的定义是系统无关（全平台兼容），如果你的包只能在部分特定系统上运行，需要修改。
     ],
 )
```

