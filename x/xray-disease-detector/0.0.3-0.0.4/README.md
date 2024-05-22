# Comparing `tmp/xray_disease_detector-0.0.3.tar.gz` & `tmp/xray_disease_detector-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xray_disease_detector-0.0.3.tar", last modified: Wed May 22 12:41:56 2024, max compression
+gzip compressed data, was "xray_disease_detector-0.0.4.tar", last modified: Wed May 22 12:44:01 2024, max compression
```

## Comparing `xray_disease_detector-0.0.3.tar` & `xray_disease_detector-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:41:56.625061 xray_disease_detector-0.0.3/
--rw-r--r--   0 k-on       (501) staff       (20)      805 2024-05-22 12:41:56.624912 xray_disease_detector-0.0.3/PKG-INFO
--rw-r--r--   0 k-on       (501) staff       (20)      239 2024-05-22 12:38:10.000000 xray_disease_detector-0.0.3/README.md
--rw-r--r--   0 k-on       (501) staff       (20)       38 2024-05-22 12:41:56.625109 xray_disease_detector-0.0.3/setup.cfg
--rw-r--r--   0 k-on       (501) staff       (20)     1165 2024-05-22 12:41:34.000000 xray_disease_detector-0.0.3/setup.py
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:41:56.624047 xray_disease_detector-0.0.3/src/
-drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:41:56.624701 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/
--rw-r--r--   0 k-on       (501) staff       (20)      805 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/PKG-INFO
--rw-r--r--   0 k-on       (501) staff       (20)      343 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/SOURCES.txt
--rw-r--r--   0 k-on       (501) staff       (20)        1 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/dependency_links.txt
--rw-r--r--   0 k-on       (501) staff       (20)       69 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/entry_points.txt
--rw-r--r--   0 k-on       (501) staff       (20)       25 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/requires.txt
--rw-r--r--   0 k-on       (501) staff       (20)       22 2024-05-22 12:41:56.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/top_level.txt
--rw-r--r--   0 k-on       (501) staff       (20)     1512 2024-05-22 12:41:24.000000 xray_disease_detector-0.0.3/src/xray_disease_detector.py
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:44:01.514494 xray_disease_detector-0.0.4/
+-rw-r--r--   0 k-on       (501) staff       (20)      805 2024-05-22 12:44:01.514373 xray_disease_detector-0.0.4/PKG-INFO
+-rw-r--r--   0 k-on       (501) staff       (20)      239 2024-05-22 12:38:10.000000 xray_disease_detector-0.0.4/README.md
+-rw-r--r--   0 k-on       (501) staff       (20)       38 2024-05-22 12:44:01.514535 xray_disease_detector-0.0.4/setup.cfg
+-rw-r--r--   0 k-on       (501) staff       (20)     1165 2024-05-22 12:43:55.000000 xray_disease_detector-0.0.4/setup.py
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:44:01.513544 xray_disease_detector-0.0.4/src/
+drwxr-xr-x   0 k-on       (501) staff       (20)        0 2024-05-22 12:44:01.514198 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/
+-rw-r--r--   0 k-on       (501) staff       (20)      805 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/PKG-INFO
+-rw-r--r--   0 k-on       (501) staff       (20)      343 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/SOURCES.txt
+-rw-r--r--   0 k-on       (501) staff       (20)        1 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/dependency_links.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       69 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/entry_points.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       25 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/requires.txt
+-rw-r--r--   0 k-on       (501) staff       (20)       22 2024-05-22 12:44:01.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/top_level.txt
+-rw-r--r--   0 k-on       (501) staff       (20)     1633 2024-05-22 12:43:47.000000 xray_disease_detector-0.0.4/src/xray_disease_detector.py
```

### Comparing `xray_disease_detector-0.0.3/PKG-INFO` & `xray_disease_detector-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xray_disease_detector
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for detecting diseases in X-ray images using a pre-trained PyTorch model
 Home-page: https://github.com/KONMIO34/xray_disease_detector
 Author: Gong Zhan
 Author-email: gongzhan34@yahoo.co.jp
 Project-URL: Bug Tracker, https://github.com/KONMIO34/xray_disease_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xray_disease_detector-0.0.3/setup.py` & `xray_disease_detector-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xray_disease_detector",
-    version="0.0.3",
+    version="0.0.4",
     author="Gong Zhan",
     author_email="gongzhan34@yahoo.co.jp",
     description="A package for detecting diseases in X-ray images using a pre-trained PyTorch model",
     long_description=long_description,      
     long_description_content_type="text/markdown",
     url="https://github.com/KONMIO34/xray_disease_detector",
     project_urls={
```

### Comparing `xray_disease_detector-0.0.3/src/xray_disease_detector.egg-info/PKG-INFO` & `xray_disease_detector-0.0.4/src/xray_disease_detector.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xray-disease-detector
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package for detecting diseases in X-ray images using a pre-trained PyTorch model
 Home-page: https://github.com/KONMIO34/xray_disease_detector
 Author: Gong Zhan
 Author-email: gongzhan34@yahoo.co.jp
 Project-URL: Bug Tracker, https://github.com/KONMIO34/xray_disease_detector/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xray_disease_detector-0.0.3/src/xray_disease_detector.py` & `xray_disease_detector-0.0.4/src/xray_disease_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # src/xray_disease_detector.py
 
 import torch
 from torchvision import transforms, models
+from torch import nn
 from PIL import Image
 import sys
 
 class XRayDiseaseDetector:
     def __init__(self, model_path=None):
         self.model = self.load_model(model_path)
         self.model.eval()
         self.transform = transforms.Compose([
             transforms.Resize((224, 224)),
             transforms.ToTensor(),
             transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
         ])
         
     def load_model(self, model_path):
-        model = models.vit_b_16(weights='DEFAULT')  # 使用预定义的ViT模型
+        model = models.vit_b_16(weights='DEFAULT')
+        num_ftrs = model.heads.head.in_features
+        model.heads.head = nn.Linear(num_ftrs, 8)  # 假设你的模型有8个输出类别
         if model_path:
             state_dict = torch.load(model_path)
             model.load_state_dict(state_dict)
         return model
         
     def predict(self, img_path):
         img = Image.open(img_path).convert('RGB')
         img = self.transform(img)
         img = img.unsqueeze(0)  # 添加批次维度
         
         with torch.no_grad():
             outputs = self.model(img)
-            _, predicted = torch.max(outputs.logits, 1)  # ViT模型的输出需要访问logits
+            _, predicted = torch.max(outputs, 1)  # ViT模型的输出需要访问logits
         
         return predicted.item()
 
 def main():
     if len(sys.argv) != 3:
         print("Usage: xray_disease_detector <model_path> <image_path>")
         sys.exit(1)
@@ -43,8 +46,7 @@
     
     detector = XRayDiseaseDetector(model_path)
     result = detector.predict(image_path)
     print(f"Prediction: {result}")
 
 if __name__ == "__main__":
     main()
-
```

