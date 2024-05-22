# Comparing `tmp/anycrc-0.7.4.tar.gz` & `tmp/anycrc-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycrc-0.7.4.tar", last modified: Mon May 20 03:36:56 2024, max compression
+gzip compressed data, was "anycrc-0.7.5.tar", last modified: Wed May 22 03:39:13 2024, max compression
```

## Comparing `anycrc-0.7.4.tar` & `anycrc-0.7.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.009386 anycrc-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-20 03:36:50.000000 anycrc-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-20 03:36:56.009386 anycrc-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-20 03:36:50.000000 anycrc-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/lib/crcany/
--rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/crc.c
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/crcdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-20 03:36:50.000000 anycrc-0.7.4/lib/crcany/model.c
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-20 03:36:50.000000 anycrc-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 03:36:56.009386 anycrc-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-20 03:36:50.000000 anycrc-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.005386 anycrc-0.7.4/src/anycrc/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/anycrc.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-20 03:36:50.000000 anycrc-0.7.4/src/anycrc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 03:36:56.009386 anycrc-0.7.4/src/anycrc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-20 03:36:55.000000 anycrc-0.7.4/src/anycrc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 03:36:56.000000 anycrc-0.7.4/src/anycrc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-22 03:39:07.000000 anycrc-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-22 03:39:13.167848 anycrc-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-22 03:39:07.000000 anycrc-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.163848 anycrc-0.7.5/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/lib/crcany/
+-rw-r--r--   0 runner    (1001) docker     (127)    25358 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/crc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/crcdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18969 2024-05-22 03:39:07.000000 anycrc-0.7.5/lib/crcany/model.c
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 03:39:07.000000 anycrc-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:39:13.167848 anycrc-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-22 03:39:07.000000 anycrc-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.163848 anycrc-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/src/anycrc/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/anycrc.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-22 03:39:07.000000 anycrc-0.7.5/src/anycrc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:39:13.167848 anycrc-0.7.5/src/anycrc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 03:39:13.000000 anycrc-0.7.5/src/anycrc.egg-info/top_level.txt
```

### Comparing `anycrc-0.7.4/LICENSE` & `anycrc-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/PKG-INFO` & `anycrc-0.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

### Comparing `anycrc-0.7.4/README.md` & `anycrc-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/lib/crcany/crc.c` & `anycrc-0.7.5/lib/crcany/crc.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/lib/crcany/crcdbl.c` & `anycrc-0.7.5/lib/crcany/crcdbl.c`

 * *Files 2% similar despite different names*

```diff
@@ -201,49 +201,46 @@
         model->table_byte[256 + k] = crc_hi;
     } while (++k);
     
     return 0;
 }
 
 void crc_bytewise_dbl(model_t *model, word_t *crc_hi, word_t *crc_lo, unsigned char const *buf, size_t len) {
+    // Use crc_bytewise() for CRCs that fit in a word_t.
+    if (model->width <= WORDBITS) {
+        *crc_lo = crc_bytewise(model, *crc_lo, buf, len);
+        *crc_hi = 0;
+        return;
+    }
+    
     // Pre-process the CRC.
     if (model->rev)
         reverse_dbl(crc_hi, crc_lo, model->width);
         
     word_t lo = *crc_lo;
     word_t hi = *crc_hi;
     unsigned short idx;
     
     // Process the input data a byte at a time.
     if (model->ref) {
-        if(model->width > WORDBITS) {
-            hi &= ONES(model->width - WORDBITS);
-        } else {
-            lo &= ONES(model->width);
-            hi = 0;
-        }
+        hi &= ONES(model->width - WORDBITS);
         while (len--) {
             idx = (lo ^ *buf++) & 0xff;
             lo = SHR_LO(hi, lo, 8) ^ model->table_byte[idx];
             hi = SHR_HI(hi, lo, 8) ^ model->table_byte[256 + idx];
         }
     }
     else {
         unsigned shift = model->width - 8;  // 1..WORDBITS-8
         while (len--) {
             idx = (SHR_LO(hi, lo, shift) ^ *buf++) & 0xff;
             lo = SHL_LO(hi, lo, 8) ^ model->table_byte[idx];
             hi = SHL_HI(hi, lo, 8) ^ model->table_byte[256 + idx];
         }
-        if(model->width > WORDBITS) {
-            hi &= ONES(model->width - WORDBITS);
-        } else {
-            lo &= ONES(model->width);
-            hi = 0;
-        }
+        hi &= ONES(model->width - WORDBITS);
     }
     
     *crc_lo = lo;
     *crc_hi = hi;
     
     // Post-process and return the CRC
     if (model->rev)
```

### Comparing `anycrc-0.7.4/lib/crcany/model.c` & `anycrc-0.7.5/lib/crcany/model.c`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/setup.py` & `anycrc-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         
 else:
     compile_args = ['-fopenmp', '-O2']
     link_args = ['-fopenmp', '-O2']
     
 setup(
     name = 'anycrc',
-    version = '0.7.4',
+    version = '0.7.5',
     package_dir = {"": "src"},
     cmdclass={"build_ext": Build},
     ext_modules = [
         Extension(
             name='anycrc.anycrc',
             extra_compile_args=compile_args,
             extra_link_args=link_args,
```

### Comparing `anycrc-0.7.4/src/anycrc/anycrc.pyx` & `anycrc-0.7.5/src/anycrc/anycrc.pyx`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/src/anycrc/models.py` & `anycrc-0.7.5/src/anycrc/models.py`

 * *Files identical despite different names*

### Comparing `anycrc-0.7.4/src/anycrc.egg-info/PKG-INFO` & `anycrc-0.7.5/src/anycrc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycrc
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python CRC Computation Library
 Project-URL: Homepage, https://github.com/marzooqy/anycrc
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a Cython module with bindings to the [crcany](https://github.com/madler/crcany) library. It supports calculating CRC hashes of arbitary sizes as well as updating a crc hash over time. It takes advantage of crcany's ability to efficiently combine multiple CRCs to parallelize the CRC's calculation.
```

