# Comparing `tmp/parcllabs-0.2.1.tar.gz` & `tmp/parcllabs-0.2.2.tar.gz`

## Comparing `parcllabs-0.2.1.tar` & `parcllabs-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/__init__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/__version__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/common.py
--rw-r--r--   0        0        0     6514 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/parcllabs_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/search/__init__.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/search/metros.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/search/top_markets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/__init__.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/investor_metrics.py
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/market_metrics.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/parcllabs_service.py
--rw-r--r--   0        0        0    17702 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/portfolio_metrics.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/price_feed.py
--rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/rental_market_metrics.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 parcllabs-0.2.1/parcllabs/services/search.py
--rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 parcllabs-0.2.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 parcllabs-0.2.1/LICENSE
--rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 parcllabs-0.2.1/README.md
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 parcllabs-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    16712 2020-02-02 00:00:00.000000 parcllabs-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/__init__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/__version__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/common.py
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/parcllabs_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/__init__.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/metros.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/search/top_markets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/__init__.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0        0        0    14217 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/investor_metrics.py
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/market_metrics.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/parcllabs_service.py
+-rw-r--r--   0        0        0    17702 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/price_feed.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/rental_market_metrics.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 parcllabs-0.2.2/parcllabs/services/search.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 parcllabs-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 parcllabs-0.2.2/LICENSE
+-rw-r--r--   0        0        0    14620 2020-02-02 00:00:00.000000 parcllabs-0.2.2/README.md
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 parcllabs-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    16712 2020-02-02 00:00:00.000000 parcllabs-0.2.2/PKG-INFO
```

### Comparing `parcllabs-0.2.1/parcllabs/parcllabs_client.py` & `parcllabs-0.2.2/parcllabs/parcllabs_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,22 +148,27 @@
             response = requests.get(full_url, headers=headers, params=params)
             response.raise_for_status()
             return response.json()
         except requests.exceptions.HTTPError:
             try:
                 error_details = response.json()
                 error_message = error_details.get("detail", "No detail provided by API")
+                error = error_message
+                if response.status_code == 403:
+                    error = f"{error_message}. Visit https://dashboard.parcllabs.com for more information or reach out to team@parcllabs.com."
+                if response.status_code == 429:
+                    error = error_details.get("error", "Rate Limit Exceeded")
             except json.JSONDecodeError:
                 error_message = "Failed to decode JSON error response"
             type_of_error = ""
             if 400 <= response.status_code < 500:
                 type_of_error = "Client"
             elif 500 <= response.status_code < 600:
                 type_of_error = "Server"
-            msg = f"{response.status_code} {type_of_error} Error: {error_message}. Visit https://dashboard.parcllabs.com for more information or reach out to team@parcllabs.com."
+            msg = f"{response.status_code} {type_of_error} Error: {error}"
             raise RequestException(msg)
         except requests.exceptions.RequestException as err:
             raise RequestException(f"Request failed: {str(err)}")
         except Exception as e:
             raise RequestException(f"An unexpected error occurred: {str(e)}")
 
     def _get_headers(self) -> Dict[str, str]:
```

### Comparing `parcllabs-0.2.1/parcllabs/search/metros.py` & `parcllabs-0.2.2/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.2.2/parcllabs/services/for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/investor_metrics.py` & `parcllabs-0.2.2/parcllabs/services/investor_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/market_metrics.py` & `parcllabs-0.2.2/parcllabs/services/market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/parcllabs_service.py` & `parcllabs-0.2.2/parcllabs/services/parcllabs_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
     def _request(
         self,
         url: str,
         params: Optional[Mapping[str, Any]] = None,
         is_next: bool = False,
     ) -> Any:
-
         return self.client.get(url=url, params=params, is_next=is_next)
 
     def _as_pd_dataframe(self, data: List[Mapping[str, Any]]) -> Any:
         output = []
 
         for key, value in data.items():
             data_df = pd.DataFrame(value)
```

### Comparing `parcllabs-0.2.1/parcllabs/services/portfolio_metrics.py` & `parcllabs-0.2.2/parcllabs/services/portfolio_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/price_feed.py` & `parcllabs-0.2.2/parcllabs/services/price_feed.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.2.2/parcllabs/services/rental_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/parcllabs/services/search.py` & `parcllabs-0.2.2/parcllabs/services/search.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/.gitignore` & `parcllabs-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/LICENSE` & `parcllabs-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/README.md` & `parcllabs-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/pyproject.toml` & `parcllabs-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parcllabs-0.2.1/PKG-INFO` & `parcllabs-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: parcllabs
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python SDK for ParclLabs API
 Project-URL: Homepage, https://github.com/ParclLabs/parcllabs-python
 Author-email: ParclLabs <team@parcllabs.com>
 License: MIT License
         
         Copyright (c) [2024] [Parcl Labs]
```

