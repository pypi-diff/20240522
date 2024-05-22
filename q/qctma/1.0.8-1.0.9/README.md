# Comparing `tmp/qctma-1.0.8.tar.gz` & `tmp/qctma-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Marc\Python Projects\QCTMA\qctma1.0.x\dist\tmpexg73o2l\qctma-1.0.8.tar", last modified: Tue May  4 07:49:15 2021, max compression
+gzip compressed data, was "D:\Marc\Python Projects\QCTMA\qctma1.0.x\dist\tmp9b_ylt1d\qctma-1.0.9.tar", last modified: Mon May 31 12:52:09 2021, max compression
```

## Comparing `qctma-1.0.8.tar` & `qctma-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2021-05-04 07:49:15.000000 qctma-1.0.8/
--rw-rw-rw-   0        0        0      619 2021-05-04 07:49:15.000000 qctma-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      302 2021-05-03 09:15:12.000000 qctma-1.0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-03-23 10:34:13.000000 qctma-1.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2021-05-04 07:49:15.000000 qctma-1.0.8/qctma.egg-info/
--rw-rw-rw-   0        0        0      619 2021-05-04 07:49:14.000000 qctma-1.0.8/qctma.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2021-05-04 07:49:14.000000 qctma-1.0.8/qctma.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-04 07:49:14.000000 qctma-1.0.8/qctma.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      911 2021-05-04 07:49:14.000000 qctma-1.0.8/qctma.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2021-05-04 07:49:14.000000 qctma-1.0.8/qctma.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    24194 2021-05-03 11:20:14.000000 qctma-1.0.8/qctma.py
--rw-rw-rw-   0        0        0     7556 2021-05-04 07:45:18.000000 qctma-1.0.8/rw_cdb.py
--rw-rw-rw-   0        0        0       42 2021-05-04 07:49:15.000000 qctma-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2191 2021-05-03 11:20:14.000000 qctma-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-31 12:52:09.000000 qctma-1.0.9/
+-rw-rw-rw-   0        0        0      610 2021-05-31 12:52:09.000000 qctma-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2021-05-03 09:15:12.000000 qctma-1.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-03-23 10:34:13.000000 qctma-1.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/
+-rw-rw-rw-   0        0        0      610 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      911 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2021-05-31 12:52:09.000000 qctma-1.0.9/qctma.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    24132 2021-05-31 12:47:16.000000 qctma-1.0.9/qctma.py
+-rw-rw-rw-   0        0        0     7556 2021-05-31 12:47:37.000000 qctma-1.0.9/rw_cdb.py
+-rw-rw-rw-   0        0        0       42 2021-05-31 12:52:09.000000 qctma-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2191 2021-05-31 12:47:42.000000 qctma-1.0.9/setup.py
```

### Comparing `qctma-1.0.8/PKG-INFO` & `qctma-1.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: qctma
-Version: 1.0.8
+Version: 1.0.9
 Summary: Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
 Home-page: https://github.com/MarcG-LBMC-Lyos/QCTMA
 Author: Marc Gardegaront
 Author-email: m.gardegaront@gmail.com
 License: GNU GPLv3
-Description: Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
 Platform: UNKNOWN
 Requires-Python: >=3.6
+
+Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
+
```

### Comparing `qctma-1.0.8/qctma.egg-info/PKG-INFO` & `qctma-1.0.9/qctma.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: qctma
-Version: 1.0.8
+Version: 1.0.9
 Summary: Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
 Home-page: https://github.com/MarcG-LBMC-Lyos/QCTMA
 Author: Marc Gardegaront
 Author-email: m.gardegaront@gmail.com
 License: GNU GPLv3
-Description: Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
 Platform: UNKNOWN
 Requires-Python: >=3.6
+
+Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young'smodulus relationships. Specifically designed to be used with Ansys .cdb meshes.
+
```

### Comparing `qctma-1.0.8/qctma.egg-info/requires.txt` & `qctma-1.0.9/qctma.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qctma-1.0.8/qctma.py` & `qctma-1.0.9/qctma.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from reportlab.lib.enums import TA_JUSTIFY
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import SimpleDocTemplate, Paragraph, Preformatted, Spacer, Image
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 class qctma(object):
     """
     Class used to load Dicom files and mesh file, and create a new mesh implementing materials based on gray level to
     density relationship and density to Young's modulus relationship.
     """
 
@@ -277,17 +277,17 @@
                 # Returns the coordinates in the correct shape for 1: use it with the interp function and 2: use it with the
                 # integrate function.
                 # i.e. interp function uses the shape [tet1, ..., teti] with teti = [v1i, v2i, v3i, v4i]
                 # integrate function uses the shape [integ_points1, ..., integ_pointsi] with integ_pointsi being the list of
                 # integration points for tetrahedron i.
                 return [interp(args[0][0][i], args[0][1][i], args[0][2][i]) for i in range(len(args[0][0]))]
 
-            scheme = qp.c3._witherden_vincent.witherden_vincent_11()  # Integration scheme
+            scheme = qp.c3.get_good_scheme(11)  # Integration scheme
         else:
-            scheme = qp.t3._witherden_vincent.witherden_vincent_10()  # Integration scheme
+            scheme = qp.t3.get_good_scheme(11)  # Integration scheme
 
         v1 = []  # List of the first vertex of each tetrahedron
         v2 = []  # List of the second vertex of each tetrahedron
         v3 = []  # List of the third vertex of each tetrahedron
         v4 = []  # List of the fourth vertex of each tetrahedron
         if is_cube:
             v_cube = []
@@ -332,19 +332,19 @@
     def reduce_material_nb(self):
         """
         Reduce the number of material by grouping material within a step defined by self.deltaE
         """
         mat_max = np.max(self.e_elems)
         self.e_pool = []
         self.matid = np.zeros(len(self.e_elems))
-        while mat_max >= np.min(self.e_elems) and mat_max != -self.deltaE - 1:
+        while mat_max >= np.min(self.e_elems) and mat_max != -np.inf:
             max_elem_group_mask = self.e_elems >= mat_max - self.deltaE  # Elements within mat_max and mat_max-deltaE
             self.e_pool.append(np.mean(self.e_elems[max_elem_group_mask]))  # np.mean() or mat_max ?
             self.matid[max_elem_group_mask] = len(self.e_pool)
-            self.e_elems[max_elem_group_mask] = -self.deltaE - 1
+            self.e_elems[max_elem_group_mask] = -np.inf
             mat_max = np.max(self.e_elems)
 
     def inv_num(self, f, ys, init_guess=[0, 2], max_err=0.001):
         """
         Find the value corresponding to the inverse of the function f at y.
         :param f: Function to be inversed.
         :param ys: Values at which the inverse function will be computed.
```

### Comparing `qctma-1.0.8/rw_cdb.py` & `qctma-1.0.9/rw_cdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 def read_cdbfile(path, type='Tet'):
     """
     Extract the elements number and their associated material from a cdb mesh file.
     :param path: Path to the cdb file.
     :return: Elements number array and associated materials, Nodes and associated coordinates x, y and z arrays.
     """
```

### Comparing `qctma-1.0.8/setup.py` & `qctma-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='qctma',
-      version='1.0.8',
+      version='1.0.9',
       description="Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young's"
                   "modulus relationships. Specifically designed to be used with Ansys .cdb meshes.",
       long_description="Injects material (Young's modulus) to each element, based on a Dicom stack, and gray level to Young's"
                        "modulus relationships. Specifically designed to be used with Ansys .cdb meshes.",
       url='https://github.com/MarcG-LBMC-Lyos/QCTMA',
       author='Marc Gardegaront',
       author_email='m.gardegaront@gmail.com',
```

