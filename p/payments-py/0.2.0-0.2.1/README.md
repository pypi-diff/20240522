# Comparing `tmp/payments_py-0.2.0.tar.gz` & `tmp/payments_py-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payments_py-0.2.0.tar", max compression
+gzip compressed data, was "payments_py-0.2.1.tar", max compression
```

## Comparing `payments_py-0.2.0.tar` & `payments_py-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-05-17 15:37:06.055850 payments_py-0.2.0/LICENSE
--rw-r--r--   0        0        0      502 2024-05-17 15:37:06.055850 payments_py-0.2.0/README.md
--rw-r--r--   0        0        0      159 2024-05-17 15:37:06.055850 payments_py-0.2.0/payments_py/__init__.py
--rw-r--r--   0        0        0     1081 2024-05-17 15:37:06.055850 payments_py-0.2.0/payments_py/environments.py
--rw-r--r--   0        0        0    15425 2024-05-17 15:37:06.055850 payments_py-0.2.0/payments_py/payments.py
--rw-r--r--   0        0        0      229 2024-05-17 15:37:06.059850 payments_py-0.2.0/payments_py/utils.py
--rw-r--r--   0        0        0      496 2024-05-17 15:37:06.059850 payments_py-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 payments_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 10:00:46.333537 payments_py-0.2.1/LICENSE
+-rw-r--r--   0        0        0      502 2024-05-22 10:00:46.333537 payments_py-0.2.1/README.md
+-rw-r--r--   0        0        0      159 2024-05-22 10:00:46.333537 payments_py-0.2.1/payments_py/__init__.py
+-rw-r--r--   0        0        0     1081 2024-05-22 10:00:46.333537 payments_py-0.2.1/payments_py/environments.py
+-rw-r--r--   0        0        0    15484 2024-05-22 10:00:46.333537 payments_py-0.2.1/payments_py/payments.py
+-rw-r--r--   0        0        0      229 2024-05-22 10:00:46.333537 payments_py-0.2.1/payments_py/utils.py
+-rw-r--r--   0        0        0      496 2024-05-22 10:00:46.333537 payments_py-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 payments_py-0.2.1/PKG-INFO
```

### Comparing `payments_py-0.2.0/LICENSE` & `payments_py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `payments_py-0.2.0/payments_py/environments.py` & `payments_py-0.2.1/payments_py/environments.py`

 * *Files identical despite different names*

### Comparing `payments_py-0.2.0/payments_py/payments.py` & `payments_py-0.2.1/payments_py/payments.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,16 @@
             Response: The response from the API call.
         """
         body = {
             **{snake_to_camel(k): v for k, v in locals().items() if v is not None and k != 'self'}
         }
         headers = {
             'Accept': 'application/json',
-            'Content-Type': 'application/json'
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.nvm_api_key}'
         }
         url = (f"{self.environment.value['backend']}/api/v1/payments/subscription/balance")
         response = requests.post(url, headers=headers, json=body)
         return response
 
     def get_service_token(self, service_did: str):
         """
```

### Comparing `payments_py-0.2.0/PKG-INFO` & `payments_py-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: payments-py
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: enrique
 Author-email: enrique@nevermined.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

