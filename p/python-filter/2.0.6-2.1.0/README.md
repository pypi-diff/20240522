# Comparing `tmp/python-filter-2.0.6.tar.gz` & `tmp/python_filter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-filter-2.0.6.tar", last modified: Tue Feb  6 13:44:51 2024, max compression
+gzip compressed data, was "python_filter-2.1.0.tar", last modified: Wed May 22 03:53:11 2024, max compression
```

## Comparing `python-filter-2.0.6.tar` & `python_filter-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 13:44:51.905085 python-filter-2.0.6/
--rw-rw-rw-   0        0        0     2182 2024-02-06 13:44:51.878085 python-filter-2.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1758 2024-02-06 13:44:07.000000 python-filter-2.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-06 13:44:51.779086 python-filter-2.0.6/pyfilter/
--rw-rw-rw-   0        0        0      175 2024-02-06 13:21:26.000000 python-filter-2.0.6/pyfilter/__init__.py
--rw-rw-rw-   0        0        0     3817 2024-02-06 13:31:43.000000 python-filter-2.0.6/pyfilter/dict_list.py
--rw-rw-rw-   0        0        0     1917 2024-02-06 13:31:50.000000 python-filter-2.0.6/pyfilter/list.py
--rw-rw-rw-   0        0        0     1616 2024-02-06 13:31:54.000000 python-filter-2.0.6/pyfilter/tuple_list.py
-drwxrwxrwx   0        0        0        0 2024-02-06 13:44:51.834087 python-filter-2.0.6/python_filter.egg-info/
--rw-rw-rw-   0        0        0     2182 2024-02-06 13:44:51.000000 python-filter-2.0.6/python_filter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-02-06 13:44:51.000000 python-filter-2.0.6/python_filter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 13:44:51.000000 python-filter-2.0.6/python_filter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-06 13:44:51.000000 python-filter-2.0.6/python_filter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-06 13:44:51.000000 python-filter-2.0.6/python_filter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-06 13:44:51.905085 python-filter-2.0.6/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-02-06 13:44:33.000000 python-filter-2.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:11.882532 python_filter-2.1.0/
+-rw-rw-rw-   0        0        0     2207 2024-05-22 03:53:11.879531 python_filter-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1758 2024-02-06 13:44:07.000000 python_filter-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:11.834008 python_filter-2.1.0/pyfilter/
+-rw-rw-rw-   0        0        0      175 2024-02-06 13:21:26.000000 python_filter-2.1.0/pyfilter/__init__.py
+-rw-rw-rw-   0        0        0     3817 2024-02-06 13:31:43.000000 python_filter-2.1.0/pyfilter/dict_list.py
+-rw-rw-rw-   0        0        0     1917 2024-02-06 13:31:50.000000 python_filter-2.1.0/pyfilter/list.py
+-rw-rw-rw-   0        0        0     1616 2024-02-06 13:31:54.000000 python_filter-2.1.0/pyfilter/tuple_list.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:53:11.877530 python_filter-2.1.0/python_filter.egg-info/
+-rw-rw-rw-   0        0        0     2207 2024-05-22 03:53:11.000000 python_filter-2.1.0/python_filter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-05-22 03:53:11.000000 python_filter-2.1.0/python_filter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:53:11.000000 python_filter-2.1.0/python_filter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 03:53:11.000000 python_filter-2.1.0/python_filter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 03:53:11.000000 python_filter-2.1.0/python_filter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:53:11.885531 python_filter-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      649 2024-05-22 03:52:50.000000 python_filter-2.1.0/setup.py
```

### Comparing `python-filter-2.0.6/PKG-INFO` & `python_filter-2.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: python-filter
-Version: 2.0.6
-Summary: A biblioteca python-filter oferece classes eficientes para manipulação de listas em Python, proporcionando operações simples e rápidas para encontrar, filtrar e manipular dados em estruturas de dados comuns.
-Author: Marcuth
-Author-email: example@gmail.com
-License: MIT License
-Keywords: filter tools
-Description-Content-Type: text/markdown
-
 # python-filter
 
 A biblioteca `python-filter` oferece classes para trabalhar com listas de forma conveniente e eficiente.
 
 ## Classes Disponíveis
 
 - `DictListFilter`: Manipula listas de dicionários.
@@ -77,8 +67,8 @@
 
 ## Contribuição
 
 Contribuições são bem-vindas! Para sugestões, melhorias ou relatórios de bugs, sinta-se à vontade para abrir uma issue ou enviar um pull request no [repositório GitHub](https://github.com/1Marcuth/python-filter).
 
 ## Licença
 
-Este projeto é licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](https://github.com/1Marcuth/python-filter/blob/main/LICENSE) para obter detalhes.
+Este projeto é licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](https://github.com/1Marcuth/python-filter/blob/main/LICENSE) para obter detalhes.
```

### Comparing `python-filter-2.0.6/pyfilter/dict_list.py` & `python_filter-2.1.0/pyfilter/dict_list.py`

 * *Files identical despite different names*

### Comparing `python-filter-2.0.6/pyfilter/list.py` & `python_filter-2.1.0/pyfilter/list.py`

 * *Files identical despite different names*

### Comparing `python-filter-2.0.6/pyfilter/tuple_list.py` & `python_filter-2.1.0/pyfilter/tuple_list.py`

 * *Files identical despite different names*

### Comparing `python-filter-2.0.6/python_filter.egg-info/PKG-INFO` & `python_filter-2.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: python-filter
-Version: 2.0.6
+Version: 2.1.0
 Summary: A biblioteca python-filter oferece classes eficientes para manipulação de listas em Python, proporcionando operações simples e rápidas para encontrar, filtrar e manipular dados em estruturas de dados comuns.
 Author: Marcuth
 Author-email: example@gmail.com
 License: MIT License
 Keywords: filter tools
 Description-Content-Type: text/markdown
+Requires-Dist: pydantic
 
 # python-filter
 
 A biblioteca `python-filter` oferece classes para trabalhar com listas de forma conveniente e eficiente.
 
 ## Classes Disponíveis
```

### Comparing `python-filter-2.0.6/setup.py` & `python_filter-2.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name = "python-filter",
-    version = "2.0.6",
+    version = "2.1.0",
     license = "MIT License",
     author = "Marcuth",
-    long_description = open("README.MD", encoding = "utf-8").read(),
+    long_description = open("README.md", encoding = "utf-8").read(),
     long_description_content_type = "text/markdown",
     author_email = "example@gmail.com",
     keywords = "filter tools",
     description = "A biblioteca python-filter oferece classes eficientes para manipulação de listas em Python, proporcionando operações simples e rápidas para encontrar, filtrar e manipular dados em estruturas de dados comuns.",
     packages = ["pyfilter"],
     install_requires = ["pydantic"],
 )
```

