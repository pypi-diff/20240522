# Comparing `tmp/danila-lib-1.5.8.tar.gz` & `tmp/danila-lib-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.5.8.tar", last modified: Wed May 22 06:35:04 2024, max compression
+gzip compressed data, was "danila-lib-1.5.9.tar", last modified: Wed May 22 07:22:11 2024, max compression
```

## Comparing `danila-lib-1.5.8.tar` & `danila-lib-1.5.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.503197 danila-lib-1.5.8/
--rw-rw-rw-   0        0        0     9615 2024-05-22 06:35:04.503197 danila-lib-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.456334 danila-lib-1.5.8/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.8/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.5.8/danila/danila.py
--rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.8/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.8/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10719 2024-05-22 06:33:28.000000 danila-lib-1.5.8/danila/danila_v3.py
--rw-rw-rw-   0        0        0    10721 2024-05-22 05:28:12.000000 danila-lib-1.5.8/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.487578 danila-lib-1.5.8/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-22 06:35:04.000000 danila-lib-1.5.8/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-22 06:35:04.000000 danila-lib-1.5.8/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 06:35:04.000000 danila-lib-1.5.8/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-22 06:35:04.000000 danila-lib-1.5.8/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 06:35:04.000000 danila-lib-1.5.8/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.487578 danila-lib-1.5.8/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.8/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.487578 danila-lib-1.5.8/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.8/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.8/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.8/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.8/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3159 2024-05-22 05:28:12.000000 danila-lib-1.5.8/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.8/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.8/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      830 2024-05-22 06:34:53.000000 danila-lib-1.5.8/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.8/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4390 2024-05-21 14:55:03.000000 danila-lib-1.5.8/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:35:04.503197 danila-lib-1.5.8/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.8/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.8/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.8/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.8/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.8/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.8/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.8/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.8/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.8/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.8/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.8/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-22 06:35:04.503197 danila-lib-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-22 06:33:28.000000 danila-lib-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.442791 danila-lib-1.5.9/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 07:22:11.442791 danila-lib-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.411549 danila-lib-1.5.9/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.5.9/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.5.9/danila/danila.py
+-rw-rw-rw-   0        0        0     9777 2024-05-20 08:47:35.000000 danila-lib-1.5.9/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10195 2024-05-14 12:46:28.000000 danila-lib-1.5.9/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10719 2024-05-22 06:33:28.000000 danila-lib-1.5.9/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    15031 2024-05-22 07:22:08.000000 danila-lib-1.5.9/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.427170 danila-lib-1.5.9/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 07:22:11.000000 danila-lib-1.5.9/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-22 07:22:11.000000 danila-lib-1.5.9/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:22:11.000000 danila-lib-1.5.9/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-22 07:22:11.000000 danila-lib-1.5.9/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 07:22:11.000000 danila-lib-1.5.9/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.427170 danila-lib-1.5.9/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.5.9/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.442791 danila-lib-1.5.9/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.5.9/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.5.9/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-04-22 11:59:10.000000 danila-lib-1.5.9/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.5.9/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3159 2024-05-22 07:22:08.000000 danila-lib-1.5.9/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.9/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.5.9/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      830 2024-05-22 06:34:53.000000 danila-lib-1.5.9/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.5.9/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.5.9/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:22:11.442791 danila-lib-1.5.9/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.5.9/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.5.9/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.5.9/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.5.9/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.5.9/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.5.9/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.5.9/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.5.9/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.5.9/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.5.9/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.5.9/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:22:11.442791 danila-lib-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-22 07:22:08.000000 danila-lib-1.5.9/setup.py
```

### Comparing `danila-lib-1.5.8/PKG-INFO` & `danila-lib-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.8
+Version: 1.5.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.8/README.md` & `danila-lib-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila/danila.py` & `danila-lib-1.5.9/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila/danila_v1.py` & `danila-lib-1.5.9/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila/danila_v2.py` & `danila-lib-1.5.9/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila/danila_v3.py` & `danila-lib-1.5.9/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila/danila_v4.py` & `danila-lib-1.5.9/danila/danila_v4.py`

 * *Files 23% similar despite different names*

```diff
@@ -174,26 +174,84 @@
             img_cut_path = 'cut_img.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_spring_ruzhimmash_text_detect_model.text_detect(img_cut_path)
 
             label_area = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
                                                                   4, 64,128, 2, 64,64)
             res_labels = {}
-            res_labels['number'] = label_area.labels[Class_text.number]
+            if len(label_area.labels[Class_text.number]) == 5:
+                res_labels['number'] = label_area.labels[Class_text.number]
+            else:
+                number_image_text_areas = image_text_areas.areas[Class_text.number]
+                image_text_areas_min = []
+                image_text_areas_max = []
+                for number_image_text_area in number_image_text_areas:
+                    w = number_image_text_area.xmax - number_image_text_area.xmin
+                    if (number_image_text_area.xmin - (w/2)) < 0:
+                        new_xmin = 0
+                    else:
+                        new_xmin = number_image_text_area.xmin - (w/2)
+                    rect_min = Rect(xmin=new_xmin, xmax=number_image_text_area.xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                    image_text_areas_min.append(rect_min)
+                    new_xmax = number_image_text_area.xmax + w/2
+                    rect_max = Rect(xmin=number_image_text_area.xmin, xmax=new_xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                    image_text_areas_max.append(rect_max)
+                image_text_areas.areas[Class_text.number] = image_text_areas_min
+                label_area_min = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
+                                                                  4, 64,128, 2, 64,64)
+                if len(label_area_min.labels[Class_text.number]) == 5:
+                    res_labels['number'] = label_area_min.labels[Class_text.number]
+                else:
+                    image_text_areas.areas[Class_text.number] = image_text_areas_max
+                    label_area_max = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
+                                                                              4, 64, 128, 2, 64, 64)
+                    if len(label_area_max.labels[Class_text.number]) == 5:
+                        res_labels['number'] = label_area_max.labels[Class_text.number]
+                    else:
+                        res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '1275'
             res_labels['year'] = label_area.labels[Class_text.year]
             return res_labels
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 return {"result" : "no_rama"}
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
             img_cut_path = 'cut_img.jpg'
             cv2.imwrite(img_cut_path, img_cut)
             image_text_areas = self.rama_no_spring_bejickaya_text_detect_model.text_detect(img_cut_path)
             label_area = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 6, 64, 192,
                                                                   2, 64, 64, 2, 64,64)
             res_labels = {}
-            res_labels['number'] = label_area.labels[Class_text.number]
+            if len(label_area.labels[Class_text.number]) == 6:
+                res_labels['number'] = label_area.labels[Class_text.number]
+            else:
+                number_image_text_areas = image_text_areas.areas[Class_text.number]
+                image_text_areas_min = []
+                image_text_areas_max = []
+                for number_image_text_area in number_image_text_areas:
+                    w = number_image_text_area.xmax - number_image_text_area.xmin
+                    if (number_image_text_area.xmin - (w/2)) < 0:
+                        new_xmin = 0
+                    else:
+                        new_xmin = number_image_text_area.xmin - (w/2)
+                    rect_min = Rect(xmin=new_xmin, xmax=number_image_text_area.xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                    image_text_areas_min.append(rect_min)
+                    new_xmax = number_image_text_area.xmax + w/2
+                    rect_max = Rect(xmin=number_image_text_area.xmin, xmax=new_xmax, ymin=number_image_text_area.ymin, ymax=number_image_text_area.ymax)
+                    image_text_areas_max.append(rect_max)
+                image_text_areas.areas[Class_text.number] = image_text_areas_min
+                label_area_min = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 5, 64,128,
+                                                                  4, 64,128, 2, 64,64)
+                if len(label_area_min.labels[Class_text.number]) == 6:
+                    res_labels['number'] = label_area_min.labels[Class_text.number]
+                else:
+                    image_text_areas.areas[Class_text.number] = image_text_areas_max
+                    label_area_max = self.text_recognize_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
+                                                                              4, 64, 128, 2, 64, 64)
+                    if len(label_area_max.labels[Class_text.number]) == 6:
+                        res_labels['number'] = label_area_max.labels[Class_text.number]
+                    else:
+                        res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '12'
             res_labels['year'] = label_area.labels[Class_text.year]
             return res_labels
```

### Comparing `danila-lib-1.5.8/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.5.9/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.5.8
+Version: 1.5.9
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.5.8/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.5.9/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/danila_lib.egg-info/requires.txt` & `danila-lib-1.5.9/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/Letters_recognize.py` & `danila-lib-1.5.9/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/Rama_classify_class.py` & `danila-lib-1.5.9/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/Rama_detect_class.py` & `danila-lib-1.5.9/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.5.9/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/Text_detect_class.py` & `danila-lib-1.5.9/data/neuro/Text_detect_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         return res2
     # find text areas on img from img_path with yolov5, returns dict with rects for each text class
     def text_detect(self, img_path):
         """find text areas on img from img_path with yolov5, returns dict with rects for each text class"""
         json_res = self.work_img(img_path)
         image_text_areas = Image_text_areas()
         for text_area_json in json_res:
-            if text_area_json['confidence']>0.29:
+            if text_area_json['confidence']>0.19:
                 text_area = Text_area(text_area_json)
                 image_text_areas.add_area(text_area)
         image_text_areas.correct_intersections()
         return image_text_areas
     # draw img_text_areas on img, returns opencv img
     def draw_text_areas_in_opencv(self, image_text_areas, img):
         """draw img_text_areas on img, returns opencv img"""
```

### Comparing `danila-lib-1.5.8/data/neuro/letters_in_image.py` & `danila-lib-1.5.9/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/models.py` & `danila-lib-1.5.9/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/objs_in_image.py` & `danila-lib-1.5.9/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/neuro/text_recognize_yolo.py` & `danila-lib-1.5.9/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/result/Image_text_areas.py` & `danila-lib-1.5.9/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/result/Rect.py` & `danila-lib-1.5.9/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/result/Text_area.py` & `danila-lib-1.5.9/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/data/result/Yolo_label_rect.py` & `danila-lib-1.5.9/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.5.8/setup.py` & `danila-lib-1.5.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.5.8',
+  version='1.5.9',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

