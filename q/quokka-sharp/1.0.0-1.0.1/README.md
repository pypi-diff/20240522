# Comparing `tmp/quokka_sharp-1.0.0.tar.gz` & `tmp/quokka_sharp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quokka_sharp-1.0.0.tar", last modified: Tue May 14 16:14:17 2024, max compression
+gzip compressed data, was "quokka_sharp-1.0.1.tar", last modified: Wed May 22 07:56:00 2024, max compression
```

## Comparing `quokka_sharp-1.0.0.tar` & `quokka_sharp-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.723086 quokka_sharp-1.0.0/
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      733 2024-05-14 16:14:17.722772 quokka_sharp-1.0.0/PKG-INFO
-drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.719165 quokka_sharp-1.0.0/quokka_sharp/
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      207 2024-03-18 14:38:39.000000 quokka_sharp-1.0.0/quokka_sharp/__init__.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     2224 2024-04-18 11:56:40.000000 quokka_sharp-1.0.0/quokka_sharp/ecmc.py
-drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.722043 quokka_sharp-1.0.0/quokka_sharp/encoding/
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      139 2024-03-18 14:38:30.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/__init__.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     9064 2024-05-14 15:44:03.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/cliffordt2cnf.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     4227 2024-04-05 11:20:57.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/cnf.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1115 2024-01-31 13:15:02.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/memory.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     4439 2024-05-14 15:58:43.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/qasm2cnf.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     5994 2024-03-18 12:57:29.000000 quokka_sharp-1.0.0/quokka_sharp/encoding/qasm_parser.py
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1216 2024-04-20 09:44:17.000000 quokka_sharp-1.0.0/quokka_sharp/qcmc.py
-drwxr-xr-x   0 meij     (1596456755) VUW\Domain Users (208802054)        0 2024-05-14 16:14:17.722461 quokka_sharp-1.0.0/quokka_sharp.egg-info/
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      733 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/PKG-INFO
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)      424 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/SOURCES.txt
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)        1 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/dependency_links.txt
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)       13 2024-05-14 16:14:17.000000 quokka_sharp-1.0.0/quokka_sharp.egg-info/top_level.txt
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)       38 2024-05-14 16:14:17.723158 quokka_sharp-1.0.0/setup.cfg
--rw-r--r--   0 meij     (1596456755) VUW\Domain Users (208802054)     1046 2024-05-14 16:13:40.000000 quokka_sharp-1.0.0/setup.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-05-22 07:56:00.817454 quokka_sharp-1.0.1/
+-rw-r--r--   0 meij     (1596456755) 208802054      733 2024-05-22 07:56:00.817105 quokka_sharp-1.0.1/PKG-INFO
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-05-22 07:56:00.811515 quokka_sharp-1.0.1/quokka_sharp/
+-rw-r--r--   0 meij     (1596456755) 208802054      207 2024-03-18 14:38:39.000000 quokka_sharp-1.0.1/quokka_sharp/__init__.py
+-rw-r--r--   0 meij     (1596456755) 208802054     2224 2024-05-22 07:53:17.000000 quokka_sharp-1.0.1/quokka_sharp/ecmc.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-05-22 07:56:00.816531 quokka_sharp-1.0.1/quokka_sharp/encoding/
+-rw-r--r--   0 meij     (1596456755) 208802054      139 2024-03-18 14:38:30.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/__init__.py
+-rw-r--r--   0 meij     (1596456755) 208802054     9064 2024-05-14 15:44:03.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/cliffordt2cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     4227 2024-04-05 11:20:57.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     1115 2024-01-31 13:15:02.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/memory.py
+-rw-r--r--   0 meij     (1596456755) 208802054     4439 2024-05-17 12:32:14.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/qasm2cnf.py
+-rw-r--r--   0 meij     (1596456755) 208802054     5994 2024-03-18 12:57:29.000000 quokka_sharp-1.0.1/quokka_sharp/encoding/qasm_parser.py
+-rw-r--r--   0 meij     (1596456755) 208802054     1216 2024-04-20 09:44:17.000000 quokka_sharp-1.0.1/quokka_sharp/qcmc.py
+drwxr-xr-x   0 meij     (1596456755) 208802054        0 2024-05-22 07:56:00.816825 quokka_sharp-1.0.1/quokka_sharp.egg-info/
+-rw-r--r--   0 meij     (1596456755) 208802054      733 2024-05-22 07:56:00.000000 quokka_sharp-1.0.1/quokka_sharp.egg-info/PKG-INFO
+-rw-r--r--   0 meij     (1596456755) 208802054      424 2024-05-22 07:56:00.000000 quokka_sharp-1.0.1/quokka_sharp.egg-info/SOURCES.txt
+-rw-r--r--   0 meij     (1596456755) 208802054        1 2024-05-22 07:56:00.000000 quokka_sharp-1.0.1/quokka_sharp.egg-info/dependency_links.txt
+-rw-r--r--   0 meij     (1596456755) 208802054       13 2024-05-22 07:56:00.000000 quokka_sharp-1.0.1/quokka_sharp.egg-info/top_level.txt
+-rw-r--r--   0 meij     (1596456755) 208802054       38 2024-05-22 07:56:00.817520 quokka_sharp-1.0.1/setup.cfg
+-rw-r--r--   0 meij     (1596456755) 208802054     1046 2024-05-22 07:52:41.000000 quokka_sharp-1.0.1/setup.py
```

### Comparing `quokka_sharp-1.0.0/PKG-INFO` & `quokka_sharp-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka_sharp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quokka Sharp
 Author: System Verification Lab
 Author-email: j.mei@liacs.leidenuniv.nl
 Keywords: python,quantum circuits
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quokka_sharp-1.0.0/quokka_sharp/ecmc.py` & `quokka_sharp-1.0.1/quokka_sharp/ecmc.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # TODO: information for arguments in functions
 
 def get_result(result):
     result = str(result)
     gpmc_ans_str = re.findall(r"exact.double.prec-sci.(.+?)\\nc s",result)[0]
     gpmc_ans = float(gpmc_ans_str)
-    if abs(gpmc_ans - 1) > 1e-15:
+    if abs(gpmc_ans - 1) > 1e-12:
         return False
     else: return True
 
 def basis(i, Z_or_X, cnf, cnf_file_root):
     cnf_temp = copy.deepcopy(cnf)
     cnf_temp.rightProjectZXi(Z_or_X, i)
     cnf_temp.leftProjectZXi(Z_or_X, i)
```

### Comparing `quokka_sharp-1.0.0/quokka_sharp/encoding/cliffordt2cnf.py` & `quokka_sharp-1.0.1/quokka_sharp/encoding/cliffordt2cnf.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-1.0.0/quokka_sharp/encoding/cnf.py` & `quokka_sharp-1.0.1/quokka_sharp/encoding/cnf.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-1.0.0/quokka_sharp/encoding/memory.py` & `quokka_sharp-1.0.1/quokka_sharp/encoding/memory.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-1.0.0/quokka_sharp/encoding/qasm2cnf.py` & `quokka_sharp-1.0.1/quokka_sharp/encoding/qasm2cnf.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
             else:
                 theta = Decimal(float(theta_str))
         return theta
     except:
         raise Exception(angle, "is not supported")
 
 def get_cos_sin(theta):
-    res_cos = str(Decimal(math.cos(theta)))
+    res_cos = Decimal(math.cos(theta))
     if abs(res_cos) < 1e-15:
         res_cos = 0
-    res_sin = str(Decimal(math.sin(theta)))
+    res_sin = Decimal(math.sin(theta))
     if abs(res_sin) < 1e-15:
         res_sin = 0
-    return [res_cos, res_sin]
+    return [str(res_cos), str(res_sin)]
 
 def QASM2CNF(circuit : Circuit) -> CNF:
 
     cnf = CNF(circuit.n)
 
     for element in circuit.circ:
         gate = element[0]
```

### Comparing `quokka_sharp-1.0.0/quokka_sharp/encoding/qasm_parser.py` & `quokka_sharp-1.0.1/quokka_sharp/encoding/qasm_parser.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-1.0.0/quokka_sharp/qcmc.py` & `quokka_sharp-1.0.1/quokka_sharp/qcmc.py`

 * *Files identical despite different names*

### Comparing `quokka_sharp-1.0.0/quokka_sharp.egg-info/PKG-INFO` & `quokka_sharp-1.0.1/quokka_sharp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quokka_sharp
-Version: 1.0.0
+Version: 1.0.1
 Summary: Quokka Sharp
 Author: System Verification Lab
 Author-email: j.mei@liacs.leidenuniv.nl
 Keywords: python,quantum circuits
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quokka_sharp-1.0.0/setup.py` & `quokka_sharp-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Quokka Sharp'
 LONG_DESCRIPTION = '''
                     Quokka Sharp for simulating and equivalence checking 
                     of quantum circuits based on weighted model counting.
                     You have to intall a weighted model counting tool first.
                     '''
```

