# Comparing `tmp/grasp_planning-0.5.7.2.tar.gz` & `tmp/grasp_planning-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.7.2.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.8.tar", max compression
```

## Comparing `grasp_planning-0.5.7.2.tar` & `grasp_planning-0.5.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1734 2024-05-16 09:02:48.947350 grasp_planning-0.5.7.2/README.md
--rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.7.2/grasp_planning/__init__.py
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.7.2/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.7.2/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.7.2/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.7.2/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.7.2/grasp_planning/constraints/orientation_constraint.py
--rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.7.2/grasp_planning/constraints/position_constraint.py
--rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.7.2/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.7.2/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.7.2/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     7742 2024-05-17 19:31:19.299293 grasp_planning-0.5.7.2/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     6216 2024-05-18 19:54:55.776462 grasp_planning-0.5.7.2/grasp_planning/solver/ik_optim.py
--rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.7.2/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      557 2024-05-18 20:02:58.529614 grasp_planning-0.5.7.2/pyproject.toml
--rw-r--r--   0        0        0     2492 1970-01-01 00:00:00.000000 grasp_planning-0.5.7.2/PKG-INFO
+-rw-r--r--   0        0        0      157 2024-05-18 20:04:19.998478 grasp_planning-0.5.8/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.8/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-22 09:32:48.438806 grasp_planning-0.5.8/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.8/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      436 2024-05-22 10:59:21.260147 grasp_planning-0.5.8/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1066 2024-05-22 08:58:55.104348 grasp_planning-0.5.8/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     2538 2024-05-22 09:01:12.368920 grasp_planning-0.5.8/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.8/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.8/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1017 2024-05-22 08:57:22.264146 grasp_planning-0.5.8/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      735 2024-05-22 11:00:19.296615 grasp_planning-0.5.8/grasp_planning/constraints/z_height_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.8/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.8/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.8/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     9377 2024-05-22 11:02:20.573531 grasp_planning-0.5.8/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     5982 2024-05-22 11:15:51.079421 grasp_planning-0.5.8/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.8/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      555 2024-05-22 11:27:30.547240 grasp_planning-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 grasp_planning-0.5.8/PKG-INFO
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/collision_constraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
         super().__init__() 
         self._robot = robot
         self.tolerance = tolerance
         self.r_link = r_link
         self.r_obst = r_obst
         self.d_safety = tolerance
         
-        T_W_link = self._robot.compute_fk_ca(q_ca, link_name)
+        T_W_link = self._robot.compute_fk_ca(q_ca[:,waypoint_ID], link_name)
 
-        self.g = ca.norm_2(T_W_link[:3,3]-param_obst_ca[:3,3]) #obstacle_pos
+        self.g = ca.norm_2(T_W_link[:3,3]-param_obst_ca) #obstacle_pos
         self.g_lb = self.r_link + self.r_obst + self.d_safety
         self.g_ub = float("inf")
 
 
     def get_constraint(self):
         return self.g, self.g_lb, self.g_ub
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/position_constraint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-class GraspPosConstraint(Constraint):
-    def __init__(self, robot, q_ca, waypoint_ID, param_grasp_ca, tolerance=0.0) -> None:
+class PositionConstraint(Constraint):
+    def __init__(self, robot, q_ca, paramca_T_W_Ref, tolerance=0.0) -> None:
         super().__init__() 
         # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
         # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
         # manip frame_pos - T_W_Grasp_pos = 0
         self._robot = robot
         self.tolerance = tolerance
-        Rpy_W_EEF = self._robot.compute_fk_rpy_ca(q_ca[:,waypoint_ID])
+        T_W_EEF = self._robot.compute_fk_ca(q_ca)
         
-        self.g = Rpy_W_EEF[:3] - param_grasp_ca[:3,3]
+        self.g = T_W_EEF[:3, 3] - paramca_T_W_Ref[:3,3]
         self.g_lb = np.zeros(3) - self.tolerance
         self.g_ub = np.zeros(3) + self.tolerance
-        self.g_eval = ca.Function('g_grasp_pos', [q_ca, param_grasp_ca], [self.g])
+        self.g_eval = ca.Function('g_pos', [q_ca, paramca_T_W_Ref], [self.g])
       
     def get_constraint(self):
         return self.g, self.g_lb, self.g_ub
 
-    def do_eval(self, q, T_W_Grasp):
-        return self.g_eval(q, T_W_Grasp)
+    def do_eval(self, q, T_W_Ref):
+        return self.g_eval(q, T_W_Ref)
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/orientation_constraint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-class GraspRotConstraint(Constraint):
-    def __init__(self, robot, q_ca, waypoint_ID, param_grasp_ca, theta=0.0, tolerance=0.1) -> None:
+class OrientationConstraint(Constraint):
+    def __init__(self, robot, q_ca, paramca_T_W_Ref, tolerance=0.0) -> None:
         super().__init__() 
         # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
         # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
         # manip frame_pos - T_W_Grasp_pos = 0
         self._robot = robot
-        self.theta = theta
         self.tolerance = tolerance
-        self.param_grasp_ca = param_grasp_ca
-        
-        R_W_EEF = self._robot.compute_fk_ca(q_ca[:,waypoint_ID])
-        R_G_EEF = self.param_grasp_ca[:3,:3].T @ R_W_EEF[:3,:3]
-        Rpy_G_EEF = sc.Rotation.from_matrix(R_G_EEF).as_euler("xyz")
-
-        self.g = ca.vertcat(Rpy_G_EEF[0], Rpy_G_EEF[1], Rpy_G_EEF[2])
-        self.g_lb = ca.vertcat(-self.tolerance, -self.theta, -self.tolerance)
-        self.g_ub = ca.vertcat(self.tolerance, self.theta, self.tolerance)
+        R_W_EEF = self._robot.compute_fk_ca(q_ca)[:3, :3]
+        R_W_Ref = paramca_T_W_Ref[:3,:3]
 
-        self.g_eval = ca.Function('g_grasp_rot', [q_ca, param_grasp_ca], [self.g])
+        
+        R_Ref_EEF= R_W_Ref.T @ R_W_EEF
+        self.g = ca.trace(R_Ref_EEF)
 
+        self.g_lb = 2*np.cos(tolerance) + 1.0
+        self.g_ub = ca.inf
+        self.g_eval = ca.Function('g_grasp_pos', [q_ca, paramca_T_W_Ref], [self.g])
+      
     def get_constraint(self):
         return self.g, self.g_lb, self.g_ub
 
-    def do_eval(self, q, T_W_Grasp):
-        return self.g_eval(q, T_W_Grasp)
+    def do_eval(self, q, T_W_Ref):
+        return self.g_eval(q, T_W_Ref)
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/orientation_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-class OrientationConstraint(Constraint):
-    def __init__(self, robot, q_ca, paramca_T_W_Ref, tolerance=0.0) -> None:
+class GraspPosConstraint(Constraint):
+    def __init__(self, robot, q_ca, waypoint_ID, paramca_T_W_Grasp, tolerance=0.0) -> None:
         super().__init__() 
         # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
         # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
         # manip frame_pos - T_W_Grasp_pos = 0
         self._robot = robot
         self.tolerance = tolerance
-        R_W_EEF = self._robot.compute_fk_ca(q_ca)[:3, :3]
-        R_W_Ref = paramca_T_W_Ref[:3,:3]
-
+        Rpy_W_EEF = self._robot.compute_fk_rpy_ca(q_ca[:,waypoint_ID])
         
-        R_Ref_EEF= R_W_Ref.T @ R_W_EEF
-        self.g = ca.trace(R_Ref_EEF)
-
-        self.g_lb = 2*np.cos(tolerance) + 1.0
-        self.g_ub = ca.inf
-        self.g_eval = ca.Function('g_grasp_pos', [q_ca, paramca_T_W_Ref], [self.g])
+        self.g = Rpy_W_EEF[:3] - paramca_T_W_Grasp[:3,3]
+        self.g_lb = np.zeros(3) - self.tolerance
+        self.g_ub = np.zeros(3) + self.tolerance
+        self.g_eval = ca.Function('g_grasp_pos', [q_ca, paramca_T_W_Grasp], [self.g])
       
     def get_constraint(self):
         return self.g, self.g_lb, self.g_ub
 
-    def do_eval(self, q, T_W_Ref):
-        return self.g_eval(q, T_W_Ref)
+    def do_eval(self, q, T_W_Grasp):
+        return self.g_eval(q, T_W_Grasp)
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/constraints/position_constraint.py` & `grasp_planning-0.5.8/grasp_planning/constraints/z_height_constraint.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import numpy as np
 import casadi as ca
 import spatial_casadi as sc
 from grasp_planning.constraints.constraint_template import Constraint
 
-class PositionConstraint(Constraint):
-    def __init__(self, robot, q_ca, paramca_T_W_Ref, tolerance=0.0) -> None:
+class ZheightConstraint(Constraint):
+    def __init__(self, robot, q_ca, waypoint_ID, z_height, tolerance=0.0) -> None:
         super().__init__() 
-        # q = q_ca[:n_dof, waypoint_ID] -> joint space of the robot (decision variable)
-        # manip_frame = q_ca[n_dof:, waypoint_ID] -> manipulation frame (decision variable)
-        # manip frame_pos - T_W_Grasp_pos = 0
         self._robot = robot
         self.tolerance = tolerance
-        T_W_EEF = self._robot.compute_fk_ca(q_ca)
+        T_W_EEF = self._robot.compute_fk_ca(q_ca[:,waypoint_ID])
         
-        self.g = T_W_EEF[:3, 3] - paramca_T_W_Ref[:3,3]
-        self.g_lb = np.zeros(3) - self.tolerance
-        self.g_ub = np.zeros(3) + self.tolerance
-        self.g_eval = ca.Function('g_grasp_pos', [q_ca, paramca_T_W_Ref], [self.g])
+        self.g = T_W_EEF[2,3]
+        self.g_lb = z_height - self.tolerance
+        self.g_ub = float("inf")
+        self.g_eval = ca.Function('g_z_coord', [q_ca], [self.g])
       
     def get_constraint(self):
         return self.g, self.g_lb, self.g_ub
 
-    def do_eval(self, q, T_W_Ref):
-        return self.g_eval(q, T_W_Ref)
+    def do_eval(self, q):
+        return self.g_eval(q)
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.8/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.2/grasp_planning/solver/ik_optim.py` & `grasp_planning-0.5.8/grasp_planning/solver/ik_optim.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,20 +20,14 @@
         self.x = ca.SX.sym("x", self.x_dim, 1)
         self.x_init = None
         
         self._objective = None
         self.l_joint_limits, self.u_joint_limits = None, None
         self.g_list = []
 
-        self.param_T_W_Ref = ca.SX.sym("param_grasp", 4, 4)
-        self.param_obst_ca = ca.SX.sym("param_obst", 4, 4)
-        self.param_optim_ca = ca.vertcat()
-        self.param_ca_list = [self.param_T_W_Ref]
-        self._collision_flag = False
-
         self.param_ca_dict = dict()
 
 
     def set_init_guess(self, q):
         self.x_init = q
 
     def set_boundary_conditions(self):
@@ -75,15 +69,15 @@
 
         # Define solver
         self.solver = ca.nlpsol('solver', 'ipopt', {'x': self.x, 'f': self.objective.eval_cost(self.x), 'g': g, 'p': self._param_ca}, options)
     
 
         
     def solve(self):
-        # Read Symbolic Paramaters
+        # Replace symbolic variables with numeric values
         for i, param in enumerate(self.param_ca_dict):
             if i == 0:
                 self._param_num = self.param_ca_dict[param]["num_param"]
             else:
                 self._param_num = ca.vertcat(self._param_num, self.param_ca_dict[param]["num_param"].reshape((-1,1), order='F'))
 
         result = self.solver(x0=self.x_init,
@@ -94,61 +88,60 @@
                              p=self._param_num)
 
         success_flag = self.solver.stats()["success"]
         success_msg = self.solver.stats()["return_status"]
         return  result['x'], success_flag
     
 
-    def add_objective_function(self):
+    def add_objective_function(self, name):
         # Define parameter sym variable
-        name = "objective_param"
         self.param_ca_dict[name] =  {
             "sym_param" : ca.SX.sym(name, self.x_dim, 1),
             "num_param" : np.zeros((self.x_dim, 1))
             }
         # Create objective function
         self.objective = DistToHome(q_home=self.param_ca_dict[name]["sym_param"] ,
                                     n_dofs=self.x_dim)
       
-    def add_position_constraint(self, tolerance=0.0):
+    def add_position_constraint(self, name, tolerance=0.0):
         # Define parameter sym variable
-        name = "position_g_param"
         self.param_ca_dict[name] =  {
             "sym_param" : ca.SX.sym(name, 4, 4),
             "num_param" : np.eye(4)
             }
         # Create constraint
         self.g_list.append(PositionConstraint(robot=self._robot_model,
                                               q_ca=self.x,
                                               paramca_T_W_Ref=self.param_ca_dict[name]["sym_param"],
                                               tolerance=tolerance))
 
 
-    def add_orientation_constraint(self, tolerance=0.0):
+    def add_orientation_constraint(self, name, tolerance=0.0):
         # Define parameter sym variable
-        name = "orientation_g_param"
         self.param_ca_dict[name] =  {
             "sym_param" : ca.SX.sym(name, 4, 4),
-            "num_param" : np.eye(4)
+            "num_param" : np.eye(4),
+            "tolerance" : tolerance
             }
         # Create constraint
         self.g_list.append(OrientationConstraint(robot=self._robot_model,
                                                  q_ca=self.x,
                                                  paramca_T_W_Ref=self.param_ca_dict[name]["sym_param"],
                                                  tolerance=tolerance))
 
 
 
     
 
     def add_collision_constraint(self, name, link_names, r_link=0.5, r_obst=0.2, tolerance=0.01):
         # Define parameter sym variable
         self.param_ca_dict[name] =  {
-            "sym_param" : ca.SX.sym(name, 4, 4),
-            "num_param" : np.eye(4)
+            "sym_param" : ca.SX.sym(name, 3, 1),
+            "num_param" : np.zeros((3,1)),
+            "tolerance" : tolerance
             }
         # Create constraint
         for link in link_names:
             self.g_list.append(CollisionConstraint(robot=self._robot_model,
                                                     q_ca=self.x,
                                                     waypoint_ID=0,
                                                     param_obst_ca=self.param_ca_dict[name]["sym_param"],
```

### Comparing `grasp_planning-0.5.7.2/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.8/grasp_planning/solver/robot_model.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.7.2/pyproject.toml` & `grasp_planning-0.5.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grasp_planning"
-version = "0.5.7.2"
+version = "0.5.8"
 description = "\"Grasp and Motion Planning Python Package.\""
 authors = ["Tomas Merva <tmerva7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TomasMerva/gomp.git"
 repository = "https://github.com/TomasMerva/gomp.git"
```

