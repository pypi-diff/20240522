# Comparing `tmp/vanguard_api-0.1.0.tar.gz` & `tmp/vanguard_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanguard_api-0.1.0.tar", last modified: Mon May 20 14:02:12 2024, max compression
+gzip compressed data, was "vanguard_api-0.1.1.tar", last modified: Wed May 22 16:35:08 2024, max compression
```

## Comparing `vanguard_api-0.1.0.tar` & `vanguard_api-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/vanguard/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-20 14:02:08.000000 vanguard_api-0.1.0/vanguard/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:02:12.399745 vanguard_api-0.1.0/vanguard_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 14:02:12.000000 vanguard_api-0.1.0/vanguard_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:08.592570 vanguard_api-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 16:35:08.592570 vanguard_api-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:35:08.592570 vanguard_api-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:08.592570 vanguard_api-0.1.1/vanguard/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/vanguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/vanguard/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/vanguard/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/vanguard/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-22 16:35:04.000000 vanguard_api-0.1.1/vanguard/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:35:08.592570 vanguard_api-0.1.1/vanguard_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-22 16:35:08.000000 vanguard_api-0.1.1/vanguard_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 16:35:08.000000 vanguard_api-0.1.1/vanguard_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:35:08.000000 vanguard_api-0.1.1/vanguard_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 16:35:08.000000 vanguard_api-0.1.1/vanguard_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 16:35:08.000000 vanguard_api-0.1.1/vanguard_api.egg-info/top_level.txt
```

### Comparing `vanguard_api-0.1.0/LICENSE` & `vanguard_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.0/PKG-INFO` & `vanguard_api-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.1.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

### Comparing `vanguard_api-0.1.0/README.md` & `vanguard_api-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.0/setup.py` & `vanguard_api-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="vanguard-api",
-    version="0.1.0",
+    version="0.1.1",
     author="MaxxRK",
     author_email="maxxrk@pm.me",
     description="An unofficial API for Vanguard Invest",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/MaxxRK/vanguard-api",
-    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz",
+    download_url="https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.1.tar.gz",
     keywords=["VANGUARD", "API"],
     install_requires=["playwright", "playwright-stealth"],
     packages=["vanguard"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Internet :: WWW/HTTP :: Session",
```

### Comparing `vanguard_api-0.1.0/vanguard/account.py` & `vanguard_api-0.1.1/vanguard/account.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.0/vanguard/order.py` & `vanguard_api-0.1.1/vanguard/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                 timeout=10000,
             )
             account_selectors = account_box.query_selector_all("tds-list-option")
             for account in account_selectors:
                 if account_id in account.text_content():
                     account.click()
                     break
-        except:
+        except PlaywrightTimeoutError:
             pass
         quote_box = self.session.page.wait_for_selector(
             "//input[@placeholder='Get Quote']"
         )
         quote_box.click()
         quote_box.fill("")
         quote_box.fill(symbol)
@@ -183,31 +183,26 @@
         try:
             if duration == "DAY":
                 self.session.page.click("xpath=//label[text()='Day']")
             elif duration == "GOOD_TILL_CANCELLED":
                 self.session.page.click("xpath=//label[text()='60-day (GTC)']")
             if order_type == "SELL":
                 self.session.page.wait_for_selector(
-                    "body > twe-root > main > twe-trade > form > div > div.row >"
-                    " div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal"
-                    " > tds-modal > div.modal.visible > div > div.modal__content",
+                    "body > twe-root > main > twe-trade > form > div > div.row > div:nth-child(1) > twe-cost-basis-control > twe-cost-basis-modal > tds-modal > div.modal.visible > div > div.modal__content",
                     timeout=10000,
                 )
                 self.session.page.wait_for_selector(
                     "//button[text()=' Continue ']",
                     timeout=10000,
                 ).click()
         except PlaywrightTimeoutError:
             pass
         try:
             self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-trade > form > div > div.row >"
-                " div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail"
-                " > tds-card > div > tds-card-body > div.twe-flex-button-wrap >"
-                " button:nth-child(2)",
+                "body > twe-root > vg-vgn-nav > div > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div.twe-flex-button-wrap > button:nth-child(2)",
                 timeout=5000,
             ).click()
         except PlaywrightTimeoutError:
             pass
         if after_hours:
             try:
                 sleep(2)
@@ -216,18 +211,15 @@
                     timeout=5000,
                 ).click()
             except PlaywrightTimeoutError:
                 pass
 
         try:
             warning = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-trade > form > div > div.row >"
-                " div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail"
-                " > tds-card > div > tds-card-body > div:nth-child(3) > div > tds-card"
-                " > div > tds-card-body",
+                "body > twe-root > main > twe-trade > form > div > div.row > div.col-lg-6.col-xxl-4.tds-mb-9.d-none.d-xxl-block > twe-trade-detail > tds-card > div > tds-card-body > div:nth-child(3) > div > tds-card > div > tds-card-body",
                 timeout=5000,
             )
             warning_header_selector = warning.query_selector("p")
             warning_header = warning_header_selector.text_content()
             warning_items = warning.query_selector_all("li")
             warning_text = {warning_header: []}
             for item in warning_items:
@@ -235,58 +227,52 @@
             order_messages["ORDER INVALID"] = warning_text
             return order_messages
         except PlaywrightTimeoutError:
             order_messages["ORDER INVALID"] = "No invalid order message found."
 
         try:
             order_preview = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-preview > div > div > div.col-lg-7 >"
-                " tds-card > div > tds-card-body > twe-order-details",
+                ".col-lg-7 > tds-card:nth-child(1) > div:nth-child(1) > tds-card-body:nth-child(1)",
                 timeout=5000,
             )
             order_preview_text = order_preview.text_content()
             preview_parts = re.split(
-                r"(Account|Transaction|Shares|Security|Order"
-                r" type|Duration|Commission|Estimated amount|\*)",
+                r"(Account|Transaction|Shares|Security|Order type|Duration|Commission|Estimated amount|\*)",
                 order_preview_text,
             )
             order_preview = {
                 "Account": preview_parts[2],
                 "Transaction": preview_parts[4],
                 "Shares": preview_parts[6],
                 "Security": preview_parts[8],
                 "Order type": preview_parts[10],
                 "Duration": preview_parts[12],
                 "Commission": preview_parts[14],
                 "Estimated amount": preview_parts[18],
                 "Note": preview_parts[20],
             }
             order_messages["ORDER PREVIEW"] = order_preview
-            if not dry_run:
-                try:
-                    self.session.page.click(
-                        "//button[text()=' Submit Order ']", timeout=10000
-                    )
-                except PlaywrightTimeoutError:
-                    raise Exception("No place order button found cannot continue.")
-            else:
+            if dry_run:
                 return order_messages
+            try:
+                self.session.page.click(
+                    "//button[text()=' Submit Order ']", timeout=10000
+                )
+            except PlaywrightTimeoutError:
+                raise Exception("No place order button found cannot continue.")
         except PlaywrightTimeoutError:
             order_messages["ORDER PREVIEW"] = "No order preview page found."
 
         try:
             order_handle_one = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-confirm > div > div >"
-                " div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > h2",
+                "body > twe-root > vg-vgn-nav > div > main > twe-confirm > div > div > div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > h2",
                 timeout=5000,
             )
             order_handle_two = self.session.page.wait_for_selector(
-                "body > twe-root > main > twe-confirm > div > div >"
-                " div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 >"
-                " div.page-heading.tds-mb-7",
+                "body > twe-root > vg-vgn-nav > div > main > twe-confirm > div > div > div.col-lg-7.order-first.order-lg-last.tds-mb-4.tds-mb-m-9 > div.page-heading.tds-mb-7 > p",
                 timeout=5000,
             )
             order_number_text = order_handle_one.text_content()
             order_match = re.search(r"Received order #(\d+)", order_number_text)
             if order_match:
                 order_number = order_match.group(1)
             else:
```

### Comparing `vanguard_api-0.1.0/vanguard/session.py` & `vanguard_api-0.1.1/vanguard/session.py`

 * *Files identical despite different names*

### Comparing `vanguard_api-0.1.0/vanguard_api.egg-info/PKG-INFO` & `vanguard_api-0.1.1/vanguard_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vanguard-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: An unofficial API for Vanguard Invest
 Home-page: https://github.com/MaxxRK/vanguard-api
-Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.0.tar.gz
+Download-URL: https://github.com/MaxxRK/vanguard-api/archive/refs/tags/v0.1.1.tar.gz
 Author: MaxxRK
 Author-email: maxxrk@pm.me
 License: MIT
 Keywords: VANGUARD,API
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: WWW/HTTP :: Session
```

