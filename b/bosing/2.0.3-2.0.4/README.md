# Comparing `tmp/bosing-2.0.3.tar.gz` & `tmp/bosing-2.0.4.tar.gz`

## Comparing `bosing-2.0.3.tar` & `bosing-2.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 bosing-2.0.3/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-05-21 07:50:58.000000 bosing-2.0.3/.github/dependabot.yml
--rw-r--r--   0     1001      127      690 2024-05-21 07:50:58.000000 bosing-2.0.3/.github/workflows/auto-dep.yml
--rw-r--r--   0     1001      127     6323 2024-05-21 07:50:58.000000 bosing-2.0.3/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-05-21 07:50:58.000000 bosing-2.0.3/.gitignore
--rw-r--r--   0     1001      127      972 2024-05-21 07:50:58.000000 bosing-2.0.3/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-05-21 07:50:58.000000 bosing-2.0.3/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-05-21 07:50:58.000000 bosing-2.0.3/README.md
--rw-r--r--   0     1001      127    10767 2024-05-21 07:50:58.000000 bosing-2.0.3/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-05-21 07:50:58.000000 bosing-2.0.3/clippy.toml
--rw-r--r--   0     1001      127      634 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-05-21 07:50:58.000000 bosing-2.0.3/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-05-21 07:50:58.000000 bosing-2.0.3/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-05-21 07:50:58.000000 bosing-2.0.3/example/hann.py
--rw-r--r--   0     1001      127      788 2024-05-21 07:50:58.000000 bosing-2.0.3/example/interp.py
--rw-r--r--   0     1001      127      696 2024-05-21 07:50:58.000000 bosing-2.0.3/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-05-21 07:50:58.000000 bosing-2.0.3/example/schedule.py
--rw-r--r--   0     1001      127     2343 2024-05-21 07:50:58.000000 bosing-2.0.3/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-05-21 07:50:58.000000 bosing-2.0.3/ruff_defaults.toml
--rw-r--r--   0     1001      127    11370 2024-05-21 07:50:58.000000 bosing-2.0.3/src/executor.rs
--rw-r--r--   0     1001      127    63696 2024-05-21 07:50:58.000000 bosing-2.0.3/src/lib.rs
--rw-r--r--   0     1001      127    14545 2024-05-21 07:50:58.000000 bosing-2.0.3/src/pulse.rs
--rw-r--r--   0     1001      127     7540 2024-05-21 07:50:58.000000 bosing-2.0.3/src/quant.rs
--rw-r--r--   0     1001      127     2367 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     9689 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/grid/helper.rs
--rw-r--r--   0     1001      127     6941 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3145 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/play.rs
--rw-r--r--   0     1001      127     2010 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3577 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/simple.rs
--rw-r--r--   0     1001      127     3132 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/stack/helper.rs
--rw-r--r--   0     1001      127     7464 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule/stack.rs
--rw-r--r--   0     1001      127     7859 2024-05-21 07:50:58.000000 bosing-2.0.3/src/schedule.rs
--rw-r--r--   0     1001      127     7677 2024-05-21 07:50:58.000000 bosing-2.0.3/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-05-21 07:50:58.000000 bosing-2.0.3/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-05-21 07:50:58.000000 bosing-2.0.3/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-05-21 07:50:58.000000 bosing-2.0.3/tests/test_basic.py
--rw-r--r--   0     1001      127    21393 2024-05-21 07:51:10.000000 bosing-2.0.3/Cargo.lock
--rw-r--r--   0     1001      127     1863 2024-05-21 07:50:58.000000 bosing-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 bosing-2.0.4/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-05-22 06:29:47.000000 bosing-2.0.4/.github/dependabot.yml
+-rw-r--r--   0     1001      127      690 2024-05-22 06:29:47.000000 bosing-2.0.4/.github/workflows/auto-dep.yml
+-rw-r--r--   0     1001      127     6323 2024-05-22 06:29:47.000000 bosing-2.0.4/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-05-22 06:29:47.000000 bosing-2.0.4/.gitignore
+-rw-r--r--   0     1001      127      972 2024-05-22 06:29:47.000000 bosing-2.0.4/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-05-22 06:29:47.000000 bosing-2.0.4/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-05-22 06:29:47.000000 bosing-2.0.4/README.md
+-rw-r--r--   0     1001      127    10767 2024-05-22 06:29:47.000000 bosing-2.0.4/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-05-22 06:29:47.000000 bosing-2.0.4/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-05-22 06:29:47.000000 bosing-2.0.4/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-05-22 06:29:47.000000 bosing-2.0.4/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-05-22 06:29:47.000000 bosing-2.0.4/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-05-22 06:29:47.000000 bosing-2.0.4/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-05-22 06:29:47.000000 bosing-2.0.4/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-05-22 06:29:47.000000 bosing-2.0.4/example/schedule.py
+-rw-r--r--   0     1001      127     2362 2024-05-22 06:29:47.000000 bosing-2.0.4/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-05-22 06:29:47.000000 bosing-2.0.4/ruff_defaults.toml
+-rw-r--r--   0     1001      127    11370 2024-05-22 06:29:47.000000 bosing-2.0.4/src/executor.rs
+-rw-r--r--   0     1001      127    63451 2024-05-22 06:29:47.000000 bosing-2.0.4/src/lib.rs
+-rw-r--r--   0     1001      127    15789 2024-05-22 06:29:47.000000 bosing-2.0.4/src/pulse.rs
+-rw-r--r--   0     1001      127     7540 2024-05-22 06:29:47.000000 bosing-2.0.4/src/quant.rs
+-rw-r--r--   0     1001      127     2367 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     9689 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/grid/helper.rs
+-rw-r--r--   0     1001      127     6941 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3145 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2010 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3577 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     3132 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/stack/helper.rs
+-rw-r--r--   0     1001      127     7464 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule/stack.rs
+-rw-r--r--   0     1001      127     7859 2024-05-22 06:29:47.000000 bosing-2.0.4/src/schedule.rs
+-rw-r--r--   0     1001      127     7677 2024-05-22 06:29:47.000000 bosing-2.0.4/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-05-22 06:29:47.000000 bosing-2.0.4/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-05-22 06:29:47.000000 bosing-2.0.4/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-05-22 06:29:47.000000 bosing-2.0.4/tests/test_basic.py
+-rw-r--r--   0     1001      127    21810 2024-05-22 06:30:01.000000 bosing-2.0.4/Cargo.lock
+-rw-r--r--   0     1001      127     1863 2024-05-22 06:29:47.000000 bosing-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 bosing-2.0.4/PKG-INFO
```

### Comparing `bosing-2.0.3/Cargo.toml` & `bosing-2.0.4/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [package]
 name = "bosing"
-version = "2.0.3"
+version = "2.0.4"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
 
 [dependencies]
 anyhow = "1.0.82"
+biquad = "0.4.2"
 bspline = "1.1.0"
 cached = "0.50.0"
 float-cmp = "0.9.0"
 hashbrown = { version = "0.14.5", features = ["rayon"] }
 indoc = "2.0.5"
 itertools = "0.12.1"
 ndarray = { version = "0.15.6", features = ["rayon"] }
```

### Comparing `bosing-2.0.3/.github/workflows/auto-dep.yml` & `bosing-2.0.4/.github/workflows/auto-dep.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/.github/workflows/ci.yml` & `bosing-2.0.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/.gitignore` & `bosing-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/.readthedocs.yaml` & `bosing-2.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/LICENSE.txt` & `bosing-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/README.md` & `bosing-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/bosing.pyi` & `bosing-2.0.4/bosing.pyi`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/Makefile` & `bosing-2.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/_templates/autosummary/module.rst` & `bosing-2.0.4/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/conf.py` & `bosing-2.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/index.rst` & `bosing-2.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/instruction.rst` & `bosing-2.0.4/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/make.bat` & `bosing-2.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/docs/schedule.rst` & `bosing-2.0.4/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/flexible.py` & `bosing-2.0.4/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/hann.py` & `bosing-2.0.4/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/interp.py` & `bosing-2.0.4/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/overlap.py` & `bosing-2.0.4/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/schedule.py` & `bosing-2.0.4/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/example/schedule_stress.py` & `bosing-2.0.4/example/schedule_stress.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     t0 = time.perf_counter()
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
     iir = get_biquad([0.1, -0.1], [100e-9, 1e-6], 2e9)
     fir = [1, 0.1, 0.01, 0.001]
     channels = (
-        {f"xy{i}": Channel(3e6 * i, 2e9, 100000, iq_matrix=[[1, 0.1], [0.1, 1]]) for i in range(nxy)}
+        {f"xy{i}": Channel(3e6 * i, 2e9, 100000, iq_matrix=[[1, 0.1], [0.1, 1]], offset=[0.1, 0.2]) for i in range(nxy)}
         | {f"u{i}": Channel(0, 2e9, 100000, iir=iir, fir=fir, is_real=True) for i in range(nu)}
         | {f"m{i}": Channel(0, 2e9, 100000) for i in range(nm)}
     )
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     spline = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
     shapes = {
         "hann": Hann(),
```

### Comparing `bosing-2.0.3/ruff_defaults.toml` & `bosing-2.0.4/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/executor.rs` & `bosing-2.0.4/src/executor.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/lib.rs` & `bosing-2.0.4/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2019,101 +2019,77 @@
         // SAFETY: These arrays are just created.
         let array = unsafe { waveforms[n].bind(py).as_array_mut() };
         sampler.add_channel(n.clone(), array, c.sample_rate, c.delay, c.align_level);
     }
     if let Some((crosstalk, names)) = &crosstalk {
         sampler.set_crosstalk(crosstalk.as_array(), names.clone());
     }
-    sampler.sample(time_tolerance)?;
+    py.allow_threads(|| sampler.sample(time_tolerance))?;
     Ok(waveforms)
 }
 
-fn post_process<'py>(
-    py: Python<'py>,
-    w: &mut Bound<'py, PyArray2<f64>>,
-    c: &Channel,
-) -> PyResult<()> {
+fn post_process(py: Python, w: &mut Bound<PyArray2<f64>>, c: &Channel) -> PyResult<()> {
     if let Some(iq_matrix) = &c.iq_matrix {
-        apply_iq_matrix(w, iq_matrix.bind(py));
+        apply_iq_matrix(py, w, iq_matrix.bind(py));
     }
     if c.filter_offset {
         if let Some(offset) = &c.offset {
-            apply_offset(py, w, offset.bind(py))?;
+            apply_offset(py, w, offset.bind(py));
         }
         if let Some(iir) = &c.iir {
-            apply_iir(py, w, iir.bind(py))?;
+            apply_iir(py, w, iir.bind(py));
         }
         if let Some(fir) = &c.fir {
             apply_fir(py, w, fir.bind(py))?;
         }
     } else {
         if let Some(iir) = &c.iir {
-            apply_iir(py, w, iir.bind(py))?;
+            apply_iir(py, w, iir.bind(py));
         }
         if let Some(fir) = &c.fir {
             apply_fir(py, w, fir.bind(py))?;
         }
         if let Some(offset) = &c.offset {
-            apply_offset(py, w, offset.bind(py))?;
+            apply_offset(py, w, offset.bind(py));
         }
     }
     Ok(())
 }
 
-fn apply_iq_matrix(w: &mut Bound<PyArray2<f64>>, iq_matrix: &Bound<PyArray2<f64>>) {
+fn apply_iq_matrix(py: Python, w: &mut Bound<PyArray2<f64>>, iq_matrix: &Bound<PyArray2<f64>>) {
     let mut w = w.readwrite();
     let w = w.as_array_mut();
     let iq_matrix = iq_matrix.readonly();
     let iq_matrix = iq_matrix.as_array();
-    pulse::apply_iq_inplace(w, iq_matrix);
+    py.allow_threads(|| {
+        pulse::apply_iq_inplace(w, iq_matrix);
+    });
 }
 
-fn apply_offset(
-    py: Python,
-    w: &Bound<PyArray2<f64>>,
-    offset: &Bound<PyArray1<f64>>,
-) -> PyResult<()> {
-    let locals = PyDict::new_bound(py);
-    locals.set_item("w", w)?;
-    locals.set_item("offset", offset)?;
-    py.run_bound(
-        indoc! {"
-            import numpy as np
-            w += offset[:, np.newaxis]
-        "},
-        None,
-        Some(&locals),
-    )?;
-    Ok(())
+fn apply_offset(py: Python, w: &Bound<PyArray2<f64>>, offset: &Bound<PyArray1<f64>>) {
+    let mut w = w.readwrite();
+    let w = w.as_array_mut();
+    let offset = offset.readonly();
+    let offset = offset.as_array();
+    py.allow_threads(|| {
+        pulse::apply_offset_inplace(w, offset);
+    });
 }
 
-fn apply_iir<'py>(
-    py: Python<'py>,
-    w: &Bound<'py, PyArray2<f64>>,
-    iir: &Bound<'py, PyArray2<f64>>,
-) -> PyResult<()> {
-    let locals = PyDict::new_bound(py);
-    locals.set_item("w", w)?;
-    locals.set_item("iir", iir)?;
-    py.run_bound(
-        indoc! {"
-            from scipy import signal
-            w[:] = signal.sosfilt(np.array(iir), w)
-        "},
-        None,
-        Some(&locals),
-    )?;
-    Ok(())
+fn apply_iir(py: Python, w: &Bound<PyArray2<f64>>, iir: &Bound<PyArray2<f64>>) {
+    let mut w = w.readwrite();
+    let w = w.as_array_mut();
+    let iir = iir.readonly();
+    let iir = iir.as_array();
+    py.allow_threads(|| {
+        pulse::apply_iir_inplace(w, iir);
+    });
 }
 
-fn apply_fir<'py>(
-    py: Python<'py>,
-    w: &Bound<'py, PyArray2<f64>>,
-    fir: &Bound<'py, PyArray1<f64>>,
-) -> PyResult<()> {
+fn apply_fir(py: Python, w: &Bound<PyArray2<f64>>, fir: &Bound<PyArray1<f64>>) -> PyResult<()> {
     let locals = PyDict::new_bound(py);
     locals.set_item("w", w)?;
     locals.set_item("fir", fir)?;
     py.run_bound(
         indoc! {"
             from scipy import signal
             for wi in w:
```

### Comparing `bosing-2.0.3/src/pulse.rs` & `bosing-2.0.4/src/pulse.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 use std::{
     ops::{Add, Mul},
     sync::Arc,
 };
 
 use anyhow::{bail, Context, Result};
+use biquad::Biquad as _;
 use cached::proc_macro::cached;
 use float_cmp::approx_eq;
 use hashbrown::HashMap;
 use itertools::{izip, Itertools};
-use ndarray::{s, ArrayView2, ArrayViewMut2};
+use ndarray::{azip, s, ArrayView1, ArrayView2, ArrayViewMut2, Axis};
 use numpy::Complex64;
 use rayon::prelude::*;
 
 use crate::{
     quant::{AlignedIndex, Amplitude, ChannelId, Frequency, Phase, Time},
     shape::Shape,
 };
@@ -467,7 +468,43 @@
             iq_matrix[(0, 0)] * col[0] + iq_matrix[(0, 1)] * col[1],
             iq_matrix[(1, 0)] * col[0] + iq_matrix[(1, 1)] * col[1],
         ];
         col[0] = y[0];
         col[1] = y[1];
     }
 }
+
+pub(crate) fn apply_offset_inplace(mut waveform: ArrayViewMut2<f64>, offset: ArrayView1<f64>) {
+    assert!(waveform.shape()[0] == offset.len());
+    azip!((mut row in waveform.axis_iter_mut(Axis(0)), &offset in &offset) row += offset);
+}
+
+pub(crate) fn apply_iir_inplace(mut waveform: ArrayViewMut2<f64>, sos: ArrayView2<f64>) {
+    let mut biquads: Vec<_> = sos
+        .axis_iter(Axis(0))
+        .map(|row| {
+            let b0 = row[0];
+            let b1 = row[1];
+            let b2 = row[2];
+            let a1 = row[4];
+            let a2 = row[5];
+            let coef = biquad::Coefficients { b0, a1, a2, b1, b2 };
+            biquad::DirectForm2Transposed::<f64>::new(coef)
+        })
+        .collect();
+    for mut row in waveform.axis_iter_mut(Axis(0)) {
+        apply_iir_inplace_1d(row.as_slice_mut().unwrap(), &mut biquads);
+    }
+}
+
+fn apply_iir_inplace_1d(waveform: &mut [f64], biquads: &mut [biquad::DirectForm2Transposed<f64>]) {
+    for biquad in biquads.iter_mut() {
+        biquad.reset_state();
+    }
+    for y in waveform.iter_mut() {
+        let mut x = *y;
+        for biquad in biquads.iter_mut() {
+            x = biquad.run(x);
+        }
+        *y = x;
+    }
+}
```

### Comparing `bosing-2.0.3/src/quant.rs` & `bosing-2.0.4/src/quant.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/absolute.rs` & `bosing-2.0.4/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/grid/helper.rs` & `bosing-2.0.4/src/schedule/grid/helper.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/grid.rs` & `bosing-2.0.4/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/play.rs` & `bosing-2.0.4/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/repeat.rs` & `bosing-2.0.4/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/simple.rs` & `bosing-2.0.4/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/stack/helper.rs` & `bosing-2.0.4/src/schedule/stack/helper.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule/stack.rs` & `bosing-2.0.4/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/schedule.rs` & `bosing-2.0.4/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/src/shape.rs` & `bosing-2.0.4/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/tests/test_basic.py` & `bosing-2.0.4/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/Cargo.lock` & `bosing-2.0.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -35,24 +35,34 @@
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
+name = "biquad"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "820524f5e3e3add696ddf69f79575772e152c0e78e9f0370b56990a7e808ec3e"
+dependencies = [
+ "libm",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.3"
+version = "2.0.4"
 dependencies = [
  "anyhow",
+ "biquad",
  "bspline",
  "cached",
  "float-cmp",
  "hashbrown",
  "indoc",
  "itertools",
  "mockall",
@@ -264,14 +274,20 @@
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
+name = "libm"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fc7aa29613bd6a620df431842069224d8bc9011086b1db4c0e0cd47fa03ec9a"
+
+[[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
```

### Comparing `bosing-2.0.3/pyproject.toml` & `bosing-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.3/PKG-INFO` & `bosing-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.3
+Version: 2.0.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

