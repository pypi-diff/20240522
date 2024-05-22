# Comparing `tmp/scrathon_payments-0.1.5.tar.gz` & `tmp/scrathon_payments-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrathon_payments-0.1.5.tar", last modified: Fri Apr 19 14:19:08 2024, max compression
+gzip compressed data, was "scrathon_payments-0.1.7.tar", last modified: Wed May 22 04:08:30 2024, max compression
```

## Comparing `scrathon_payments-0.1.5.tar` & `scrathon_payments-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:08.380488 scrathon_payments-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 14:19:04.000000 scrathon_payments-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-19 14:19:08.380488 scrathon_payments-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-19 14:19:04.000000 scrathon_payments-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:08.380488 scrathon_payments-0.1.5/ScrathonPayments/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-19 14:19:04.000000 scrathon_payments-0.1.5/ScrathonPayments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:19:08.380488 scrathon_payments-0.1.5/scrathon_payments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-19 14:19:08.000000 scrathon_payments-0.1.5/scrathon_payments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-19 14:19:08.000000 scrathon_payments-0.1.5/scrathon_payments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:19:08.000000 scrathon_payments-0.1.5/scrathon_payments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 14:19:08.000000 scrathon_payments-0.1.5/scrathon_payments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 14:19:08.000000 scrathon_payments-0.1.5/scrathon_payments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:19:08.380488 scrathon_payments-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-19 14:19:04.000000 scrathon_payments-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:08:30.394234 scrathon_payments-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 04:08:26.000000 scrathon_payments-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-22 04:08:30.394234 scrathon_payments-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-22 04:08:26.000000 scrathon_payments-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:08:30.390234 scrathon_payments-0.1.7/ScrathonPayments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-22 04:08:26.000000 scrathon_payments-0.1.7/ScrathonPayments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:08:30.394234 scrathon_payments-0.1.7/scrathon_payments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-22 04:08:30.000000 scrathon_payments-0.1.7/scrathon_payments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 04:08:30.000000 scrathon_payments-0.1.7/scrathon_payments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:08:30.000000 scrathon_payments-0.1.7/scrathon_payments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 04:08:30.000000 scrathon_payments-0.1.7/scrathon_payments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 04:08:30.000000 scrathon_payments-0.1.7/scrathon_payments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:08:30.394234 scrathon_payments-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 04:08:26.000000 scrathon_payments-0.1.7/setup.py
```

### Comparing `scrathon_payments-0.1.5/LICENSE` & `scrathon_payments-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.1.5/PKG-INFO` & `scrathon_payments-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.1.5
+Version: 0.1.7
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.1.5/README.md` & `scrathon_payments-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `scrathon_payments-0.1.5/ScrathonPayments/__init__.py` & `scrathon_payments-0.1.7/ScrathonPayments/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,34 +7,34 @@
         self.username = "None"
         try:
             scratch3.get_user(username)
             userexists = True
         except scratch3.exceptions.UserNotFound:
             userexists = False
         if userexists:
-            if requests.post("http://196.27.127.58:12211/userexist/", json={"username": username}).json == {"userexist": "True"}:
+            if requests.post("http://45.140.188.129:6623/userexist/", json={"username": username}).json == {"userexist": "True"}:
                 self.username = str(username)
             else:
                 print("User {} did not use Scrathon before!".format(username))
         else:
             print("User {} does not exist on scratch!".format(username))
 
         if self.username != "None":
             print("Started Scrathon as {}! All funds earned will go to mentioned user".format(self.username))
 
     def purchase(self, price, user):
-        request = requests.post("http://196.27.127.58:12211/transaction", json={
+        request = requests.post("http://45.140.188.129:6623//transaction", json={
             "price": price,
             "buyer": user,
             "seller": self.username
         })
 
         return request.json()
     
     def purchasecheck(self, price, user):
-        request = requests.post("http://196.27.127.58:12211/checkpurchase", json={
+        request = requests.post("http://45.140.188.129:6623//checkpurchase", json={
             "price": price,
             "buyer": user,
             "seller": self.username
         })
 
         return request.json()
```

### Comparing `scrathon_payments-0.1.5/scrathon_payments.egg-info/PKG-INFO` & `scrathon_payments-0.1.7/scrathon_payments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrathon-payments
-Version: 0.1.5
+Version: 0.1.7
 Summary: API Wrapper for ScrathonPayments
 Home-page: https://github.com/Ryan-shamu-YT/ScrathonPayments
 Author: Ryan_shamu
 Author-email: Ryanshamu418@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scrathon_payments-0.1.5/setup.py` & `scrathon_payments-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='scrathon-payments',
-    version='0.1.5',
+    version='0.1.7',
     author='Ryan_shamu',
     author_email='Ryanshamu418@gmail.com',
     description='API Wrapper for ScrathonPayments',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Ryan-shamu-YT/ScrathonPayments',
     packages=find_packages(exclude=[]),
```

