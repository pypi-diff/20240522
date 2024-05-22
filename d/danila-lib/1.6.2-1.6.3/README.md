# Comparing `tmp/danila-lib-1.6.2.tar.gz` & `tmp/danila-lib-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.6.2.tar", last modified: Wed May 22 08:43:52 2024, max compression
+gzip compressed data, was "danila-lib-1.6.3.tar", last modified: Wed May 22 08:49:58 2024, max compression
```

## Comparing `danila-lib-1.6.2.tar` & `danila-lib-1.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.831972 danila-lib-1.6.2/
--rw-rw-rw-   0        0        0     9615 2024-05-22 08:43:52.831972 danila-lib-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.753866 danila-lib-1.6.2/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.6.2/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.6.2/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.6.2/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.6.2/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.6.2/danila/danila_v3.py
--rw-rw-rw-   0        0        0    15320 2024-05-22 08:43:39.000000 danila-lib-1.6.2/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.769488 danila-lib-1.6.2/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-22 08:43:52.000000 danila-lib-1.6.2/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-22 08:43:52.000000 danila-lib-1.6.2/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 08:43:52.000000 danila-lib-1.6.2/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-22 08:43:52.000000 danila-lib-1.6.2/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 08:43:52.000000 danila-lib-1.6.2/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.769488 danila-lib-1.6.2/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.6.2/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.831972 danila-lib-1.6.2/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.6.2/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.6.2/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.6.2/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.6.2/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-05-22 08:43:39.000000 danila-lib-1.6.2/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.6.2/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.6.2/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 08:43:39.000000 danila-lib-1.6.2/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.6.2/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.6.2/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:43:52.831972 danila-lib-1.6.2/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.6.2/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.6.2/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.6.2/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.6.2/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.6.2/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.6.2/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.6.2/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.6.2/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.6.2/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.6.2/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.6.2/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-22 08:43:52.831972 danila-lib-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-22 08:43:48.000000 danila-lib-1.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.077414 danila-lib-1.6.3/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 08:49:58.077414 danila-lib-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.046173 danila-lib-1.6.3/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.6.3/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.6.3/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.6.3/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.6.3/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.6.3/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    15320 2024-05-22 08:43:39.000000 danila-lib-1.6.3/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.061795 danila-lib-1.6.3/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 08:49:57.000000 danila-lib-1.6.3/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-22 08:49:58.000000 danila-lib-1.6.3/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:49:57.000000 danila-lib-1.6.3/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-22 08:49:57.000000 danila-lib-1.6.3/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 08:49:57.000000 danila-lib-1.6.3/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.061795 danila-lib-1.6.3/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.6.3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.077414 danila-lib-1.6.3/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.6.3/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.6.3/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.6.3/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.6.3/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3143 2024-05-22 08:49:48.000000 danila-lib-1.6.3/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.6.3/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.6.3/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 08:43:39.000000 danila-lib-1.6.3/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.6.3/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.6.3/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:49:58.077414 danila-lib-1.6.3/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.6.3/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.6.3/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.6.3/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.6.3/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.6.3/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.6.3/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.6.3/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.6.3/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.6.3/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.6.3/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.6.3/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:49:58.077414 danila-lib-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-22 08:49:56.000000 danila-lib-1.6.3/setup.py
```

### Comparing `danila-lib-1.6.2/PKG-INFO` & `danila-lib-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.6.2
+Version: 1.6.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.6.2/README.md` & `danila-lib-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila/danila.py` & `danila-lib-1.6.3/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila/danila_v1.py` & `danila-lib-1.6.3/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila/danila_v2.py` & `danila-lib-1.6.3/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila/danila_v3.py` & `danila-lib-1.6.3/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila/danila_v4.py` & `danila-lib-1.6.3/danila/danila_v4.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.6.3/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.6.2
+Version: 1.6.3
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.6.2/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.6.3/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/danila_lib.egg-info/requires.txt` & `danila-lib-1.6.3/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/Letters_recognize.py` & `danila-lib-1.6.3/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/Rama_classify_class.py` & `danila-lib-1.6.3/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/Rama_detect_class.py` & `danila-lib-1.6.3/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.6.3/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/Text_detect_class.py` & `danila-lib-1.6.3/data/neuro/Text_detect_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,22 @@
         public_key = model_path  # Сюда вписываете вашу ссылку
         # Получаем загрузочную ссылку
         final_url = base_url + urlencode(dict(public_key=public_key))
         response = requests.get(final_url)
         download_url = response.json()['href']
         # Загружаем файл и сохраняем его
         download_response = requests.get(download_url)
-        zip_path = model_name + '_weights.zip'
+        zip_path = model_name + '.zip'
         # print(download_response.content)
         with open(zip_path, 'wb') as f:
             f.write(download_response.content)
 
         with zipfile.ZipFile(zip_path, 'r') as zip_ref:
             zip_ref.extractall()
-        weights_file_path = model_name + '_weights.pt'
+        weights_file_path = model_name + '.pt'
         self.model = torch.hub.load(yolo_path, 'custom', weights_file_path, source='local')
     # find text areas on img from img_path with yolov5, returns yolojson
     def work_img(self, img_path):
         """find text areas on img from img_path with yolov5, returns yolojson"""
         results = self.model([img_path])
         json_res = results.pandas().xyxy[0].to_json(orient="records")
         res2 = json.loads(json_res)
```

### Comparing `danila-lib-1.6.2/data/neuro/letters_in_image.py` & `danila-lib-1.6.3/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/models.py` & `danila-lib-1.6.3/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/objs_in_image.py` & `danila-lib-1.6.3/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/neuro/text_recognize_yolo.py` & `danila-lib-1.6.3/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/result/Image_text_areas.py` & `danila-lib-1.6.3/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/result/Rect.py` & `danila-lib-1.6.3/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/result/Text_area.py` & `danila-lib-1.6.3/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/data/result/Yolo_label_rect.py` & `danila-lib-1.6.3/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.6.2/setup.py` & `danila-lib-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.6.2',
+  version='1.6.3',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

