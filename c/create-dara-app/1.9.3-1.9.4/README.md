# Comparing `tmp/create_dara_app-1.9.3-py3-none-any.whl.zip` & `tmp/create_dara_app-1.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 268591 bytes, number of entries: 22
+Zip file size: 268592 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      658 b- defN 80-Jan-01 00:00 create_dara_app/__init__.py
 -rw-r--r--  2.0 unx     3735 b- defN 80-Jan-01 00:00 create_dara_app/cli.py
 -rw-r--r--  2.0 unx     3182 b- defN 80-Jan-01 00:00 create_dara_app/default_command_group.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 create_dara_app/templates/__init__.py
 -rw-r--r--  2.0 unx      318 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/cookiecutter.json
 -rw-r--r--  2.0 unx     1285 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/hooks/post_gen_project.py
 -rw-r--r--  2.0 unx      294 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/hooks/pre_gen_project.py
@@ -12,13 +12,13 @@
 -rw-r--r--  2.0 unx     1277 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml
 -rw-r--r--  2.0 unx   318043 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/static/dara_light.svg
 -rw-r--r--  2.0 unx      733 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py
 -rw-r--r--  2.0 unx     4929 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/components_page.py
 -rw-r--r--  2.0 unx     1590 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/intro_page.py
 -rw-r--r--  2.0 unx    65462 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py
 -rw-r--r--  2.0 unx      737 b- defN 80-Jan-01 00:00 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py
--rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 create_dara_app-1.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1950 b- defN 80-Jan-01 00:00 create_dara_app-1.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 create_dara_app-1.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 create_dara_app-1.9.3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2686 b- defN 16-Jan-01 00:00 create_dara_app-1.9.3.dist-info/RECORD
-22 files, 419611 bytes uncompressed, 263903 bytes compressed:  37.1%
+-rw-r--r--  2.0 unx    10944 b- defN 80-Jan-01 00:00 create_dara_app-1.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1950 b- defN 80-Jan-01 00:00 create_dara_app-1.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 create_dara_app-1.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 80-Jan-01 00:00 create_dara_app-1.9.4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2686 b- defN 16-Jan-01 00:00 create_dara_app-1.9.4.dist-info/RECORD
+22 files, 419611 bytes uncompressed, 263904 bytes compressed:  37.1%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py
 Comment: 
 
 Filename: create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py
 Comment: 
 
-Filename: create_dara_app-1.9.3.dist-info/LICENSE
+Filename: create_dara_app-1.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: create_dara_app-1.9.3.dist-info/METADATA
+Filename: create_dara_app-1.9.4.dist-info/METADATA
 Comment: 
 
-Filename: create_dara_app-1.9.3.dist-info/WHEEL
+Filename: create_dara_app-1.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: create_dara_app-1.9.3.dist-info/entry_points.txt
+Filename: create_dara_app-1.9.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: create_dara_app-1.9.3.dist-info/RECORD
+Filename: create_dara_app-1.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `create_dara_app-1.9.3.dist-info/LICENSE` & `create_dara_app-1.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `create_dara_app-1.9.3.dist-info/METADATA` & `create_dara_app-1.9.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: create-dara-app
-Version: 1.9.3
+Version: 1.9.4
 Summary: CLI to quickly bootstrap a Dara app
 Home-page: https://dara.causalens.com/
 License: Apache-2.0
 Author: Krzysztof Bielikowicz
 Author-email: krzysztof@causalens.com
 Requires-Python: >=3.8,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -16,15 +16,15 @@
 Requires-Dist: click (==8.1.3)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/causalens/dara
 Description-Content-Type: text/markdown
 
 # Create Dara App
 
-<img src="https://github.com/causalens/dara/blob/VERSION-1.9.3/img/dara_light.svg?raw=true">
+<img src="https://github.com/causalens/dara/blob/VERSION-1.9.4/img/dara_light.svg?raw=true">
 
 ![Master tests](https://github.com/causalens/dara/actions/workflows/tests.yml/badge.svg?branch=master)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![PyPI](https://img.shields.io/pypi/v/create-dara-app.svg?color=dark-green)](https://pypi.org/project/create-dara-app/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/create-dara-app.svg?color=dark-green)](https://pypi.org/project/create-dara-app/)
 
 ### Build decision apps in Python
```

## Comparing `create_dara_app-1.9.3.dist-info/RECORD` & `create_dara_app-1.9.4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/pyproject.toml,sha256=aiMMd6Ww6jvX-p3hdl8cvhv7lVDNH0KPPl0e4xZDBJ4,1277
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/static/dara_light.svg,sha256=rX8oRQ3Uhcm7yQPO6NXsgRydcz4-mXkkChpZqEY8dOU,318043
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/main.py,sha256=yntXq115p6VWoWF7SFi6r5_sE_1ZUL_oxWzmZf3Fskk,733
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/components_page.py,sha256=Ij1Brq2tRkorpmmNY-63KRUdfZwl51YY9eb7m3QdeEo,4929
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/pages/intro_page.py,sha256=_G4z_9N66t6eMhIenzIFbIM-p_EzJM8LPGiJ_emRI8k,1590
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/components.py,sha256=xAjhKxPC1cgMda5tpLyCwZEEJTVOALR4C7V3REUpxbo,65462
 create_dara_app/templates/default/{{ cookiecutter.__project_slug }}/{{ cookiecutter.__package_name }}/utils/template.py,sha256=R8EgjNKD5bou9HkT7CEEISAcO5H7R-sSWFtifFJyK5M,737
-create_dara_app-1.9.3.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
-create_dara_app-1.9.3.dist-info/METADATA,sha256=9zFXK_IwUORTXMzzo-S5o1Olec7ZlVHLoBZ5-Lke9uc,1950
-create_dara_app-1.9.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-create_dara_app-1.9.3.dist-info/entry_points.txt,sha256=RZETW6Q9lb0vM1gptGnobZGlD2qvU-0ZgztNoboRRTk,59
-create_dara_app-1.9.3.dist-info/RECORD,,
+create_dara_app-1.9.4.dist-info/LICENSE,sha256=r9u1w2RvpLMV6YjuXHIKXRBKzia3fx_roPwboGcLqCc,10944
+create_dara_app-1.9.4.dist-info/METADATA,sha256=dxHScEWSmNUN09Xc9k8zPfxcA2UAQIeo7SNbwRGedrw,1950
+create_dara_app-1.9.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+create_dara_app-1.9.4.dist-info/entry_points.txt,sha256=RZETW6Q9lb0vM1gptGnobZGlD2qvU-0ZgztNoboRRTk,59
+create_dara_app-1.9.4.dist-info/RECORD,,
```

