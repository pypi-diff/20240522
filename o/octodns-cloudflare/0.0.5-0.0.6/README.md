# Comparing `tmp/octodns_cloudflare-0.0.5.tar.gz` & `tmp/octodns_cloudflare-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns_cloudflare-0.0.5.tar", last modified: Mon Apr 15 14:24:27 2024, max compression
+gzip compressed data, was "octodns_cloudflare-0.0.6.tar", last modified: Wed May 22 19:31:55 2024, max compression
```

## Comparing `octodns_cloudflare-0.0.5.tar` & `octodns_cloudflare-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.327114 octodns_cloudflare-0.0.5/
--rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:28.000000 octodns_cloudflare-0.0.5/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     6709 2024-04-15 14:24:27.325736 octodns_cloudflare-0.0.5/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     5654 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.307160 octodns_cloudflare-0.0.5/octodns_cloudflare/
--rw-r--r--   0 ross       (501) staff       (20)    40769 2024-04-15 14:24:19.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.316381 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/
--rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)     2632 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/proxycname.py
--rw-r--r--   0 ross       (501) staff       (20)     1145 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/ttl.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.320279 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     6709 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      562 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      246 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       19 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      431 2023-11-29 21:54:17.000000 octodns_cloudflare-0.0.5/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-15 14:24:27.327378 octodns_cloudflare-0.0.5/setup.cfg
--rwxr-xr-x   0 ross       (501) staff       (20)     1661 2024-03-21 02:14:57.000000 octodns_cloudflare-0.0.5/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.319384 octodns_cloudflare-0.0.5/tests/
--rw-r--r--   0 ross       (501) staff       (20)    98587 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare.py
--rw-r--r--   0 ross       (501) staff       (20)     4631 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_proxycname.py
--rw-r--r--   0 ross       (501) staff       (20)     1670 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_ttl.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-22 19:31:55.373857 octodns_cloudflare-0.0.6/
+-rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:28.000000 octodns_cloudflare-0.0.6/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     6757 2024-05-22 19:31:55.372613 octodns_cloudflare-0.0.6/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     5654 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.6/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-22 19:31:55.363735 octodns_cloudflare-0.0.6/octodns_cloudflare/
+-rw-r--r--   0 ross       (501) staff       (20)    41911 2024-05-22 19:31:46.000000 octodns_cloudflare-0.0.6/octodns_cloudflare/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-22 19:31:55.367743 octodns_cloudflare-0.0.6/octodns_cloudflare/processor/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.6/octodns_cloudflare/processor/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     2632 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.6/octodns_cloudflare/processor/proxycname.py
+-rw-r--r--   0 ross       (501) staff       (20)     1145 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.6/octodns_cloudflare/processor/ttl.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-22 19:31:55.369779 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     6757 2024-05-22 19:31:55.000000 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      562 2024-05-22 19:31:55.000000 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-05-22 19:31:55.000000 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      263 2024-05-22 19:31:55.000000 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       19 2024-05-22 19:31:55.000000 octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      431 2023-11-29 21:54:17.000000 octodns_cloudflare-0.0.6/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-05-22 19:31:55.374509 octodns_cloudflare-0.0.6/setup.cfg
+-rwxr-xr-x   0 ross       (501) staff       (20)     1826 2024-04-17 17:53:55.000000 octodns_cloudflare-0.0.6/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-05-22 19:31:55.369258 octodns_cloudflare-0.0.6/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    98587 2024-05-22 19:27:42.000000 octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare.py
+-rw-r--r--   0 ross       (501) staff       (20)     4631 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare_processor_proxycname.py
+-rw-r--r--   0 ross       (501) staff       (20)     1670 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare_processor_ttl.py
```

### Comparing `octodns_cloudflare-0.0.5/LICENSE` & `octodns_cloudflare-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/PKG-INFO` & `octodns_cloudflare-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-cloudflare
-Version: 0.0.5
+Version: 0.0.6
 Summary:  Cloudflare provider for octoDNS
 Home-page: https://github.com/octodns/octodns-cloudflare
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
 Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `octodns_cloudflare-0.0.5/README.md` & `octodns_cloudflare-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/octodns_cloudflare/__init__.py` & `octodns_cloudflare-0.0.6/octodns_cloudflare/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from octodns import __VERSION__ as octodns_version
 from octodns.idna import IdnaDict
 from octodns.provider import ProviderException, SupportsException
 from octodns.provider.base import BaseProvider
 from octodns.record import Create, Record, Update
 
 # TODO: remove __VERSION__ with the next major version release
-__version__ = __VERSION__ = '0.0.5'
+__version__ = __VERSION__ = '0.0.6'
 
 
 class CloudflareError(ProviderException):
     def __init__(self, data):
         try:
             message = data['errors'][0]['message']
         except (IndexError, KeyError, TypeError):
@@ -47,14 +47,15 @@
     SUPPORTS = set(
         (
             'ALIAS',
             'A',
             'AAAA',
             'CAA',
             'CNAME',
+            'DS',
             'LOC',
             'MX',
             'NAPTR',
             'NS',
             'PTR',
             'SSHFP',
             'SRV',
@@ -238,14 +239,34 @@
             'type': _type,
             'value': f'{only["content"]}.' if only['content'] != '.' else '.',
         }
 
     _data_for_ALIAS = _data_for_CNAME
     _data_for_PTR = _data_for_CNAME
 
+    def _data_for_DS(self, _type, records):
+        values = []
+        for record in records:
+            key_tag, algorithm, digest_type, digest = record['content'].split(
+                ' ', 3
+            )
+            values.append(
+                {
+                    'algorithm': int(algorithm),
+                    'digest': digest,
+                    'digest_type': digest_type,
+                    'key_tag': int(key_tag),
+                }
+            )
+        return {
+            'type': _type,
+            'values': values,
+            'ttl': self._ttl_data(records[0]['ttl']),
+        }
+
     def _data_for_LOC(self, _type, records):
         values = []
         for record in records:
             r = record['data']
             values.append(
                 {
                     'lat_degrees': int(r['lat_degrees']),
@@ -398,15 +419,20 @@
             page = 1
             while page:
                 resp = self._try_request(
                     'GET',
                     path,
                     params={'page': page, 'per_page': self.records_per_page},
                 )
-                records += resp['result']
+                # populate DNS records, ensure only supported types are considered
+                records += [
+                    record
+                    for record in resp['result']
+                    if record['type'] in self.SUPPORTS
+                ]
                 info = resp['result_info']
                 if info['count'] > 0 and info['count'] == info['per_page']:
                     page += 1
                 else:
                     page = None
             if self.pagerules:
                 path = f'/zones/{zone_id}/pagerules'
@@ -504,16 +530,15 @@
                     _values['ttl'] = 300
                     values[name][_type].append(_values)
                 # the dns_records branch
                 # elif 'name' in record:
                 else:
                     name = zone.hostname_from_fqdn(record['name'])
                     _type = record['type']
-                    if _type in self.SUPPORTS:
-                        values[name][record['type']].append(record)
+                    values[name][record['type']].append(record)
 
             for name, types in values.items():
                 for _type, records in types.items():
                     record = self._record_for(
                         zone, name, _type, records, lenient
                     )
 
@@ -608,14 +633,25 @@
                 'data': {
                     'flags': value.flags,
                     'tag': value.tag,
                     'value': value.value,
                 }
             }
 
+    def _contents_for_DS(self, record):
+        for value in record.values:
+            yield {
+                'data': {
+                    'key_tag': value.key_tag,
+                    'algorithm': value.algorithm,
+                    'digest_type': value.digest_type,
+                    'digest': value.digest,
+                }
+            }
+
     def _contents_for_TXT(self, record):
         for value in record.values:
             yield {'content': value.replace('\\;', ';')}
 
     def _contents_for_CNAME(self, record):
         yield {'content': record.value}
```

### Comparing `octodns_cloudflare-0.0.5/octodns_cloudflare/processor/proxycname.py` & `octodns_cloudflare-0.0.6/octodns_cloudflare/processor/proxycname.py`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/octodns_cloudflare/processor/ttl.py` & `octodns_cloudflare-0.0.6/octodns_cloudflare/processor/ttl.py`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/PKG-INFO` & `octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-cloudflare
-Version: 0.0.5
+Version: 0.0.6
 Summary:  Cloudflare provider for octoDNS
 Home-page: https://github.com/octodns/octodns-cloudflare
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -14,14 +14,15 @@
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
 Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
+Requires-Dist: docutils<=0.20.1; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
```

### Comparing `octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/SOURCES.txt` & `octodns_cloudflare-0.0.6/octodns_cloudflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/setup.py` & `octodns_cloudflare-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         + (
             # we need to manually/explicitely bump major versions as they're
             # likely to result in formatting changes that should happen in their
             # own PR. This will basically happen yearly
             # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
             'black>=24.3.0,<25.0.0',
             'build>=0.7.0',
+            # docutils 0.21.x bumped to >=3.9 and 3.8 is still active. we'll
+            # have to clamp it down until we remove 3.8
+            'docutils<=0.20.1',
             'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
     },
```

### Comparing `octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare.py` & `octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 00001f90: 6561 6428 2929 0a0a 2020 2020 2020 2020  ead())..        
 00001fa0: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
 00001fb0: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
 00001fc0: 5d29 0a20 2020 2020 2020 2020 2020 2070  ]).            p
 00001fd0: 726f 7669 6465 722e 706f 7075 6c61 7465  rovider.populate
 00001fe0: 287a 6f6e 6529 0a20 2020 2020 2020 2020  (zone).         
 00001ff0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00002000: 7561 6c28 3232 2c20 6c65 6e28 7a6f 6e65  ual(22, len(zone
+00002000: 7561 6c28 3233 2c20 6c65 6e28 7a6f 6e65  ual(23, len(zone
 00002010: 2e72 6563 6f72 6473 2929 0a0a 2020 2020  .records))..    
 00002020: 2020 2020 2020 2020 6368 616e 6765 7320          changes 
 00002030: 3d20 7365 6c66 2e65 7870 6563 7465 642e  = self.expected.
 00002040: 6368 616e 6765 7328 7a6f 6e65 2c20 7072  changes(zone, pr
 00002050: 6f76 6964 6572 290a 0a20 2020 2020 2020  ovider)..       
 00002060: 2020 2020 2023 2064 656c 6574 6520 6120       # delete a 
 00002070: 7572 6c66 7764 2c20 6372 6561 7465 2033  urlfwd, create 3
@@ -529,15 +529,15 @@
 00002100: 206f 6620 6361 6368 652c 206e 6f20 6361   of cache, no ca
 00002110: 6c6c 730a 2020 2020 2020 2020 6167 6169  lls.        agai
 00002120: 6e20 3d20 5a6f 6e65 2827 756e 6974 2e74  n = Zone('unit.t
 00002130: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
 00002140: 2020 2020 7072 6f76 6964 6572 2e70 6f70      provider.pop
 00002150: 756c 6174 6528 6167 6169 6e29 0a20 2020  ulate(again).   
 00002160: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002170: 4571 7561 6c28 3232 2c20 6c65 6e28 6167  Equal(22, len(ag
+00002170: 4571 7561 6c28 3233 2c20 6c65 6e28 6167  Equal(23, len(ag
 00002180: 6169 6e2e 7265 636f 7264 7329 290a 0a20  ain.records)).. 
 00002190: 2020 2064 6566 2074 6573 745f 6170 706c     def test_appl
 000021a0: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
 000021b0: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
 000021c0: 6466 6c61 7265 5072 6f76 6964 6572 280a  dflareProvider(.
 000021d0: 2020 2020 2020 2020 2020 2020 2774 6573              'tes
 000021e0: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
@@ -553,27 +553,27 @@
 00002280: 2073 656c 662e 656d 7074 792c 2020 2320   self.empty,  # 
 00002290: 6e6f 207a 6f6e 6573 0a20 2020 2020 2020  no zones.       
 000022a0: 2020 2020 207b 2772 6573 756c 7427 3a20       {'result': 
 000022b0: 7b27 6964 273a 2034 327d 7d2c 2020 2320  {'id': 42}},  # 
 000022c0: 7a6f 6e65 2063 7265 6174 650a 2020 2020  zone create.    
 000022d0: 2020 2020 5d20 2b20 5b0a 2020 2020 2020      ] + [.      
 000022e0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
-000022f0: 2020 205d 202a 2033 3020 2023 2069 6e64     ] * 30  # ind
+000022f0: 2020 205d 202a 2033 3120 2023 2069 6e64     ] * 31  # ind
 00002300: 6976 6964 7561 6c20 7265 636f 7264 2063  ividual record c
 00002310: 7265 6174 6573 0a0a 2020 2020 2020 2020  reates..        
 00002320: 2320 6e6f 6e2d 6578 6973 7465 6e74 207a  # non-existent z
 00002330: 6f6e 652c 2063 7265 6174 6520 6576 6572  one, create ever
 00002340: 7974 6869 6e67 0a20 2020 2020 2020 2070  ything.        p
 00002350: 6c61 6e20 3d20 7072 6f76 6964 6572 2e70  lan = provider.p
 00002360: 6c61 6e28 7365 6c66 2e65 7870 6563 7465  lan(self.expecte
 00002370: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00002380: 6173 7365 7274 4571 7561 6c28 3138 2c20  assertEqual(18, 
+00002380: 6173 7365 7274 4571 7561 6c28 3139 2c20  assertEqual(19, 
 00002390: 6c65 6e28 706c 616e 2e63 6861 6e67 6573  len(plan.changes
 000023a0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-000023b0: 6173 7365 7274 4571 7561 6c28 3138 2c20  assertEqual(18, 
+000023b0: 6173 7365 7274 4571 7561 6c28 3139 2c20  assertEqual(19, 
 000023c0: 7072 6f76 6964 6572 2e61 7070 6c79 2870  provider.apply(p
 000023d0: 6c61 6e29 290a 2020 2020 2020 2020 7365  lan)).        se
 000023e0: 6c66 2e61 7373 6572 7446 616c 7365 2870  lf.assertFalse(p
 000023f0: 6c61 6e2e 6578 6973 7473 290a 0a20 2020  lan.exists)..   
 00002400: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
 00002410: 6571 7565 7374 2e61 7373 6572 745f 6861  equest.assert_ha
 00002420: 735f 6361 6c6c 7328 0a20 2020 2020 2020  s_calls(.       
@@ -713,15 +713,15 @@
 00002c80: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
 00002c90: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
 00002ca0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
 00002cb0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
 00002cc0: 2020 2023 2065 7870 6563 7465 6420 6e75     # expected nu
 00002cd0: 6d62 6572 206f 6620 746f 7461 6c20 6361  mber of total ca
 00002ce0: 6c6c 730a 2020 2020 2020 2020 7365 6c66  lls.        self
-00002cf0: 2e61 7373 6572 7445 7175 616c 2833 322c  .assertEqual(32,
+00002cf0: 2e61 7373 6572 7445 7175 616c 2833 332c  .assertEqual(33,
 00002d00: 2070 726f 7669 6465 722e 5f72 6571 7565   provider._reque
 00002d10: 7374 2e63 616c 6c5f 636f 756e 7429 0a0a  st.call_count)..
 00002d20: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
 00002d30: 2e5f 7265 7175 6573 742e 7265 7365 745f  ._request.reset_
 00002d40: 6d6f 636b 2829 0a0a 2020 2020 2020 2020  mock()..        
 00002d50: 7072 6f76 6964 6572 2e7a 6f6e 655f 7265  provider.zone_re
 00002d60: 636f 7264 7320 3d20 4d6f 636b 280a 2020  cords = Mock(.  
@@ -1279,27 +1279,27 @@
 00004fe0: 7074 792c 2020 2320 6e6f 207a 6f6e 6573  pty,  # no zones
 00004ff0: 0a20 2020 2020 2020 2020 2020 207b 2772  .            {'r
 00005000: 6573 756c 7427 3a20 7b27 6964 273a 2034  esult': {'id': 4
 00005010: 327d 7d2c 2020 2320 7a6f 6e65 2063 7265  2}},  # zone cre
 00005020: 6174 650a 2020 2020 2020 2020 5d20 2b20  ate.        ] + 
 00005030: 5b0a 2020 2020 2020 2020 2020 2020 4e6f  [.            No
 00005040: 6e65 0a20 2020 2020 2020 205d 202a 2033  ne.        ] * 3
-00005050: 3020 2023 2069 6e64 6976 6964 7561 6c20  0  # individual 
+00005050: 3120 2023 2069 6e64 6976 6964 7561 6c20  1  # individual 
 00005060: 7265 636f 7264 2063 7265 6174 6573 0a0a  record creates..
 00005070: 2020 2020 2020 2020 2320 6e6f 6e2d 6578          # non-ex
 00005080: 6973 7465 6e74 207a 6f6e 652c 2063 7265  istent zone, cre
 00005090: 6174 6520 6576 6572 7974 6869 6e67 0a20  ate everything. 
 000050a0: 2020 2020 2020 2070 6c61 6e20 3d20 7072         plan = pr
 000050b0: 6f76 6964 6572 2e70 6c61 6e28 7365 6c66  ovider.plan(self
 000050c0: 2e65 7870 6563 7465 6429 0a20 2020 2020  .expected).     
 000050d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000050e0: 7561 6c28 3138 2c20 6c65 6e28 706c 616e  ual(18, len(plan
+000050e0: 7561 6c28 3139 2c20 6c65 6e28 706c 616e  ual(19, len(plan
 000050f0: 2e63 6861 6e67 6573 2929 0a20 2020 2020  .changes)).     
 00005100: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00005110: 7561 6c28 3138 2c20 7072 6f76 6964 6572  ual(18, provider
+00005110: 7561 6c28 3139 2c20 7072 6f76 6964 6572  ual(19, provider
 00005120: 2e61 7070 6c79 2870 6c61 6e29 290a 2020  .apply(plan)).  
 00005130: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
 00005140: 7446 616c 7365 2870 6c61 6e2e 6578 6973  tFalse(plan.exis
 00005150: 7473 290a 0a20 2020 2020 2020 2070 726f  ts)..        pro
 00005160: 7669 6465 722e 5f72 6571 7565 7374 2e61  vider._request.a
 00005170: 7373 6572 745f 6861 735f 6361 6c6c 7328  ssert_has_calls(
 00005180: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
@@ -1448,15 +1448,15 @@
 00005a70: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
 00005a80: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
 00005a90: 2020 2020 2020 2020 2054 7275 652c 0a20           True,. 
 00005aa0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 00005ab0: 2023 2065 7870 6563 7465 6420 6e75 6d62   # expected numb
 00005ac0: 6572 206f 6620 746f 7461 6c20 6361 6c6c  er of total call
 00005ad0: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
-00005ae0: 7373 6572 7445 7175 616c 2833 322c 2070  ssertEqual(32, p
+00005ae0: 7373 6572 7445 7175 616c 2833 332c 2070  ssertEqual(33, p
 00005af0: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
 00005b00: 2e63 616c 6c5f 636f 756e 7429 0a0a 2020  .call_count)..  
 00005b10: 2020 6465 6620 7465 7374 5f75 7064 6174    def test_updat
 00005b20: 655f 6164 645f 7377 6170 2873 656c 6629  e_add_swap(self)
 00005b30: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
 00005b40: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
 00005b50: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
@@ -5385,15 +5385,15 @@
 00015080: 6875 622d 7a73 612e 636f 6d2e 600a 2020  hub-zsa.com.`.  
 00015090: 2020 2020 2020 2020 2020 7a6f 6e65 203d            zone =
 000150a0: 205a 6f6e 6528 2767 c3ad 7468 7562 2e63   Zone('g..thub.c
 000150b0: 6f6d 2e27 2c20 5b5d 290a 2020 2020 2020  om.', []).      
 000150c0: 2020 2020 2020 7072 6f76 6964 6572 2e70        provider.p
 000150d0: 6f70 756c 6174 6528 7a6f 6e65 290a 2020  opulate(zone).  
 000150e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-000150f0: 7445 7175 616c 2838 2c20 6c65 6e28 7a6f  tEqual(8, len(zo
+000150f0: 7445 7175 616c 2839 2c20 6c65 6e28 7a6f  tEqual(9, len(zo
 00015100: 6e65 2e72 6563 6f72 6473 2929 0a20 2020  ne.records)).   
 00015110: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
 00015120: 4571 7561 6c28 7a6f 6e65 2e6e 616d 652c  Equal(zone.name,
 00015130: 2069 646e 615f 656e 636f 6465 2827 67c3   idna_encode('g.
 00015140: ad74 6875 622e 636f 6d2e 2729 290a 0a20  .thub.com.')).. 
 00015150: 2020 2064 6566 2074 6573 745f 6163 636f     def test_acco
 00015160: 756e 745f 6964 5f66 696c 7465 7228 7365  unt_id_filter(se
```

### Comparing `octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_proxycname.py` & `octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare_processor_proxycname.py`

 * *Files identical despite different names*

### Comparing `octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_ttl.py` & `octodns_cloudflare-0.0.6/tests/test_octodns_provider_cloudflare_processor_ttl.py`

 * *Files identical despite different names*

