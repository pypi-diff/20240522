# Comparing `tmp/lusid_express-1.1.8.tar.gz` & `tmp/lusid_express-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.1.8.tar", last modified: Wed May 15 14:31:34 2024, max compression
+gzip compressed data, was "lusid_express-1.1.9.tar", last modified: Wed May 15 15:27:17 2024, max compression
```

## Comparing `lusid_express-1.1.8.tar` & `lusid_express-1.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.243222 lusid_express-1.1.8/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-15 14:30:45.000000 lusid_express-1.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-15 14:30:45.000000 lusid_express-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 14:31:34.242222 lusid_express-1.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-15 14:30:45.000000 lusid_express-1.1.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 14:31:34.243222 lusid_express-1.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-15 14:30:45.000000 lusid_express-1.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.235222 lusid_express-1.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.237222 lusid_express-1.1.8/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.238222 lusid_express-1.1.8/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-15 14:31:33.000000 lusid_express-1.1.8/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.241222 lusid_express-1.1.8/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3157 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/utils/
--rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.242222 lusid_express-1.1.8/src/lusid_express/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     7731 2024-05-15 14:30:45.000000 lusid_express-1.1.8/src/lusid_express/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 14:31:34.238222 lusid_express-1.1.8/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 14:31:34.000000 lusid_express-1.1.8/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.726744 lusid_express-1.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-15 15:26:28.000000 lusid_express-1.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-15 15:26:28.000000 lusid_express-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 15:27:17.725744 lusid_express-1.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7562 2024-05-15 15:26:28.000000 lusid_express-1.1.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 15:27:17.726744 lusid_express-1.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-15 15:26:28.000000 lusid_express-1.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.718744 lusid_express-1.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.720744 lusid_express-1.1.9/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5913 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.721744 lusid_express-1.1.9/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.724744 lusid_express-1.1.9/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.725744 lusid_express-1.1.9/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3157 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.725744 lusid_express-1.1.9/src/lusid_express/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.725744 lusid_express-1.1.9/src/lusid_express/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2024-05-15 15:26:28.000000 lusid_express-1.1.9/src/lusid_express/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 15:27:17.721744 lusid_express-1.1.9/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8202 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-15 15:27:17.000000 lusid_express-1.1.9/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.1.8/LICENSE` & `lusid_express-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/PKG-INFO` & `lusid_express-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.1.8
+Version: 1.1.9
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.8/README.md` & `lusid_express-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/setup.py` & `lusid_express-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.1.8',
+    version='1.1.9',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.1.8/src/lusid_express/__main__.py` & `lusid_express-1.1.9/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/apis/__init__.py` & `lusid_express-1.1.9/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.1.9/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/display/__init__.py` & `lusid_express-1.1.9/src/lusid_express/display/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/load.le` & `lusid_express-1.1.9/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/utils/__init__.py` & `lusid_express-1.1.9/src/lusid_express/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.1.8/src/lusid_express/widgets/__init__.py` & `lusid_express-1.1.9/src/lusid_express/widgets/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,25 +56,26 @@
         self.create_transaction_form(txn)
 
     def create_transaction_form(self, txn: lu.TransactionRequest):
         # Default values derived from the variables
         default_transaction_id = txn.transaction_id
         default_type = txn.type
         default_source = txn.source
-        default_instrument_identifiers = txn.instrument_identifiers["Instrument/default/ClientInternal"]
+        default_instrument_identifiers = list(txn.instrument_identifiers.keys())[0]
         default_transaction_date = txn.transaction_date
         default_settlement_date = txn.settlement_date
         default_units = txn.units
         default_transaction_currency = txn.transaction_currency
         default_amount = txn.total_consideration.amount
         default_settlement_currency = txn.total_consideration.currency
         default_net_amount = txn.properties[f'Transaction/{self.scope}/NetAmount'].value.metric_value.value
+        default_properties = txn.properties
 
         # Create widgets with custom layout for labels and fields
-        label_layout = widgets.Layout(width='200px')  # Adjust width as needed
+        label_layout = widgets.Layout(width='200px',)  # Adjust width as needed
         field_layout = widgets.Layout(width='350px')  # Adjust to fit the form container
 
         transaction_id = widgets.Text(value=default_transaction_id, layout=field_layout, style={'description_width': 'initial'})
         type = widgets.Text(value=default_type, layout=field_layout, style={'description_width': 'initial'})
         source = widgets.Text(value=default_source, layout=field_layout, style={'description_width': 'initial'})
         instrument_identifiers = widgets.Text(value=default_instrument_identifiers, layout=field_layout, style={'description_width': 'initial'})
         transaction_date = widgets.DatePicker(value=datetime.strptime(default_transaction_date, "%Y-%m-%d"), layout=field_layout, style={'description_width': 'initial'})
@@ -88,26 +89,21 @@
 
         # Function to create the transaction request based on user input
         def create_transaction_request():
             txn_ = lm.TransactionRequest(
                 transaction_id=transaction_id.value,
                 type=type.value,
                 source=source.value,
-                instrument_identifiers={"Instrument/default/ClientInternal": instrument_identifiers.value},
+                instrument_identifiers={default_instrument_identifiers: instrument_identifiers.value},
                 transaction_date=transaction_date.value.strftime("%Y-%m-%d"),
                 settlement_date=settlement_date.value.strftime("%Y-%m-%d"),
                 units=units.value,
                 transaction_currency=transaction_currency.value, 
                 total_consideration=lm.CurrencyAndAmount(amount=amount.value, currency=settlement_currency.value), 
-                properties={
-                    f"Transaction/{self.scope}/NetAmount": lu.PerpetualProperty(
-                        key=f"Transaction/{self.scope}/NetAmount",
-                        value=lu.PropertyValue(metric_value=lu.MetricValue(value=net_amount.value)),
-                    ),
-                },
+                properties=default_properties,
             )
             return txn_
 
         # Function to handle button click
         def on_button_click(b):
             transaction_request = create_transaction_request()
             display(transaction_portfolios_api.upsert_transactions(
```

### Comparing `lusid_express-1.1.8/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.1.9/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.1.8
+Version: 1.1.9
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.1.8/src/lusid_express.egg-info/SOURCES.txt` & `lusid_express-1.1.9/src/lusid_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

