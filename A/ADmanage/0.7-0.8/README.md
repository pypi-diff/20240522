# Comparing `tmp/admanage-0.7.tar.gz` & `tmp/admanage-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "admanage-0.7.tar", last modified: Sun May 12 16:52:25 2024, max compression
+gzip compressed data, was "admanage-0.8.tar", last modified: Wed May 22 19:46:37 2024, max compression
```

## Comparing `admanage-0.7.tar` & `admanage-0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.467577 admanage-0.7/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.444335 admanage-0.7/ADmanage/
--rw-rw-rw-   0        0        0    13798 2024-05-12 16:51:46.000000 admanage-0.7/ADmanage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:52:25.463881 admanage-0.7/ADmanage.egg-info/
--rw-rw-rw-   0        0        0     7702 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-12 16:52:25.000000 admanage-0.7/ADmanage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7702 2024-05-12 16:52:25.467577 admanage-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7557 2024-05-12 16:50:02.000000 admanage-0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 16:52:25.467577 admanage-0.7/setup.cfg
--rw-rw-rw-   0        0        0      363 2024-05-12 16:50:49.000000 admanage-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:46:37.689095 admanage-0.8/
+drwxrwxrwx   0        0        0        0 2024-05-22 19:46:37.657838 admanage-0.8/ADmanage/
+-rw-rw-rw-   0        0        0    13926 2024-05-22 19:42:55.000000 admanage-0.8/ADmanage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:46:37.689095 admanage-0.8/ADmanage.egg-info/
+-rw-rw-rw-   0        0        0     7702 2024-05-22 19:46:37.000000 admanage-0.8/ADmanage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2024-05-22 19:46:37.000000 admanage-0.8/ADmanage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 19:46:37.000000 admanage-0.8/ADmanage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 19:46:37.000000 admanage-0.8/ADmanage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 19:46:37.000000 admanage-0.8/ADmanage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7702 2024-05-22 19:46:37.689095 admanage-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7557 2024-05-22 19:40:17.000000 admanage-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 19:46:37.689095 admanage-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      363 2024-05-22 19:45:27.000000 admanage-0.8/setup.py
```

### Comparing `admanage-0.7/ADmanage/__init__.py` & `admanage-0.8/ADmanage/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 import ldap3
-from ldap3 import Server, Connection, ALL, SUBTREE, MODIFY_ADD, MODIFY_DELETE, MODIFY_REPLACE, NTLM
+from ldap3 import Server, Connection, ALL, SUBTREE, MODIFY_ADD, MODIFY_DELETE, MODIFY_REPLACE, NTLM, SIMPLE
 from impacket.structure import Structure
 import socket
 import dns.resolver
 import datetime
 import json
 
 class ADclient:
     def __init__(self, domain, username, password, hashes, dc_ip, base_dn=None, secure=False):
         self.domain = domain
         self.username = username
-        self.sam = f"{domain}\\{username}"
+        self.sam = f"{domain.split('.')[0]}\\{username}"
         self.password = password or hashes
         self.dc_ip = dc_ip
         self.base_dn = base_dn
         self.secure = secure
         self.domain_root = f"DC={domain.split('.')[0]},DC={domain.split('.')[1]}"
         self.dnsroot = f"DC={domain},CN=MicrosoftDNS,DC=DomainDnsZones,{self.domain_root}"
         self.conn = self.connect_to_ldap()
 
     def connect_to_ldap(self):
-        dc_url = f"ldaps://{self.dc_ip}:636" if self.secure else f"ldap://{self.dc_ip}:389"
+        dc_url = f"ldap://{self.dc_ip}:389"
+        auth = NTLM
+        if self.secure:
+            auth = SIMPLE
+            dc_url = f"ldaps://{self.dc_ip}:636"
+        
         if not self.base_dn:
             self.base_dn = self.domain_root
 
-        server = Server(dc_url, get_info=ALL)
-        conn = Connection(server, user=self.sam, password=self.password, authentication=NTLM, auto_bind=True)
+        server = Server(dc_url, use_ssl=self.secure, get_info=ALL)
+        conn = Connection(server, user=self.sam, password=self.password, authentication=auth, auto_bind=True)
         return conn
 
     def disconnect(self):
         self.conn.unbind()
 
     class DNS_RECORD(Structure):
         """
```

### Comparing `admanage-0.7/ADmanage.egg-info/PKG-INFO` & `admanage-0.8/ADmanage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADmanage
-Version: 0.7
+Version: 0.8
 Description-Content-Type: text/markdown
 Requires-Dist: ldap3
 Requires-Dist: impacket
 
 # ADmanage
 
 The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
```

### Comparing `admanage-0.7/PKG-INFO` & `admanage-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ADmanage
-Version: 0.7
+Version: 0.8
 Description-Content-Type: text/markdown
 Requires-Dist: ldap3
 Requires-Dist: impacket
 
 # ADmanage
 
 The provided script is a Python program that interacts with an Active Directory (AD) server using the LDAP protocol. It allows you to perform various operations on DNS entries and AD objects (users, groups and computers).
```

### Comparing `admanage-0.7/README.md` & `admanage-0.8/README.md`

 * *Files identical despite different names*

