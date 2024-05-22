# Comparing `tmp/setup_django_apex-0.1.3-py3-none-any.whl.zip` & `tmp/setup_django_apex-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5463 bytes, number of entries: 11
+Zip file size: 5462 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-22 04:26 setup_django_apex/__init__.py
 -rw-rw-rw-  2.0 fat     2871 b- defN 24-May-22 06:10 setup_django_apex/installer.py
--rw-rw-rw-  2.0 fat      281 b- defN 24-May-22 06:11 setup_django_apex/setup.py
+-rw-rw-rw-  2.0 fat      281 b- defN 24-May-22 06:12 setup_django_apex/setup.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-May-22 03:09 tests/__init__.py
 -rw-rw-rw-  2.0 fat     2111 b- defN 24-May-22 04:43 tests/mytest.py
 -rw-rw-rw-  2.0 fat     1195 b- defN 24-May-22 04:34 tests/test_installer.py
--rw-rw-rw-  2.0 fat     1174 b- defN 24-May-22 06:11 setup_django_apex-0.1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      860 b- defN 24-May-22 06:11 setup_django_apex-0.1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 06:11 setup_django_apex-0.1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 24-May-22 06:11 setup_django_apex-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      910 b- defN 24-May-22 06:11 setup_django_apex-0.1.3.dist-info/RECORD
-11 files, 9518 bytes uncompressed, 3907 bytes compressed:  59.0%
+-rw-rw-rw-  2.0 fat     1174 b- defN 24-May-22 06:13 setup_django_apex-0.1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      860 b- defN 24-May-22 06:13 setup_django_apex-0.1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 06:13 setup_django_apex-0.1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 24-May-22 06:13 setup_django_apex-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      910 b- defN 24-May-22 06:13 setup_django_apex-0.1.4.dist-info/RECORD
+11 files, 9518 bytes uncompressed, 3906 bytes compressed:  59.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: tests/mytest.py
 Comment: 
 
 Filename: tests/test_installer.py
 Comment: 
 
-Filename: setup_django_apex-0.1.3.dist-info/LICENSE
+Filename: setup_django_apex-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: setup_django_apex-0.1.3.dist-info/METADATA
+Filename: setup_django_apex-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: setup_django_apex-0.1.3.dist-info/WHEEL
+Filename: setup_django_apex-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: setup_django_apex-0.1.3.dist-info/top_level.txt
+Filename: setup_django_apex-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: setup_django_apex-0.1.3.dist-info/RECORD
+Filename: setup_django_apex-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## setup_django_apex/setup.py

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='setup_django_apex',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'setup-django-apex = setup_django_apex.installer:main',
         ],
     },
 )
```

## Comparing `setup_django_apex-0.1.3.dist-info/LICENSE` & `setup_django_apex-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `setup_django_apex-0.1.3.dist-info/METADATA` & `setup_django_apex-0.1.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.3
+Version: 0.1.4
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `setup_django_apex-0.1.3.dist-info/RECORD` & `setup_django_apex-0.1.4.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 setup_django_apex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 setup_django_apex/installer.py,sha256=WeUeEvN4kt-L5i8sH_P5kHREAcDk8lBE8Mje1_Kkg7U,2871
-setup_django_apex/setup.py,sha256=gfyCDlK7IQ0GjppQQrQ-cyRIH5Vy58_faK4_RCsZY6I,281
+setup_django_apex/setup.py,sha256=63IQHm8CGv4tTIrMRc5iqyJi_kYfaxcOs6CqtZ96hPw,281
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/mytest.py,sha256=G9eEUeTiw2eyG15pL5O8mA6YJ_mFNpIArHcUs9bb0no,2111
 tests/test_installer.py,sha256=M4Guu1acRd-HklKu_7ugs3Wndx3hPKS7HTFAVBQV4LI,1195
-setup_django_apex-0.1.3.dist-info/LICENSE,sha256=KQHQjbe8T5Ig45yoIoOwKYbJVvfFukwB1ktjq_QWtV8,1174
-setup_django_apex-0.1.3.dist-info/METADATA,sha256=nZzVsv2GJL2M_0Us3M12tO-SjpugJ9kzwH-kQYm9Z0I,860
-setup_django_apex-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-setup_django_apex-0.1.3.dist-info/top_level.txt,sha256=MvFrseq8vTYaiJgO2G-uCOvXGelmaFMavBF-EpgPLG8,24
-setup_django_apex-0.1.3.dist-info/RECORD,,
+setup_django_apex-0.1.4.dist-info/LICENSE,sha256=KQHQjbe8T5Ig45yoIoOwKYbJVvfFukwB1ktjq_QWtV8,1174
+setup_django_apex-0.1.4.dist-info/METADATA,sha256=mgI0Ai9Ktu1PlvJZG9AJZgLCTV0jWVUsYM6UEAV9uos,860
+setup_django_apex-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+setup_django_apex-0.1.4.dist-info/top_level.txt,sha256=MvFrseq8vTYaiJgO2G-uCOvXGelmaFMavBF-EpgPLG8,24
+setup_django_apex-0.1.4.dist-info/RECORD,,
```

