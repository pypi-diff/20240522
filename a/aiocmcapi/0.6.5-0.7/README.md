# Comparing `tmp/aiocmcapi-0.6.5.tar.gz` & `tmp/aiocmcapi-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.6.5.tar", last modified: Mon May 20 10:06:37 2024, max compression
+gzip compressed data, was "aiocmcapi-0.7.tar", last modified: Tue May 21 10:32:49 2024, max compression
```

## Comparing `aiocmcapi-0.6.5.tar` & `aiocmcapi-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.018355 aiocmcapi-0.6.5/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6.5/LICENSE
--rw-rw-rw-   0        0        0     3423 2024-05-20 10:06:37.017354 aiocmcapi-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     3153 2024-05-20 09:59:10.000000 aiocmcapi-0.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.012373 aiocmcapi-0.6.5/aiocmcapi/
--rw-rw-rw-   0        0        0       61 2024-05-13 02:36:12.000000 aiocmcapi-0.6.5/aiocmcapi/__init__.py
--rw-rw-rw-   0        0        0      738 2024-05-12 15:05:54.000000 aiocmcapi-0.6.5/aiocmcapi/client.py
--rw-rw-rw-   0        0        0     1352 2024-05-20 09:36:16.000000 aiocmcapi-0.6.5/aiocmcapi/currency.py
-drwxrwxrwx   0        0        0        0 2024-05-20 10:06:37.016357 aiocmcapi-0.6.5/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     3423 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-05-20 10:06:37.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-20 10:06:36.000000 aiocmcapi-0.6.5/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      354 2024-05-20 10:06:30.000000 aiocmcapi-0.6.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 10:06:37.018355 aiocmcapi-0.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 10:32:49.136330 aiocmcapi-0.7/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.7/LICENSE
+-rw-rw-rw-   0        0        0     3421 2024-05-21 10:32:49.135330 aiocmcapi-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3153 2024-05-21 10:26:41.000000 aiocmcapi-0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 10:32:49.128329 aiocmcapi-0.7/aiocmcapi/
+-rw-rw-rw-   0        0        0       58 2024-05-21 07:51:43.000000 aiocmcapi-0.7/aiocmcapi/__init__.py
+-rw-rw-rw-   0        0        0      814 2024-05-21 10:11:34.000000 aiocmcapi-0.7/aiocmcapi/client.py
+-rw-rw-rw-   0        0        0     1080 2024-05-21 10:25:37.000000 aiocmcapi-0.7/aiocmcapi/currency.py
+drwxrwxrwx   0        0        0        0 2024-05-21 10:32:49.134331 aiocmcapi-0.7/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     3421 2024-05-21 10:32:49.000000 aiocmcapi-0.7/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2024-05-21 10:32:49.000000 aiocmcapi-0.7/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 10:32:49.000000 aiocmcapi-0.7/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 10:32:49.000000 aiocmcapi-0.7/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 10:32:49.000000 aiocmcapi-0.7/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      352 2024-05-21 10:28:48.000000 aiocmcapi-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 10:32:49.136330 aiocmcapi-0.7/setup.cfg
```

### Comparing `aiocmcapi-0.6.5/LICENSE` & `aiocmcapi-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.6.5/PKG-INFO` & `aiocmcapi-0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.6.5
+Version: 0.7
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
 
@@ -29,51 +29,53 @@
 ```
 
 ## Example for currency data with CoinMarketCap ID
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient, Currency
+from aiocmcapi import Client, Currency
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     btc = Currency(cmc_id=1)
+    await btc.update(client)
 
-    await btc.update_data(client)
-    print(f"{btc.name} | {btc.symbol}\nPrice: {round(btc.price, 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{btc.slug}")
+    print(f"{btc.name} | {btc.symbol}\nPrice: {round(btc.quote['USD']['price'], 2)}$"\
+    f"\nCMC Link: https://www.coinmarketcap.com/currencies/{btc.slug}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 or
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient
+from aiocmcapi import Client
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     cmc_id = 1
 
-    r_json = await client.get(
+    r = await client.get(
         endpoint="/v2/cryptocurrency/quotes/latest",
         params={
             'id': cmc_id
-        }
+        },
+        close=True
     )
-    data = r_json['data'][str(cmc_id)]
+    data = r['data'][str(cmc_id)]
 
     print(f"{data['name']} | {data['symbol']}\nPrice: {round(data['quote']['USD']['price'], 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{data['slug']}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
@@ -86,25 +88,25 @@
 ```
 
 ### For currency metadata
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient, Currency
+from aiocmcapi import Client, Currency
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     btc = Currency(cmc_id=1)
-    await btc.update_meta(client)
+    await btc.update(client)
 
-    print(f"{btc.meta['name']} | {btc.meta['symbol']}\nDescription: {btc.meta['description']}\nWebsite: {btc.meta['urls']['website'][0]}")
+    print(f"{btc.meta.name} | {btc.meta.symbol}\nDescription: {btc.meta.description}\nWebsite: {btc.meta.urls['website'][0]}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
 
@@ -117,26 +119,26 @@
 ## Example for other API endpoints
 
 [CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient
+from aiocmcapi import Client
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
-    r_json = await client.get(
-        endpoint="/v1/cryptocurrency/listings/latest"
+    r = await client.get(
+        endpoint="/v1/cryptocurrency/listings/latest",
+        close=True
     )
-
-    print(r_json)
+    print(r)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
```

### Comparing `aiocmcapi-0.6.5/README.md` & `aiocmcapi-0.7/aiocmcapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: aiocmcapi
+Version: 0.7
+Summary: Async wrapper for CoinMarketCap API
+Author-email: alobuzy <amozebus@gmail.com>
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp>=3.9.5
+
 ![logo](https://github.com/alobuzy/aiocmcapi/assets/115936023/5e8fb136-9613-4369-9c68-260144a4f6bf)
 
 # aiocmcapi
 
 CoinMarketCap API async wrapper
 
 ## Installation
@@ -19,51 +29,53 @@
 ```
 
 ## Example for currency data with CoinMarketCap ID
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient, Currency
+from aiocmcapi import Client, Currency
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     btc = Currency(cmc_id=1)
+    await btc.update(client)
 
-    await btc.update_data(client)
-    print(f"{btc.name} | {btc.symbol}\nPrice: {round(btc.price, 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{btc.slug}")
+    print(f"{btc.name} | {btc.symbol}\nPrice: {round(btc.quote['USD']['price'], 2)}$"\
+    f"\nCMC Link: https://www.coinmarketcap.com/currencies/{btc.slug}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 or
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient
+from aiocmcapi import Client
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     cmc_id = 1
 
-    r_json = await client.get(
+    r = await client.get(
         endpoint="/v2/cryptocurrency/quotes/latest",
         params={
             'id': cmc_id
-        }
+        },
+        close=True
     )
-    data = r_json['data'][str(cmc_id)]
+    data = r['data'][str(cmc_id)]
 
     print(f"{data['name']} | {data['symbol']}\nPrice: {round(data['quote']['USD']['price'], 2)}$\nCMC Link: https://www.coinmarketcap.com/currencies/{data['slug']}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
@@ -76,25 +88,25 @@
 ```
 
 ### For currency metadata
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient, Currency
+from aiocmcapi import Client, Currency
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
     btc = Currency(cmc_id=1)
-    await btc.update_meta(client)
+    await btc.update(client)
 
-    print(f"{btc.meta['name']} | {btc.meta['symbol']}\nDescription: {btc.meta['description']}\nWebsite: {btc.meta['urls']['website'][0]}")
+    print(f"{btc.meta.name} | {btc.meta.symbol}\nDescription: {btc.meta.description}\nWebsite: {btc.meta.urls['website'][0]}")
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
 
@@ -107,29 +119,29 @@
 ## Example for other API endpoints
 
 [CoinMarketCap API endpoint overview](https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview)
 
 ```python
 import asyncio
 
-from aiocmcapi import APIClient
+from aiocmcapi import Client
 
 async def main():
-    client = APIClient(
+    client = Client(
         api_key="YOUR_API_KEY_HERE"
     )
 
-    r_json = await client.get(
-        endpoint="/v1/cryptocurrency/listings/latest"
+    r = await client.get(
+        endpoint="/v1/cryptocurrency/listings/latest",
+        close=True
     )
-
-    print(r_json)
+    print(r)
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
 Output:
 
 ```
 {'status': {'timestamp': '2024-05-11T05:09:27.205Z', 'error_code': 0, 'error_message': None, 'elapsed': 21, 'credit_count': 1, 'notice': None, 'total_count': 9933}, 'data': [{'id': 1, 'name': 'Bitcoin', 'symbol': 'BTC', 'slug': ...
-```
+```
```

### Comparing `aiocmcapi-0.6.5/aiocmcapi/client.py` & `aiocmcapi-0.7/aiocmcapi/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,23 @@
             }
         )
     
     async def close_session(self):
         await self._session.connector.close()
         await self._session.close()
 
-class APIClient(BaseClient):
-    async def get(self, endpoint: str, params: dict = None) -> dict:
+class Client(BaseClient):
+    async def get(
+        self,
+        endpoint: str,
+        params: dict = None,
+        close: bool = False
+    ) -> dict:
         async with self._session.get(
             url=endpoint,
             params=params
         ) as r:
             json = await r.json()
-            await self.close_session()
-            
+            if close:
+                await self.close_session()
+
             return json
```

