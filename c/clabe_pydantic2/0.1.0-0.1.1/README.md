# Comparing `tmp/clabe_pydantic2-0.1.0.tar.gz` & `tmp/clabe_pydantic2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clabe_pydantic2-0.1.0.tar", max compression
+gzip compressed data, was "clabe_pydantic2-0.1.1.tar", max compression
```

## Comparing `clabe_pydantic2-0.1.0.tar` & `clabe_pydantic2-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1067 2024-05-22 11:25:52.823885 clabe_pydantic2-0.1.0/LICENSE
--rw-r--r--   0        0        0     1205 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.0/README.md
--rw-r--r--   0        0        0      392 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.0/clabe_pydantic2/__init__.py
--rw-r--r--   0        0        0     4103 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.0/clabe_pydantic2/banks.py
--rw-r--r--   0        0        0      339 2024-05-22 10:54:26.707362 clabe_pydantic2-0.1.0/clabe_pydantic2/errors.py
--rw-r--r--   0        0        0     1678 2024-05-22 11:01:07.654035 clabe_pydantic2-0.1.0/clabe_pydantic2/types.py
--rw-r--r--   0        0        0     1822 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.0/clabe_pydantic2/validations.py
--rw-r--r--   0        0        0       22 2024-05-22 10:52:41.138658 clabe_pydantic2-0.1.0/clabe_pydantic2/version.py
--rw-r--r--   0        0        0      443 2024-05-22 11:28:16.392843 clabe_pydantic2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 clabe_pydantic2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-22 11:25:52.823885 clabe_pydantic2-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1352 2024-05-22 11:33:00.358737 clabe_pydantic2-0.1.1/README.md
+-rw-r--r--   0        0        0      392 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.1/clabe_pydantic2/__init__.py
+-rw-r--r--   0        0        0     4103 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.1/clabe_pydantic2/banks.py
+-rw-r--r--   0        0        0      339 2024-05-22 10:54:26.707362 clabe_pydantic2-0.1.1/clabe_pydantic2/errors.py
+-rw-r--r--   0        0        0     1678 2024-05-22 11:01:07.654035 clabe_pydantic2-0.1.1/clabe_pydantic2/types.py
+-rw-r--r--   0        0        0     1822 2024-05-02 13:16:32.000000 clabe_pydantic2-0.1.1/clabe_pydantic2/validations.py
+-rw-r--r--   0        0        0       22 2024-05-22 10:52:41.138658 clabe_pydantic2-0.1.1/clabe_pydantic2/version.py
+-rw-r--r--   0        0        0      443 2024-05-22 11:33:25.346903 clabe_pydantic2-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 clabe_pydantic2-0.1.1/PKG-INFO
```

### Comparing `clabe_pydantic2-0.1.0/LICENSE` & `clabe_pydantic2-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clabe_pydantic2-0.1.0/clabe_pydantic2/banks.py` & `clabe_pydantic2-0.1.1/clabe_pydantic2/banks.py`

 * *Files identical despite different names*

### Comparing `clabe_pydantic2-0.1.0/clabe_pydantic2/types.py` & `clabe_pydantic2-0.1.1/clabe_pydantic2/types.py`

 * *Files identical despite different names*

### Comparing `clabe_pydantic2-0.1.0/clabe_pydantic2/validations.py` & `clabe_pydantic2-0.1.1/clabe_pydantic2/validations.py`

 * *Files identical despite different names*

### Comparing `clabe_pydantic2-0.1.0/PKG-INFO` & `clabe_pydantic2-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: clabe_pydantic2
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Maksim Dyurdeev
 Author-email: m.dyurdeev@ya.ru
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # CLABE
 
-[![test](https://github.com/cuenca-mx/clabe-python/workflows/test/badge.svg)](https://github.com/cuenca-mx/clabe-python/actions?query=workflow%3Atest)
-[![codecov](https://codecov.io/gh/cuenca-mx/clabe-python/branch/main/graph/badge.svg)](https://codecov.io/gh/cuenca-mx/clabe-python)
-[![PyPI](https://img.shields.io/pypi/v/clabe.svg)](https://pypi.org/project/clabe/)
-[![Downloads](https://pepy.tech/badge/clabe)](https://pepy.tech/project/clabe)
+[//]: # ([![test]&#40;https://github.com/cuenca-mx/clabe-python/workflows/test/badge.svg&#41;]&#40;https://github.com/cuenca-mx/clabe-python/actions?query=workflow%3Atest&#41;)
+
+[//]: # ([![codecov]&#40;https://codecov.io/gh/cuenca-mx/clabe-python/branch/main/graph/badge.svg&#41;]&#40;https://codecov.io/gh/cuenca-mx/clabe-python&#41;)
+
+[//]: # ([![PyPI]&#40;https://img.shields.io/pypi/v/clabe.svg&#41;]&#40;https://pypi.org/project/clabe/&#41;)
+
+[//]: # ([![Downloads]&#40;https://pepy.tech/badge/clabe&#41;]&#40;https://pepy.tech/project/clabe&#41;)
 
 Librería para validar y calcular un número CLABE basado en
 https://es.wikipedia.org/wiki/CLABE
 
 ## Requerimientos
 
-Python 3.6 o superior.
+Python ^3.11
 
 ## Instalación
 
 Se puede instalar desde Pypi usando
 
 ```
-pip install clabe
+pip install clabe_pydantic2
 ```
 
 ## Pruebas
 
 Para ejecutar las pruebas
 
 ```
@@ -42,32 +45,32 @@
 ```
 
 ## Uso básico
 
 Obtener el dígito de control de un número CLABE
 
 ```python
-import clabe
+import clabe_pydantic2
 clabe.compute_control_digit('00200000000000000')
 ```
 
 Para validar si un número CLABE es válido
 
 ```python
-import clabe
+import clabe_pydantic2
 clabe.validate_clabe('002000000000000008')
 ```
 
 Para obtener el banco a partir de 3 dígitos
 
 ```python
-import clabe
+import clabe_pydantic2
 clabe.get_bank_name('002')
 ```
 
 Para generar nuevo válido CLABES
 
 ```python
-import clabe
+import clabe_pydantic2
 clabe.generate_new_clabes(10, '002123456')
 ```
```

