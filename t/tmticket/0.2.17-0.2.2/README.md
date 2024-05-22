# Comparing `tmp/tmticket-0.2.17.tar.gz` & `tmp/tmticket-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmticket-0.2.17.tar", last modified: Wed May 22 03:16:41 2024, max compression
+gzip compressed data, was "tmticket-0.2.2.tar", last modified: Wed May  8 00:06:29 2024, max compression
```

## Comparing `tmticket-0.2.17.tar` & `tmticket-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:16:41.351453 tmticket-0.2.17/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-22 03:16:41.350453 tmticket-0.2.17/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 03:16:41.351453 tmticket-0.2.17/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      519 2024-05-22 03:16:21.000000 tmticket-0.2.17/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:16:41.348453 tmticket-0.2.17/tmticket/
--rw-r--r--   0 root         (0) root         (0)      363 2024-05-22 03:00:15.000000 tmticket-0.2.17/tmticket/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5755 2024-05-22 03:12:00.000000 tmticket-0.2.17/tmticket/client.py
--rw-r--r--   0 root         (0) root         (0)    12896 2024-05-22 03:11:37.000000 tmticket-0.2.17/tmticket/model.py
--rw-r--r--   0 root         (0) root         (0)     4315 2024-05-22 03:10:00.000000 tmticket-0.2.17/tmticket/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:16:41.350453 tmticket-0.2.17/tmticket.egg-info/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-22 03:16:40.000000 tmticket-0.2.17/tmticket.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-05-22 03:16:41.000000 tmticket-0.2.17/tmticket.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 03:16:40.000000 tmticket-0.2.17/tmticket.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 03:16:40.000000 tmticket-0.2.17/tmticket.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 03:16:40.000000 tmticket-0.2.17/tmticket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.254469 tmticket-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-05-07 22:01:04.000000 tmticket-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:29.253469 tmticket-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-07 22:01:04.000000 tmticket-0.2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-08 00:06:29.254469 tmticket-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2024-05-08 00:06:04.000000 tmticket-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.250469 tmticket-0.2.2/tmticket/
+-rw-r--r--   0 root         (0) root         (0)      363 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5702 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/client.py
+-rw-r--r--   0 root         (0) root         (0)    13241 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/model.py
+-rw-r--r--   0 root         (0) root         (0)     4525 2024-05-08 00:06:04.000000 tmticket-0.2.2/tmticket/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-08 00:06:29.252469 tmticket-0.2.2/tmticket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      736 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      261 2024-05-08 00:06:29.000000 tmticket-0.2.2/tmticket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-08 00:06:28.000000 tmticket-0.2.2/tmticket.egg-info/top_level.txt
```

### Comparing `tmticket-0.2.17/tmticket/client.py` & `tmticket-0.2.2/tmticket/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 log.setLevel(logging.INFO)
 sh = logging.StreamHandler()
 sh.setLevel(logging.INFO)
 sf = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 sh.setFormatter(sf)
 log.addHandler(sh)
 
+
 class AsyncApiClient:
     """AsyncApiClient is the main wrapper for the Discovery API, updated for asynchronous operation.
     
     Example:    
     Get the first page result for venues matching keyword 'Tabernacle':
     
     ```
@@ -65,15 +66,14 @@
             'venues': self.__method_url('venues'),
             'attractions': self.__method_url('attractions'),
             'classifications': self.__method_url('classifications')
         }
 
         async with aiohttp.ClientSession() as session:
             async with session.get(urls[method], params=kwargs) as resp:
-                resp.raise_for_status()
                 return await self._handle_response(resp)
 
     async def _handle_response(self, response):
         """Handles response, raising ApiException if needed or returning response JSON object asynchronously"""
         if response.status == 200:
             return await response.json()
         elif response.status == 401:
@@ -84,15 +84,14 @@
             self.__unknown_error(await response.json())
 
     async def get_url(self, link):
         """Gets a specific href from '_links' object in a response, asynchronously"""
         parsed_link = self._parse_link(link)
         async with aiohttp.ClientSession() as session:
             async with session.get(parsed_link.url, params=parsed_link.params) as resp:
-                resp.raise_for_status()
                 return Page.from_json(await self._handle_response(resp))
 
     @property
     def api_key(self):
         return self.__api_key
 
     @api_key.setter
@@ -108,23 +107,25 @@
         s = str(s).lower()
         if s in ['true', 'yes']:
             s = 'yes'
         elif s in ['false', 'no']:
             s = 'no'
         return s
 
+
 class ApiException(Exception):
     """Exception thrown for API-related error messages"""
     def __init__(self, *args):
         super().__init__(*args)
 
 class AsyncPagedResponse:
     """Asynchronously iterates through API response pages."""
     def __init__(self, api_client, response):
         self.api_client = api_client
+        self.page = None
         self.page = Page.from_json(response)
 
     async def limit(self, max_pages=5):
         """Asynchronously retrieve a number of pages, returning a list of all entities."""
         all_items = []
         counter = 0
         async for pg in self:
```

### Comparing `tmticket-0.2.17/tmticket/model.py` & `tmticket-0.2.2/tmticket/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,15 @@
                 details_json = await response.json()
                 # Here you would process the details_json to extract and integrate additional details
                 print(details_json)  # Placeholder for actual logic
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+
 class Classification:
     """Classification object (segment/genre/sub-genre)"""
     def __init__(self, segment=None, classification_type=None, subtype=None, primary=None, links=None):
         self.segment = segment
         self.type = classification_type
         self.subtype = subtype
         self.primary = primary
@@ -259,31 +260,36 @@
 
         _assign_links(ec, json_obj)
         return ec
 
     def __str__(self):
         return f"Segment: {self.segment} / Genre: {self.genre} / Subgenre: {self.subgenre} / Type: {self.type} / Subtype: {self.subtype}"
 
+
 class ClassificationType:
     def __init__(self, type_id=None, type_name=None, subtypes=None):
         self.id = type_id
         self.name = type_name
         self.subtypes = subtypes
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# No changes needed here unless dynamic fetching of subtype details becomes necessary
+
 class ClassificationSubType:
     def __init__(self, type_id=None, type_name=None):
         self.id = type_id
         self.name = type_name
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Similar to ClassificationType, asynchronous behavior might be added for dynamic data fetching
+
 class Segment:
     def __init__(self, segment_id=None, segment_name=None, genres=None, links=None):
         self.id = segment_id
         self.name = segment_name
         self.genres = genres  # Could be a list of Genre instances
         self.links = links
 
@@ -298,14 +304,16 @@
             seg.genres = [Genre.from_json(g) for g in genres]
         _assign_links(seg, json_obj)
         return seg
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Could integrate asynchronous methods if genres require fetching additional details
+
 class Genre:
     def __init__(self, genre_id=None, genre_name=None, subgenres=None, links=None):
         self.id = genre_id
         self.name = genre_name
         self.subgenres = subgenres  # Could be a list of SubGenre instances
         self.links = links
 
@@ -319,14 +327,16 @@
             g.subgenres = [SubGenre.from_json(sg) for sg in subgenres]
         _assign_links(g, json_obj)
         return g
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
+# Asynchronous enhancements could be added for dynamic subgenre data fetching
+
 class SubGenre:
     def __init__(self, subgenre_id=None, subgenre_name=None, links=None):
         self.id = subgenre_id
         self.name = subgenre_name
         self.links = links
 
     @staticmethod
@@ -337,14 +347,14 @@
         _assign_links(sg, json_obj)
         return sg
 
     def __str__(self):
         return self.name if self.name is not None else 'Unknown'
 
 # Example async usage to fetch and process event details
-#async def main():
-#    event = Event.from_json({'id': '123', 'name': 'Sample Event', 'links': {'self': 'http://example.com/event/123'}})
-#    await event.fetch_additional_details()
-
-#if __name__ == '__main__':
-#    import asyncio
-#    asyncio.run(main())
+async def main():
+    event = Event.from_json({'id': '123', 'name': 'Sample Event', 'links': {'self': 'http://example.com/event/123'}})
+    await event.fetch_additional_details()
+
+if __name__ == '__main__':
+    import asyncio
+    asyncio.run(main())
```

### Comparing `tmticket-0.2.17/tmticket/query.py` & `tmticket-0.2.2/tmticket/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
         self.method = method
         self.model = model
 
     async def __get(self, **kwargs):
         """Asynchronously sends final request to `ApiClient`"""
         async with aiohttp.ClientSession() as session:
             async with session.get(f"{self.api_client.url}/{self.method}", params={**self.api_client.api_key, **kwargs}) as response:
-                response.raise_for_status()
                 return await response.json()
 
     async def _get(self, keyword=None, entity_id=None, sort=None, include_test=None, page=None, size=None, locale=None, **kwargs):
         """Asynchronously handles basic API search request"""
         search_args = {
             'keyword': keyword,
             'id': entity_id,
@@ -63,53 +62,66 @@
 
     async def by_id(self, entity_id):
         """Asynchronously get a specific object by its ID"""
         return await self._get(entity_id=entity_id)
 
     def _search_params(self, **kwargs):
         """Maps parameter names to API-friendly parameters"""
-        return {self.attr_map.get(k, k): v for k, v in kwargs.items() if v is not None}
+        kw_map = {}
+        for k, v in kwargs.items():
+            api_key = self.attr_map.get(k)
+            if api_key:
+                kw_map[api_key] = v
+            else:
+                kw_map[k] = v
+        return {k: v for k, v in kw_map.items() if v is not None}
 
 class AttractionQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'attractions', Attraction)
 
     async def find(self, **kwargs):
         return await self._get(**kwargs)
 
 class ClassificationQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'classifications', Classification)
 
-    async def find(self, **kwargs):
-        return await self._get(**kwargs)
 
-    async def segment_by_id(self, segment_id):
+    def segment_by_id(self, segment_id):
         """Return a ``Segment`` matching this ID"""
-        return (await self.by_id(segment_id)).segment
+        return self.by_id(segment_id).segment
 
-    async def genre_by_id(self, genre_id):
+    def genre_by_id(self, genre_id):
         """Return a ``Genre`` matching this ID"""
         genre = None
-        resp = await self.by_id(genre_id)
+        resp = self.by_id(genre_id)
         if resp.segment:
             for genre in resp.segment.genres:
                 if genre.id == genre_id:
-                    return genre
+                    genre = genre
         return genre
 
-    async def subgenre_by_id(self, subgenre_id):
+    def subgenre_by_id(self, subgenre_id):
         """Return a ``SubGenre`` matching this ID"""
-        segment = (await self.by_id(subgenre_id)).segment
+        subgenre = None
+        segment = self.by_id(subgenre_id).segment
         if segment:
-            for genre in segment.genres:
-                for subg in genre.subgenres:
-                    if subg.id == subgenre_id:
-                        return subg
-        return None
+            subgenres = [
+                subg for genre in segment.genres
+                for subg in genre.subgenres
+            ]
+            for subg in subgenres:
+                if subg.id == subgenre_id:
+                    subgenre = subg
+        return subgenre
+
+
+    async def find(self, **kwargs):
+        return await self._get(**kwargs)
 
 class EventQuery(BaseQuery):
     def __init__(self, api_client):
         super().__init__(api_client, 'events', Event)
 
     async def find(self, **kwargs):
         return await self._get(**kwargs)
```

