# Comparing `tmp/MARCIA-0.1.3.tar.gz` & `tmp/marcia-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hadrien/Documents/MARCIA/dist/tmp5qngn9de/MARCIA-0.1.3.tar", last modified: Sun May  9 09:26:46 2021, max compression
+gzip compressed data, was "MARCIA-0.1.4.tar", last modified: Wed May 22 19:28:01 2024, max compression
```

## Comparing `MARCIA-0.1.3.tar` & `marcia-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2021-05-09 09:26:46.000000 MARCIA-0.1.3/
--rw-r--r--   0 hadrien    (501) staff       (20)     1608 2021-05-09 09:26:46.000000 MARCIA-0.1.3/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)    35149 2021-01-31 22:57:29.000000 MARCIA-0.1.3/LICENSE
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/
--rw-r--r--   0 hadrien    (501) staff       (20)     1608 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/PKG-INFO
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2021-05-09 09:26:45.000000 MARCIA-0.1.3/MARCIA.egg-info/not-zip-safe
--rw-r--r--   0 hadrien    (501) staff       (20)      238 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/SOURCES.txt
--rw-r--r--   0 hadrien    (501) staff       (20)      125 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/requires.txt
--rw-r--r--   0 hadrien    (501) staff       (20)       21 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/top_level.txt
--rw-r--r--   0 hadrien    (501) staff       (20)        1 2021-05-09 09:26:46.000000 MARCIA-0.1.3/MARCIA.egg-info/dependency_links.txt
--rw-r--r--   0 hadrien    (501) staff       (20)      698 2021-05-09 09:24:41.000000 MARCIA-0.1.3/README.md
--rw-r--r--   0 hadrien    (501) staff       (20)     1226 2021-05-09 09:24:20.000000 MARCIA-0.1.3/setup.py
--rw-r--r--   0 hadrien    (501) staff       (20)       38 2021-05-09 09:26:46.000000 MARCIA-0.1.3/setup.cfg
-drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2021-05-09 09:26:46.000000 MARCIA-0.1.3/marcia/
--rw-r--r--   0 hadrien    (501) staff       (20)    37667 2021-05-09 09:22:58.000000 MARCIA-0.1.3/marcia/mask.py
--rw-r--r--   0 hadrien    (501) staff       (20)        0 2021-01-31 22:57:30.000000 MARCIA-0.1.3/marcia/__init__.py
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-22 19:28:01.978878 MARCIA-0.1.4/
+-rw-r--r--   0 hadrien    (501) staff       (20)    35149 2024-05-22 19:23:29.000000 MARCIA-0.1.4/LICENSE
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-22 19:28:01.976893 MARCIA-0.1.4/MARCIA.egg-info/
+-rw-r--r--   0 hadrien    (501) staff       (20)     1404 2024-05-22 19:28:01.000000 MARCIA-0.1.4/MARCIA.egg-info/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      238 2024-05-22 19:28:01.000000 MARCIA-0.1.4/MARCIA.egg-info/SOURCES.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2024-05-22 19:28:01.000000 MARCIA-0.1.4/MARCIA.egg-info/dependency_links.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)        1 2024-05-22 19:24:11.000000 MARCIA-0.1.4/MARCIA.egg-info/not-zip-safe
+-rw-r--r--   0 hadrien    (501) staff       (20)       68 2024-05-22 19:28:01.000000 MARCIA-0.1.4/MARCIA.egg-info/requires.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)       21 2024-05-22 19:28:01.000000 MARCIA-0.1.4/MARCIA.egg-info/top_level.txt
+-rw-r--r--   0 hadrien    (501) staff       (20)     1404 2024-05-22 19:28:01.978622 MARCIA-0.1.4/PKG-INFO
+-rw-r--r--   0 hadrien    (501) staff       (20)      687 2024-05-22 19:23:55.000000 MARCIA-0.1.4/README.md
+drwxr-xr-x   0 hadrien    (501) staff       (20)        0 2024-05-22 19:28:01.977401 MARCIA-0.1.4/marcia/
+-rw-r--r--   0 hadrien    (501) staff       (20)        0 2024-05-22 19:23:55.000000 MARCIA-0.1.4/marcia/__init__.py
+-rw-r--r--   0 hadrien    (501) staff       (20)    37627 2024-05-22 19:23:55.000000 MARCIA-0.1.4/marcia/mask.py
+-rw-r--r--   0 hadrien    (501) staff       (20)       38 2024-05-22 19:28:01.978993 MARCIA-0.1.4/setup.cfg
+-rw-r--r--   0 hadrien    (501) staff       (20)     1226 2024-05-22 19:23:55.000000 MARCIA-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MARCIA-0.1.3/PKG-INFO` & `MARCIA-0.1.4/MARCIA.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: MARCIA
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manual hyperspectral data classifier
 Home-page: https://github.com/hameye/marcia
 Author: Hadrien Meyer
 Author-email: meyerhadrien96@gmail.com
 License: GPL v3
 Project-URL: Example, https://github.com/hameye/MARCIA/blob/master/examples/Tutorial.ipynb
 Project-URL: Source, https://github.com/hameye/MARCIA
 Project-URL: Report a bug, https://github.com/hameye/MARCIA/issues
-Description: 
-        # MARCIA - MAsking spectRosCopIc dAtacube
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3929745.svg)](https://doi.org/10.5281/zenodo.3929745)
-        [![PyPI](https://img.shields.io/badge/MARCIA-v0.1.3-blue.svg?maxAge=2592000)](https://pypi.org/project/MARCIA/)
-        
-        ## Manual classifier for µXRF and EDS/SEM hypercubes
-         - Classification is achieved by defining masks that are linear combination of elemental intensities in spectra.
-         - Classes can then be extracted and read with hyperspy or PyMca or Esprit
-        
-        
-        ## Install
-        Just do
-        ```bash
-        pip install marcia
-        ```
-        
-        ## Use in python
-        ```python
-        from marcia.mask import Mask
-        ```
-        
-        ## Gallery
-        ![Example](https://github.com/hameye/MARCIA/blob/master/gallery.png)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# MARCIA - MAsking spectRosCopIc dAtacube
+[![DOI](https://zenodo.org/badge/263880541.svg)](https://zenodo.org/badge/latestdoi/263880541)
+[![PyPI](https://img.shields.io/badge/MARCIA-v0.1.3-blue.svg?maxAge=2592000)](https://pypi.org/project/MARCIA/)
+
+## Manual classifier for µXRF and EDS/SEM hypercubes
+ - Classification is achieved by defining masks that are linear combination of elemental intensities in spectra.
+ - Classes can then be extracted and read with hyperspy or PyMca or Esprit
+
+
+## Install
+Just do
+```bash
+pip install marcia
+```
+
+## Use in python
+```python
+from marcia.mask import Mask
+```
+
+## Gallery
+![Example](https://github.com/hameye/MARCIA/blob/master/gallery.png)
```

### Comparing `MARCIA-0.1.3/LICENSE` & `MARCIA-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MARCIA-0.1.3/MARCIA.egg-info/PKG-INFO` & `MARCIA-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: MARCIA
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manual hyperspectral data classifier
 Home-page: https://github.com/hameye/marcia
 Author: Hadrien Meyer
 Author-email: meyerhadrien96@gmail.com
 License: GPL v3
 Project-URL: Example, https://github.com/hameye/MARCIA/blob/master/examples/Tutorial.ipynb
 Project-URL: Source, https://github.com/hameye/MARCIA
 Project-URL: Report a bug, https://github.com/hameye/MARCIA/issues
-Description: 
-        # MARCIA - MAsking spectRosCopIc dAtacube
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3929745.svg)](https://doi.org/10.5281/zenodo.3929745)
-        [![PyPI](https://img.shields.io/badge/MARCIA-v0.1.3-blue.svg?maxAge=2592000)](https://pypi.org/project/MARCIA/)
-        
-        ## Manual classifier for µXRF and EDS/SEM hypercubes
-         - Classification is achieved by defining masks that are linear combination of elemental intensities in spectra.
-         - Classes can then be extracted and read with hyperspy or PyMca or Esprit
-        
-        
-        ## Install
-        Just do
-        ```bash
-        pip install marcia
-        ```
-        
-        ## Use in python
-        ```python
-        from marcia.mask import Mask
-        ```
-        
-        ## Gallery
-        ![Example](https://github.com/hameye/MARCIA/blob/master/gallery.png)
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# MARCIA - MAsking spectRosCopIc dAtacube
+[![DOI](https://zenodo.org/badge/263880541.svg)](https://zenodo.org/badge/latestdoi/263880541)
+[![PyPI](https://img.shields.io/badge/MARCIA-v0.1.3-blue.svg?maxAge=2592000)](https://pypi.org/project/MARCIA/)
+
+## Manual classifier for µXRF and EDS/SEM hypercubes
+ - Classification is achieved by defining masks that are linear combination of elemental intensities in spectra.
+ - Classes can then be extracted and read with hyperspy or PyMca or Esprit
+
+
+## Install
+Just do
+```bash
+pip install marcia
+```
+
+## Use in python
+```python
+from marcia.mask import Mask
+```
+
+## Gallery
+![Example](https://github.com/hameye/MARCIA/blob/master/gallery.png)
```

### Comparing `MARCIA-0.1.3/README.md` & `MARCIA-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # MARCIA - MAsking spectRosCopIc dAtacube
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3929745.svg)](https://doi.org/10.5281/zenodo.3929745)
+[![DOI](https://zenodo.org/badge/263880541.svg)](https://zenodo.org/badge/latestdoi/263880541)
 [![PyPI](https://img.shields.io/badge/MARCIA-v0.1.3-blue.svg?maxAge=2592000)](https://pypi.org/project/MARCIA/)
 
 ## Manual classifier for µXRF and EDS/SEM hypercubes
  - Classification is achieved by defining masks that are linear combination of elemental intensities in spectra.
  - Classes can then be extracted and read with hyperspy or PyMca or Esprit
```

### Comparing `MARCIA-0.1.3/setup.py` & `MARCIA-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='MARCIA',
-    version='0.1.3',
+    version='0.1.4',
     description='Manual hyperspectral data classifier',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/hameye/marcia',
     author='Hadrien Meyer',
     author_email='meyerhadrien96@gmail.com',
     license='GPL v3',
@@ -25,15 +25,15 @@
             'doc.*']),
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.6",
         "Typing :: Typed",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     install_requires=requirements(),
     zip_safe=False,
     project_urls={
         'Example': 'https://github.com/hameye/MARCIA/blob/master/examples/Tutorial.ipynb',
         'Source': 'https://github.com/hameye/MARCIA',
         'Report a bug': 'https://github.com/hameye/MARCIA/issues',
     })
```

### Comparing `MARCIA-0.1.3/marcia/mask.py` & `MARCIA-0.1.4/marcia/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -507,19 +507,19 @@
         finite_data = self.data_cube[:, :, indice][np.isfinite(
             self.data_cube[:, :, indice])]
         im = ax[0].imshow(self.data_cube[:, :, indice])
         ax[0].grid()
         ax[0].set_title("Carte élémentaire : " + self.Elements[indice])
         fig.colorbar(im, ax=ax[0])
         plt.ylim(0, np.max(finite_data))
-        sns.distplot(finite_data,
+        sns.histplot(y=finite_data,
                      kde=False,
                      ax=axes[1],
-                     hist_kws={'range': (0.0, np.max(finite_data))},
-                     vertical=True)
+                     binwidth=2,
+                     ec=None)
 
         # Logarithm scale because background has a lof ot points and flatten
         # interesting information if linear
         ax[1].set_xscale('log')
         ax[1].set_title("Histograme d'intensité : " + self.Elements[indice])
         fig.tight_layout()
         plt.show()
```

