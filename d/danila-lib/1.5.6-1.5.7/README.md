# Comparing `tmp/danila-lib-1.5.6.tar.gz` & `tmp/danila-lib-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.5.6.tar", last modified: Tue May 21 17:56:31 2024, max compression
+gzip compressed data, was "danila-lib-1.5.7.tar", last modified: Wed May 22 05:28:37 2024, max compression
```

## Comparing `danila-lib-1.5.6.tar` & `danila-lib-1.5.7.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.245978 danila-lib-1.5.6/
--rw-rw-rw-   0        0        0     9615 2024-05-21 17:56:31.245978 danila-lib-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.121024 danila-lib-1.5.6/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.6/danila/__init__.py
--rw-rw-rw-   0        0        0     2004 2024-05-14 12:46:28.000000 danila-lib-1.5.6/danila/danila.py
--rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.6/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.6/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10719 2024-05-21 15:00:35.000000 danila-lib-1.5.6/danila/danila_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.152255 danila-lib-1.5.6/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-21 17:56:31.000000 danila-lib-1.5.6/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-05-21 17:56:31.000000 danila-lib-1.5.6/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 17:56:31.000000 danila-lib-1.5.6/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-21 17:56:31.000000 danila-lib-1.5.6/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 17:56:31.000000 danila-lib-1.5.6/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.152255 danila-lib-1.5.6/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.6/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.199116 danila-lib-1.5.6/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.6/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.6/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.6/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.6/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-04-22 19:35:07.000000 danila-lib-1.5.6/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.6/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.6/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-21 14:57:11.000000 danila-lib-1.5.6/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.6/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4390 2024-05-21 14:55:03.000000 danila-lib-1.5.6/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-21 17:56:31.245978 danila-lib-1.5.6/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.6/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.6/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.6/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.6/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.6/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.6/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.6/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.6/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.6/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.6/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.6/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-21 17:56:31.245978 danila-lib-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-21 17:56:27.000000 danila-lib-1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.696715 danila-lib-1.5.7/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 05:28:37.696715 danila-lib-1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.587370 danila-lib-1.5.7/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.7/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.5.7/danila/danila.py
+-rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.7/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.7/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10719 2024-05-21 15:00:35.000000 danila-lib-1.5.7/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    10721 2024-05-22 05:28:12.000000 danila-lib-1.5.7/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.602991 danila-lib-1.5.7/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 05:28:37.000000 danila-lib-1.5.7/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-22 05:28:37.000000 danila-lib-1.5.7/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 05:28:37.000000 danila-lib-1.5.7/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-22 05:28:37.000000 danila-lib-1.5.7/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 05:28:37.000000 danila-lib-1.5.7/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.602991 danila-lib-1.5.7/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.7/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.649854 danila-lib-1.5.7/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.7/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.7/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.7/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.7/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-05-22 05:28:12.000000 danila-lib-1.5.7/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.7/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.7/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-21 14:57:11.000000 danila-lib-1.5.7/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.7/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4390 2024-05-21 14:55:03.000000 danila-lib-1.5.7/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:28:37.696715 danila-lib-1.5.7/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.7/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.7/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.7/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.7/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.7/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.7/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.7/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.7/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.7/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.7/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.7/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 05:28:37.696715 danila-lib-1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-22 05:28:34.000000 danila-lib-1.5.7/setup.py
```

### Comparing `danila-lib-1.5.6/PKG-INFO` & `danila-lib-1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.6
+Version: 1.5.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.6/README.md` & `danila-lib-1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/danila/danila.py` & `danila-lib-1.5.7/danila/danila.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import os
 
 import cv2
 
 from danila.danila_v1 import Danila_v1
 from danila.danila_v2 import Danila_v2
 from danila.danila_v3 import Danila_v3
+from danila.danila_v4 import Danila_v4
 
 """main module for user"""
 
 
 class Danila:
     """main class for user"""
     def __init__(self, version, yolov5_dir):
         if (version == 1):
             self.danila = Danila_v1(yolov5_dir)
         elif (version == 2):
             self.danila = Danila_v2(yolov5_dir)
-        else:
+        elif (version == 3):
             self.danila = Danila_v3(yolov5_dir)
+        else:
+            self.danila = Danila_v4(yolov5_dir)
     # returns string - class of rama using CNN network
     # img - openCV frame
 
     def rama_classify(self, img, size = 256):
         """rama_classify(Img : openCv frame): String - returns class of rama using CNN network"""
         """rama_classify uses Rama_classify_class method - classify(Img)"""
         return self.danila.rama_classify(img, size)
```

### Comparing `danila-lib-1.5.6/danila/danila_v1.py` & `danila-lib-1.5.7/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/danila/danila_v2.py` & `danila-lib-1.5.7/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/danila/danila_v3.py` & `danila-lib-1.5.7/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.5.7/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.6
+Version: 1.5.7
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.6/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.5.7/danila_lib.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.cfg
 setup.py
 danila/__init__.py
 danila/danila.py
 danila/danila_v1.py
 danila/danila_v2.py
 danila/danila_v3.py
+danila/danila_v4.py
 danila_lib.egg-info/PKG-INFO
 danila_lib.egg-info/SOURCES.txt
 danila_lib.egg-info/dependency_links.txt
 danila_lib.egg-info/requires.txt
 danila_lib.egg-info/top_level.txt
 data/__init__.py
 data/neuro/Letters_recognize.py
```

### Comparing `danila-lib-1.5.6/danila_lib.egg-info/requires.txt` & `danila-lib-1.5.7/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/Letters_recognize.py` & `danila-lib-1.5.7/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/Rama_classify_class.py` & `danila-lib-1.5.7/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/Rama_detect_class.py` & `danila-lib-1.5.7/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.5.7/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/Text_detect_class.py` & `danila-lib-1.5.7/data/neuro/Text_detect_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return res2
     # find text areas on img from img_path with yolov5, returns dict with rects for each text class
     def text_detect(self, img_path):
         """find text areas on img from img_path with yolov5, returns dict with rects for each text class"""
         json_res = self.work_img(img_path)
         image_text_areas = Image_text_areas()
         for text_area_json in json_res:
-            if text_area_json['confidence']>0.49:
+            if text_area_json['confidence']>0.29:
                 text_area = Text_area(text_area_json)
                 image_text_areas.add_area(text_area)
         image_text_areas.correct_intersections()
         return image_text_areas
     # draw img_text_areas on img, returns opencv img
     def draw_text_areas_in_opencv(self, image_text_areas, img):
         """draw img_text_areas on img, returns opencv img"""
```

### Comparing `danila-lib-1.5.6/data/neuro/letters_in_image.py` & `danila-lib-1.5.7/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/models.py` & `danila-lib-1.5.7/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/objs_in_image.py` & `danila-lib-1.5.7/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/neuro/text_recognize_yolo.py` & `danila-lib-1.5.7/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/result/Image_text_areas.py` & `danila-lib-1.5.7/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/result/Rect.py` & `danila-lib-1.5.7/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/result/Text_area.py` & `danila-lib-1.5.7/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/data/result/Yolo_label_rect.py` & `danila-lib-1.5.7/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.6/setup.py` & `danila-lib-1.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.5.6',
+  version='1.5.7',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```
