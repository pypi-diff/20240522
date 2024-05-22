# Comparing `tmp/sklearnpro-0.1.0.tar.gz` & `tmp/sklearnpro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearnpro-0.1.0.tar", last modified: Wed May 22 02:38:02 2024, max compression
+gzip compressed data, was "sklearnpro-0.1.1.tar", last modified: Wed May 22 07:19:33 2024, max compression
```

## Comparing `sklearnpro-0.1.0.tar` & `sklearnpro-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 02:38:02.708574 sklearnpro-0.1.0/
--rw-rw-rw-   0        0        0     1094 2024-03-06 01:18:14.000000 sklearnpro-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      411 2024-05-22 02:38:02.705607 sklearnpro-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        5 2024-03-06 01:31:44.000000 sklearnpro-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 02:38:02.708574 sklearnpro-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1248 2024-05-22 02:37:10.000000 sklearnpro-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:38:02.689988 sklearnpro-0.1.0/sklearnPro/
--rw-rw-rw-   0        0        0     1257 2024-05-22 02:36:00.000000 sklearnpro-0.1.0/sklearnPro/Bot.py
--rw-rw-rw-   0        0        0        0 2024-03-06 01:38:12.000000 sklearnpro-0.1.0/sklearnPro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:38:02.703613 sklearnpro-0.1.0/sklearnPro.egg-info/
--rw-rw-rw-   0        0        0      411 2024-05-22 02:38:02.000000 sklearnpro-0.1.0/sklearnPro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-22 02:38:02.000000 sklearnpro-0.1.0/sklearnPro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 02:38:02.000000 sklearnpro-0.1.0/sklearnPro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-22 02:38:02.000000 sklearnpro-0.1.0/sklearnPro.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-22 02:38:02.000000 sklearnpro-0.1.0/sklearnPro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 07:19:33.940353 sklearnpro-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2024-03-06 01:18:14.000000 sklearnpro-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      411 2024-05-22 07:19:33.938358 sklearnpro-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2024-03-06 01:31:44.000000 sklearnpro-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:19:33.940353 sklearnpro-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2024-05-22 07:19:14.000000 sklearnpro-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:19:33.930380 sklearnpro-0.1.1/sklearnPro/
+-rw-rw-rw-   0        0        0     1519 2024-05-22 07:18:47.000000 sklearnpro-0.1.1/sklearnPro/Bot.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 01:38:12.000000 sklearnpro-0.1.1/sklearnPro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:19:33.937361 sklearnpro-0.1.1/sklearnPro.egg-info/
+-rw-rw-rw-   0        0        0      411 2024-05-22 07:19:33.000000 sklearnpro-0.1.1/sklearnPro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-22 07:19:33.000000 sklearnpro-0.1.1/sklearnPro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:19:33.000000 sklearnpro-0.1.1/sklearnPro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-22 07:19:33.000000 sklearnpro-0.1.1/sklearnPro.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 07:19:33.000000 sklearnpro-0.1.1/sklearnPro.egg-info/top_level.txt
```

### Comparing `sklearnpro-0.1.0/LICENSE` & `sklearnpro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearnpro-0.1.0/setup.py` & `sklearnpro-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sklearnPro",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.1.0",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
+    version="0.1.1",  # 包版本号，便于维护版本,保证每次发布都是版本都是唯一的
     author="高手",  # 作者，可以写自己的姓名
     author_email="111@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="A small example package",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="https://github.com/",  # 自己项目地址，比如github的项目地址
     packages=setuptools.find_packages(),
```

### Comparing `sklearnpro-0.1.0/sklearnPro/Bot.py` & `sklearnpro-0.1.1/sklearnPro/Bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,22 @@
     spark_api_key=SPARKAI_API_KEY,
     spark_api_secret=SPARKAI_API_SECRET,
     spark_llm_domain=SPARKAI_DOMAIN,
     streaming=False,
 )
 
 if __name__ == '__main__':
+    messages = []
     while True:
         txt = input(":")
-        messages = [ChatMessage(
-            role="user",
-            content = txt
-        )]
-        handler = ChunkPrintHandler()
-        a = spark.generate([messages], callbacks=[handler])
-        print(a)
+        if txt != "":
+            messages.append(ChatMessage(
+                role="user",
+                content = txt
+            ))
+            handler = ChunkPrintHandler()
+            a = spark.generate([messages], callbacks=[handler])
+            messages.append(ChatMessage(
+                role="assistant",
+                content=a.generations[0][0].message.content
+            ))
+            print(a.generations[0][0].message.content)
```

