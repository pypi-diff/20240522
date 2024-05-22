# Comparing `tmp/gmalglib-0.5.3.tar.gz` & `tmp/gmalglib-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.3.tar", last modified: Tue Apr 23 13:15:57 2024, max compression
+gzip compressed data, was "gmalglib-0.5.4.tar", last modified: Wed May 22 15:19:09 2024, max compression
```

## Comparing `gmalglib-0.5.3.tar` & `gmalglib-0.5.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 13:15:51.000000 gmalglib-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-23 13:15:57.218980 gmalglib-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-23 13:15:51.000000 gmalglib-0.5.3/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-23 13:15:51.000000 gmalglib-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-23 13:15:51.000000 gmalglib-0.5.3/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-23 13:15:51.000000 gmalglib-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:15:57.218980 gmalglib-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-23 13:15:51.000000 gmalglib-0.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.214980 gmalglib-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    18369 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    36380 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-23 13:15:51.000000 gmalglib-0.5.3/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:15:57.218980 gmalglib-0.5.3/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 13:15:57.000000 gmalglib-0.5.3/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 15:19:04.000000 gmalglib-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:19:09.672788 gmalglib-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-22 15:19:04.000000 gmalglib-0.5.4/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-22 15:19:04.000000 gmalglib-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 15:19:04.000000 gmalglib-0.5.4/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 15:19:04.000000 gmalglib-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:19:09.672788 gmalglib-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 15:19:04.000000 gmalglib-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.668788 gmalglib-0.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 15:19:04.000000 gmalglib-0.5.4/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:19:09.672788 gmalglib-0.5.4/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 15:19:09.000000 gmalglib-0.5.4/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.3/LICENSE` & `gmalglib-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/PKG-INFO` & `gmalglib-0.5.4/README.en.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gmalglib
-Version: 0.5.3
-Summary: Python package implementing GM algorithms in C.
-Author-email: ww-rm <ww-rm@qq.com>
-Project-URL: Homepage, https://github.com/ww-rm/gmalglib
-Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
-Project-URL: Documentation, https://gmalglib.readthedocs.io
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
 [![docs](https://readthedocs.org/projects/gmalglib/badge/?version=latest)](https://gmalglib.readthedocs.io/zh-cn/latest/?badge=latest)
 
 Python extension library for GM (GuoMi) cryptographic algorithms, providing a set of fundamental cryptographic algorithms.
@@ -31,14 +14,15 @@
 pip install gmalglib
 ```
 
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
+  - Key exchange 
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
 - ZUC Stream Cipher Algorithm
 
 ## Usage
 
@@ -68,7 +52,30 @@
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
 If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
+
+## Benchmark Test
+
+The benchmark test code can be found in `benchmark.py`. The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
+
+```plain
+==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
+SM2.encrypt             : 2.391558s
+SM2.decrypt             : 1.092445s
+SM2.sign_digest         : 1.062552s
+SM2.verify_digest       : 2.096187s
+SM2.sign                : 1.067850s
+SM2.verify              : 2.055190s
+SM2.begin_key_exchange  : 1.159822s
+SM2.end_key_exchange    : 1.633471s
+==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
+SM3.update & SM3.digest : 5.118763s
+==================== SM4 Benchmark Test (1000000 times) ====================
+SM4.encrypt             : 0.369991s
+SM4.decrypt             : 0.297077s
+==================== ZUC Benchmark Test (1000000 times) ====================
+zuc.generate            : 0.050301s
+```
```

### Comparing `gmalglib-0.5.3/README.md` & `gmalglib-0.5.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 
 ```bash
 pip install gmalglib
 ```
 
 ## 已实现的核心算法
 
+- SM2 椭圆曲线公钥密码算法
+    - 签名验签
+    - 密钥交换
+    - 加密解密
 - SM3 密码杂凑算法
     - 消息摘要
     - 密钥派生
     - 消息认证
 - SM4 分组密码算法
 - ZUC 序列密码算法
-- SM2 椭圆曲线公钥密码算法
-    - 签名验签
-    - 加密解密
 
 ## 用法
 
 对于 `gmalglib` 下的子模块, 分别导出了不同算法封装后结构, 按面向对象方式使用.
 
 ```python
 from gmalglib.sm3 import SM3
@@ -54,7 +55,30 @@
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
 如不传入随机数发生器, 则使用默认的系统相关随机数发生器, 在 Windows 下使用 `BCryptGenRandom`, 其余系统使用 `/dev/urandom` 实现, 其实现类似于 Python 标准库函数 [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 具体实现见 [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) 内 `OsRandomProc`.
+
+## 性能测试
+
+性能测试代码见 `benchmark.py`, `13th Gen Intel(R) Core(TM) i7-13700H` 上测试结果如下:
+
+```plain
+==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
+SM2.encrypt             : 2.391558s
+SM2.decrypt             : 1.092445s
+SM2.sign_digest         : 1.062552s
+SM2.verify_digest       : 2.096187s
+SM2.sign                : 1.067850s
+SM2.verify              : 2.055190s
+SM2.begin_key_exchange  : 1.159822s
+SM2.end_key_exchange    : 1.633471s
+==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
+SM3.update & SM3.digest : 5.118763s
+==================== SM4 Benchmark Test (1000000 times) ====================
+SM4.encrypt             : 0.369991s
+SM4.decrypt             : 0.297077s
+==================== ZUC Benchmark Test (1000000 times) ====================
+zuc.generate            : 0.050301s
+```
```

### Comparing `gmalglib-0.5.3/include/gmalglib/bignum.h` & `gmalglib-0.5.4/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/include/gmalglib/random.h` & `gmalglib-0.5.4/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/include/gmalglib/sm2.h` & `gmalglib-0.5.4/include/gmalglib/sm2.h`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 #define SM2_ERR_INVALID_SIGN            -7
 #define SM2_ERR_NEED_PK                 -8
 #define SM2_ERR_NO_MEMORY               -9
 #define SM2_ERR_DATA_OVERFLOW           -10
 #define SM2_ERR_INVALID_C1              -11
 #define SM2_ERR_INVALID_C3              -12
 #define SM2_ERR_INVALID_CIPHER          -13
+#define SM2_ERR_INVALID_SPOINT          -14
+#define SM2_ERR_KEY_OVERFLOW            -15
+#define SM2_ERR_INVALID_T               -16
+#define SM2_ERR_INVALID_R               -17
 
 typedef UInt256 SM2ModN;
 typedef SM2ModN SM2ModNMont;
 
 typedef struct _SM2 {
     int has_sk;
     SM2ModN sk;
@@ -76,13 +80,15 @@
 int SM2_GetEntityInfo(SM2* self, uint8_t* entity_info);
 int SM2_SignDigest(SM2* self, const uint8_t* digest, uint8_t* signature);
 int SM2_VerifyDigest(SM2* self, const uint8_t* digest, const uint8_t* signature);
 int SM2_Sign(SM2* self, const uint8_t* msg, uint64_t msg_len, uint8_t* signature);
 int SM2_Verify(SM2* self, const uint8_t* msg, uint64_t msg_len, const uint8_t* signature);
 int SM2_Encrypt(SM2* self, const uint8_t* plain, uint64_t plain_len, uint8_t* cipher);
 int SM2_Decrypt(SM2* self, const uint8_t* cipher, uint64_t cipher_len, uint8_t* plain, uint64_t* plain_len);
+int SM2_BeginKeyExchange(SM2* self, SM2ModN* t, uint8_t* random_pt);
+int SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const uint8_t* random_pt, uint64_t random_pt_len, const uint8_t* pk, uint64_t pk_len, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key);
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif // !GMALGLIB_SM2_H
```

### Comparing `gmalglib-0.5.3/include/gmalglib/sm2curve.h` & `gmalglib-0.5.4/include/gmalglib/sm2curve.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/include/gmalglib/sm3.h` & `gmalglib-0.5.4/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/pyproject.toml` & `gmalglib-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/setup.py` & `gmalglib-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/bignum.c` & `gmalglib-0.5.4/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/random.c` & `gmalglib-0.5.4/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/sm2.c` & `gmalglib-0.5.4/src/gmalglib/core/sm2.c`

 * *Files 16% similar despite different names*

```diff
@@ -698,7 +698,138 @@
     }
     *plain_len = c2_len;
 
 cleanup:
     free(plain_buffer);
     return err;
 }
+
+static
+int _SM2_BeginKeyExchange(SM2* self, SM2JacobPointMont* random_pt, SM2ModN* t)
+{
+    SM2ModNMont r = { 0 };
+    SM2Point R = { 0 };
+
+    if (!RandomUInt256(&self->rand_alg, CONSTS_N_MINUS_ONE, &r))
+        return SM2_ERR_RANDOM_FAILED;
+
+    SM2JacobPointMont_MulG(&r, random_pt);
+
+    // w        =   ceil(ceil(log2(N)) / 2) - 1         = 127
+    // 2^w      =   0x80000000000000000000000000000000
+    // 2^w - 1  =   0x7fffffffffffffffffffffffffffffff
+    // x_bar    =   2^w + (x & (2^w - 1))
+    SM2JacobPointMont_ToPoint(random_pt, &R);
+    R.x.u64[3] = 0;
+    R.x.u64[2] = 0;
+    R.x.u64[1] |= 0x8000000000000000;
+
+    SM2ModN_ToMont(&R.x, &R.x);
+    SM2ModN_ToMont(&r, &r);
+
+    SM2ModN_MontMul(&R.x, &r, t);
+    SM2ModN_FromMont(t, t);
+    SM2ModN_Add(&self->sk, t, t);
+
+    return 0;
+}
+
+int SM2_BeginKeyExchange(SM2* self, SM2ModN* t, uint8_t* random_pt)
+{
+    int ret = 0;
+    SM2JacobPointMont R = { 0 };
+
+    if (!self->has_sk)
+        return SM2_ERR_NEED_SK;
+
+    ret = _SM2_BeginKeyExchange(self, &R, t);
+    if (ret != 0)
+        return ret;
+
+    SM2JacobPointMont_ToBytes(&R, self->pc_mode, random_pt);
+    return 0;
+}
+
+static
+int _SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const SM2JacobPointMont* random_pt, const SM2JacobPointMont* pk, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key)
+{
+    SM2JacobPointMont S = { 0 };
+    SM2Point R = { 0 };
+    SM3 sm3 = { 0 };
+    uint8_t buffer[32] = { 0 };
+
+    // x_bar
+    SM2JacobPointMont_ToPoint(random_pt, &R);
+    R.x.u64[3] = 0;
+    R.x.u64[2] = 0;
+    R.x.u64[1] |= 0x8000000000000000;
+
+    SM2JacobPointMont_Mul(&R.x, random_pt, &S);
+    SM2JacobPointMont_Add(pk, &S, &S);
+    SM2JacobPointMont_Mul(t, &S, &S);
+
+    if (SM2JacobPointMont_IsInf(&S))
+        return SM2_ERR_INVALID_SPOINT;
+
+    SM2JacobPointMont_ToPoint(&S, &R);
+
+    SM3_Init(&sm3);
+
+    UInt256_ToBytes(&R.x, buffer);
+    SM3_Update(&sm3, buffer, 32);
+    UInt256_ToBytes(&R.y, buffer);
+    SM3_Update(&sm3, buffer, 32);
+
+    _SM2_GetEntityInfo(pk, uid, uid_len, buffer);
+
+    if (is_responder)
+    {
+        SM3_Update(&sm3, buffer, 32);
+        SM3_Update(&sm3, self->entity_info, 32);
+    }
+    else
+    {
+        SM3_Update(&sm3, self->entity_info, 32);
+        SM3_Update(&sm3, buffer, 32);
+    }
+
+    if (SM3_DeriveKey(&sm3, klen, key) != 0)
+        return SM2_ERR_KEY_OVERFLOW;
+
+    return 0;
+}
+
+int SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const uint8_t* random_pt, uint64_t random_pt_len, const uint8_t* pk, uint64_t pk_len, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key)
+{
+    SM2JacobPointMont R = { 0 };
+    SM2JacobPointMont P = { 0 };
+    int ret = 0;
+
+    if (!self->has_pk)
+        return SM2_ERR_NEED_PK;
+
+    if (UInt256_IsZero(t) || UInt256_Cmp(t, CONSTS_N_MINUS_ONE) > 0)
+        return SM2_ERR_INVALID_T;
+
+    if (SM2JacobPointMont_FromBytes(random_pt, random_pt_len, &R) != 0)
+        return SM2_ERR_INVALID_R;
+
+    if (SM2JacobPointMont_FromBytes(pk, pk_len, &P) != 0)
+        return SM2_ERR_INVALID_PK;
+
+    if (uid == NULL)
+    {
+        uid = SM2_DEFAULT_UID;
+        uid_len = SM2_DEFAULT_UID_LENGTH;
+    }
+    else
+    {
+        if (uid_len > SM2_UID_MAX_LENGTH)
+            return SM2_ERR_UID_OVERFLOW;
+    }
+
+    ret = _SM2_EndKeyExchange(self, t, &R, &P, uid, uid_len, is_responder, klen, key);
+    if (ret != 0)
+        return ret;
+
+    return 0;
+}
```

### Comparing `gmalglib-0.5.3/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.4/src/gmalglib/core/sm2curve.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/sm3.c` & `gmalglib-0.5.4/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/sm4.c` & `gmalglib-0.5.4/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/core/zuc.c` & `gmalglib-0.5.4/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/coremodule.c` & `gmalglib-0.5.4/src/gmalglib/coremodule.c`

 * *Files 2% similar despite different names*

```diff
@@ -923,28 +923,126 @@
 cleanup:
     if (plain)
         free(plain);
     PyBuffer_Release(&py_buffer_cipher);
     return ret;
 }
 
+static PyObject* PySM2_begin_key_exchange(PySM2Object* self, PyObject* Py_UNUSED(args))
+{
+    uint8_t random_pt[SM2_POINTBYTES_MAX_LENGTH] = { 0 };
+    SM2ModN t = { 0 };
+    uint8_t t_bytes[32] = { 0 };
+    int sm2_ret = 0;
+
+    sm2_ret = SM2_BeginKeyExchange(&self->sm2, &t, random_pt);
+
+    switch (sm2_ret)
+    {
+    case SM2_ERR_NEED_SK:           PyErr_SetString(PyExc_AttributeError, "Need secret key.");              return NULL;
+    case SM2_ERR_RANDOM_FAILED:     PyErr_SetString(PyExc_RuntimeError, "Failed to get random bytes.");     return NULL;
+    default: 
+        break;
+    }
+
+    UInt256_ToBytes(&t, t_bytes);
+    return Py_BuildValue("y#y#", (char*)t_bytes, (Py_ssize_t)32, random_pt, (Py_ssize_t)SM2_GET_POINTBYTES_LENGTH(self->sm2.pc_mode));
+}
+
+static PyObject* PySM2_end_key_exchange(PySM2Object* self, PyObject* args, PyObject* kwargs)
+{
+    char* keys[] = { "t", "random_pt", "pk", "is_responder", "klen", "uid" , NULL };
+
+    Py_buffer py_buffer_t = { 0 };
+    Py_buffer py_buffer_random_pt = { 0 };
+    Py_buffer py_buffer_pk = { 0 };
+    Py_buffer py_buffer_uid = { 0 };
+    uint64_t klen = 0;
+    int is_responder = 0;
+
+    PyObject* ret = NULL;
+    int sm2_ret = 0;
+
+    SM2ModN t = { 0 };
+    uint8_t* key = NULL;
+
+    if (!PyArg_ParseTupleAndKeywords(
+        args, kwargs, "y*y*y*pK|y*:end_key_exchange", keys,
+        &py_buffer_t,
+        &py_buffer_random_pt,
+        &py_buffer_pk,
+        &is_responder,
+        &klen,
+        &py_buffer_uid))
+        return NULL;
+
+    if (py_buffer_t.len != 32)
+    {
+        PyErr_SetString(PyExc_ValueError, "Incorrect t length.");
+        goto cleanup;
+    }
+
+    key = (uint8_t*)calloc(klen, sizeof(uint8_t));
+    if (!key)
+    {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate buffer.");
+        goto cleanup;
+    }
+
+    UInt256_FromBytes(py_buffer_t.buf, &t);
+
+    sm2_ret = SM2_EndKeyExchange(
+        &self->sm2,
+        &t,
+        py_buffer_random_pt.buf, py_buffer_random_pt.len,
+        py_buffer_pk.buf, py_buffer_pk.len,
+        py_buffer_uid.buf, py_buffer_uid.len,
+        is_responder,
+        klen,
+        key
+    );
+    switch (sm2_ret)
+    {
+    case SM2_ERR_NEED_PK:           PyErr_SetString(PyExc_AttributeError, "Need public key.");              goto cleanup;
+    case SM2_ERR_INVALID_T:         PyErr_SetString(PyExc_ValueError, "Invalid t value.");                  goto cleanup;
+    case SM2_ERR_INVALID_R:         PyErr_SetString(PyExc_ValueError, "Invalid R point.");                  goto cleanup;
+    case SM2_ERR_INVALID_PK:        PyErr_SetString(PyExc_ValueError, "Invalid public key.");               goto cleanup;
+    case SM2_ERR_UID_OVERFLOW:      PyErr_SetString(PyExc_OverflowError, "uid too long.");                  goto cleanup;
+    case SM2_ERR_INVALID_SPOINT:    PyErr_SetString(PyExc_ValueError, "Invalid S point.");                  goto cleanup;
+    case SM2_ERR_KEY_OVERFLOW:      PyErr_SetString(PyExc_OverflowError, "Key stream too long.");           goto cleanup;
+    default:
+        ret = PyBytes_FromStringAndSize((char*)key, klen);
+    }
+
+cleanup:
+    if (key) free(key);
+    PyBuffer_Release(&py_buffer_t);
+    PyBuffer_Release(&py_buffer_random_pt);
+    PyBuffer_Release(&py_buffer_pk);
+    PyBuffer_Release(&py_buffer_uid);
+
+    return ret;
+}
+
 static PyMethodDef py_methods_def_SM2[] = {
     {"is_sk_valid",         (PyCFunction)PySM2_is_sk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check sk is valid.")},
     {"is_pk_valid",         (PyCFunction)PySM2_is_pk_valid,         METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check pk is valid.")},
     {"is_keypair",          (PyCFunction)PySM2_is_keypair,          METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Check if a valid keypair.")},
     {"get_pk",              (PyCFunction)PySM2_get_pk,              METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Get public key bytes.")},
     {"convert_pk",          (PyCFunction)PySM2_convert_pk,          METH_VARARGS | METH_KEYWORDS | METH_STATIC,     PyDoc_STR("Convert public key bytes to other pc_mode.")},
     {"generate_keypair",    (PyCFunction)PySM2_generate_keypair,    METH_NOARGS,                                    PyDoc_STR("Generate key pair.")},
     {"get_entity_info",     (PyCFunction)PySM2_get_entity_info,     METH_NOARGS,                                    PyDoc_STR("Get entity info.")},
     {"sign_digest",         (PyCFunction)PySM2_sign_digest,         METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on digest.")},
     {"verify_digest",       (PyCFunction)PySM2_verify_digest,       METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on digest.")},
     {"sign",                (PyCFunction)PySM2_sign,                METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Sign on full message.")},
     {"verify",              (PyCFunction)PySM2_verify,              METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Verify on full message.")},
     {"encrypt",             (PyCFunction)PySM2_encrypt,             METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Encrypt data.")},
     {"decrypt",             (PyCFunction)PySM2_decrypt,             METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("Decrypt data.")},
+    {"begin_key_exchange",  (PyCFunction)PySM2_begin_key_exchange,  METH_NOARGS,                                    PyDoc_STR("Begin key exchange.")},
+    {"end_key_exchange",    (PyCFunction)PySM2_end_key_exchange,    METH_VARARGS | METH_KEYWORDS,                   PyDoc_STR("End key exchange.")},
     {NULL}
 };
 
 static PyTypeObject py_type_SM2 = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "gmalglib.core.SM2",
     .tp_doc = PyDoc_STR("SM2 Object."),
```

### Comparing `gmalglib-0.5.3/src/gmalglib/sm3.pyi` & `gmalglib-0.5.4/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/wrapped.py` & `gmalglib-0.5.4/src/gmalglib/wrapped.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib/zuc.pyi` & `gmalglib-0.5.4/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.3/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.3
+Version: 0.5.4
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -31,14 +31,15 @@
 pip install gmalglib
 ```
 
 ## Core Algorithms Implemented
 
 - SM2 Public Key Cryptograhpic Algorithm Based on Elliptic Curves
   - Sign/Verify
+  - Key exchange 
   - Encrypt/Decrypt
 - SM3 Cryptogrpahic Hash Algorithm
 - SM4 Block Cipher Algorithm
 - ZUC Stream Cipher Algorithm
 
 ## Usage
 
@@ -68,7 +69,30 @@
 ```python
 def rnd_fn(n: int) -> bytes: ...
 ```
 
 If no random number generator is passed, the default system-related random number generator is used. On Windows, it utilizes `BCryptGenRandom`, while other systems use `/dev/urandom` for implementation, which is similar to the Python standard library function [`os.urandom`](https://docs.python.org/3/library/os.html#os.urandom).
 
 For specific implementation details, refer to [random.c](https://github.com/ww-rm/gmalglib/blob/main/src/gmalglib/core/random.c) under the `OsRandomProc` function.
+
+## Benchmark Test
+
+The benchmark test code can be found in `benchmark.py`. The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
+
+```plain
+==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
+SM2.encrypt             : 2.391558s
+SM2.decrypt             : 1.092445s
+SM2.sign_digest         : 1.062552s
+SM2.verify_digest       : 2.096187s
+SM2.sign                : 1.067850s
+SM2.verify              : 2.055190s
+SM2.begin_key_exchange  : 1.159822s
+SM2.end_key_exchange    : 1.633471s
+==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
+SM3.update & SM3.digest : 5.118763s
+==================== SM4 Benchmark Test (1000000 times) ====================
+SM4.encrypt             : 0.369991s
+SM4.decrypt             : 0.297077s
+==================== ZUC Benchmark Test (1000000 times) ====================
+zuc.generate            : 0.050301s
+```
```

### Comparing `gmalglib-0.5.3/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.4/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

