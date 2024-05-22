# Comparing `tmp/nadl-1.4.0.tar.gz` & `tmp/nadl-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.4.0.tar", last modified: Tue May 21 15:38:56 2024, max compression
+gzip compressed data, was "nadl-1.4.1.tar", last modified: Wed May 22 03:11:58 2024, max compression
```

## Comparing `nadl-1.4.0.tar` & `nadl-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2275 2024-05-21 15:38:56.528277 nadl-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.0/readme.org
--rw-r--r--   0        0        0     1784 2024-05-21 15:34:55.693364 nadl-1.4.0/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.0/src/nadl/blocks.py
--rw-r--r--   0        0        0     5133 2024-05-21 15:34:33.076254 nadl-1.4.0/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.0/src/nadl/images.py
--rw-r--r--   0        0        0     3483 2024-05-18 03:07:59.101302 nadl-1.4.0/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.0/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.0/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.0/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.0/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.0/src/nadl/py.typed
--rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.0/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.0/src/nadl/transformers.py
--rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.0/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-22 03:11:58.171534 nadl-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.1/readme.org
+-rw-r--r--   0        0        0     1806 2024-05-22 03:11:17.681084 nadl-1.4.1/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.1/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5149 2024-05-21 19:59:54.581010 nadl-1.4.1/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.1/src/nadl/images.py
+-rw-r--r--   0        0        0     3483 2024-05-21 19:45:50.651928 nadl-1.4.1/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.1/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.1/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.1/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.1/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.1/src/nadl/py.typed
+-rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.1/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.1/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.1/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.1/PKG-INFO
```

### Comparing `nadl-1.4.0/pyproject.toml` & `nadl-1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.4.0"
+version = "1.4.1"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.4.0/readme.org` & `nadl-1.4.1/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/__init__.py` & `nadl-1.4.1/src/nadl/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,40 +33,42 @@
 license  : GPL-3.0+
 
 NADL
 """
 
 from .data import DState, IdxDataloader, es_loop
 from .keys import Keys, new_key
-from .loops import PG
+from .loops import PG, RESC, PGThread
 from .metrics import dice_coef, iou_coef
 from .preprocessing import (
-    SCALER,
-    identity_scaler,
-    min_max_scaler,
-    normalizer,
-    select_scaler,
-    standard_scaler,
+  SCALER,
+  identity_scaler,
+  min_max_scaler,
+  normalizer,
+  select_scaler,
+  standard_scaler,
 )
 from .states import BaseTrainState, state_fn
 from .utils import (
-    classit,
-    rle,
-    rle_array,
+  classit,
+  rle,
+  rle_array,
 )
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 
 __all__ = [
   "PG",
+  "RESC",
   "SCALER",
   "BaseTrainState",
   "DState",
   "IdxDataloader",
   "Keys",
+  "PGThread",
   "classit",
   "dice_coef",
   "es_loop",
   "identity_scaler",
   "iou_coef",
   "min_max_scaler",
   "new_key",
```

### Comparing `nadl-1.4.0/src/nadl/blocks.py` & `nadl-1.4.1/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/data.py` & `nadl-1.4.1/src/nadl/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,15 +82,15 @@
       self.drop_num = self.length % batch_size
 
     length = length if not drop_last else length - length % batch_size
     pad = (batch_size - r) % batch_size if (r := length % batch_size) else 0
     self.pad = pad = pad if pad != batch_size else 0
 
     self.batch_size = batch_size
-    self.transform = transform
+    self.transform = eqx.filter_jit(transform)
 
   @eqx.filter_jit
   def __call__(self, key: jax.Array | None = None) -> DState[T]:
     """Get the indexes."""
     if key is None:
       idxes = jnp.arange(self.length)
     else:
@@ -120,15 +120,15 @@
       pg.pg.reset(pg.tasks[es])
     else:
       pg.add_task(es, total=epochs, res="")
     pg.advance(pg.tasks[es], start_epoch - 1)
 
   vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
   if keys:
-    keys.reverse(epochs)
+    keys.reserve(epochs)
   ds: DState[T] = vdl() if keys is None else vdl(keys(jnp.arange(epochs)))
   ds = tree_at(lambda d: d.name, ds, prefix, is_leaf=lambda x: x is None)
 
   if ss in pg.tasks:
     pg.pg.reset(pg.tasks[ss])
   else:
     pg.add_task(ss, total=ds.shape[0] * epochs, res="")
```

### Comparing `nadl-1.4.0/src/nadl/images.py` & `nadl-1.4.1/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/keys.py` & `nadl-1.4.1/src/nadl/keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   idx: jax.Array = field(default_factory=lambda: jax.numpy.array(0))
 
   @property
   def key(self) -> jax.Array:
     """Get key."""
     if self.keys:
       return self.keys[-1]
-    self.reverse(1)
+    self.reserve(1)
     return self.keys[-1]
 
   @property
   def state(self) -> tuple[jax.Array, Sequence[jax.Array], jax.Array]:
     """Get state."""
     return self.init_key, self.keys, self.idx
 
@@ -82,15 +82,15 @@
   @classmethod
   def from_state(
     cls: type[Keys], key: jax.Array, keys: Sequence[jax.Array], idx: jax.Array
   ) -> Keys:
     """Convert state to Keys."""
     return cls(key, list(keys), idx)
 
-  def reverse(self, num: int | jax.Array) -> Keys:
+  def reserve(self, num: int | jax.Array) -> Keys:
     """Reverse the keys."""
     while (num := num - 1) >= 0:
       if self.keys:
         self.keys.append(jax.random.fold_in(self.keys[-1], 0))
       else:
         self.keys.append(jax.random.fold_in(self.init_key, 0))
     return self
@@ -105,25 +105,25 @@
 
   def __next__(self) -> Keys:
     """Get next key."""
     return self.next_key()
 
   def take(self, num: int) -> jax.Array:
     """Take num keys."""
-    self.reverse(jnp.max(num - len(self.keys), 0))
+    self.reserve(jnp.max(num - len(self.keys), 0))
     return jnp.r_[*self.keys[-num:]]
 
   def __call__(self, epoch: int | jax.Array | None = None) -> jax.Array:
     """Get keys for epoch."""
     match epoch:
       case int():
         if epoch + 1 > len(self.keys):
-          self.reverse(epoch + 1 - len(self.keys))
+          self.reserve(epoch + 1 - len(self.keys))
         return self.keys[epoch]
       case jax.Array():
-        self.reverse(jnp.maximum((epoch + 1 - len(self.keys)).max(), 0))
+        self.reserve(jnp.maximum((epoch + 1 - len(self.keys)).max(), 0))
         return jnp.r_[*self.keys][epoch]
       case None:
         return self(self.idx)
 
 
 new_key = Keys.from_int_or_key
```

### Comparing `nadl-1.4.0/src/nadl/loops.py` & `nadl-1.4.1/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/metrics.py` & `nadl-1.4.1/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/nets.py` & `nadl-1.4.1/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/preprocessing.py` & `nadl-1.4.1/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/states.py` & `nadl-1.4.1/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/transformers.py` & `nadl-1.4.1/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/src/nadl/utils.py` & `nadl-1.4.1/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.0/PKG-INFO` & `nadl-1.4.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.4.0
+Version: 1.4.1
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

