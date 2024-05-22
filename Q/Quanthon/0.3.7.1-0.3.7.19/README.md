# Comparing `tmp/quanthon-0.3.7.1.tar.gz` & `tmp/quanthon-0.3.7.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quanthon-0.3.7.1.tar", last modified: Tue May 14 23:57:23 2024, max compression
+gzip compressed data, was "quanthon-0.3.7.19.tar", last modified: Wed May 22 14:03:59 2024, max compression
```

## Comparing `quanthon-0.3.7.1.tar` & `quanthon-0.3.7.19.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:57:23.746791 quanthon-0.3.7.1/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.7.1/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-05-14 23:57:23.746569 quanthon-0.3.7.1/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:57:23.744030 quanthon-0.3.7.1/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.7.1/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      340 2024-04-29 12:30:59.000000 quanthon-0.3.7.1/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)    10022 2024-05-14 11:12:34.000000 quanthon-0.3.7.1/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     5421 2024-05-14 23:56:34.000000 quanthon-0.3.7.1/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    12678 2024-05-14 23:51:46.000000 quanthon-0.3.7.1/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.7.1/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)      465 2024-05-01 13:34:06.000000 quanthon-0.3.7.1/Quanthon/history.py
--rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.7.1/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.7.1/Quanthon/mappers_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.7.1/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.7.1/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1560 2024-05-04 17:32:55.000000 quanthon-0.3.7.1/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.7.1/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     7204 2024-05-14 23:53:03.000000 quanthon-0.3.7.1/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:57:23.746329 quanthon-0.3.7.1/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2521 2024-05-14 23:57:23.000000 quanthon-0.3.7.1/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      577 2024-05-14 23:57:23.000000 quanthon-0.3.7.1/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-05-14 23:57:23.000000 quanthon-0.3.7.1/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-05-14 23:57:23.000000 quanthon-0.3.7.1/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-05-14 23:57:23.000000 quanthon-0.3.7.1/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.7.1/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-05-14 23:57:23.746841 quanthon-0.3.7.1/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-05-14 23:57:12.000000 quanthon-0.3.7.1/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-14 23:57:23.745893 quanthon-0.3.7.1/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.7.1/tests/test_cmp_qk.py
--rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.7.1/tests/test_mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.7.1/tests/test_utils.py
--rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.7.1/tests/test_vqes.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-22 14:03:59.892073 quanthon-0.3.7.19/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 quanthon-0.3.7.19/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2522 2024-05-22 14:03:59.891804 quanthon-0.3.7.19/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-22 14:03:59.886495 quanthon-0.3.7.19/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 quanthon-0.3.7.19/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      391 2024-05-21 14:20:55.000000 quanthon-0.3.7.19/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)    10516 2024-05-21 20:30:42.000000 quanthon-0.3.7.19/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5775 2024-05-21 20:35:37.000000 quanthon-0.3.7.19/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    15121 2024-05-22 14:03:47.000000 quanthon-0.3.7.19/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 quanthon-0.3.7.19/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3042 2024-05-21 18:11:28.000000 quanthon-0.3.7.19/Quanthon/exponential.py
+-rw-r--r--   0 bukser     (501) staff       (20)      465 2024-05-01 13:34:06.000000 quanthon-0.3.7.19/Quanthon/history.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4775 2024-04-24 11:29:34.000000 quanthon-0.3.7.19/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6791 2024-04-25 10:03:08.000000 quanthon-0.3.7.19/Quanthon/mappers_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)      455 2024-04-18 10:41:02.000000 quanthon-0.3.7.19/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 quanthon-0.3.7.19/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1560 2024-05-04 17:32:55.000000 quanthon-0.3.7.19/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 quanthon-0.3.7.19/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     7237 2024-05-20 19:25:59.000000 quanthon-0.3.7.19/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-22 14:03:59.891503 quanthon-0.3.7.19/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2522 2024-05-22 14:03:59.000000 quanthon-0.3.7.19/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      601 2024-05-22 14:03:59.000000 quanthon-0.3.7.19/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-05-22 14:03:59.000000 quanthon-0.3.7.19/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-05-22 14:03:59.000000 quanthon-0.3.7.19/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-05-22 14:03:59.000000 quanthon-0.3.7.19/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1656 2024-04-22 07:53:30.000000 quanthon-0.3.7.19/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-05-22 14:03:59.892120 quanthon-0.3.7.19/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1512 2024-05-20 19:25:12.000000 quanthon-0.3.7.19/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-05-22 14:03:59.891312 quanthon-0.3.7.19/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     4052 2024-04-09 23:49:00.000000 quanthon-0.3.7.19/tests/test_cmp_qk.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1472 2024-04-25 10:07:26.000000 quanthon-0.3.7.19/tests/test_mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)      173 2024-04-18 11:07:53.000000 quanthon-0.3.7.19/tests/test_utils.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3784 2024-04-25 10:07:37.000000 quanthon-0.3.7.19/tests/test_vqes.py
```

### Comparing `quanthon-0.3.7.1/PKG-INFO` & `quanthon-0.3.7.19/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.7.1
+Version: 0.3.7.19
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.7.1/Quanthon/Models.py` & `quanthon-0.3.7.19/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/algorithms.py` & `quanthon-0.3.7.19/Quanthon/algorithms.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             result = self.minimise(self._objective, 
                                    self.params, 
                                    method=method,
                                 #    method='Powell',
                                 #    method='Nelder-Mead',
                                     #  method='COBYLA',
                                     #  method='TNC',
-                                   bounds=bounds, 
+                                #    bounds=bounds, 
                                    options= {"maxiter": 100}
                                    )
             min_params = result.x
             min_energy = result.fun
             
             # print(min_params)
             return min_params, min_energy
@@ -115,15 +115,15 @@
         # apply all gates first
 
         grad = state.conj().T @ (self.H_mat @ A - A @ self.H_mat) @ state
 
         
         return grad
 
-    def _append_operator(self, eps=10e-2):
+    def _append_operator(self, eps, decompose_exp, decompose_method):
         
         '''
             Append a new operator to the ansatz which has the largest greadient ~ [H, A]
             return:
                 True if largest gradient is < eps and a new operator is added, False otherwise.
         '''
 
@@ -149,15 +149,15 @@
             print(f"end of adapt, grad = {max_abs_grad}")
             return False # gradient = 0, end of adapt  
         # print(f"appending, op: {op_cand}, grad: {max_abs_grad}")
         # grow the ansatz
         # self.old_gates.append(op_cand) # type(op_cand) == str
         print("max_abs_grad: ", max_abs_grad)
         self.params = np.append(self.params, 0)
-        self.ansatz.append_op(op_cand)
+        self.ansatz.append_op(op_cand, decompose_exp=decompose_exp, decompose_method=decompose_method)
 
         self.hist.update_grad(max_abs_grad)
         self.hist.update_operators(op_cand)
         
 
         return True
     
@@ -168,17 +168,24 @@
         qc.set_state(state)
 
         if self.estimate_energy:
             energy = self.expectation(qc, self.H_str, self.num_shots)
         else:
             energy = state.conj().T @ self.H_mat @ state
 
-        return energy
+        return energy.real
     
-    def run_adapt_circuit(self, H, num_shots=10000, max_iter=100, grad_eps=1e-4, method='COBYLA'):
+    def run_adapt_circuit(self, 
+                          H, 
+                          num_shots=10000, 
+                          max_iter=100, 
+                          grad_eps=1e-4, 
+                          method='SLSQP', 
+                          decompose_exp=False,
+                          decompose_method='inverted staircase'):
         '''
         args:
             H: list of 2-tuple such as [('II', 0.5)]
             num_shots: number of shots,
             max_iter: maximum number of iterations,
         
         return: 
@@ -192,25 +199,26 @@
             # print(self.ansatz.qubits)
             # self.ansatz.run(self.params) # ??????
             old_params, energy = self.minimise_eigenvalue(num_shots, method=method) # state is not updated here
             self.params = old_params
             print(f"i: {i}, min_energy = {energy}")
             self.hist.update_energies(energy)
 
-            if not self._append_operator(eps=grad_eps): # new parameter is added here 
+            if not self._append_operator(eps=grad_eps, decompose_exp=decompose_exp, decompose_method=decompose_method): 
+                # new parameter is added here 
                 break
             
         if i == max_iter - 1:
             print("Maximum adapt iteration reached, energy did not converge.")
             # warnings.warn('Adapt circuit did not converge.')
         self.ansatz.run(self.params) # update the state with the final parameters
         return self.ansatz, energy
     
 
-    def minimise_eigenvalue(self, num_shots=10000, method='SLSQP'):
+    def minimise_eigenvalue(self, num_shots, method):
 
 
         '''
             Rotates the parametrised circuit to find the minimised energy using classical 
             minimisation algorithms.
             args:
                 H_pauli_str: the Hamiltonian of the system in transformed in terms of Pauli strings,
@@ -220,41 +228,43 @@
         '''
         self.num_shots = num_shots
         
         # print(self.params)
 
         lb = -np.pi * np.ones(len(self.params))
         ub = np.pi * np.ones(len(self.params))
-        bounds = Bounds(lb, ub)
+        kfs = np.ones(len(self.params), dtype=bool)
+
+        bounds = Bounds(lb, ub, keep_feasible=kfs)
 
         # old_energy = self._objective(self.params)
         # min_energy = old_energy
 
         if self.params.size == 0:
             result = self.minimise(self._objective, 
                                 0, 
                                 method=method, 
-                                #    bounds=bounds,
-                                options= {"maxiter": 100000}
+                                # bounds=bounds,
+                                options= {"maxiter": 10000}
                                 )
         else:
             result = self.minimise(self._objective, 
                                 self.params, 
                                 method=method, 
-                                #    bounds=bounds,
-                                options= {"maxiter": 100000}
+                                bounds=bounds,
+                                options= {"maxiter": 10000}
                                 )
 
         min_energy = result.fun
         min_params = result.x
 
         old_energy = self._objective(self.params)
-        print(f"old energy: {old_energy}")
-        print(f"min_energy: {min_energy}")
-        if old_energy < min_energy:
+        print(f"old energy: {old_energy.real}")
+        print(f"min_energy: {min_energy.real}")
+        if old_energy.real < min_energy.real:
             warnings.warn("New energy is higher than the old energy.")
 
         # self.ansatz.run(min_params) # update the state using only the optimal parameters
          
         return min_params, min_energy
```

### Comparing `quanthon-0.3.7.1/Quanthon/ansatzs.py` & `quanthon-0.3.7.19/Quanthon/ansatzs.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import numpy as np
 from scipy.linalg import expm
 
 
 from .base import Qubits, Gate
 from .utils import pauli_sum
+from .exponential import exponential_pauli
 
 class Ansatz:
 
 	'''Should work for any type of ansatz that are not evolving, do not use on its own.'''
 	def __init__(self, n_qubits, reps=1) -> None:
 
 		self.n_qubits = n_qubits
@@ -145,79 +146,95 @@
 		new_pool.append('i' + (n-2) * 'I' + 'YI')
 
 
 		return new_pool
 	
 	def create_complete_G_pool(self, n):
 		
+		if n == 1:
+			return ['iY', 'Z']
 		pool = self._get_ys(n)
-		pool.extend(self._get_zy(n))
+		# print("get ys", pool)
+		pool.extend(self._get_yzs(n))
+		# print("get yzs", pool)
 		return pool
 
 	
 	def _get_ys(self,n):
 		'''Get a list of all the operators with a single Y in them'''
 		op = n*'I'
 		ops = []
 		for i in range(1, n):
 			y_op = list(op)
 			y_op[i] = 'Y'
-			ops.append(''.join(y_op))
+			ops.append('i' + ''.join(y_op))
 		
 		return ops
 
-	def _get_zys(self, n):
+	def _get_yzs(self, n):
 		op = n*'I'
 		ops = []
 		for i in range(n-1):
 			yz_op = list(op)
 			yz_op[i] = 'Y'
 			yz_op[i+1] = 'Z'
-			ops.append(''.join(yz_op))
-		
+			ops.append('i' + ''.join(yz_op))
 		return ops
 
-	def append_op(self, op):
+	def append_op(self, op, decompose_exp, decompose_method):
 
 		'''
 		op: string, representing one of the operators in the pool
 		
 		'''
 		# no longer need to append all the gates since they are now saved
 
 		qprint(f"append_op op: {op}")
-		op_mat = pauli_sum([(op.strip('i'), 1j)])
 
-		def parametrised_mat(param, op_mat):
-			return expm(param * op_mat)
-		
-		# self.params.append(0) # the corresponding parameter for the gate, initialised to 0.
-		
-		adapt_gate = Gate(f'exp({op})', matrix=lambda param: parametrised_mat(param, op_mat), n_qubits=self.qubits.n_qubit)
-		self.qubits.circuit.append(adapt_gate)
-		
+		if decompose_exp:
+			exponential_pauli(self.qubits, op.strip('i'), coeff=None, method=decompose_method)
+			print(f"len circuit: {len(self.qubits.circuit)}")
+		else:	
+			op_mat = pauli_sum([(op.strip('i'), 1j)])
+			def parametrised_mat(param, op_mat):
+				return expm(param * op_mat)
+			
+			
+			adapt_gate = Gate(f'exp({op})', matrix=lambda param: parametrised_mat(param, op_mat), n_qubits=self.qubits.n_qubit, is_parametrised=True)
+			self.qubits.circuit.append(adapt_gate)
+			
 	
 	def run(self, params):
-		for i, gate in enumerate(self.qubits.circuit):
+		param_indx = 0
+		for gate in self.qubits.circuit:
 			# print(gate.matrix(params[i]))
-			self.qubits.state = gate.act(self.qubits.state, params[i])
+			if gate.is_parametrised:
+				self.qubits.state = gate.act(self.qubits.state, -1 * params[param_indx])
+				param_indx += 1
+			else:
+				self.qubits.state = gate.act(self.qubits.state)
 		
 		# print(self.qubits.circuit)
 	
 	def run_without_update(self, params):
 		'''Run the circuit without updating the state.'''
-		old_state = self.qubits.state
-		for i, gate in enumerate(self.qubits.circuit):
-			self.qubits.state = gate.act(self.qubits.state, params[i])
-			if not np.isclose(np.linalg.norm(self.qubits.state), 1):
+		state = self.qubits.state
+		param_indx = 0
+
+		for gate in self.qubits.circuit:
+			if gate.is_parametrised:
+				state = gate.act(state, -1 * params[param_indx])
+				param_indx += 1
+			else:
+				state = gate.act(state)
+			
+			if not np.isclose(np.linalg.norm(state), 1, atol=1e-4):
 				raise ValueError(f"Probability does not sum to unity, prob: {self.qubits.prob}, state: {self.qubits.state}.")
 		
-		new_state = self.qubits.state
-		self.qubits.state = old_state # return to the new state while returning the result of the circuit
-		return new_state
+		return state
```

### Comparing `quanthon-0.3.7.1/Quanthon/base.py` & `quanthon-0.3.7.19/Quanthon/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 '''The basic classes for quantum computing. Replaced base.py, which was discontinued after Quanthon 0.3.0'''
 
-# TODO: Add n dimension rotation 
-
 import numpy as np
 from collections import Counter
 from .utils import one_fixed_bit, flip_bit, swap_bits, get_bit, make_op_mat, is_valid_state
 
 # Constants
 rng = np.random.default_rng()
 rangle = '\u27E9'
 
 class Gate:
 
-    def __init__(self, name, matrix, n_qubits):
+    def __init__(self, name, matrix, n_qubits, is_parametrised=False):
         '''
         args:
             name: string, the name of the gate;
             matrix: operator matrix or a function which takes params is an argument and returns the matrix of the correct size;
             n_qubits: int, the number of qubits the gate acts on;
+            targets: the target qubit or qubits the gate acts on.
             '''
         self.name = name
         self.matrix = matrix
 
         self.n_qubits = n_qubits
+        self.is_parametrised = is_parametrised
         # self.params = params
 
 
     def __repr__(self):
         return f"Gate: {self.name} \n Matrix: \n {self.matrix} \n"
     
     def _check_is_unitary(self, matrix):
-
-        if not np.allclose(matrix @ matrix.conj().T, np.eye(matrix.shape[0])):
-            raise ValueError(f"{self.name} is not unitary, matrix: {matrix}.")
+        
+        uudag = matrix @ matrix.conj().T
+        if not np.allclose(uudag, np.eye(matrix.shape[0]), atol=1e-4):
+            raise ValueError(f"{self.name} is not unitary, matrix UU+: {uudag}.")
     
     def act(self, state, param=None):
-        if param is not None:
+
+        if self.is_parametrised:
+            assert param is not None
             self._check_is_unitary(self.matrix(param))
             result = self.matrix(param) @ state
         
         else:
             self._check_is_unitary(self.matrix)
             result = self.matrix @ state
         
 
         if is_valid_state(result):
+            result /= np.linalg.norm(result)
             return result
         else:
-            raise ValueError(f"Invalid state. {result} {np.abs(result**2)}")
-    
+            raise ValueError(f"Invalid state. {result} {sum(np.abs(result**2))}")
+
     
 class Qubits:
 
     def __init__(self,n):
         self.state = np.zeros(2**n, dtype=np.complex_)
         self.state[0] = 1
         self.n_qubit = n
@@ -81,22 +85,22 @@
         # print(self.gate_history)
     
     def _update_gate_history(self, gate, i):
         
         if gate in ['H', 'X', 'Y', 'Z', 'Sdag']:
             self.gate_history[f'{i}'].append(gate) 
         
-        elif gate.startswith('Rx') or gate.startswith('Ry'):
+        elif gate.startswith('R'):
             self.gate_history[f'{i}'].append(gate)
  
-        elif gate == 'CNOT':
+        elif gate.startswith('CNOT'):
             self.gate_history[f'{i[0]}'].append(gate + f"ctrl{i[1]-i[0]}") 
             self.gate_history[f'{i[1]}'].append(gate + "trgt")
         
-        elif gate == 'SWAP':
+        elif gate.startswith('SWAP'):
             self.gate_history[f'{i[0]}'].append(gate + f"1{i[1]-i[0]}")
             self.gate_history[f'{i[1]}'].append(gate + "2")
 
         else:
             raise ValueError(f"Invalid gate {gate}")
         
         for j in range(self.n_qubit):
@@ -106,15 +110,15 @@
             else:
                 if j != i:
                     self.gate_history[f'{j}'].append('I')
 
 
     def set_state(self, state):
         assert len(state) == 2**self.n_qubit, f"Invalid state: must have length {2**self.n_qubit}"
-        assert np.isclose(np.linalg.norm(state), 1), "Invalid state: must be normalised."
+        assert np.isclose(np.linalg.norm(state), 1, atol=1e-4), "Invalid state: must be normalised."
         self.state = state
 
     def reset_state(self):
         self.state = np.zeros(2**self.n_qubit, dtype=np.complex_)
         self.state[0] = 1
     
     def reset_circuit(self):
@@ -149,55 +153,94 @@
 
         # Return the computational basis notation
         return computational_str
 
     def H(self,i):
         # self.operate(self.h,i)
         matrix = make_op_mat(self.n_qubit, self.h, i)
-        self.circuit.append(Gate('H', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'H_{i}', matrix, self.n_qubit))
         self._update_gate_history('H', i)
     
     def X(self,i):
         # self.operate(self.x, i)
         matrix = make_op_mat(self.n_qubit, self.x, i)
-        self.circuit.append(Gate('X', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'X_{i}', matrix, self.n_qubit))
         self._update_gate_history('X', i)
 
     def Y(self,i):
         # self.operate(self.y, i)
         matrix = make_op_mat(self.n_qubit, self.y, i)
-        self.circuit.append(Gate('Y', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'Y_{i}', matrix, self.n_qubit))
         self._update_gate_history('Y', i)
 
     def Z(self,i):
         # self.operate(self.z, i)
         matrix = make_op_mat(self.n_qubit, self.z, i)
-        self.circuit.append(Gate('Z', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'Z_{i}', matrix, self.n_qubit))
         self._update_gate_history('Z', i)
     
     def Sdag(self,i):
         # self.operate(self.s.conj(), i)
         matrix = make_op_mat(self.n_qubit, self.s.conj(), i)
-        self.circuit.append(Gate('Sdag', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'Sdag_{i}', matrix, self.n_qubit))
         self._update_gate_history('Sdag', i)
 
     def Rx(self, theta, i):
 
-        rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
-        # self.operate(Rx, i) 
-        matrix = make_op_mat(self.n_qubit, rx, i)
-        self.circuit.append(Gate('Rx', matrix, self.n_qubit))
-        self._update_gate_history(f'Rx_{theta}', i)
-
-    def Ry(self, phi, i):
-        ry = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
-        # self.operate(Ry, i)
-        matrix = make_op_mat(self.n_qubit, ry, i)
-        self.circuit.append(Gate('Ry', matrix, self.n_qubit))
-        self._update_gate_history(f'Ry_{phi}', i)
+        def rx(theta):
+            return np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
+        
+        if theta is None:
+            self.circuit.append(Gate(f'Rx_{i}', 
+                                     lambda param: make_op_mat(self.n_qubit, rx(param), i), 
+                                     self.n_qubit, 
+                                     is_parametrised=True))
+            
+            self._update_gate_history(f'Rx_θ', i)
+        else:
+            matrix = make_op_mat(self.n_qubit, rx(theta), i)
+            self.circuit.append(Gate(f'Rx_{theta}_{i}', matrix, self.n_qubit))
+
+            self._update_gate_history(f'Rx_{theta}', i)
+
+    def Ry(self, theta, i):
+
+        def ry(theta):
+            return np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.y
+        
+        if theta is None:
+            self.circuit.append(Gate(f'Ry_{i}', 
+                                     lambda param: make_op_mat(self.n_qubit, ry(param), i), 
+                                     self.n_qubit, 
+                                     is_parametrised=True))
+            
+            self._update_gate_history(f'Ry_θ', i)
+        else:
+            matrix = make_op_mat(self.n_qubit, ry(theta), i)
+            self.circuit.append(Gate(f'Ry_{theta}_{i}', matrix, self.n_qubit))
+
+            self._update_gate_history(f'Ry_{theta}', i)
+
+    def Rz(self, theta, i):
+
+        def rz(theta):
+            return np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.z
+        
+        if theta is None:
+            self.circuit.append(Gate(f'Rz_{i}', 
+                                     lambda param: make_op_mat(self.n_qubit, rz(param), i), 
+                                     self.n_qubit, 
+                                     is_parametrised=True))
+            
+            self._update_gate_history(f'Rz_θ', i)
+        else:
+            matrix = make_op_mat(self.n_qubit, rz(theta), i)
+            self.circuit.append(Gate(f'Rz_{theta}_{i}', matrix, self.n_qubit))
+
+            self._update_gate_history(f'Rz_{theta}', i)
 
     def controlled_U1(self, op, control, target):
         '''
         Apply the two-qubit controlled gate. Control before target. '''
         if self.n_qubit == 1:
             raise ValueError("The CNOT gate can not be applied to a single qubit.")
 
@@ -231,15 +274,15 @@
             # print(i)
             f = flip_bit(i, self.n_qubit - target - 1) # same reason
             # print(f)
             matrix[i, i] = 0
             matrix[f, i] = 1
             matrix[i, f] = 1
 
-        self.circuit.append(Gate('CNOT', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'CNOT{control}{target}', matrix, self.n_qubit))
         # self.state = matrix @ self.state
         self._update_gate_history("CNOT", (control, target))
 
 
     def SWAP(self, qubit1, qubit2):
         if self.n_qubit == 1:
             raise ValueError("The SWAP gate can not be applied to a single qubit.")
@@ -248,24 +291,33 @@
         matrix = np.zeros((self.operator_size, self.operator_size))
         for i in range(self.operator_size):
             j = swap_bits(i, self.n_qubit - qubit1 - 1, self.n_qubit - qubit2 - 1)
             matrix[i, j] = 1
             matrix[j, i] = 1
 
         # self.state = matrix @ self.state
-        self.circuit.append(Gate('SWAP', matrix, self.n_qubit))
+        self.circuit.append(Gate(f'SWAP{qubit1}{qubit2}', matrix, self.n_qubit))
         self._update_gate_history("SWAP", (qubit1, qubit2))
     
-    def run(self):
+    def run(self, params=None):
         
         '''
-        Execute the circuit. Return the result.
+        Execute the circuit. 
+        args:
+            params: the parameter to be inserted into the parametrised gates, must be in order of the gates in the circuit
+            
         '''
+        param_indx = 0
         for gate in self.circuit:
-            self.state = gate.act(self.state)
+            if gate.is_parametrised:
+                self.state = gate.act(self.state, params[param_indx])
+                param_indx += 1
+            else:
+                self.state = gate.act(self.state)
+            
          
     def run_and_reset(self):
         '''Execute the circuit and reset the circuit. Return the result.'''
         self.run()
         state = self.state
         self.reset_circuit()
         return state
@@ -275,25 +327,33 @@
         
         return prob
 
     def measure(self, n_shots=1):
         ''' n: number of shots 
             indexs: the index of the qubit(s) being measured '''
         
+        n_shots = int(n_shots)
+        self.atol = 1/n_shots
+        
         prob = self.prob()
         allowed_outcomes = np.arange(len(self.state))
         # print(self.state)
         try:
             outcomes = np.random.choice(allowed_outcomes, p=prob, size = n_shots)
         except ValueError:
-            raise ValueError(f"Prob: {prob}.")
+            if np.isclose(np.sum(prob), 1, atol=self.atol):
+                new_prob = prob / np.sum(prob)
+                outcomes = np.random.choice(allowed_outcomes, p=new_prob, size = n_shots) 
+            else:
+                raise ValueError(f"Prob: {prob}, {np.sum(prob)}.")
         
         self.state = np.zeros_like(self.state)
         self.state[outcomes[-1]] = 1
         counts = Counter(outcomes)
+
         
         outcomes_count = np.zeros((len(self.state),2)) # 2: state and count
         for i in range(len(self.state)):
             if i in counts:
                 outcomes_count[i] = counts[i], format(i, f"0{self.n_qubit}b")
             else:
                 outcomes_count[i] = 0,format(i, f"0{self.n_qubit}b")
```

### Comparing `quanthon-0.3.7.1/Quanthon/expectation.py` & `quanthon-0.3.7.19/Quanthon/expectation.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/mappers.py` & `quanthon-0.3.7.19/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/mappers_utils.py` & `quanthon-0.3.7.19/Quanthon/mappers_utils.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/ut_pyscf_mel.py` & `quanthon-0.3.7.19/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/ut_qiskit_hamiltonian.py` & `quanthon-0.3.7.19/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/ut_test_jw.py` & `quanthon-0.3.7.19/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/Quanthon/utils.py` & `quanthon-0.3.7.19/Quanthon/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,22 +155,22 @@
     return: list of all the possible Pauli strings of length n.
     '''
     paulis = 'IXYZ'
     return [''.join(p) for p in product(paulis, repeat=n)] 
 
 
 def is_hermitian(mat):
-    return np.allclose(mat, mat.T.conj())
+    return np.allclose(mat, mat.T.conj(), rtol=1e-4)
 
 def is_unitary(mat):
-    return np.allclose(mat @ mat.T.conj(), np.eye(len(mat)))
+    return np.allclose(mat @ mat.T.conj(), np.eye(len(mat)), rtol=1e-4)
 
 def is_valid_state(state):
     # print(state)
-    return np.isclose(sum(np.abs((state**2))), 1)
+    return np.isclose(sum(np.abs((state**2))), 1, rtol=1e-4)
     
 if __name__ == "__main__":
     # Test Pauli operators
     # pauli_ops = [('IZZZ', 3), ('ZXYI', 2)]
     qubit_op = [('IIIIII', 0.1875), ('IIIIIZ', -0.5625), 
                     ('IIIIZI', -0.0625), ('IIIZII', 0.4375), 
                     ('IIZIII', -0.5625), ('IIZIIZ', 0.0625),
```

### Comparing `quanthon-0.3.7.1/Quanthon.egg-info/PKG-INFO` & `quanthon-0.3.7.19/Quanthon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.7.1
+Version: 0.3.7.19
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `quanthon-0.3.7.1/Quanthon.egg-info/SOURCES.txt` & `quanthon-0.3.7.19/Quanthon.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 Quanthon/Models.py
 Quanthon/__init__.py
 Quanthon/algorithms.py
 Quanthon/ansatzs.py
 Quanthon/base.py
 Quanthon/expectation.py
+Quanthon/exponential.py
 Quanthon/history.py
 Quanthon/mappers.py
 Quanthon/mappers_utils.py
 Quanthon/physics.py
 Quanthon/ut_pyscf_mel.py
 Quanthon/ut_qiskit_hamiltonian.py
 Quanthon/ut_test_jw.py
```

### Comparing `quanthon-0.3.7.1/README.md` & `quanthon-0.3.7.19/README.md`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/setup.py` & `quanthon-0.3.7.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.7.1" #####
+version = "0.3.7.19" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `quanthon-0.3.7.1/tests/test_cmp_qk.py` & `quanthon-0.3.7.19/tests/test_cmp_qk.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/tests/test_mappers.py` & `quanthon-0.3.7.19/tests/test_mappers.py`

 * *Files identical despite different names*

### Comparing `quanthon-0.3.7.1/tests/test_vqes.py` & `quanthon-0.3.7.19/tests/test_vqes.py`

 * *Files identical despite different names*

