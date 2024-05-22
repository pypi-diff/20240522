# Comparing `tmp/sentinel_sdk-0.0.3.tar.gz` & `tmp/sentinel_sdk-0.0.4.tar.gz`

## Comparing `sentinel_sdk-0.0.3.tar` & `sentinel_sdk-0.0.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/sdk.py
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/types.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/__init__.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/deposit.py
--rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/node.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/plan.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/provider.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/session.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/subscription.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/modules/swap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/__init__.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/multiquerier.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/querier.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/deposit.py
--rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/node.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/plan.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/provider.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/session.py
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/subscription.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/swap.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/__init__.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/transactor.py
--rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/connect.py
--rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/connect.sdk.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/test/queryall.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/LICENSE
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/README.md
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/sdk.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/types.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/__init__.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/deposit.py
+-rw-r--r--   0        0        0     7949 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/node.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/plan.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/provider.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/session.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/subscription.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/modules/swap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/multiquerier.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/querier.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/deposit.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/node.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/plan.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/provider.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/session.py
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/subscription.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/swap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/transactor/__init__.py
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/src/sentinel_sdk/transactor/transactor.py
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/test/connect.py
+-rw-r--r--   0        0        0     3804 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/test/connect.sdk.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/test/queryall.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 sentinel_sdk-0.0.4/PKG-INFO
```

### Comparing `sentinel_sdk-0.0.3/.pre-commit-config.yaml` & `sentinel_sdk-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/sdk.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/types.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class NodeType(Enum):
     WIREGUARD = 1
     V2RAY = 2
 
 @dataclass
 class TxParams:
     denom: str = "udvpn"
-    fee_amount: int = 20000
+    fee_amount: int = 314159
     gas: float = 0
     gas_multiplier: float = 1.5
 
 
 class PageRequest:
     """
     // key is a value returned in PageResponse.next_key to begin
```

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/utils.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/deposit.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/deposit.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/node.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/node.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/plan.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/plan.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/provider.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/provider.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/session.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/session.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/subscription.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/subscription.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/modules/swap.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/modules/swap.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/multiquerier.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/multiquerier.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/querier.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/querier.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/deposit.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/deposit.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/node.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/node.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/plan.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/plan.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/provider.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/provider.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/session.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/session.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/subscription.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/subscription.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/querier/modules/swap.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/querier/modules/swap.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/src/sentinel_sdk/transactor/transactor.py` & `sentinel_sdk-0.0.4/src/sentinel_sdk/transactor/transactor.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/test/connect.py` & `sentinel_sdk-0.0.4/test/connect.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/test/connect.sdk.py` & `sentinel_sdk-0.0.4/test/connect.sdk.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/test/queryall.py` & `sentinel_sdk-0.0.4/test/queryall.py`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/.gitignore` & `sentinel_sdk-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/LICENSE` & `sentinel_sdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/README.md` & `sentinel_sdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sentinel_sdk-0.0.3/pyproject.toml` & `sentinel_sdk-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sentinel_sdk"
-version = "0.0.3"
+version = "0.0.4"
 description = "A Sentinel SDK Written in Python"
 authors = [
     { name = "NAST0R" },
     { name = "Tkd-Alex", email = "alex.tkd.alex@gmail.com" },
     { name = "MathNodes", email = "freQniK@mathnodes.com'" },
 ]
 readme = "README.md"
```

### Comparing `sentinel_sdk-0.0.3/PKG-INFO` & `sentinel_sdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sentinel_sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Sentinel SDK Written in Python
 Author: NAST0R
 Author-email: Tkd-Alex <alex.tkd.alex@gmail.com>, MathNodes <freQniK@mathnodes.com'>
 License: GPL-3.0 license
 License-File: LICENSE
 Keywords: cosmos,mospy,protobuf,sentinel,sentinel_protobuf,sentinel_sdk
 Classifier: Development Status :: 3 - Alpha
```

