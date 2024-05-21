# Comparing `tmp/lavague_drivers_selenium-0.1.2.tar.gz` & `tmp/lavague_drivers_selenium-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_drivers_selenium-0.1.2.tar", max compression
+gzip compressed data, was "lavague_drivers_selenium-0.1.3.tar", max compression
```

## Comparing `lavague_drivers_selenium-0.1.2.tar` & `lavague_drivers_selenium-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       34 2024-05-18 13:00:01.403135 lavague_drivers_selenium-0.1.2/README.md
--rw-r--r--   0        0        0       57 2024-05-18 13:00:01.403135 lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/__init__.py
--rw-r--r--   0        0        0    11834 2024-05-18 13:00:20.363119 lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/base.py
--rw-r--r--   0        0        0      976 2024-05-18 13:05:44.627475 lavague_drivers_selenium-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.3/README.md
+-rw-r--r--   0        0        0       57 2024-05-15 22:13:36.166566 lavague_drivers_selenium-0.1.3/lavague/drivers/selenium/__init__.py
+-rw-r--r--   0        0        0     9287 2024-05-21 22:50:43.796201 lavague_drivers_selenium-0.1.3/lavague/drivers/selenium/base.py
+-rw-r--r--   0        0        0      976 2024-05-21 23:05:52.321114 lavague_drivers_selenium-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lavague_drivers_selenium-0.1.3/PKG-INFO
```

### Comparing `lavague_drivers_selenium-0.1.2/lavague/drivers/selenium/base.py` & `lavague_drivers_selenium-0.1.3/lavague/drivers/selenium/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 from typing import Any, Optional, Callable
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.common.by import By
 from lavague.core.base_driver import BaseDriver
-from PIL import Image
-from lavague.core.utilities.format_utils import (
-    return_assigned_variables,
-    keep_assignments,
-)
 
 
 class SeleniumDriver(BaseDriver):
     driver: WebDriver
 
     def __init__(
         self,
@@ -95,82 +89,14 @@
         self.driver.set_window_size(width, targeted_height)
 
         viewport_height = self.driver.execute_script("return window.innerHeight;")
 
         height_difference = targeted_height - viewport_height
         self.driver.set_window_size(width, targeted_height + height_difference)
 
-    def get_highlighted_element(self, generated_code):
-        # Extract the assignments from the generated code
-        assignment_code = keep_assignments(generated_code)
-
-        # We add imports to the code to be executed
-        code = f"""
-from selenium.webdriver.common.by import By
-from selenium.webdriver.common.keys import Keys
-from selenium.webdriver.common.action_chains import ActionChains
-{assignment_code}
-        """.strip()
-
-        local_scope = {"driver": self.driver}
-
-        exec(code, local_scope, local_scope)
-
-        # We extract pairs of variables assigned during execution with their name and pointer
-        variable_names = return_assigned_variables(generated_code)
-
-        elements = {}
-
-        for variable_name in variable_names:
-            var = local_scope[variable_name]
-            if type(var) == WebElement:
-                elements[variable_name] = var
-
-        if len(elements) == 0:
-            raise ValueError(f"No element found.")
-
-        outputs = []
-        for element_name, element in elements.items():
-            local_scope = {"driver": self.driver, element_name: element}
-
-            code = f"""
-element = {element_name}
-driver.execute_script("arguments[0].setAttribute('style', arguments[1]);", element, "border: 2px solid red;")
-driver.execute_script("arguments[0].scrollIntoView({{block: 'center'}});", element)
-driver.save_screenshot("screenshot.png")
-
-x1 = element.location['x']
-y1 = element.location['y']
-
-x2 = x1 + element.size['width']
-y2 = y1 + element.size['height']
-
-viewport_width = driver.execute_script("return window.innerWidth;")
-viewport_height = driver.execute_script("return window.innerHeight;")
-"""
-            exec(code, globals(), local_scope)
-            bounding_box = {
-                "x1": local_scope["x1"],
-                "y1": local_scope["y1"],
-                "x2": local_scope["x2"],
-                "y2": local_scope["y2"],
-            }
-            viewport_size = {
-                "width": local_scope["viewport_width"],
-                "height": local_scope["viewport_height"],
-            }
-            image = Image.open("screenshot.png")
-            output = {
-                "image": image,
-                "bounding_box": bounding_box,
-                "viewport_size": viewport_size,
-            }
-            outputs.append(output)
-        return outputs
-
     def get_capability(self) -> str:
         return '''
 
 Your goal is to write Selenium code to answer queries.
 
 Your answer must be a Python markdown only.
 You can have access to external websites and libraries.
```

### Comparing `lavague_drivers_selenium-0.1.2/pyproject.toml` & `lavague_drivers_selenium-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-drivers-selenium"
-version = "0.1.2"
+version = "0.1.3"
 description = "Selenium integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_drivers_selenium-0.1.2/PKG-INFO` & `lavague_drivers_selenium-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-drivers-selenium
-Version: 0.1.2
+Version: 0.1.3
 Summary: Selenium integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,selenium
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

