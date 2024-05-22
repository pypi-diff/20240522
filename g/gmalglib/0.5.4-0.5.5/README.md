# Comparing `tmp/gmalglib-0.5.4.tar.gz` & `tmp/gmalglib-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.4.tar", last modified: Wed May 22 15:19:09 2024, max compression
+gzip compressed data, was "gmalglib-0.5.5.tar", last modified: Wed May 22 15:53:43 2024, max compression
```

## Comparing `gmalglib-0.5.4.tar` & `gmalglib-0.5.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 15:19:04.000000 gmalglib-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:19:09.672788 gmalglib-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-22 15:19:04.000000 gmalglib-0.5.4/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-22 15:19:04.000000 gmalglib-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 15:19:04.000000 gmalglib-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:19:09.672788 gmalglib-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 15:19:04.000000 gmalglib-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 15:53:39.000000 gmalglib-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:53:43.793902 gmalglib-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-22 15:53:39.000000 gmalglib-0.5.5/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-22 15:53:39.000000 gmalglib-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.785902 gmalglib-0.5.5/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.789902 gmalglib-0.5.5/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 15:53:39.000000 gmalglib-0.5.5/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 15:53:39.000000 gmalglib-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:53:43.793902 gmalglib-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 15:53:39.000000 gmalglib-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.785902 gmalglib-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.789902 gmalglib-0.5.5/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 15:53:39.000000 gmalglib-0.5.5/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:53:43.793902 gmalglib-0.5.5/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:53:43.000000 gmalglib-0.5.5/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.4/LICENSE` & `gmalglib-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/PKG-INFO` & `gmalglib-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.5.4/README.en.md` & `gmalglib-0.5.5/README.en.md`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/README.md` & `gmalglib-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/include/gmalglib/bignum.h` & `gmalglib-0.5.5/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/include/gmalglib/random.h` & `gmalglib-0.5.5/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/include/gmalglib/sm2.h` & `gmalglib-0.5.5/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/include/gmalglib/sm2curve.h` & `gmalglib-0.5.5/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/include/gmalglib/sm3.h` & `gmalglib-0.5.5/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/pyproject.toml` & `gmalglib-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/setup.py` & `gmalglib-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/bignum.c` & `gmalglib-0.5.5/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/random.c` & `gmalglib-0.5.5/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/sm2.c` & `gmalglib-0.5.5/src/gmalglib/core/sm2.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.5/src/gmalglib/core/sm2curve.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/sm3.c` & `gmalglib-0.5.5/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/sm4.c` & `gmalglib-0.5.5/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/core/zuc.c` & `gmalglib-0.5.5/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/coremodule.c` & `gmalglib-0.5.5/src/gmalglib/coremodule.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/sm2.pyi` & `gmalglib-0.5.5/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/sm3.pyi` & `gmalglib-0.5.5/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib/wrapped.py` & `gmalglib-0.5.5/src/gmalglib/wrapped.py`

 * *Files 20% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 def sm2_get_pk(sk: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> bytes:
     """由私钥得到公钥."""
 
     return __sm2.SM2.get_pk(sk, __sm2_pcmode[pc_mode])
 
 
 def sm2_convert_pk(pk: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> bytes:
-    """由私钥得到公钥."""
+    """转换公钥格式."""
 
     return __sm2.SM2.convert_pk(pk, __sm2_pcmode[pc_mode])
 
 
 def sm2_generate_keypair(pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> __T.Tuple[bytes, bytes]:
     """生成密钥对.
 
@@ -90,62 +90,78 @@
         sk: 私钥.
         pk: 公钥.
     """
 
     return __sm2.SM2(pc_mode=__sm2_pcmode[pc_mode]).generate_keypair()
 
 
-def sm2_get_entity_info(pk: bytes, uid: __T.Optional[bytes] = None) -> bytes:
+def sm2_get_entity_info(pk: bytes, uid: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
     """获取实体信息."""
 
-    if uid is None:
-        uid = __sm2.SM2_DEFAULT_UID
-
     return __sm2.SM2(pk=pk, uid=uid).get_entity_info()
 
 
-def sm2_sign_digest(sk: bytes, digest: bytes, uid: __T.Optional[bytes] = None) -> bytes:
+def sm2_sign_digest(sk: bytes, digest: bytes, uid: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
     """对摘要进行签名."""
 
-    if uid is None:
-        uid = __sm2.SM2_DEFAULT_UID
-
     return __sm2.SM2(sk=sk, uid=uid).sign_digest(digest)
 
 
-def sm2_sign(sk: bytes, msg: bytes, uid: __T.Optional[bytes] = None) -> bytes:
+def sm2_sign(sk: bytes, msg: bytes, uid: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
     """对消息进行签名."""
 
-    if uid is None:
-        uid = __sm2.SM2_DEFAULT_UID
-
     return __sm2.SM2(sk=sk, uid=uid).sign(msg)
 
 
-def sm2_verify_digest(pk: bytes, digest: bytes, uid: __T.Optional[bytes] = None) -> bytes:
+def sm2_verify_digest(pk: bytes, digest: bytes, uid: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
     """对摘要进行验签."""
 
-    if uid is None:
-        uid = __sm2.SM2_DEFAULT_UID
-
     return __sm2.SM2(pk=pk, uid=uid).verify_digest(digest)
 
 
-def sm2_verify(pk: bytes, msg: bytes, uid: __T.Optional[bytes] = None) -> bytes:
+def sm2_verify(pk: bytes, msg: bytes, uid: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
     """对消息进行验签."""
 
-    if uid is None:
-        uid = __sm2.SM2_DEFAULT_UID
-
     return __sm2.SM2(pk=pk, uid=uid).verify(msg)
 
 
 def sm2_encrypt(pk: bytes, plain: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> bytes:
     """加密数据."""
 
     return __sm2.SM2(pk=pk, pc_mode=__sm2_pcmode[pc_mode]).encrypt(plain)
 
 
 def sm2_decrypt(sk: bytes, cipher: bytes) -> bytes:
     """解密数据."""
 
     return __sm2.SM2(sk=sk).decrypt(cipher)
+
+
+def sm2_begin_key_exchange(sk: bytes, pc_mode: __T.Literal["raw", "compress", "mix"] = "raw") -> __T.Tuple[bytes, bytes]:
+    """开始密钥交换.
+
+    Returns:
+        t: t 值.
+        random_pt: 随机点 R.
+    """
+
+    return __sm2.SM2(sk, pc_mode=pc_mode).begin_key_exchange()
+
+
+def sm2_end_key_exchange(pk: bytes, t: bytes, random_pt: bytes, pk_another: bytes, is_responder: bool, klen: int, uid: bytes = __sm2.SM2_DEFAULT_UID, uid_another: bytes = __sm2.SM2_DEFAULT_UID) -> bytes:
+    """结束密钥交换.
+
+    Args:
+        pk: 自己的公钥.
+        t: 从 begin_key_exchange 得到的 t 值.
+        random_pt: 对方的随机点 R.
+        pk_another: 对方的公钥.
+        is_responder: 自己是否是响应方, 否则是发起方.
+        klen: 要生成的密钥长度.
+        uid: 自己的用户 ID.
+        uid_another: 对方的用户 ID.
+
+    Returns:
+        key: 交换的密钥.
+    """
+
+    return __sm2.SM2(pk=pk, uid=uid).end_key_exchange(t, random_pt, pk_another, is_responder, klen, uid_another)
```

### Comparing `gmalglib-0.5.4/src/gmalglib/zuc.pyi` & `gmalglib-0.5.5/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.4/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.5/src/gmalglib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.5.4/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.5/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

