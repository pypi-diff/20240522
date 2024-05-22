# Comparing `tmp/lambkid-0.2.5.tar.gz` & `tmp/lambkid-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.2.5.tar", last modified: Wed May 22 02:41:13 2024, max compression
+gzip compressed data, was "lambkid-0.2.6.tar", last modified: Wed May 22 02:45:36 2024, max compression
```

## Comparing `lambkid-0.2.5.tar` & `lambkid-0.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:13.968567 lambkid-0.2.5/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.5/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-05-22 02:41:13.966574 lambkid-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:13.886786 lambkid-0.2.5/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.5/docs/cli.md
--rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.5/docs/csv.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.5/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.5/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.5/docs/sshclient.md
--rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.5/docs/utils.md
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:13.890776 lambkid-0.2.5/lambkid/
--rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.5/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.5/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:13.942636 lambkid-0.2.5/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.5/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1516 2024-05-22 02:39:43.000000 lambkid-0.2.5/lambkid/libs/log.py
--rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.5/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     9707 2024-05-20 03:26:20.000000 lambkid-0.2.5/lambkid/libs/ssh.py
--rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.5/lambkid/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:41:13.954604 lambkid-0.2.5/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 02:41:13.000000 lambkid-0.2.5/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 02:41:13.968567 lambkid-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-22 02:40:36.000000 lambkid-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:45:36.582371 lambkid-0.2.6/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-22 02:45:36.581374 lambkid-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 02:45:36.550456 lambkid-0.2.6/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.6/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.6/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.6/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.6/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.6/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.6/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-22 02:45:36.552451 lambkid-0.2.6/lambkid/
+-rw-rw-rw-   0        0        0      154 2024-05-22 02:45:09.000000 lambkid-0.2.6/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.6/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:45:36.579379 lambkid-0.2.6/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.6/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1516 2024-05-22 02:39:43.000000 lambkid-0.2.6/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1825 2024-05-17 02:16:37.000000 lambkid-0.2.6/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     9707 2024-05-20 03:26:20.000000 lambkid-0.2.6/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.6/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 02:45:36.580376 lambkid-0.2.6/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 02:45:36.000000 lambkid-0.2.6/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 02:45:36.583368 lambkid-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-22 02:45:16.000000 lambkid-0.2.6/setup.py
```

### Comparing `lambkid-0.2.5/LICENSE` & `lambkid-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/PKG-INFO` & `lambkid-0.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.5
+Version: 0.2.6
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.5/README.md` & `lambkid-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/docs/log.md` & `lambkid-0.2.6/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/docs/sshclient.md` & `lambkid-0.2.6/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid/cli.py` & `lambkid-0.2.6/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid/libs/log.py` & `lambkid-0.2.6/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid/libs/minio_client.py` & `lambkid-0.2.6/lambkid/libs/minio_client.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid/libs/ssh.py` & `lambkid-0.2.6/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid/libs/utils.py` & `lambkid-0.2.6/lambkid/libs/utils.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.5/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.6/lambkid.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.5
+Version: 0.2.6
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.5/setup.py` & `lambkid-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.2.5",
+    version="0.2.6",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

