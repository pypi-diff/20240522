# Comparing `tmp/plataforma-automaxia-api-0.0.6.tar.gz` & `tmp/plataforma-automaxia-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\plataforma-automaxia-api-0.0.6.tar", last modified: Wed Mar 27 19:15:15 2024, max compression
+gzip compressed data, was "plataforma-automaxia-api-0.0.7.tar", last modified: Wed May 22 16:37:19 2024, max compression
```

## Comparing `plataforma-automaxia-api-0.0.6.tar` & `plataforma-automaxia-api-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 19:15:15.023137 plataforma-automaxia-api-0.0.6/
--rw-rw-rw-   0        0        0     4685 2024-03-27 19:15:15.001750 plataforma-automaxia-api-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3224 2024-03-27 19:10:10.000000 plataforma-automaxia-api-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 19:15:14.986753 plataforma-automaxia-api-0.0.6/plataforma/
--rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 plataforma-automaxia-api-0.0.6/plataforma/__init__.py
--rw-rw-rw-   0        0        0    13696 2024-03-27 19:08:52.000000 plataforma-automaxia-api-0.0.6/plataforma/automaxia_api.py
-drwxrwxrwx   0        0        0        0 2024-03-27 19:15:15.000749 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/
--rw-rw-rw-   0        0        0     4685 2024-03-27 19:15:14.000000 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-03-27 19:15:14.000000 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 19:15:14.000000 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-27 19:15:14.000000 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-27 19:15:14.000000 plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 19:15:15.023137 plataforma-automaxia-api-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-03-27 19:09:05.000000 plataforma-automaxia-api-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:37:19.856307 plataforma-automaxia-api-0.0.7/
+-rw-rw-rw-   0        0        0     1109 2023-02-27 17:07:43.000000 plataforma-automaxia-api-0.0.7/LICENCE
+-rw-rw-rw-   0        0        0     3845 2024-05-22 16:37:19.855785 plataforma-automaxia-api-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2024-03-27 19:16:26.000000 plataforma-automaxia-api-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 16:37:19.814529 plataforma-automaxia-api-0.0.7/plataforma/
+-rw-rw-rw-   0        0        0        0 2022-06-23 22:06:41.000000 plataforma-automaxia-api-0.0.7/plataforma/__init__.py
+-rw-rw-rw-   0        0        0    14122 2024-05-22 16:34:34.000000 plataforma-automaxia-api-0.0.7/plataforma/automaxia_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:37:19.852949 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/
+-rw-rw-rw-   0        0        0     3845 2024-05-22 16:37:19.000000 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2024-05-22 16:37:19.000000 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:37:19.000000 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 16:37:19.000000 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 16:37:19.000000 plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:37:19.856838 plataforma-automaxia-api-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      534 2024-05-22 16:25:29.000000 plataforma-automaxia-api-0.0.7/setup.py
```

### Comparing `plataforma-automaxia-api-0.0.6/PKG-INFO` & `plataforma-automaxia-api-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,134 @@
 Metadata-Version: 2.1
 Name: plataforma-automaxia-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrapper oficial da Plataforma Automaxia para Python
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: wesleyromualdo@gmail.com
 License: MIT License
-Description: # Material de apoio
-        
-        O primeiro passo Ã© ter o cÃ³digo de sua biblioteca separado em uma pasta
-        
-          
-        
-        *   meu\_pacote/ # Pasta do projeto
-            *   codigos\_da\_biblioteca/ # DiretÃ³rio onde deve ficar os cÃ³digos de sua biblioteca
-            *   LICENCE # Um arquivo com a licenÃ§a da sua lib
-            *   [README.MD](http://README.MD) # Uma descriÃ§Ã£o do projeto
-            *   [setup.py](http://setup.py) # CÃ³digo Python responsÃ¡vel pelo empacotamento
-        
-          
-        
-        Adicione uma licenÃ§a
-        
-        ```plain
-        The MIT License (MIT)
-        
-        Copyright (c) [year] [fullname]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-        the Software, and to permit persons to whom the Software is furnished to do so,
-        subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-        FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-        COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-        IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-        CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        ```
-        
-          
-        
-        Adicione um readme
-        
-        ```markdown
-        # Sua descriÃ§Ã£o aqui
-        ```
-        
-          
-        
-        Instale a lib setuptools
-        
-        ```plain
-        pip install setuptools
-        ```
-        
-          
-        
-        Crie o [setup.py](http://setup.py)
-        
-        ```plain
-        from setuptools import setup
-        
-        with open("README.md", "r") as arq:
-            readme = arq.read()
-        
-        setup(name='wrapper-panda-video',
-            version='0.0.1',
-            license='MIT License',
-            author='Caio Sampaio',
-            long_description=readme,
-            long_description_content_type="text/markdown",
-            author_email='caio@pythonando.com.br',
-            keywords='panda video',
-            description=u'Wrapper nÃ£o oficial do Panda Video',
-            packages=['panda_video'],
-            install_requires=['requests'],)
-        ```
-        
-          
-        
-        Execute o comando
-        
-        ```plain
-        python setup.py sdist
-        ```
-        
-          
-        
-        Instale o twine para fazer o upload para o pypi
-        
-        ```plain
-        pip install twine
-        ```
-        
-          
-        
-        Crie uma conta no pypi
-        
-          
-        
-        Execute o comando para criar um repositÃ³rio de teste
-        
-        ```plain
-        twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-        ```
-        
-          
-        
-        Ou para criar um repositÃ³rio oficial:
-        
-        ```plain
-        python setup.py sdist
-        twine upload dist/*
-        user: __token__
-        pass: pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q
-        
-        
-        twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q dist/*
-        ```
-        pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
 Keywords: plataforma automaxia api
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Material de apoio
+
+O primeiro passo Ã© ter o cÃ³digo de sua biblioteca separado em uma pasta
+
+  
+
+*   meu\_pacote/ # Pasta do projeto
+    *   codigos\_da\_biblioteca/ # DiretÃ³rio onde deve ficar os cÃ³digos de sua biblioteca
+    *   LICENCE # Um arquivo com a licenÃ§a da sua lib
+    *   [README.MD](http://README.MD) # Uma descriÃ§Ã£o do projeto
+    *   [setup.py](http://setup.py) # CÃ³digo Python responsÃ¡vel pelo empacotamento
+
+  
+
+Adicione uma licenÃ§a
+
+```plain
+The MIT License (MIT)
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+```
+
+  
+
+Adicione um readme
+
+```markdown
+# Sua descriÃ§Ã£o aqui
+```
+
+  
+
+Instale a lib setuptools
+
+```plain
+pip install setuptools
+```
+
+  
+
+Crie o [setup.py](http://setup.py)
+
+```plain
+from setuptools import setup
+
+with open("README.md", "r") as arq:
+    readme = arq.read()
+
+setup(name='wrapper-panda-video',
+    version='0.0.1',
+    license='MIT License',
+    author='Caio Sampaio',
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    author_email='caio@pythonando.com.br',
+    keywords='panda video',
+    description=u'Wrapper nÃ£o oficial do Panda Video',
+    packages=['panda_video'],
+    install_requires=['requests'],)
+```
+
+  
+
+Execute o comando
+
+```plain
+python setup.py sdist
+```
+
+  
+
+Instale o twine para fazer o upload para o pypi
+
+```plain
+pip install twine
+```
+
+  
+
+Crie uma conta no pypi
+
+  
+
+Execute o comando para criar um repositÃ³rio de teste
+
+```plain
+twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+```
+
+  
+
+Ou para criar um repositÃ³rio oficial:
+
+```plain
+python setup.py sdist
+twine upload dist/*
+user: __token__
+pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
+
+
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
+```
+pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
+
```

### Comparing `plataforma-automaxia-api-0.0.6/README.md` & `plataforma-automaxia-api-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -108,13 +108,13 @@
 
 Ou para criar um repositório oficial:
 
 ```plain
 python setup.py sdist
 twine upload dist/*
 user: __token__
-pass: pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q
+pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
 
 
-twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q dist/*
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
 ```
 pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
```

### Comparing `plataforma-automaxia-api-0.0.6/plataforma/automaxia_api.py` & `plataforma-automaxia-api-0.0.7/plataforma/automaxia_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,24 @@
         return response
 
     def get_tarefa_by_id(self, tarefa_id):
         url = str(self.url)+"/tarefa/"+str(tarefa_id)
         response = self.get(url)
         return response
 
+    def get_configuracao_by_tarefa(self, tx_nome, tarefa_id):
+        url = str(self.url)+f"/configuracao?tx_nome={tx_nome}&tarefa_id={tarefa_id}&bo_status=True"
+        response = self.get(url)
+        return response
+    
+    def get_configuracao_by_chave(self, tx_chave, tarefa_id):
+        url = str(self.url)+f"/configuracao/{tx_chave}/{tarefa_id}"
+        response = self.get(url)
+        return response
+    
     def get_tarefa_by_constante_virtual(self, constante_virtual):
         url = str(self.url)+"/tarefa/constante_virtual/"+str(constante_virtual)
         response = self.get(url)
         return response
 
     def get_automacao_by_id(self, automacao_id):
         url = str(self.url)+"/automacao/"+str(automacao_id)
```

### Comparing `plataforma-automaxia-api-0.0.6/plataforma_automaxia_api.egg-info/PKG-INFO` & `plataforma-automaxia-api-0.0.7/plataforma_automaxia_api.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,134 @@
 Metadata-Version: 2.1
 Name: plataforma-automaxia-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrapper oficial da Plataforma Automaxia para Python
 Home-page: UNKNOWN
 Author: Wesley Romualdo da Silva
 Author-email: wesleyromualdo@gmail.com
 License: MIT License
-Description: # Material de apoio
-        
-        O primeiro passo Ã© ter o cÃ³digo de sua biblioteca separado em uma pasta
-        
-          
-        
-        *   meu\_pacote/ # Pasta do projeto
-            *   codigos\_da\_biblioteca/ # DiretÃ³rio onde deve ficar os cÃ³digos de sua biblioteca
-            *   LICENCE # Um arquivo com a licenÃ§a da sua lib
-            *   [README.MD](http://README.MD) # Uma descriÃ§Ã£o do projeto
-            *   [setup.py](http://setup.py) # CÃ³digo Python responsÃ¡vel pelo empacotamento
-        
-          
-        
-        Adicione uma licenÃ§a
-        
-        ```plain
-        The MIT License (MIT)
-        
-        Copyright (c) [year] [fullname]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy of
-        this software and associated documentation files (the "Software"), to deal in
-        the Software without restriction, including without limitation the rights to
-        use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-        the Software, and to permit persons to whom the Software is furnished to do so,
-        subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-        FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-        COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-        IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-        CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        ```
-        
-          
-        
-        Adicione um readme
-        
-        ```markdown
-        # Sua descriÃ§Ã£o aqui
-        ```
-        
-          
-        
-        Instale a lib setuptools
-        
-        ```plain
-        pip install setuptools
-        ```
-        
-          
-        
-        Crie o [setup.py](http://setup.py)
-        
-        ```plain
-        from setuptools import setup
-        
-        with open("README.md", "r") as arq:
-            readme = arq.read()
-        
-        setup(name='wrapper-panda-video',
-            version='0.0.1',
-            license='MIT License',
-            author='Caio Sampaio',
-            long_description=readme,
-            long_description_content_type="text/markdown",
-            author_email='caio@pythonando.com.br',
-            keywords='panda video',
-            description=u'Wrapper nÃ£o oficial do Panda Video',
-            packages=['panda_video'],
-            install_requires=['requests'],)
-        ```
-        
-          
-        
-        Execute o comando
-        
-        ```plain
-        python setup.py sdist
-        ```
-        
-          
-        
-        Instale o twine para fazer o upload para o pypi
-        
-        ```plain
-        pip install twine
-        ```
-        
-          
-        
-        Crie uma conta no pypi
-        
-          
-        
-        Execute o comando para criar um repositÃ³rio de teste
-        
-        ```plain
-        twine upload --repository-url https://test.pypi.org/legacy/ dist/*
-        ```
-        
-          
-        
-        Ou para criar um repositÃ³rio oficial:
-        
-        ```plain
-        python setup.py sdist
-        twine upload dist/*
-        user: __token__
-        pass: pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q
-        
-        
-        twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJDcwNDk1ZGM5LTA3MmQtNDc0Mi05YzhjLTNiZjgzMWRjMzJlMwACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiCi1Q7z6n4xADvsM8AJZDA-Q85MgkElshRg6bu4I_Vv6Q dist/*
-        ```
-        pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
 Keywords: plataforma automaxia api
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Material de apoio
+
+O primeiro passo Ã© ter o cÃ³digo de sua biblioteca separado em uma pasta
+
+  
+
+*   meu\_pacote/ # Pasta do projeto
+    *   codigos\_da\_biblioteca/ # DiretÃ³rio onde deve ficar os cÃ³digos de sua biblioteca
+    *   LICENCE # Um arquivo com a licenÃ§a da sua lib
+    *   [README.MD](http://README.MD) # Uma descriÃ§Ã£o do projeto
+    *   [setup.py](http://setup.py) # CÃ³digo Python responsÃ¡vel pelo empacotamento
+
+  
+
+Adicione uma licenÃ§a
+
+```plain
+The MIT License (MIT)
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+```
+
+  
+
+Adicione um readme
+
+```markdown
+# Sua descriÃ§Ã£o aqui
+```
+
+  
+
+Instale a lib setuptools
+
+```plain
+pip install setuptools
+```
+
+  
+
+Crie o [setup.py](http://setup.py)
+
+```plain
+from setuptools import setup
+
+with open("README.md", "r") as arq:
+    readme = arq.read()
+
+setup(name='wrapper-panda-video',
+    version='0.0.1',
+    license='MIT License',
+    author='Caio Sampaio',
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    author_email='caio@pythonando.com.br',
+    keywords='panda video',
+    description=u'Wrapper nÃ£o oficial do Panda Video',
+    packages=['panda_video'],
+    install_requires=['requests'],)
+```
+
+  
+
+Execute o comando
+
+```plain
+python setup.py sdist
+```
+
+  
+
+Instale o twine para fazer o upload para o pypi
+
+```plain
+pip install twine
+```
+
+  
+
+Crie uma conta no pypi
+
+  
+
+Execute o comando para criar um repositÃ³rio de teste
+
+```plain
+twine upload --repository-url https://test.pypi.org/legacy/ dist/*
+```
+
+  
+
+Ou para criar um repositÃ³rio oficial:
+
+```plain
+python setup.py sdist
+twine upload dist/*
+user: __token__
+pass: pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8
+
+
+twine upload -u __token__ -p pypi-AgEIcHlwaS5vcmcCJGU2OGEwM2NjLTQ4MDItNDMzMS05MmJjLTAyZTFjMTUwMGM2NQACIFsxLFsicGxhdGFmb3JtYS1hdXRvbWF4aWEtYXBpIl1dAAIsWzIsWyI3ODRkZmYyMC0xNDZhLTQ2NTUtOTc5NS1lY2VjMWQ0NzdlMzciXV0AAAYgwB_NoILnFF6BjXl7NUhe_y8Z5ib5_sCD2KXcVAvbEM8 dist/*
+```
+pypi-AgEIcHlwaS5vcmcCJDdkMTI4NjY5LWM5YmEtNDJiOC04OGNkLTFkMmRmOWEzNzE3NAACKlszLCI0OWI3YTc0OS03NDViLTQ2ZTAtYjkzZS05OTAxZGZhMGI2ZTIiXQAABiAAEL1XGUJwrn_9_-rTAtFiTogKFdOfDMpqb649_YCerw
+
```

### Comparing `plataforma-automaxia-api-0.0.6/setup.py` & `plataforma-automaxia-api-0.0.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='plataforma-automaxia-api',
-    version='0.0.6',
+    version='0.0.7',
     license='MIT License',
     author='Wesley Romualdo da Silva',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='wesleyromualdo@gmail.com',
     keywords='plataforma automaxia api',
     description=u'Wrapper oficial da Plataforma Automaxia para Python',
```

