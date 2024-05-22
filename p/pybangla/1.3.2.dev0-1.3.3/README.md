# Comparing `tmp/pybangla-1.3.2.dev0.tar.gz` & `tmp/pybangla-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.3.2.dev0.tar", last modified: Mon May 20 12:48:03 2024, max compression
+gzip compressed data, was "pybangla-1.3.3.tar", last modified: Wed May 22 12:29:48 2024, max compression
```

## Comparing `pybangla-1.3.2.dev0.tar` & `pybangla-1.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.511443 pybangla-1.3.2.dev0/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 12:48:03.000000 pybangla-1.3.2.dev0/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 12:48:03.515443 pybangla-1.3.2.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-20 12:47:59.000000 pybangla-1.3.2.dev0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:44.000000 pybangla-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-22 12:29:48.586884 pybangla-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19713 2024-05-22 12:29:44.000000 pybangla-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.582884 pybangla-1.3.3/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28329 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-22 12:29:44.000000 pybangla-1.3.3/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 12:29:48.000000 pybangla-1.3.3/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:29:48.586884 pybangla-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-22 12:29:44.000000 pybangla-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:29:48.586884 pybangla-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-22 12:29:44.000000 pybangla-1.3.3/tests/test.py
```

### Comparing `pybangla-1.3.2.dev0/PKG-INFO` & `pybangla-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.3.2.dev0
+Version: 1.3.3
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.3.2.dev0/README.md` & `pybangla-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/matching.py` & `pybangla-1.3.3/pybangla/matching.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/module/config.py` & `pybangla-1.3.3/pybangla/module/config.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/module/date_extractor.py` & `pybangla-1.3.3/pybangla/module/date_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,25 +16,25 @@
         en_month_name = ['jan','feb', 'mar', 'apr', 'may', 'june', 'july', 'aug', 'sept', 'oct', 'nov', 'dec']
         bn_month_name = ["জানুয়ারি", "ফেব্রুয়ারি", "মার্চ", "এপ্রিল", "মে", "জুন", "জুলাই", "অগাস্ট", "আগস্ট", "সেপ্টেম্বর", "অক্টোবর", "নভেম্বর", "ডিসেম্বর"]
 
         en_dd_mm_yy= "\\d{1,4}(( )+)?[-\\/,.;: ](( )+)?\\d{1,4}(( )+)?[-\\/,.;: ](( )+)?\\d{1,4}\\b"
         en_number_month_year = "\\d{1,2}[-\\/,.;: ](( )+)?("+ '|'.join(en_month_name) +")[a-z]{0,6}((( )+)?[-\\/,.;: ](( )+)?\\d{1,4})?\\b"
         en_month_number_year = "(" + '|'.join(en_month_name) +")[a-z]{0,6}(( )+)?[-\\/,.;: ](( )+)?\\d{1,2}([-\\/,.;: ](( )+)?\\d{1,4})?\\b"
         en_month_year = "("+ '|'.join(en_month_name) +")[a-z]{0,6}(( )+)?[-\\/,.;: ](( )+)?\\d{1,4}\\b"
-        en_plain_date ='\\d{8}\\b'
+        # en_plain_date ='\\d{8}\\b'
 
         bn_dd_mm_yy= "[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}"
         bn_number_month_year = "[০-৯]{1,2}[-\\/,.;: ](( )+)?("+ '|'.join(bn_month_name) +")((( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4})?"
         bn_month_number_year = "("+ '|'.join(bn_month_name) +")(( )+)?[-\\/,.;: ][০-৯]{1,2}(?![০-৯])((( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4})?"
         bn_month_year = "("+ '|'.join(bn_month_name) +")(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}"
         bn_year_date_num_month_name = "[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?(সালে|সালের)(( )+)?[-\\/,.;: ]?[০-৯]{1,2}(( )+)?[-\\/,.;: ]?(( )+)?("+ '|'.join(bn_month_name) +")?"
-        bn_plain_date = "[০-৯]{8}"
+        # bn_plain_date = "[০-৯]{8}"
 
-        en_regex = '|'.join([en_dd_mm_yy, en_number_month_year, en_month_number_year, en_month_year, en_plain_date])
-        bn_regex = '|'.join([bn_dd_mm_yy, bn_number_month_year, bn_month_number_year, bn_month_year, bn_year_date_num_month_name, bn_plain_date])
+        en_regex = '|'.join([en_dd_mm_yy, en_number_month_year, en_month_number_year, en_month_year]) # , en_plain_date])
+        bn_regex = '|'.join([bn_dd_mm_yy, bn_number_month_year, bn_month_number_year, bn_month_year, bn_year_date_num_month_name]) #, bn_plain_date])
         combined_regex = en_regex + '|' + bn_regex
         return combined_regex
     
     def __init__(self) -> None:
         self.date_regex = self.get_regex_patterns()
         
     def get_dates(self, sentence):
@@ -84,16 +84,16 @@
     "06-04-2023 df", 
     "04/01/2023 er",  
     "07 April, 2023 er", 
     "Apr 1, 2023 er",  
     "2023/04/01 er", 
     "01-Apr-2023 erv", 
     "01-Apr/2023 sere",  
-    "20230401 ",  
-    "20042024 ",
+    # "20230401 ",  
+    # "20042024 ",
 ]
     Bangla_sentences = [
     "১৯৯৬ সালের ৬তারিখে নির্ধারিত করা হয়েছে.",
     "১৯৯৬ সালের৬ সেপ্টেম্বর ভ্রমণ পরিকল্পনা করছি.",
     "আমি জুলাই ২০২৩ তে একটি সমুদ্র ভ্রমণ পরিকল্পনা করছি.",
     "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে.",
     "আমরা খ্রীষ্টমাসের জন্য ডিসেম্বর ২৫ ২০২৩ তারিখে পরিবারের সংগঠন করব.",
```

### Comparing `pybangla-1.3.2.dev0/pybangla/module/main.py` & `pybangla-1.3.3/pybangla/module/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,16 +107,21 @@
         Arg:
             data_{str or list} :  date may string or list of list like ["dd", "mm", "yyyy"]
             language{str}      : specific language format, support bangla and english
 
         return : 
                 Dictonary :  {"date":day, "month": month[0], "year": year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}       
         """
-        formated_date = dp.date_processing(date_, language=language)
-        return formated_date
+        date = dt.get_dates(date_)
+        # print(date)
+        if len(date):
+            formated_date = dp.date_processing(date_, language=language)
+            return formated_date
+        else:
+            print("No date found")
 
     def number_convert(self, number, language="bn"):
         """
         Convert the number digits English -> Bangla  or Bangla -> English
 
         Arg:
             number{str}  :  number string
@@ -155,15 +160,18 @@
         return text
     
     def date_extraction(self, text):
 
         dates = dt.get_dates(text)
         formated_date = [self.date_format(i)for i in dates]
         # print(f"Input: {sentence}: Output: {dates}")
-        return formated_date
+        if len(formated_date):
+            return formated_date
+        else:
+            print("No date found")
 
     
 if __name__ == "__main__":
 
 
     # Testing Date format
     date_list = [
```

### Comparing `pybangla-1.3.2.dev0/pybangla/module/number_parser.py` & `pybangla-1.3.3/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/module/parser.py` & `pybangla-1.3.3/pybangla/module/parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/module/word_to_number.py` & `pybangla-1.3.3/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla/test.py` & `pybangla-1.3.3/pybangla/test.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.3.2.dev0/pybangla.egg-info/PKG-INFO` & `pybangla-1.3.3/pybangla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.3.2.dev0
+Version: 1.3.3
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybangla-1.3.2.dev0/setup.py` & `pybangla-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.3.2-dev',
+    version='1.3.3',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
```

### Comparing `pybangla-1.3.2.dev0/tests/test.py` & `pybangla-1.3.3/tests/test.py`

 * *Files identical despite different names*

