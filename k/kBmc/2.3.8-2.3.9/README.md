# Comparing `tmp/kBmc-2.3.8.tar.gz` & `tmp/kBmc-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kBmc-2.3.8.tar", last modified: Fri Apr  5 13:55:11 2024, max compression
+gzip compressed data, was "kBmc-2.3.9.tar", last modified: Tue Apr  9 05:05:47 2024, max compression
```

## Comparing `kBmc-2.3.8.tar` & `kBmc-2.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.666340 kBmc-2.3.8/
--rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.8/LICENSE
--rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-04-05 13:55:11.666340 kBmc-2.3.8/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.8/README.md
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.664339 kBmc-2.3.8/kBmc/
--rw-r--r--   0 kage      (1000) kage      (1000)   208397 2024-04-04 05:46:06.000000 kBmc-2.3.8/kBmc/__init__.py
-drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-05 13:55:11.665340 kBmc-2.3.8/kBmc.egg-info/
--rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/PKG-INFO
--rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/SOURCES.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/dependency_links.txt
--rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-04-05 13:55:11.000000 kBmc-2.3.8/kBmc.egg-info/top_level.txt
--rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-04-05 13:55:11.666340 kBmc-2.3.8/setup.cfg
--rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.8/setup.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-09 05:05:47.622831 kBmc-2.3.9/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1066 2021-12-17 05:54:12.000000 kBmc-2.3.9/LICENSE
+-rw-r--r--   0 kage      (1000) kage      (1000)     2875 2024-04-09 05:05:47.622831 kBmc-2.3.9/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2457 2021-12-19 02:10:48.000000 kBmc-2.3.9/README.md
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-09 05:05:47.621831 kBmc-2.3.9/kBmc/
+-rw-r--r--   0 kage      (1000) kage      (1000)   208622 2024-04-09 05:04:51.000000 kBmc-2.3.9/kBmc/__init__.py
+drwxr-xr-x   0 kage      (1000) kage      (1000)        0 2024-04-09 05:05:47.622831 kBmc-2.3.9/kBmc.egg-info/
+-rw-rw-r--   0 kage      (1000) kage      (1000)     2875 2024-04-09 05:05:47.000000 kBmc-2.3.9/kBmc.egg-info/PKG-INFO
+-rw-rw-r--   0 kage      (1000) kage      (1000)      155 2024-04-09 05:05:47.000000 kBmc-2.3.9/kBmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        1 2024-04-09 05:05:47.000000 kBmc-2.3.9/kBmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kage      (1000) kage      (1000)        5 2024-04-09 05:05:47.000000 kBmc-2.3.9/kBmc.egg-info/top_level.txt
+-rw-r--r--   0 kage      (1000) kage      (1000)       38 2024-04-09 05:05:47.622831 kBmc-2.3.9/setup.cfg
+-rw-rw-r--   0 kage      (1000) kage      (1000)     1975 2021-12-17 05:56:02.000000 kBmc-2.3.9/setup.py
```

### Comparing `kBmc-2.3.8/LICENSE` & `kBmc-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.8/PKG-INFO` & `kBmc-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.8
+Version: 2.3.9
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.8/README.md` & `kBmc-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `kBmc-2.3.8/kBmc/__init__.py` & `kBmc-2.3.9/kBmc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2105,16 +2105,21 @@
     def find_user_pass(self,ip=None,default_range=12,check_cmd='ipmi power status',cancel_func=None,error=True,trace=False,extra_test_user=[],extra_test_pass=[],no_redfish=False,first_user=None,first_passwd=None,failed_passwd=None):
         # Check Network
         chk_err=self.error(_type='net')
         if chk_err[0]: return False,None,None
         if cancel_func is None: cancel_func=self.cancel_func
         if ip is None: ip=self.ip
         if not IpV4(ip): return False,None,None
-        test_user=MoveData(self.test_user[:],self.user,to='first')
-        if not test_user: test_user=['ADMIN']
+        test_user=None
+        if self.test_user:
+            if isinstance(self.test_user,list):
+                test_user=MoveData(self.test_user[:],self.user,to='first')
+            elif isinstance(self.test_user,str):
+                test_user=[self.user,self.test_user]
+        if not isinstance(test_user,list): test_user=['ADMIN']
         if 'ADMIN' not in test_user: test_user=['ADMIN']+test_user
         if isinstance(first_user,str) and first_user: test_user=MoveData(test_user[:],first_user,to='first')
         if extra_test_user and isinstance(extra_test_user,list):
             for i in Iterable(extra_test_user):
                 if i not in test_user: test_user.append(i)
         test_passwd=self.test_passwd[:]
         if 'ADMIN' in test_passwd:
```

### Comparing `kBmc-2.3.8/kBmc.egg-info/PKG-INFO` & `kBmc-2.3.9/kBmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kBmc
-Version: 2.3.8
+Version: 2.3.9
 Summary: Kage's Intelgent BMC handler
 Home-page: https://github.com/kagepark/kBmc
 Author: Kage Park
 License: MIT
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `kBmc-2.3.8/setup.py` & `kBmc-2.3.9/setup.py`

 * *Files identical despite different names*

