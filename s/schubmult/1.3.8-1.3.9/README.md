# Comparing `tmp/schubmult-1.3.8.tar.gz` & `tmp/schubmult-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.8.tar", last modified: Sun May 19 21:32:16 2024, max compression
+gzip compressed data, was "schubmult-1.3.9.tar", last modified: Wed May 22 10:54:39 2024, max compression
```

## Comparing `schubmult-1.3.8.tar` & `schubmult-1.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.890000 schubmult-1.3.8/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.8/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-19 21:32:16.835000 schubmult-1.3.8/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.8/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:14.482000 schubmult-1.3.8/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.8/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    18084 2024-05-18 15:28:41.000000 schubmult-1.3.8/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.229000 schubmult-1.3.8/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.8/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.8/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5027 2024-05-17 15:39:33.000000 schubmult-1.3.8/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.514000 schubmult-1.3.8/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.8/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.8/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5757 2024-05-17 15:05:46.000000 schubmult-1.3.8/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:15.833000 schubmult-1.3.8/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.8/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.8/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    10420 2024-05-17 14:57:50.000000 schubmult-1.3.8/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.120000 schubmult-1.3.8/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.8/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.8/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3456 2024-05-17 15:40:28.000000 schubmult-1.3.8/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.435000 schubmult-1.3.8/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    11896 2024-05-19 18:52:48.000000 schubmult-1.3.8/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:16.762000 schubmult-1.3.8/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.8/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.8/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    47306 2024-05-19 18:33:48.000000 schubmult-1.3.8/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-19 21:32:14.937000 schubmult-1.3.8/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-19 21:32:13.000000 schubmult-1.3.8/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-19 21:32:12.000000 schubmult-1.3.8/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-19 21:32:16.872000 schubmult-1.3.8/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-19 21:31:58.000000 schubmult-1.3.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:39.314000 schubmult-1.3.9/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.9/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-22 10:54:39.263000 schubmult-1.3.9/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     5299 2024-05-12 18:38:20.000000 schubmult-1.3.9/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:36.625000 schubmult-1.3.9/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.9/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    18348 2024-05-20 18:10:32.000000 schubmult-1.3.9/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.410000 schubmult-1.3.9/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.9/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.9/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5027 2024-05-17 15:39:33.000000 schubmult-1.3.9/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.778000 schubmult-1.3.9/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.9/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.9/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5757 2024-05-17 15:05:46.000000 schubmult-1.3.9/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.138000 schubmult-1.3.9/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.9/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.9/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    10420 2024-05-17 14:57:50.000000 schubmult-1.3.9/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.504000 schubmult-1.3.9/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.9/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.9/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3456 2024-05-17 15:40:28.000000 schubmult-1.3.9/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:38.829000 schubmult-1.3.9/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12623 2024-05-21 17:59:25.000000 schubmult-1.3.9/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:39.188000 schubmult-1.3.9/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.9/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.9/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    47692 2024-05-21 13:46:50.000000 schubmult-1.3.9/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 10:54:37.083000 schubmult-1.3.9/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5681 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-05-22 10:54:34.000000 schubmult-1.3.9/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-05-22 10:54:35.000000 schubmult-1.3.9/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-05-22 10:54:39.298000 schubmult-1.3.9/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-05-22 10:54:17.000000 schubmult-1.3.9/setup.py
```

### Comparing `schubmult-1.3.8/LICENSE` & `schubmult-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/PKG-INFO` & `schubmult-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.8
+Version: 1.3.9
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.8/README.md` & `schubmult-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/schubmult/perm_lib.py` & `schubmult-1.3.9/schubmult/perm_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,14 +318,21 @@
 	for k,v in d2.items():
 		d1[k] = d1.get(k,0)+v
 	return d1
 
 zero = sympify(0)
 one = sympify(1)
 
+def elem_sym_poly_q(p,k,varl1,varl2):
+	if p == 0 and k>=0:
+		return one
+	if p<0 or p>k:
+		return zero
+	return (varl1[k-1] - varl2[k-p])*elem_sym_poly_q(p-1,k-1,varl1,varl2)+elem_sym_poly_q(p,k-1,varl1,varl2)+q_var[k-1]*elem_sym_poly_q(p-2,k-2,varl1,varl2)
+
 def elem_sym_poly(p,k,varl1,varl2,xstart=0,ystart=0):
 	global zero, one
 	if p>k:
 		return zero
 	if p == 0:
 		return one
 	if p == 1:
```

### Comparing `schubmult-1.3.8/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.9/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.9/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.9/schubmult/schubmult_q/schubmult_q.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.9/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.9/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 var2 = symarray("y",100)
 var3 = symarray("z",100)
 
 var_y = var2.tolist()
 var_z = var3.tolist()
 var_x = symarray("x",100).tolist()
 
+x = var_x
+y = var_y
+z = var_z
+
+def E(p,k,varl=var_y[1:]):
+	return elem_sym_poly_q(p,k,var_x[1:],varl)
+
 def single_variable(coeff_dict,varnum):
 	ret = {}
 	for u in coeff_dict:
 		if varnum -1 < len(u):
 			ret[u] = ret.get(u,0) + var2[u[varnum-1]]*coeff_dict[u]
 		else:
 			ret[u] = ret.get(u,0) + var2[varnum]*coeff_dict[u]
@@ -263,21 +270,29 @@
 		msg = False
 		just_nil = False
 		mult = False
 		
 		nil_N = 0
 		
 		mulstring = ""
+		norep = False
+		expa = False
 		
 		try:
 			for s in sys.argv[1:]:
 				if just_nil:
 					just_nil = False
 					nil_N = int(s)
 					continue
+				if s == "--norep":
+					norep = True
+					continue
+				if s == "--expand":
+					expa = True
+					continue
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
 				if mult:
 					mulstring += s
 					continue					
 				if s == "-mult":
@@ -318,31 +333,38 @@
 		
 		
 		if ascode:
 			for i in range(len(perms)):
 				perms[i] = tuple(permtrim(uncode(perms[i])))
 		else:
 			for i in range(len(perms)):
+				if len(perms[i])<2 and (len(perms[i])==0 or perms[i][0]==1):
+					perms[i] = (1,2)
 				perms[i] = tuple(permtrim([*perms[i]]))
 		
 		size = 0
 		L = len(perms)
 		
 		if nilhecke:
 			coeff_dict = nil_hecke({(1,2): 1},perms[0],nil_N)			
 			rep = ("y","x")		
 		else:
 			coeff_dict = {perms[0]: 1}
 			for perm in perms[1:]:
 				coeff_dict = schubmult(coeff_dict,perm)
 			if mult:
-				mul_exp = sympify(mulstring)
+				for v in var2:
+					globals()[str(v)] = v
+				for v in var3:
+					globals()[str(v)] = v	
+				for v in var_x:
+					globals()[str(v)] = v	
+				mul_exp = eval(mulstring)
 				coeff_dict = mult_poly(coeff_dict,mul_exp)
-			rep = ("","")
-			rep = ("","")
+			rep = ("","")			
 		
 		if pr:
 			if ascode:
 				width = max([len(str(trimcode(perm))) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			else:
 				width = max([len(str(perm)) for perm in coeff_dict.keys() if expand(coeff_dict[perm])!=0])
 			
@@ -394,17 +416,25 @@
 							if check and expand(val - val2)!=0:
 								if mult:
 									val2 = val
 								else:
 									print(f"error: value not equal; write to schubmult@gmail.com with the case {perms=} {perm=} {val=} {coeff_dict.get(perm,0)=}")
 									exit(1)
 							val = val2
+					if expa:
+						val = expand(val)
 					if val!=0:
 						if ascode:
-							print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
+							if norep:
+								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace(*rep)}")	
+							else:
+								print(f"{str(trimcode(perm)):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 						else:
-							print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
+							if norep:
+								print(f"{str(perm):>{width}}  {str(val).replace(*rep)}")	
+							else:
+								print(f"{str(perm):>{width}}  {str(val).replace('**','^').replace('*',' ').replace(*rep)}")	
 	except BrokenPipeError:
 		pass
 		
 if __name__ == "__main__":
 	main()
```

### Comparing `schubmult-1.3.8/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.9/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,23 @@
 n = 100
 
 var = tuple(symarray('x',n).tolist())
 var2 = tuple(symarray('y',n).tolist())
 var3 = tuple(symarray('z',n).tolist())
 
 var_x = symarray("x",100).tolist()
+var_y = var2
+var_z = var3
+
+x = var_x
+y = var_y
+z = var_z
+
+def E(p,k,varl=var_y[1:]):
+	return elem_sym_poly(p,k,var_x[1:],varl)
 
 def single_variable(coeff_dict,varnum):
 	ret = {}
 	for u in coeff_dict:
 		if varnum -1 < len(u):
 			ret[u] = ret.get(u,0) + var2[u[varnum-1]]*coeff_dict[u]
 		else:
@@ -1596,37 +1605,47 @@
 									print(f"{trimcode(firstperm)}{' ':>{width2}}{trimcode(secondperm)}  {str(val).replace('**','^').replace('*',' ')}")
 		else:
 			if ascode:
 				for i in range(len(perms)):
 					perms[i] = tuple(permtrim(uncode(perms[i])))
 			else:
 				for i in range(len(perms)):
+					if len(perms[i])<2 and (len(perms[i])==0 or perms[i][0]==1):
+						perms[i] = (1,2)
 					perms[i] = tuple(permtrim([*perms[i]]))
 			
 			size = 0
 			L = len(perms)
 			orig_perms = [*perms]
 			while len(perms) != size:
 				size = len(perms)
 				perms = split_perms(perms)
 			
 			coeff_dict = {perms[0]: 1}
 			check_coeff_dict = {perms[0]: 1}
 			
+			if mult:
+				for v in var2:
+					globals()[str(v)] = v
+				for v in var3:
+					globals()[str(v)] = v	
+				for v in var_x:
+					globals()[str(v)] = v	
+			
 			if down:
 				for perm in orig_perms[1:]:
 					check_coeff_dict = schubmult_down(check_coeff_dict,perm)
 				if mult:
-					mul_exp = sympify(mulstring)
+					mul_exp = eval(mulstring)
 					check_coeff_dict = mult_poly_down(check_coeff_dict,mul_exp)				
 			else:
 				for perm in orig_perms[1:]:
 					check_coeff_dict = schubmult(check_coeff_dict,perm)
 				if mult:
-					mul_exp = sympify(mulstring)
+					mul_exp = eval(mulstring)
 					check_coeff_dict = mult_poly(check_coeff_dict,mul_exp)
 			
 			
 			if display_positive and len(perms)==2 and will_formula_work(perms[0],perms[1]) and not mult and not down:
 				coeff_dict = {}
 				th = theta(perms[1])
 				muv = uncode(th)
```

### Comparing `schubmult-1.3.8/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.9/schubmult.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.8
+Version: 1.3.9
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schubmult-1.3.8/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.9/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.8/setup.py` & `schubmult-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.8",
+    version="1.3.9",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

