# Comparing `tmp/mexpress-0.1.5.tar.gz` & `tmp/mexpress-0.1.6.tar.gz`

## Comparing `mexpress-0.1.5.tar` & `mexpress-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 mexpress-0.1.5/Cargo.toml
--rw-r--r--   0     1001      123     2658 2023-04-22 22:58:36.000000 mexpress-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0     1001      123      437 2023-04-22 22:58:36.000000 mexpress-0.1.5/.github/workflows/test.yml
--rw-r--r--   0     1001      123       87 2023-04-22 22:58:36.000000 mexpress-0.1.5/.gitignore
--rw-r--r--   0     1001      123     1071 2023-04-22 22:58:36.000000 mexpress-0.1.5/LICENSE
--rw-r--r--   0     1001      123     3361 2023-04-22 22:58:36.000000 mexpress-0.1.5/README.md
--rw-r--r--   0     1001      123       10 2023-04-22 22:59:30.000000 mexpress-0.1.5/dist/mexpress-0.1.5.tar.gz
--rw-r--r--   0     1001      123     1431 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/demo/evaluators.py
--rw-r--r--   0     1001      123     2557 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/demo/opt.py
--rw-r--r--   0     1001      123     1933 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/mexpress/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/test/__init__.py
--rw-r--r--   0     1001      123     1157 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/test/test_meta.py
--rw-r--r--   0     1001      123     2109 2023-04-22 22:58:36.000000 mexpress-0.1.5/py/test/test_mexpress.py
--rw-r--r--   0     1001      123      312 2023-04-22 22:58:36.000000 mexpress-0.1.5/pyproject.toml
--rw-r--r--   0     1001      123       57 2023-04-22 22:58:36.000000 mexpress-0.1.5/requirements-dev.txt
--rw-r--r--   0     1001      123     2514 2023-04-22 22:58:36.000000 mexpress-0.1.5/src/lib.rs
--rw-r--r--   0     1001      123    11988 2023-04-22 22:59:28.000000 mexpress-0.1.5/Cargo.lock
--rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 mexpress-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 mexpress-0.1.6/Cargo.toml
+-rw-r--r--   0     1001      127     2793 2024-05-22 20:25:56.000000 mexpress-0.1.6/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      438 2024-05-22 20:25:56.000000 mexpress-0.1.6/.github/workflows/test.yml
+-rw-r--r--   0     1001      127       76 2024-05-22 20:25:56.000000 mexpress-0.1.6/.gitignore
+-rw-r--r--   0     1001      127     1071 2024-05-22 20:25:56.000000 mexpress-0.1.6/LICENSE
+-rw-r--r--   0     1001      127     3361 2024-05-22 20:25:56.000000 mexpress-0.1.6/README.md
+-rw-r--r--   0     1001      127     1430 2024-05-22 20:25:56.000000 mexpress-0.1.6/demo/evaluators.py
+-rw-r--r--   0     1001      127     2556 2024-05-22 20:25:56.000000 mexpress-0.1.6/demo/opt.py
+-rw-r--r--   0     1001      127     1919 2024-05-22 20:25:56.000000 mexpress-0.1.6/mexpress/__init__.py
+-rw-r--r--   0     1001      127       57 2024-05-22 20:25:56.000000 mexpress-0.1.6/requirements-dev.txt
+-rw-r--r--   0     1001      127     2539 2024-05-22 20:25:56.000000 mexpress-0.1.6/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-05-22 20:25:56.000000 mexpress-0.1.6/test/__init__.py
+-rw-r--r--   0     1001      127     1157 2024-05-22 20:25:56.000000 mexpress-0.1.6/test/test_meta.py
+-rw-r--r--   0     1001      127     2107 2024-05-22 20:25:56.000000 mexpress-0.1.6/test/test_mexpress.py
+-rw-r--r--   0     1001      127    11588 2024-05-22 20:25:56.000000 mexpress-0.1.6/Cargo.lock
+-rw-r--r--   0     1001      127      395 2024-05-22 20:25:56.000000 mexpress-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3708 1970-01-01 00:00:00.000000 mexpress-0.1.6/PKG-INFO
```

### Comparing `mexpress-0.1.5/.github/workflows/publish.yml` & `mexpress-0.1.6/.github/workflows/publish.yml`

 * *Files 6% similar despite different names*

```diff
@@ -7,105 +7,106 @@
 permissions:
   contents: read
 
 jobs:
   sdist:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Build sdist
         uses: PyO3/maturin-action@v1
         with:
           command: sdist
           args: --out dist
       - name: Upload sdist
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-sdist
           path: dist
 
   linux:
     runs-on: ubuntu-latest
     needs: [sdist]
     strategy:
       matrix:
         target: [x86_64, x86, aarch64]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
           manylinux: auto
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-linux-${{ strategy.job-index}}
           path: dist
 
   windows:
     runs-on: windows-latest
     needs: [sdist]
     strategy:
       matrix:
         target: [x64, x86]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.10'
           architecture: ${{ matrix.target }}
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
         uses: actions/upload-artifact@v3
         with:
-          name: wheels
+          name: wheels-win-${{ strategy.job-index }}
           path: dist
 
   macos:
     runs-on: macos-latest
     needs: [sdist]
     strategy:
       matrix:
         target: [x86_64, aarch64]
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist --find-interpreter
           sccache: 'true'
       - name: Upload wheels
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-macos-${{ strategy.job-index }}
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [linux, windows, macos, sdist]
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
-          name: wheels
+          pattern: wheels-*
+          merge-multiple: true
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
           args: --skip-existing *
```

### Comparing `mexpress-0.1.5/LICENSE` & `mexpress-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mexpress-0.1.5/README.md` & `mexpress-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `mexpress-0.1.5/py/demo/evaluators.py` & `mexpress-0.1.6/demo/evaluators.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
             res = func(**kwargs)
     elapsed = time() - t0
     print(f"evaluating {n_runs} times {name:18} took {elapsed:.10f}")
     return res
 
 
 def main():
-
     s = "sin(x) + tan(y) / (sin(z)**2 + cos(z)**2)"
 
     mexpr = timed_parse("mexpress", mx.parse_f64, s)
     parser = Parser()
     axia = timed_parse("py_expression_eval", parser.parse, s)
     symp_expr = timed_parse("sympy", sympify, s)
```

### Comparing `mexpress-0.1.5/py/demo/opt.py` & `mexpress-0.1.6/demo/opt.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         f"{elapsed:.10f} sec",
         f"jac {str(jac is not None):5}",
         f"hess {str(hess is not None):5}",
     )
 
 
 def main(func_str):
-
     methods = [
         ("CG", lambda f: f.grad, lambda _: None),
         ("CG", lambda _: None, lambda _: None),
         ("Newton-CG", lambda f: f.grad, lambda f: f.hess),
         ("Newton-CG", lambda f: f.grad, lambda _: None),
         ("trust-krylov", lambda f: f.grad, lambda f: f.hess),  # needs Hessian
         ("trust-ncg", lambda f: f.grad, lambda f: f.hess),  # needs Hessian
```

### Comparing `mexpress-0.1.5/py/mexpress/__init__.py` & `mexpress-0.1.6/mexpress/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from .mexpress import native_parse_f64, native_parse_f32
+from mexpress import _mexpress as mx
 
 
 def _transform_x(x):
     x = np.asarray(x)
     # since we want to have both options f(*x) and f(x) we need to check the dimension
     return x if x.ndim == 1 else x.squeeze()
 
@@ -52,12 +52,12 @@
         return hess
 
     def __str__(self) -> str:
         return self.interfex.unparse()
 
 
 def parse_f64(s: str) -> Mexpress:
-    return Mexpress(native_parse_f64(s.replace("**", "^")), dtype=np.float64)
+    return Mexpress(mx.native_parse_f64(s.replace("**", "^")), dtype=np.float64)
 
 
 def parse_f32(s: str) -> Mexpress:
-    return Mexpress(native_parse_f32(s.replace("**", "^")), dtype=np.float32)
+    return Mexpress(mx.native_parse_f32(s.replace("**", "^")), dtype=np.float32)
```

### Comparing `mexpress-0.1.5/py/test/test_meta.py` & `mexpress-0.1.6/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `mexpress-0.1.5/py/test/test_mexpress.py` & `mexpress-0.1.6/test/test_mexpress.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 
 def _assert_float_eq(x, y, tol=1e-12):
     assert np.linalg.norm(x - y) < tol
 
 
 def test_eval():
-
     with pytest.raises(TypeError):
         mx.parse_f64("")
 
     expr = mx.parse_f64("x^2 + 7")
     _assert_float_eq(expr(2.0), 11)
 
     expr = mx.parse_f64("x^2 + 7")
@@ -38,15 +37,14 @@
     expr = mx.parse_f64("2*x + y^2 + cos(z) + sin(Δ)")
     ref = lambda _, y, z, Δ: (2, 2 * y, -np.sin(z), np.cos(Δ))
     x = np.random.random(4)
     _assert_float_eq(expr.grad(*x), ref(*x))
 
 
 def test_hess():
-
     expr = mx.parse_f64("2*x * y**2 + cos(z) + sin(Δ)")
     res = expr.hess(2.0, 3.0, 4.0, 5.0)
     ref = np.array(
         [
             [0, 12, 0, 0],
             [12, 8, 0, 0],
             [0, 0, -np.cos(4), 0],
```

### Comparing `mexpress-0.1.5/src/lib.rs` & `mexpress-0.1.6/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-use std::fmt::Debug;
-use std::str::FromStr;
-
-use exmex::{Differentiate, Express, FlatEx};
+use exmex::{DiffDataType, Differentiate, Express, FlatEx};
 use num::Float;
-use numpy::PyArray1;
+use numpy::PyReadonlyArray1;
 use pyo3::exceptions::PyTypeError;
 use pyo3::prelude::*;
+use std::fmt::Debug;
+use std::str::FromStr;
 
 pub trait DataType: Clone + FromStr + Debug + Default {}
 impl<T: Clone + FromStr + Debug + Default> DataType for T {}
 
 fn partial<T>(expr: &FlatEx<T>, i: i64) -> PyResult<FlatEx<T>>
 where
-    T: Float + DataType,
+    T: Float + DiffDataType,
     <T as FromStr>::Err: Debug,
 {
     expr.clone()
         .partial(i as usize)
         .map_err(|e| PyTypeError::new_err(e.msg().to_string()))
 }
 
-fn eval<T>(expr: &FlatEx<T>, x: &PyArray1<T>) -> PyResult<T>
+fn eval<T>(expr: &FlatEx<T>, x: &PyReadonlyArray1<T>) -> PyResult<T>
 where
     T: DataType + Float + numpy::Element,
     <T as FromStr>::Err: Debug,
 {
-    unsafe {
-        expr.eval(x.as_slice()?)
-            .map_err(|e| PyTypeError::new_err(e.msg().to_string()))
-    }
+    expr.eval(x.as_slice()?)
+        .map_err(|e| PyTypeError::new_err(e.msg().to_string()))
 }
 
-fn unparse<T>(expr: &FlatEx<T>) -> PyResult<String> 
+fn unparse<T>(expr: &FlatEx<T>) -> PyResult<String>
 where
     T: Float + DataType,
     <T as FromStr>::Err: Debug,
 {
     Ok(expr.unparse().to_string())
 }
 
@@ -52,16 +49,16 @@
         #[pyclass]
         struct $interf_ex_name {
             expr: FlatEx<$float>,
         }
 
         #[pymethods]
         impl $interf_ex_name {
-            fn __call__(&self, x: &PyArray1<$float>) -> PyResult<$float> {
-                eval(&self.expr, x)
+            fn __call__(&self, x: PyReadonlyArray1<$float>) -> PyResult<$float> {
+                eval(&self.expr, &x)
             }
 
             fn partial(&self, i: i64) -> PyResult<$interf_ex_name> {
                 Ok(Self {
                     expr: partial(&self.expr, i)?,
                 })
             }
@@ -83,14 +80,14 @@
     };
 }
 
 interf_ex!(InterfExF64, f64, native_parse_f64);
 interf_ex!(InterfExF32, f32, native_parse_f32);
 
 #[pymodule]
-fn mexpress(_py: Python, m: &PyModule) -> PyResult<()> {
+fn _mexpress(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(native_parse_f64, m)?)?;
     m.add_class::<InterfExF64>()?;
     m.add_function(wrap_pyfunction!(native_parse_f32, m)?)?;
     m.add_class::<InterfExF32>()?;
     Ok(())
 }
```

### Comparing `mexpress-0.1.5/Cargo.lock` & `mexpress-0.1.6/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -27,29 +27,44 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "exmex"
-version = "0.17.2"
+version = "0.20.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "22ad4c3ff389c7cd2478a1ae0b45275cfea2d69028e949b01d54edc60f8e5c79"
+checksum = "b3d756a702ec06bb080cf553645cfec9adcc78c054ddb0a3436636f812d3553e"
 dependencies = [
  "lazy_static",
  "num",
  "regex",
  "smallvec",
 ]
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+
+[[package]]
+name = "instant"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+dependencies = [
+ "cfg-if",
+]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
@@ -76,30 +91,30 @@
 checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.5.0"
+version = "2.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mexpress"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
  "exmex",
  "num",
  "numpy",
  "pyo3",
 ]
 
@@ -114,17 +129,17 @@
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
+checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -190,17 +205,17 @@
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.18.0"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
+checksum = "ec170733ca37175f5d75a5bea5911d6ff45d2cd52849ce98b685394e4f2f37f4"
 dependencies = [
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
@@ -211,100 +226,111 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
 dependencies = [
+ "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
  "cfg-if",
+ "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "winapi",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
 version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
@@ -327,28 +353,40 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
+dependencies = [
+ "aho-corasick",
+ "memchr",
+ "regex-automata",
+ "regex-syntax",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -356,23 +394,23 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
-version = "1.10.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "1.0.109"
+version = "2.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -385,76 +423,32 @@
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
-
-[[package]]
-name = "windows-sys"
-version = "0.45.0"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets",
-]
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "windows-targets"
-version = "0.42.2"
+name = "winapi"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
 ]
 
 [[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "windows_x86_64_msvc"
-version = "0.42.2"
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
```

### Comparing `mexpress-0.1.5/PKG-INFO` & `mexpress-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mexpress
-Version: 0.1.5
+Version: 0.1.6
 Requires-Dist: numpy
 License-File: LICENSE
 Summary: Math parser and evaluator capable of computing gradients and Hessians.
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/bertiqwerty/mexpress
```

