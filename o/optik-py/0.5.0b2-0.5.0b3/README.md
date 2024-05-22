# Comparing `tmp/optik_py-0.5.0b2.tar.gz` & `tmp/optik_py-0.5.0b3.tar.gz`

## Comparing `optik_py-0.5.0b2.tar` & `optik_py-0.5.0b3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0     1001      127      688 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/Cargo.toml
--rw-r--r--   0     1001      127     2387 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/benches/bench.rs
--rw-r--r--   0     1001      127     1531 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/config.rs
--rw-r--r--   0     1001      127    10434 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/kinematics.rs
--rw-r--r--   0     1001      127    10708 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/lib.rs
--rw-r--r--   0     1001      127     6871 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/math.rs
--rw-r--r--   0     1001      127     3616 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/src/objective.rs
--rw-r--r--   0     1001      127     6888 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_fk_inputs.json
--rw-r--r--   0     1001      127    11169 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_fk_outputs.json
--rw-r--r--   0     1001      127     2281 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_inputs.json
--rw-r--r--   0     1001      127     1162 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_log.json
--rw-r--r--   0     1001      127     5836 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
--rw-r--r--   0     1001      127      808 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_log.json
--rw-r--r--   0     1001      127     1717 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
--rwxr-xr-x   0     1001      127    12531 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/data/ur3e.urdf
--rw-r--r--   0     1001      127      670 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_fk.rs
--rw-r--r--   0     1001      127     1829 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_gradient.rs
--rw-r--r--   0     1001      127     4300 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_ik.rs
--rw-r--r--   0     1001      127     1897 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik/tests/test_math.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/crates/optik-py/Cargo.toml
--rw-r--r--   0     1001      127       71 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik-py/build.rs
--rw-r--r--   0     1001      127     3458 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/crates/optik-py/src/lib.rs
--rw-r--r--   0     1001      127    31698 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/Cargo.lock
--rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/Cargo.toml
--rw-r--r--   0     1001      127      533 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/pyproject.toml
--rw-r--r--   0     1001      127     5866 2024-04-26 06:01:40.000000 optik_py-0.5.0b2/README.md
--rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 optik_py-0.5.0b2/PKG-INFO
+-rw-r--r--   0     1001      127      688 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/Cargo.toml
+-rw-r--r--   0     1001      127     2652 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/benches/bench.rs
+-rw-r--r--   0     1001      127     1531 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/src/config.rs
+-rw-r--r--   0     1001      127    10552 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/src/kinematics.rs
+-rw-r--r--   0     1001      127    10794 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/src/lib.rs
+-rw-r--r--   0     1001      127     6871 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/src/math.rs
+-rw-r--r--   0     1001      127     3612 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/src/objective.rs
+-rw-r--r--   0     1001      127     6888 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_fk_inputs.json
+-rw-r--r--   0     1001      127    11169 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_fk_outputs.json
+-rw-r--r--   0     1001      127     2281 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_math_inputs.json
+-rw-r--r--   0     1001      127     1162 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_se3_log.json
+-rw-r--r--   0     1001      127     5836 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
+-rw-r--r--   0     1001      127      808 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_so3_log.json
+-rw-r--r--   0     1001      127     1717 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
+-rwxr-xr-x   0     1001      127    12531 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/data/ur3e.urdf
+-rw-r--r--   0     1001      127      740 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/test_fk.rs
+-rw-r--r--   0     1001      127     1888 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/test_gradient.rs
+-rw-r--r--   0     1001      127     5183 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/test_ik.rs
+-rw-r--r--   0     1001      127     1897 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik/tests/test_math.rs
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 optik_py-0.5.0b3/crates/optik-py/Cargo.toml
+-rw-r--r--   0     1001      127       71 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik-py/build.rs
+-rw-r--r--   0     1001      127     3619 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/crates/optik-py/src/lib.rs
+-rw-r--r--   0     1001      127    29066 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/Cargo.lock
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 optik_py-0.5.0b3/Cargo.toml
+-rw-r--r--   0     1001      127      570 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/pyproject.toml
+-rw-r--r--   0     1001      127     5866 2024-05-22 16:07:12.000000 optik_py-0.5.0b3/README.md
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 optik_py-0.5.0b3/PKG-INFO
```

### Comparing `optik_py-0.5.0b2/crates/optik/Cargo.toml` & `optik_py-0.5.0b3/crates/optik/Cargo.toml`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/benches/bench.rs` & `optik_py-0.5.0b3/crates/optik/benches/bench.rs`

 * *Files 11% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     let robot = load_benchmark_model();
 
     let q = robot.random_configuration(&mut rand::thread_rng());
     let mut g = vec![0.0; q.len()];
     let tfm_target = Isometry3::identity();
 
     c.bench_function("gradient", |b| {
-        let fk = robot.fk(&q);
+        let fk = robot.fk(&q, &Isometry3::identity());
         b.iter(|| {
             objective_grad(
                 &robot,
                 &tfm_target,
                 &fk,
                 &mut g,
                 vector![1.0, 1.0, 1.0],
@@ -35,15 +35,15 @@
 
 fn bench_objective(c: &mut Criterion) {
     use optik::objective::objective;
 
     let robot = load_benchmark_model();
 
     let q = robot.random_configuration(&mut rand::thread_rng());
-    let fk = robot.fk(&q);
+    let fk = robot.fk(&q, &Isometry3::identity());
     let tfm_target = Isometry3::identity();
     c.bench_function("objective", |b| {
         b.iter(|| {
             objective(
                 &robot,
                 &tfm_target,
                 &fk,
@@ -54,34 +54,43 @@
     });
 }
 
 fn bench_fk(c: &mut Criterion) {
     let robot = load_benchmark_model();
     let x0 = vec![0.1, 0.2, 0.0, 0.3, -0.2, -1.1];
 
-    c.bench_function("fk", |b| b.iter(|| robot.fk(&x0)));
+    c.bench_function("fk", |b| b.iter(|| robot.fk(&x0, &Isometry3::identity())));
 }
 
 fn bench_joint_jacobian(c: &mut Criterion) {
     let robot = load_benchmark_model();
     let x0 = vec![0.1, 0.2, 0.0, 0.3, -0.2, -1.1];
 
-    let fk = robot.fk(&x0);
+    let fk = robot.fk(&x0, &Isometry3::identity());
     c.bench_function("joint_jacobian", |b| b.iter(|| robot.joint_jacobian(&fk)));
 }
 
 fn bench_ik(c: &mut Criterion) {
     let robot = load_benchmark_model();
     let config = SolverConfig::default();
 
     let x0 = vec![0.1, 0.2, 0.0, 0.3, -0.2, -1.1];
-    let tfm_target = robot.fk(&[-0.1, -0.2, 0.0, -0.3, 0.2, 1.1]).ee_tfm();
+    let tfm_target = robot
+        .fk(&[-0.1, -0.2, 0.0, -0.3, 0.2, 1.1], &Isometry3::identity())
+        .ee_tfm();
 
     c.bench_function("ik", |b| {
-        b.iter(|| robot.ik(&config, black_box(&tfm_target), x0.clone()))
+        b.iter(|| {
+            robot.ik(
+                &config,
+                black_box(&tfm_target),
+                &Isometry3::identity(),
+                x0.clone(),
+            )
+        })
     });
 }
 
 criterion_group!(
     benches,
     bench_gradient,
     bench_objective,
```

### Comparing `optik_py-0.5.0b2/crates/optik/src/config.rs` & `optik_py-0.5.0b3/crates/optik/src/config.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/src/kinematics.rs` & `optik_py-0.5.0b3/crates/optik/src/kinematics.rs`

 * *Files 4% similar despite different names*

```diff
@@ -109,22 +109,27 @@
         self.joints.iter().map(|j| j.typ.nq()).sum()
     }
 
     /// Computes the forward kinematics of this kinematic chain at the
     /// generalized position vector `q`.
     ///
     /// Panics of `q.len() != self.num_positions()`.
-    pub fn forward_kinematics(&self, q: &[f64]) -> ForwardKinematics {
+    pub fn forward_kinematics(&self, q: &[f64], ee_offset: &Isometry3<f64>) -> ForwardKinematics {
         let mut fk = ForwardKinematics::empty();
-        self.forward_kinematics_mut(q, &mut fk);
+        self.forward_kinematics_mut(q, ee_offset, &mut fk);
         fk
     }
 
     /// Like [`forward_kinematics()`], but mutate the given result in-place.
-    pub fn forward_kinematics_mut(&self, q: &[f64], fk: &mut ForwardKinematics) {
+    pub fn forward_kinematics_mut(
+        &self,
+        q: &[f64],
+        ee_offset: &Isometry3<f64>,
+        fk: &mut ForwardKinematics,
+    ) {
         assert_eq!(
             q.len(),
             self.num_positions(),
             "generalized position vector `q` is of incorrect length"
         );
 
         // To compute the forward kinematics, we scan across the ordered joints
@@ -151,15 +156,15 @@
                 Some(state.tfm)
             },
         );
 
         fk.joint_tfms.clear();
         fk.joint_tfms.extend(joint_tfms);
 
-        fk.ee_tfm = *fk.joint_tfms.last().unwrap();
+        fk.ee_tfm = *fk.joint_tfms.last().unwrap() * ee_offset;
     }
 
     pub fn joint_jacobian(&self, fk: &ForwardKinematics) -> Matrix6xX<f64> {
         let tfm_w_ee = fk.ee_tfm();
 
         let mut m = Matrix6xX::zeros(self.num_positions());
         let mut col = 0;
```

### Comparing `optik_py-0.5.0b2/crates/optik/src/lib.rs` & `optik_py-0.5.0b3/crates/optik/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -83,22 +83,23 @@
             .collect()
     }
 
     pub fn joint_jacobian(&self, fk: &ForwardKinematics) -> Matrix6xX<f64> {
         self.chain.joint_jacobian(fk)
     }
 
-    pub fn fk(&self, q: &[f64]) -> ForwardKinematics {
-        self.chain.forward_kinematics(q)
+    pub fn fk(&self, q: &[f64], ee_offset: &Isometry3<f64>) -> ForwardKinematics {
+        self.chain.forward_kinematics(q, ee_offset)
     }
 
     pub fn ik(
         &self,
         config: &SolverConfig,
         tfm_target: &Isometry3<f64>,
+        ee_offset: &Isometry3<f64>,
         x0: Vec<f64>,
     ) -> Option<(Vec<f64>, f64)> {
         // Complain if the provided seed is out side the joint limits. The
         // solver may be able to handle this, but it seems likely that there is
         // a bug in the user's program if this occurs and we should notify them.
         let (lb, ub) = self.joint_limits();
         if x0.iter().enumerate().any(|(i, q)| *q < lb[i] || *q > ub[i]) {
@@ -159,15 +160,15 @@
                             // thread has already found a satisfactory solution.
                             if is_timed_out() || should_exit.load(Ordering::Relaxed) {
                                 return None;
                             }
 
                             // Share kinematic results between the gradient and
                             // objective function evaluations, when possible.
-                            self.chain.forward_kinematics_mut(x, fk);
+                            self.chain.forward_kinematics_mut(x, ee_offset, fk);
 
                             // Compute the gradient only if it was requested by
                             // the optimizer.
                             if let Some(g) = grad {
                                 objective_grad(
                                     self,
                                     tfm_target,
```

### Comparing `optik_py-0.5.0b2/crates/optik/src/math.rs` & `optik_py-0.5.0b3/crates/optik/src/math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/src/objective.rs` & `optik_py-0.5.0b3/crates/optik/src/objective.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,27 @@
     angular_weight: &Vector3<f64>,
 ) -> Vector6<f64> {
     if !linear_weight.is_identity(IDENTITY_EPS) {
         // Rotate the error vector into the world frame.
         let e_lin_w = tfm_target * e.fixed_rows::<3>(0).clone_owned();
 
         // Apply the weights.
-        let e_lin_w_scaled = e_lin_w.component_mul(&linear_weight);
+        let e_lin_w_scaled = e_lin_w.component_mul(linear_weight);
 
         // Rotate back into the target frame.
         let e_lin_scaled = tfm_target.inverse_transform_vector(&e_lin_w_scaled);
         e.fixed_rows_mut::<3>(0).copy_from(&e_lin_scaled);
     }
 
     if !angular_weight.is_identity(IDENTITY_EPS) {
         // Rotate the error vector into the world frame.
         let e_ang_w = tfm_target * e.fixed_rows::<3>(3).clone_owned();
 
         // Apply the weights.
-        let e_ang_w_scaled = e_ang_w.component_mul(&angular_weight);
+        let e_ang_w_scaled = e_ang_w.component_mul(angular_weight);
 
         // Rotate back into the target frame.
         let e_ang_scaled = tfm_target.inverse_transform_vector(&e_ang_w_scaled);
         e.fixed_rows_mut::<3>(3).copy_from(&e_ang_scaled);
     }
 
     e
@@ -45,15 +45,15 @@
     angular_weight: Vector3<f64>,
 ) -> f64 {
     // Compute the pose error w.r.t. the target pose:
     let x_world_act = fk.ee_tfm();
     let x_target_act = tfm_target.inv_mul(&x_world_act);
 
     let e = se3::log(&x_target_act);
-    let e = apply_weighting(e, &tfm_target, &linear_weight, &angular_weight);
+    let e = apply_weighting(e, tfm_target, &linear_weight, &angular_weight);
 
     // Minimize the sqaure Euclidean distance of the log pose error. We choose
     // to use the square distance due to its smoothness.
     e.norm_squared()
 }
 
 /// Compute the gradient `g` w.r.t. the local parameterization.
@@ -97,14 +97,14 @@
     //   f = || g ||^2
     //   h' = (f' ∘ g) * g' = (2.0 * log6(X)) * J
 
     let e = se3::log(&x_target_act);
 
     let linear_weight_2 = linear_weight.component_mul(&linear_weight);
     let angular_weight_2 = angular_weight.component_mul(&angular_weight);
-    let e = apply_weighting(e, &tfm_target, &linear_weight_2, &angular_weight_2);
+    let e = apply_weighting(e, tfm_target, &linear_weight_2, &angular_weight_2);
 
     let fdot_g = 2.0 * e.transpose();
     let grad_h = fdot_g * j_task;
 
     g.copy_from_slice(grad_h.as_slice());
 }
```

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_fk_inputs.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_fk_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_fk_outputs.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_fk_outputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_math_inputs.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_math_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_log.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_se3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_log.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_so3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json` & `optik_py-0.5.0b3/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/data/ur3e.urdf` & `optik_py-0.5.0b3/crates/optik/tests/data/ur3e.urdf`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik/tests/test_fk.rs` & `optik_py-0.5.0b3/crates/optik/tests/test_fk.rs`

 * *Files 10% similar despite different names*

```diff
@@ -13,10 +13,14 @@
 #[test]
 fn test_fk() {
     let inputs: Vec<Vec<f64>> = fetch_data!("data/test_fk_inputs.json");
     let outputs: Vec<Isometry3<f64>> = fetch_data!("data/test_fk_outputs.json");
 
     let robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
     for (input, output) in inputs.into_iter().zip(outputs) {
-        assert_abs_diff_eq!(robot.fk(&input).ee_tfm(), output, epsilon = 1e-6);
+        assert_abs_diff_eq!(
+            robot.fk(&input, &Isometry3::identity()).ee_tfm(),
+            output,
+            epsilon = 1e-6
+        );
     }
 }
```

### Comparing `optik_py-0.5.0b2/crates/optik/tests/test_gradient.rs` & `optik_py-0.5.0b3/crates/optik/tests/test_gradient.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use approx::assert_abs_diff_eq;
-use nalgebra::{vector, DVector, Vector6};
+use nalgebra::{vector, DVector, Isometry3, Vector6};
 use optik::{
     objective::{objective, objective_grad},
     Robot,
 };
 use rand::{rngs::StdRng, Rng, SeedableRng};
 
 const TEST_MODEL_STR: &str = include_str!("data/ur3e.urdf");
@@ -34,18 +34,18 @@
 #[test]
 fn test_gradient_analytical_vs_numerical() {
     let robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
     let linear_weight = vector![0.0, 5.0, 0.25];
     let angular_weight = vector![0.005, 1.0, 0.99];
 
     let mut rng = StdRng::seed_from_u64(42);
-    for i in 0..100 {
+    for _ in 0..100 {
         let x0: Vector6<f64> = rng.gen();
         let tfm_target = rng.gen();
-        let fk = robot.fk(x0.as_slice());
+        let fk = robot.fk(x0.as_slice(), &Isometry3::identity());
 
         // Analytical gradient
         let mut g_a = Vector6::zeros();
         objective_grad(
             &robot,
             &tfm_target,
             &fk,
@@ -53,15 +53,15 @@
             linear_weight,
             angular_weight,
         );
 
         // Numerical gradient
         let g_n = finite_difference(
             |x| {
-                let fk = robot.fk(x);
+                let fk = robot.fk(x, &Isometry3::identity());
                 objective(&robot, &tfm_target, &fk, linear_weight, angular_weight)
             },
             x0.as_slice(),
         );
 
         assert_abs_diff_eq!(g_a.as_slice(), g_n.as_slice(), epsilon = 1e-6);
     }
```

### Comparing `optik_py-0.5.0b2/crates/optik/tests/test_ik.rs` & `optik_py-0.5.0b3/crates/optik/tests/test_ik.rs`

 * *Files 27% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     let config = SolverConfig::default();
     let tfm_target = Isometry3::identity();
 
     let (_, ub) = robot.joint_limits();
     let mut x0 = vec![0.0; 6];
     x0[4] = ub[4] + 1.0;
 
-    robot.ik(&config, &tfm_target, x0);
+    robot.ik(&config, &tfm_target, &Isometry3::identity(), x0);
 }
 
 #[test]
 fn test_stopping_maxtime() {
     const MAX_TIME: f64 = 0.05;
 
     let robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
@@ -31,47 +31,59 @@
 
     let config = SolverConfig {
         max_time: MAX_TIME,
         ..Default::default()
     };
 
     let start = Instant::now();
-    robot.ik(&config, &tfm_target, x0);
+    robot.ik(&config, &tfm_target, &Isometry3::identity(), x0);
     let end = Instant::now();
     let duration = end - start;
 
     assert_abs_diff_eq!(duration.as_secs_f64(), MAX_TIME, epsilon = 1e-1);
 }
 
 #[test]
 fn test_determinism() {
     let mut robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
     robot.set_parallelism(1);
 
     let mut rng = StdRng::seed_from_u64(42);
     let x_target: Vector6<f64> = rng.gen();
-    let tfm_target = robot.fk(x_target.as_slice()).ee_tfm();
+    let tfm_target = robot
+        .fk(x_target.as_slice(), &Isometry3::identity())
+        .ee_tfm();
 
     let config = SolverConfig {
         max_time: 0.0,
         max_restarts: 25,
         ..Default::default()
     };
     let x_sol = DVector::from(
         robot
-            .ik(&config, &tfm_target, vec![0.0; robot.num_positions()])
+            .ik(
+                &config,
+                &tfm_target,
+                &Isometry3::identity(),
+                vec![0.0; robot.num_positions()],
+            )
             .unwrap()
             .0,
     );
 
     // `robot.ik()` should return the same solution every time.
     for _ in 0..10 {
         let x_sol_i = DVector::from(
             robot
-                .ik(&config, &tfm_target, vec![0.0; robot.num_positions()])
+                .ik(
+                    &config,
+                    &tfm_target,
+                    &Isometry3::identity(),
+                    vec![0.0; robot.num_positions()],
+                )
                 .unwrap()
                 .0,
         );
 
         assert_abs_diff_eq!(x_sol, x_sol_i, epsilon = 1e-6);
     }
 }
@@ -88,23 +100,30 @@
         max_time: 0.0,
         max_restarts: 25,
         ..Default::default()
     };
 
     for _ in 0..10 {
         let x_target: Vector6<f64> = rng.gen();
-        let tfm_target = robot.fk(x_target.as_slice()).ee_tfm();
+        let tfm_target = robot
+            .fk(x_target.as_slice(), &Isometry3::identity())
+            .ee_tfm();
 
         let x_sol = DVector::from(
             robot
-                .ik(&config, &tfm_target, vec![0.0; robot.num_positions()])
+                .ik(
+                    &config,
+                    &tfm_target,
+                    &Isometry3::identity(),
+                    vec![0.0; robot.num_positions()],
+                )
                 .unwrap()
                 .0,
         );
-        let tfm_sol = robot.fk(x_sol.as_slice()).ee_tfm();
+        let tfm_sol = robot.fk(x_sol.as_slice(), &Isometry3::identity()).ee_tfm();
 
         // NOTE: epsilon here isn't exactly the same as the epsilon we pass into
         // the solver since we're not comparing within the manifold here. I've
         // chosen a reasonable epsilon here that passes the test with the given
         // solver tolerance.
         assert_abs_diff_eq!(tfm_target, tfm_sol, epsilon = 1e-6);
     }
@@ -126,20 +145,37 @@
         solution_mode: SolutionMode::Quality,
         ..config_speed
     };
 
     for _ in 0..20 {
         let x0 = vec![0.0; robot.num_positions()];
         let x_target: Vector6<f64> = rng.gen();
-        let tfm_target = robot.fk(x_target.as_slice()).ee_tfm();
+        let tfm_target = robot
+            .fk(x_target.as_slice(), &Isometry3::identity())
+            .ee_tfm();
 
-        let sol_speed = DVector::from(robot.ik(&config_speed, &tfm_target, x0.clone()).unwrap().0);
+        let sol_speed = DVector::from(
+            robot
+                .ik(
+                    &config_speed,
+                    &tfm_target,
+                    &Isometry3::identity(),
+                    x0.clone(),
+                )
+                .unwrap()
+                .0,
+        );
         let sol_quality = DVector::from(
             robot
-                .ik(&config_quality, &tfm_target, x0.clone())
+                .ik(
+                    &config_quality,
+                    &tfm_target,
+                    &Isometry3::identity(),
+                    x0.clone(),
+                )
                 .unwrap()
                 .0,
         );
 
         let x0 = DVector::from_row_slice(x0.as_slice());
         assert!(sol_quality.metric_distance(&x0) <= sol_speed.metric_distance(&x0));
     }
```

### Comparing `optik_py-0.5.0b2/crates/optik/tests/test_math.rs` & `optik_py-0.5.0b3/crates/optik/tests/test_math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/crates/optik-py/src/lib.rs` & `optik_py-0.5.0b3/crates/optik-py/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #![allow(non_local_definitions)] // silence warning from pyo3::pymethods macro
 
 use optik::{Robot, SolverConfig};
 
 use nalgebra::{Isometry3, Matrix4};
 use pyo3::prelude::*;
 
+fn parse_pose(v: Vec<Vec<f64>>) -> Isometry3<f64> {
+    let m = Matrix4::from_iterator(v.into_iter().flatten()).transpose();
+    nalgebra::try_convert(m).expect("invalid target transform specified")
+}
+
 #[pyclass]
 #[pyo3(name = "SolverConfig")]
 struct PySolverConfig(SolverConfig);
 
 #[pymethods]
 impl PySolverConfig {
     #[new]
@@ -74,56 +79,53 @@
 
         (
             robot.joint_limits().0.as_slice().to_vec(),
             robot.joint_limits().1.as_slice().to_vec(),
         )
     }
 
-    fn joint_jacobian(&self, x: Vec<f64>) -> Vec<Vec<f64>> {
+    fn joint_jacobian(&self, x: Vec<f64>, ee_offset: Vec<Vec<f64>>) -> Vec<Vec<f64>> {
         let robot = &self.0;
 
         assert_eq!(x.len(), robot.num_positions());
 
-        let fk = robot.fk(&x);
+        let fk = robot.fk(&x, &parse_pose(ee_offset));
         let jac = robot.joint_jacobian(&fk);
         jac.row_iter()
             .map(|row| row.iter().copied().collect())
             .collect()
     }
 
-    fn fk(&self, x: Vec<f64>) -> Vec<Vec<f64>> {
+    fn fk(&self, x: Vec<f64>, ee_offset: Vec<Vec<f64>>) -> Vec<Vec<f64>> {
         let robot = &self.0;
 
         assert_eq!(x.len(), robot.num_positions());
 
-        let ee_pose = robot.fk(&x).ee_tfm();
+        let ee_pose = robot.fk(&x, &parse_pose(ee_offset)).ee_tfm();
         ee_pose
             .to_matrix()
             .row_iter()
             .map(|row| row.iter().copied().collect())
             .collect()
     }
 
     fn ik(
         &self,
         config: &PySolverConfig,
         target: Vec<Vec<f64>>,
+        ee_offset: Vec<Vec<f64>>,
         x0: Vec<f64>,
     ) -> Option<(Vec<f64>, f64)> {
         let robot = &self.0;
 
         assert_eq!(x0.len(), self.num_positions());
 
-        fn parse_pose(v: Vec<Vec<f64>>) -> Isometry3<f64> {
-            let m = Matrix4::from_iterator(v.into_iter().flatten()).transpose();
-            nalgebra::try_convert(m).expect("invalid target transform specified")
-        }
-
         let target = parse_pose(target);
-        robot.ik(&config.0, &target, x0)
+        let ee_offset = parse_pose(ee_offset);
+        robot.ik(&config.0, &target, &ee_offset, x0)
     }
 }
 
 #[pymodule()]
 #[pyo3(name = "optik")]
 fn optik_extension(_py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyRobot>()?;
```

### Comparing `optik_py-0.5.0b2/Cargo.lock` & `optik_py-0.5.0b3/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -15,62 +15,62 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstyle"
-version = "1.0.6"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+checksum = "038dfcf04a5feb68e9c60b21c9625a54c2c0616e79b72b0fd87075a056ae1d1b"
 
 [[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -188,29 +188,29 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "either"
-version = "1.11.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -218,17 +218,17 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -239,17 +239,17 @@
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -308,29 +308,29 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -399,17 +399,17 @@
 source = "git+https://github.com/kylc/rust-nlopt.git?branch=optik-patches#050c9dc0000d5f896297de330cd7511af532cbe4"
 dependencies = [
  "cmake",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "num-integer"
@@ -418,28 +418,27 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
@@ -451,15 +450,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "optik"
-version = "0.5.0-beta.2"
+version = "0.5.0-beta.3"
 dependencies = [
  "approx",
  "criterion",
  "nalgebra",
  "nlopt",
  "ordered-float",
  "petgraph",
@@ -469,24 +468,24 @@
  "serde",
  "serde_json",
  "urdf-rs",
 ]
 
 [[package]]
 name = "optik-cpp"
-version = "0.5.0-beta.2"
+version = "0.5.0-beta.3"
 dependencies = [
  "nalgebra",
  "optik",
  "rand",
 ]
 
 [[package]]
 name = "optik-py"
-version = "0.5.0-beta.2"
+version = "0.5.0-beta.3"
 dependencies = [
  "nalgebra",
  "optik",
  "pyo3",
  "pyo3-build-config",
 ]
 
@@ -497,75 +496,75 @@
 checksum = "a76df7075c7d4d01fdcb46c912dd17fba5b60c78ea480b475f2b6ab6f666584e"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "paste"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
 
 [[package]]
 name = "petgraph"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
+checksum = "b4c5cc86750666a3ed20bdaf5ca2a0344f9c67674cae0515bec2da16fbaa47db"
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "plotters"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+checksum = "a15b6eccb8484002195a3e44fe65a4ce8e93a625797a063735536fd59cb01cf3"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+checksum = "414cec62c6634ae900ea1c56128dfe87cf63e7caece0852ec76aba307cebadb7"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.5"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+checksum = "81b30686a7d9c3e010b84284bdd26a29f2138574f52f5eb6f794fc0ad924e705"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -576,26 +575,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.83"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -603,55 +602,55 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -723,17 +722,17 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
@@ -761,17 +760,17 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "ryu"
-version = "1.0.17"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
@@ -791,37 +790,37 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -852,47 +851,47 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.65"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
@@ -966,15 +965,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -988,15 +987,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.65",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -1011,179 +1010,100 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.16"
+version = "0.7.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81a1851a719f11d1d2fea40e15c72f6c00de8c142d7ac47c1441cc7e4d0d5bc6"
+checksum = "21e005a4cc35784183a9e39cb22e9a9c46353ef6a7f113fd8d36ddc58c15ef3c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
-
-[[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.5",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
-dependencies = [
- "windows_aarch64_gnullvm 0.48.5",
- "windows_aarch64_msvc 0.48.5",
- "windows_i686_gnu 0.48.5",
- "windows_i686_msvc 0.48.5",
- "windows_x86_64_gnu 0.48.5",
- "windows_x86_64_gnullvm 0.48.5",
- "windows_x86_64_msvc 0.48.5",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.5",
- "windows_aarch64_msvc 0.52.5",
- "windows_i686_gnu 0.52.5",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
  "windows_i686_gnullvm",
- "windows_i686_msvc 0.52.5",
- "windows_x86_64_gnu 0.52.5",
- "windows_x86_64_gnullvm 0.52.5",
- "windows_x86_64_msvc 0.52.5",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
 
 [[package]]
 name = "windows_i686_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.48.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xml-rs"
 version = "0.8.20"
```

### Comparing `optik_py-0.5.0b2/README.md` & `optik_py-0.5.0b3/README.md`

 * *Files identical despite different names*

### Comparing `optik_py-0.5.0b2/PKG-INFO` & `optik_py-0.5.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: optik-py
-Version: 0.5.0b2
+Version: 0.5.0b3
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE(3)
 Author: Kyle Cesare
 Author-email: kcesare@gmail.com
 License: MIT OR Apache-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: optik-py Version: 0.5.0b2 Classifier: Topic ::
+Metadata-Version: 2.3 Name: optik-py Version: 0.5.0b3 Classifier: Topic ::
 Scientific/Engineering License-File: LICENSE-APACHE License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE
 (3) Author: Kyle Cesare Author-email: kcesare@gmail.com License: MIT OR Apache-
 2.0 Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://github.com/kylc/optik
 # OptIK
 _[_M_I_T_]_[_A_p_a_c_h_e_]_[_c_i_]_[_P_y_P_I_]_[_D_O_I_]
```

