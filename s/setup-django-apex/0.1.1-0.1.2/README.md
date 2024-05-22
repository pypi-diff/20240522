# Comparing `tmp/setup_django_apex-0.1.1.tar.gz` & `tmp/setup_django_apex-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_django_apex-0.1.1.tar", last modified: Wed May 22 05:30:29 2024, max compression
+gzip compressed data, was "setup_django_apex-0.1.2.tar", last modified: Wed May 22 05:36:14 2024, max compression
```

## Comparing `setup_django_apex-0.1.1.tar` & `setup_django_apex-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.547876 setup_django_apex-0.1.1/
--rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      857 2024-05-22 05:30:29.542948 setup_django_apex-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 05:30:29.547876 setup_django_apex-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-22 05:30:15.000000 setup_django_apex-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.499935 setup_django_apex-0.1.1/setup_django_apex/
--rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.1/setup_django_apex/__init__.py
--rw-rw-rw-   0        0        0     1892 2024-05-22 05:12:38.000000 setup_django_apex-0.1.1/setup_django_apex/installer.py
--rw-rw-rw-   0        0        0      281 2024-05-22 05:30:18.000000 setup_django_apex-0.1.1/setup_django_apex/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.538388 setup_django_apex-0.1.1/setup_django_apex.egg-info/
--rw-rw-rw-   0        0        0      857 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.530849 setup_django_apex-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.1/tests/__init__.py
--rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.1/tests/mytest.py
--rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.1/tests/test_installer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:36:14.020673 setup_django_apex-0.1.2/
+-rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      857 2024-05-22 05:36:14.016593 setup_django_apex-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 05:36:14.021674 setup_django_apex-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-22 05:33:41.000000 setup_django_apex-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:36:13.976377 setup_django_apex-0.1.2/setup_django_apex/
+-rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.2/setup_django_apex/__init__.py
+-rw-rw-rw-   0        0        0     2047 2024-05-22 05:33:29.000000 setup_django_apex-0.1.2/setup_django_apex/installer.py
+-rw-rw-rw-   0        0        0      281 2024-05-22 05:33:44.000000 setup_django_apex-0.1.2/setup_django_apex/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:36:14.012997 setup_django_apex-0.1.2/setup_django_apex.egg-info/
+-rw-rw-rw-   0        0        0      857 2024-05-22 05:36:13.000000 setup_django_apex-0.1.2/setup_django_apex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-22 05:36:13.000000 setup_django_apex-0.1.2/setup_django_apex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 05:36:13.000000 setup_django_apex-0.1.2/setup_django_apex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-22 05:36:13.000000 setup_django_apex-0.1.2/setup_django_apex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-22 05:36:13.000000 setup_django_apex-0.1.2/setup_django_apex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 05:36:14.007641 setup_django_apex-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.2/tests/mytest.py
+-rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.2/tests/test_installer.py
```

### Comparing `setup_django_apex-0.1.1/LICENSE` & `setup_django_apex-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.1/PKG-INFO` & `setup_django_apex-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `setup_django_apex-0.1.1/setup.py` & `setup_django_apex-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.check_call(['python', '-m', 'setup_django_apex.installer'])
 
 setup(
     name='setup_django_apex',
-    version='0.1.1',
+    version='0.1.2',
     author='Anirudha Udgirkar',
     author_email='anirudhaudgirkar.work.email@example.com',
     description='A library to set up Django projects with multiple apps',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Anirudha1821/setup_django_apex',
     packages=find_packages(),
```

### Comparing `setup_django_apex-0.1.1/setup_django_apex/installer.py` & `setup_django_apex-0.1.2/setup_django_apex/installer.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,23 +33,26 @@
         app_entry = f"    '{app_name}',\n"
         if app_entry not in settings:
             settings.insert(installed_apps_index + 1, app_entry)
 
     with open(settings_path, 'w') as file:
         file.writelines(settings)
 
-def main():
-    project_name = input("Enter the name of your Django project: ")
+def main(project_name=None, num_apps=None, app_names=None):
+    if not project_name:
+        project_name = input("Enter the name of your Django project: ")
     create_django_project(project_name)
 
-    num_apps = int(input("How many apps do you want to create? "))
-    app_names = []
-    for _ in range(num_apps):
-        app_name = input("Enter the name of the app: ")
-        create_django_app(app_name)
-        app_names.append(app_name)
+    if num_apps is None:
+        num_apps = int(input("How many apps do you want to create? "))
+    if app_names is None:
+        app_names = []
+        for _ in range(num_apps):
+            app_name = input("Enter the name of the app: ")
+            create_django_app(app_name)
+            app_names.append(app_name)
 
     update_settings(app_names, project_name)
     print(f"Successfully created project {project_name} with apps: {', '.join(app_names)}")
 
 if __name__ == "__main__":
     main()
```

### Comparing `setup_django_apex-0.1.1/setup_django_apex.egg-info/PKG-INFO` & `setup_django_apex-0.1.2/setup_django_apex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.1
+Version: 0.1.2
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `setup_django_apex-0.1.1/tests/mytest.py` & `setup_django_apex-0.1.2/tests/mytest.py`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.1/tests/test_installer.py` & `setup_django_apex-0.1.2/tests/test_installer.py`

 * *Files identical despite different names*

