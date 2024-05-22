# Comparing `tmp/ipiranga-inovai-project-lib-0.6.tar.gz` & `tmp/ipiranga-inovai-project-lib-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipiranga-inovai-project-lib-0.6.tar", last modified: Fri May 17 15:33:00 2024, max compression
+gzip compressed data, was "ipiranga-inovai-project-lib-0.7.tar", last modified: Wed May 22 17:59:32 2024, max compression
```

## Comparing `ipiranga-inovai-project-lib-0.6.tar` & `ipiranga-inovai-project-lib-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:33:00.509412 ipiranga-inovai-project-lib-0.6/
--rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.6/LICENSE
--rw-rw-rw-   0        0        0      516 2024-05-17 15:33:00.507519 ipiranga-inovai-project-lib-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:33:00.490363 ipiranga-inovai-project-lib-0.6/inovai/
--rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.6/inovai/__init__.py
--rw-rw-rw-   0        0        0    12749 2024-05-17 15:32:14.000000 ipiranga-inovai-project-lib-0.6/inovai/entities.py
--rw-rw-rw-   0        0        0      368 2024-05-16 23:31:54.000000 ipiranga-inovai-project-lib-0.6/inovai/enums.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:33:00.504530 ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/
--rw-rw-rw-   0        0        0      516 2024-05-17 15:33:00.000000 ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-05-17 15:33:00.000000 ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:33:00.000000 ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 15:33:00.000000 ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:33:00.510418 ipiranga-inovai-project-lib-0.6/setup.cfg
--rw-rw-rw-   0        0        0      689 2024-05-17 15:32:55.000000 ipiranga-inovai-project-lib-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.204436 ipiranga-inovai-project-lib-0.7/
+-rw-rw-rw-   0        0        0      198 2024-04-05 19:57:15.000000 ipiranga-inovai-project-lib-0.7/LICENSE
+-rw-rw-rw-   0        0        0      516 2024-05-22 17:59:32.202439 ipiranga-inovai-project-lib-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-05 19:18:28.000000 ipiranga-inovai-project-lib-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.186511 ipiranga-inovai-project-lib-0.7/inovai/
+-rw-rw-rw-   0        0        0        0 2024-04-05 20:33:51.000000 ipiranga-inovai-project-lib-0.7/inovai/__init__.py
+-rw-rw-rw-   0        0        0    12749 2024-05-22 17:57:29.000000 ipiranga-inovai-project-lib-0.7/inovai/entities.py
+-rw-rw-rw-   0        0        0      847 2024-05-22 17:58:20.000000 ipiranga-inovai-project-lib-0.7/inovai/enums.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:59:32.200231 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/
+-rw-rw-rw-   0        0        0      516 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 17:59:32.000000 ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:59:32.205599 ipiranga-inovai-project-lib-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      689 2024-05-22 17:59:20.000000 ipiranga-inovai-project-lib-0.7/setup.py
```

### Comparing `ipiranga-inovai-project-lib-0.6/PKG-INFO` & `ipiranga-inovai-project-lib-0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.6
+Version: 0.7
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.6/inovai/entities.py` & `ipiranga-inovai-project-lib-0.7/inovai/entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     __tablename__ = 'documento_integracao'
     __table_args__ = {'schema': 'fiscal'}
 
     document_id = Column('no_seq_doc_integr', Integer, primary_key=True, nullable=False)
     access_key = Column('cd_chave_doc_integr', String(44))
     json_content = Column('aq_json', JSON, nullable=False)
     document_movement_type = Column('cd_tipo_mov_doc_integr', String(1))
-    document_type = Column('cd_tipo_doc_integr', String(4))
+    document_type = Column('cd_tipo_doc_integr', String(8))
     document_series = Column('cd_serie_doc_integr', String(3), nullable=False)
     document_number = Column('no_doc_integr', Numeric(precision=11, scale=0), nullable=False)
     document_model = Column('cd_modl_doc_integr', String(3), nullable=False)
     branch_code = Column('cd_filial', Numeric(precision=6, scale=0), nullable=False)
     recipient_cnpj = Column('cd_cnpj_dest', String(14), nullable=False)
     issuer_cnpj = Column('cd_cnpj_emit', String(14), nullable=False)
     issuance_date = Column('dt_emis_doc_integr', Date, nullable=False)
@@ -153,15 +153,15 @@
     __tablename__ = 'param_processamento_kit'
     __table_args__ = {'schema': 'fiscal'}
 
     param_processing_kit_id = Column('no_seq_proc', Numeric(precision=8, scale=0), primary_key=True, nullable=False)
     kit_id = Column('cd_kit', Integer, ForeignKey('fiscal.kit_obi.no_seq_kit'), nullable=False)
     process_code = Column('cd_proc_obi', String(30))
     status = Column('id_status_param', Boolean, nullable=False)
-    document_type = Column('cd_tipo_doc_integr', String(4))
+    document_type = Column('cd_tipo_doc_integr', String(8))
     created_at = Column('dt_incl', DateTime, nullable=False, server_default='NOW()')
 
     def __init__(self, param_processing_kit_id, kit_id, process_code, status, document_type):
         super().__init__()
         self.param_processing_kit_id = param_processing_kit_id
         self.kit_id = kit_id
         self.process_code = process_code
```

### Comparing `ipiranga-inovai-project-lib-0.6/ipiranga_inovai_project_lib.egg-info/PKG-INFO` & `ipiranga-inovai-project-lib-0.7/ipiranga_inovai_project_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipiranga-inovai-project-lib
-Version: 0.6
+Version: 0.7
 Summary: Projeto criado para importação genérica de entidades
 Home-page: https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib
 Author: Clayton Sandes Monteiro
 Author-email: clayton.monteiro.ext@ipiranga.ipiranga
 License: MIT
 Keywords: inovai
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ipiranga-inovai-project-lib-0.6/setup.py` & `ipiranga-inovai-project-lib-0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ipiranga-inovai-project-lib",
-    version="0.6",
+    version="0.7",
     packages=find_packages(),
     description="Projeto criado para importação genérica de entidades",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Clayton Sandes Monteiro",
     author_email="clayton.monteiro.ext@ipiranga.ipiranga",
     url="https://gitlab.ipirangacloud.com/clayton.monteiro.ext/ipiranga-inovai-project-lib",
```

