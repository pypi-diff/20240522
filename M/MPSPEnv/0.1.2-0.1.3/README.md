# Comparing `tmp/mpspenv-0.1.2.tar.gz` & `tmp/mpspenv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpspenv-0.1.2.tar", last modified: Tue May 21 14:14:42 2024, max compression
+gzip compressed data, was "mpspenv-0.1.3.tar", last modified: Wed May 22 09:32:28 2024, max compression
```

## Comparing `mpspenv-0.1.2.tar` & `mpspenv-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.041638 mpspenv-0.1.2/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.2/MANIFEST.in
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.038864 mpspenv-0.1.2/MPSPEnv/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.2/MPSPEnv/__init__.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.038001 mpspenv-0.1.2/MPSPEnv/c/
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.040994 mpspenv-0.1.2/MPSPEnv/c/src/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.2/MPSPEnv/c/src/array.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.2/MPSPEnv/c/src/array.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.2/MPSPEnv/c/src/bay.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.2/MPSPEnv/c/src/bay.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)    10621 2024-05-21 13:47:42.000000 mpspenv-0.1.2/MPSPEnv/c/src/env.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      620 2024-05-20 17:04:20.000000 mpspenv-0.1.2/MPSPEnv/c/src/env.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.2/MPSPEnv/c/src/random.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.2/MPSPEnv/c/src/random.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.2/MPSPEnv/c/src/sort.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.2/MPSPEnv/c/src/sort.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.2/MPSPEnv/c/src/transportation_matrix.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.2/MPSPEnv/c/src/transportation_matrix.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1904 2024-05-21 14:09:26.000000 mpspenv-0.1.2/MPSPEnv/c_interface.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7910 2024-05-21 14:10:38.000000 mpspenv-0.1.2/MPSPEnv/env.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.2/MPSPEnv/visualizer.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.041252 mpspenv-0.1.2/MPSPEnv.egg-info/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-21 14:14:42.000000 mpspenv-0.1.2/MPSPEnv.egg-info/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-21 14:14:42.000000 mpspenv-0.1.2/MPSPEnv.egg-info/SOURCES.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-21 14:14:42.000000 mpspenv-0.1.2/MPSPEnv.egg-info/dependency_links.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-21 14:14:42.000000 mpspenv-0.1.2/MPSPEnv.egg-info/requires.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-21 14:14:42.000000 mpspenv-0.1.2/MPSPEnv.egg-info/top_level.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-21 14:14:42.041455 mpspenv-0.1.2/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.2/README.md
--rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-21 14:14:42.041677 mpspenv-0.1.2/setup.cfg
--rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-21 14:14:23.000000 mpspenv-0.1.2/setup.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 14:14:42.041106 mpspenv-0.1.2/tests/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2546 2024-05-21 14:13:17.000000 mpspenv-0.1.2/tests/test_env.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469648 mpspenv-0.1.3/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.3/MANIFEST.in
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.466798 mpspenv-0.1.3/MPSPEnv/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.3/MPSPEnv/__init__.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.465975 mpspenv-0.1.3/MPSPEnv/c/
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469007 mpspenv-0.1.3/MPSPEnv/c/src/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.3/MPSPEnv/c/src/array.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.3/MPSPEnv/c/src/array.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.3/MPSPEnv/c/src/bay.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.3/MPSPEnv/c/src/bay.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)    10139 2024-05-22 09:25:42.000000 mpspenv-0.1.3/MPSPEnv/c/src/env.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      615 2024-05-22 09:26:14.000000 mpspenv-0.1.3/MPSPEnv/c/src/env.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.3/MPSPEnv/c/src/random.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.3/MPSPEnv/c/src/random.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.3/MPSPEnv/c/src/sort.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.3/MPSPEnv/c/src/sort.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1909 2024-05-22 09:21:19.000000 mpspenv-0.1.3/MPSPEnv/c_interface.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7469 2024-05-22 09:22:28.000000 mpspenv-0.1.3/MPSPEnv/env.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.3/MPSPEnv/visualizer.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469269 mpspenv-0.1.3/MPSPEnv.egg-info/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/requires.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-22 09:32:28.000000 mpspenv-0.1.3/MPSPEnv.egg-info/top_level.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-22 09:32:28.469450 mpspenv-0.1.3/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.3/README.md
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-22 09:32:28.469690 mpspenv-0.1.3/setup.cfg
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-22 09:32:12.000000 mpspenv-0.1.3/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-22 09:32:28.469129 mpspenv-0.1.3/tests/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2503 2024-05-22 09:22:28.000000 mpspenv-0.1.3/tests/test_env.py
```

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/array.c` & `mpspenv-0.1.3/MPSPEnv/c/src/array.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/array.h` & `mpspenv-0.1.3/MPSPEnv/c/src/array.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/bay.c` & `mpspenv-0.1.3/MPSPEnv/c/src/bay.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/bay.h` & `mpspenv-0.1.3/MPSPEnv/c/src/bay.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/env.c` & `mpspenv-0.1.3/MPSPEnv/c/src/env.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,14 @@
 #include "env.h"
 #include "bay.h"
 #include <assert.h>
 #include <stdio.h>
 #include <stdlib.h>
 #include <string.h>
 
-void insert_flat_T_matrix(Env env)
-{
-    int index = 0;
-
-    // Upper Triangular Indeces:
-    // i in [0, N)
-    // j in [i + 1, N]
-    for (int i = 0; i < env.T->N - 1; i++)
-    {
-        for (int j = i + 1; j < env.T->N; j++)
-        {
-            env.flat_T_matrix.values[index] = env.T->matrix.values[i * env.T->N + j];
-            index++;
-        }
-    }
-}
-
 int columns_identical(Bay bay, int c1, int c2)
 {
     for (int r = bay.R - 1; r >= 0; r--)
     {
         int value1 = bay.matrix.values[r * bay.C + c1];
         int value2 = bay.matrix.values[r * bay.C + c2];
 
@@ -136,20 +119,14 @@
     }
     if (n_legal_actions == 1)
         return last_legal_action;
     else
         return -1;
 }
 
-void initialize_flat_T(Env *env, int N)
-{
-    int upper_triangle_size = (N * (N - 1)) / 2;
-    env->flat_T_matrix = get_zeros(upper_triangle_size);
-}
-
 Env build_env(int R, int C, int N, int auto_move, Transportation_Info *T)
 {
     assert(R > 0 && C > 0 && N > 0);
     assert(auto_move == 0 || auto_move == 1);
     Env env;
 
     env.auto_move = auto_move;
@@ -158,16 +135,16 @@
     env.mask = get_zeros(2 * env.bay.R * env.bay.C);
     env.total_reward = malloc(sizeof(int));
     *env.total_reward = 0;
     env.containers_placed = malloc(sizeof(int));
     *env.containers_placed = 0;
     env.containers_left = malloc(sizeof(int));
     *env.containers_left = get_sum(T->matrix);
-    initialize_flat_T(&env, N);
-    insert_flat_T_matrix(env);
+    env.terminated = malloc(sizeof(int));
+    *env.terminated = 0;
 
     int only_legal_action = insert_mask(env);
     if (auto_move && only_legal_action != -1)
     {
         step(env, only_legal_action);
     }
 
@@ -187,36 +164,37 @@
 }
 
 Env copy_env(Env env)
 {
     Env copy;
     copy.T = copy_transportation_info(env.T);
     copy.bay = copy_bay(env.bay);
-    copy.flat_T_matrix = copy_array(env.flat_T_matrix);
     copy.mask = copy_array(env.mask);
     copy.auto_move = env.auto_move;
     copy.total_reward = malloc(sizeof(int));
     *copy.total_reward = *env.total_reward;
     copy.containers_placed = malloc(sizeof(int));
     *copy.containers_placed = *env.containers_placed;
     copy.containers_left = malloc(sizeof(int));
     *copy.containers_left = *env.containers_left;
+    copy.terminated = malloc(sizeof(int));
+    *copy.terminated = *env.terminated;
 
     return copy;
 }
 
 void free_env(Env env)
 {
     free_bay(env.bay);
     free_transportation_matrix(env.T);
-    free_array(env.flat_T_matrix);
     free_array(env.mask);
     free(env.total_reward);
     free(env.containers_placed);
     free(env.containers_left);
+    free(env.terminated);
 }
 
 int get_add_reward(Env env, int column, int next_container, int n_containers)
 {
     if (is_container_blocking(env.bay, column, next_container))
         return -n_containers;
     else
@@ -311,17 +289,17 @@
 
 StepInfo step(Env env, int action)
 {
     assert(action >= 0 && action < 2 * env.bay.C * env.bay.R);
     assert(env.mask.values[action] == 1);
     StepInfo step_info;
     step_info.reward = step_action(env, action);
-    step_info.is_terminal = decide_is_terminated(env);
+    step_info.terminated = decide_is_terminated(env);
+    *env.terminated = step_info.terminated;
     *env.total_reward += step_info.reward;
 
-    insert_flat_T_matrix(env);
     int only_legal_action = insert_mask(env);
-    if (env.auto_move && !step_info.is_terminal && only_legal_action != -1)
+    if (env.auto_move && !step_info.terminated && only_legal_action != -1)
         return step(env, only_legal_action);
 
     return step_info;
 }
```

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/env.h` & `mpspenv-0.1.3/MPSPEnv/c/src/env.h`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 #include "bay.h"
 #include "array.h"
 
 typedef struct Env
 {
     Transportation_Info *T;
     Bay bay;
-    Array flat_T_matrix;
     Array mask;
     int auto_move;
     int *total_reward;
     int *containers_left;
     int *containers_placed;
+    int *terminated;
 } Env;
 
 typedef struct StepInfo
 {
-    int is_terminal;
+    int terminated;
     int reward;
 } StepInfo;
 
 StepInfo step(Env env, int action);
 
 Env copy_env(Env env);
```

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/random.c` & `mpspenv-0.1.3/MPSPEnv/c/src/random.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/sort.c` & `mpspenv-0.1.3/MPSPEnv/c/src/sort.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/transportation_matrix.c` & `mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c/src/transportation_matrix.h` & `mpspenv-0.1.3/MPSPEnv/c/src/transportation_matrix.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv/c_interface.py` & `mpspenv-0.1.3/MPSPEnv/c_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,26 @@
     ]
 
 
 class Env(Structure):
     _fields_ = [
         ("T", POINTER(Transportation_Info)),
         ("bay", Bay),
-        ("flat_T_matrix", Array),
         ("mask", Array),
         ("auto_move", c_int),
         ("total_reward", POINTER(c_int)),
         ("containers_left", POINTER(c_int)),
         ("containers_placed", POINTER(c_int)),
+        ("terminated", POINTER(c_int)),
     ]
 
 
 class StepInfo(Structure):
     _fields_ = [
-        ("is_terminal", c_int),
+        ("terminated", c_int),
         ("reward", c_int),
     ]
 
 
 directory = os.path.dirname(os.path.abspath(__file__))
 c_lib_files = glob.glob(os.path.join(directory, "c_lib*.so"))
```

### Comparing `mpspenv-0.1.2/MPSPEnv/env.py` & `mpspenv-0.1.3/MPSPEnv/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,56 +63,52 @@
 
     def step(self, action: int):
         assert self._env is not None, "The environment must be reset before stepping."
         self._check_action(action)
 
         step_info = c_lib.step(self._env, action)
         reward = step_info.reward
-        self.terminal = bool(step_info.is_terminal)
 
         if self.speedy:
             return None
         else:
             return (
                 self._get_observation(),
                 reward,
-                self.terminal,
+                self.terminated,
                 False,
                 {},
             )
 
     def copy(self):
         new_env = Env(
             R=self.R,
             C=self.C,
             N=self.N,
             auto_move=self.auto_move,
             speedy=self.speedy,
         )
         new_env._env = c_lib.copy_env(self._env)
-        new_env.terminal = self.terminal
         new_env._set_stores()
 
         return new_env
 
     def reset(self, seed: int = None, options=None):
         self._reset_random_c_env(seed)
         self._set_stores()
-        self.terminal = False
 
         if self.speedy:
             return None
         else:
             return self._get_observation(), {}
 
     def reset_to_transportation(self, transportation: np.ndarray):
         self._assert_transportation(transportation)
         self._reset_specific_c_env(transportation)
         self._set_stores()
-        self.terminal = False
 
         if self.speedy:
             return None
         else:
             return self._get_observation(), {}
 
     def render(self):
@@ -141,41 +137,38 @@
         return self._env.containers_left.contents.value
 
     @property
     def containers_placed(self) -> int:
         return self._env.containers_placed.contents.value
 
     @property
+    def terminated(self) -> bool:
+        return self._env.terminated.contents.value
+
+    @property
     def remaining_ports(self) -> int:
         return self.N - 1 - self._env.T.contents.current_port
 
     @property
     def bay(self) -> np.ndarray:
         return self.bay_store.ndarray.copy()
 
     @property
     def T(self) -> np.ndarray:
         return self.T_store.ndarray.copy()
 
     @property
-    def flat_T(self) -> np.ndarray:
-        return self.flat_T_store.ndarray.copy()
-
-    @property
     def mask(self) -> np.ndarray:
         return self.mask_store.ndarray.copy()
 
     def _set_stores(self):
         self.bay_store = LazyNdarray(self._env, ["bay", "matrix"], (self.R, self.C))
         self.T_store = LazyNdarray(
             self._env, ["T", "contents", "matrix"], (self.N, self.N)
         )
-        self.flat_T_store = LazyNdarray(
-            self._env, ["flat_T_matrix"], ((self.N - 1) * self.N // 2,)
-        )
         self.mask_store = LazyNdarray(self._env, ["mask"], (2 * self.C * self.R,))
 
     def _assert_transportation(self, transportation: np.ndarray):
         assert (
             transportation.dtype == np.int32
         ), f"Transportation matrix must be of type np.int32 but was {transportation.dtype}"
         assert transportation.shape == (
@@ -205,20 +198,15 @@
                     total += transportation[k, j]
             if total > capacity:
                 return False
 
         return True
 
     def _get_observation(self):
-        return {
-            "bay": self.bay / self.remaining_ports,
-            "flat_T": self.flat_T / (self.R * self.C),
-            "mask": self.mask,
-            "containers_left": self.containers_left,
-        }
+        return {"bay": self.bay, "T": self.T, "mask": self.mask}
 
     def _reset_random_c_env(self, seed: int = None):
         if self._env is not None:
             c_lib.free_env(self._env)
 
         if seed is not None:
             c_lib.set_seed(seed)
@@ -245,17 +233,17 @@
                 "Env was not closed properly. Please call .close() to avoid memory leaks."
             )
             self.close()
 
     def __hash__(self):
         return hash(
             self.bay_store.ndarray.tobytes()
-            + self.flat_T_store.ndarray.tobytes()
+            + self.T_store.ndarray.tobytes()
             + self.mask_store.ndarray.tobytes()
         )
 
     def __eq__(self, other: "Env"):
         return (
             np.array_equal(self.bay_store.ndarray, other.bay_store.ndarray)
-            and np.array_equal(self.flat_T_store.ndarray, other.flat_T_store.ndarray)
+            and np.array_equal(self.T_store.ndarray, other.T_store.ndarray)
             and np.array_equal(self.mask_store.ndarray, other.mask_store.ndarray)
         )
```

### Comparing `mpspenv-0.1.2/MPSPEnv/visualizer.py` & `mpspenv-0.1.3/MPSPEnv/visualizer.py`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/MPSPEnv.egg-info/PKG-INFO` & `mpspenv-0.1.3/MPSPEnv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.2/MPSPEnv.egg-info/SOURCES.txt` & `mpspenv-0.1.3/MPSPEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/PKG-INFO` & `mpspenv-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.2
+Version: 0.1.3
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.2/README.md` & `mpspenv-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.2/setup.py` & `mpspenv-0.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MPSPEnv",
-    version="0.1.2",
+    version="0.1.3",
     author="Axel Højmark",
     author_email="axelhojmark@gmail.com",
     description="A reinforcement learning environment for the Multi Port Stowage Planning problem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[ext_modules],
     packages=["MPSPEnv"],
```

### Comparing `mpspenv-0.1.2/tests/test_env.py` & `mpspenv-0.1.3/tests/test_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for _ in range(episodes):
         settings = get_random_settings()
         seed = np.random.randint(0, 1000000)
         initial_containers = get_initial_containers(settings, seed)
         env = recreate_env(settings, seed)
         additional_info = get_additional_env_info(env)
 
-        while not env.terminal:
+        while not env.terminated:
             sanity_check_env(env, **additional_info)
             action = get_random_action(env.mask)
             env.step(action)
 
         sanity_check_env(env, **additional_info)
         assert initial_containers - env.total_reward == env.containers_placed
         env.close()
@@ -75,15 +75,14 @@
     env = recreate_env(settings, seed)
     env.step(get_random_action(env.mask))
     copy = env.copy()
 
     assert np.all(env.bay == copy.bay)
     assert np.all(env.T == copy.T)
     assert np.all(env.mask == copy.mask)
-    assert np.all(env.flat_T == copy.flat_T)
     assert env.auto_move == copy.auto_move
     assert env.speedy == copy.speedy
     assert env.total_reward == copy.total_reward
     assert env.containers_left == copy.containers_left
     assert env.containers_placed == copy.containers_placed
     assert env.remaining_ports == copy.remaining_ports
     assert env == copy
```

