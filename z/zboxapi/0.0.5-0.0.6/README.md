# Comparing `tmp/zboxapi-0.0.5.tar.gz` & `tmp/zboxapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zboxapi-0.0.5.tar", max compression
+gzip compressed data, was "zboxapi-0.0.6.tar", max compression
```

## Comparing `zboxapi-0.0.5.tar` & `zboxapi-0.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      545 2024-05-10 20:21:05.312952 zboxapi-0.0.5/README.md
--rw-r--r--   0        0        0      896 2024-05-20 15:35:20.449504 zboxapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-20 15:35:20.457504 zboxapi-0.0.5/src/zboxapi/__init__.py
--rw-r--r--   0        0        0     7305 2024-05-17 13:55:19.421135 zboxapi-0.0.5/src/zboxapi/main.py
--rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      545 2024-05-10 20:21:05.312952 zboxapi-0.0.6/README.md
+-rw-r--r--   0        0        0      896 2024-05-22 19:01:17.258256 zboxapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-22 19:01:17.262256 zboxapi-0.0.6/src/zboxapi/__init__.py
+-rw-r--r--   0        0        0     7288 2024-05-21 17:26:55.296032 zboxapi-0.0.6/src/zboxapi/main.py
+-rw-r--r--   0        0        0     1043 1970-01-01 00:00:00.000000 zboxapi-0.0.6/PKG-INFO
```

### Comparing `zboxapi-0.0.5/README.md` & `zboxapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `zboxapi-0.0.5/pyproject.toml` & `zboxapi-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zboxapi"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["Kelby Valenti <kelby.valenti@gmail.com>", "Timo Sugliani <timo.sugliani@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 zboxapi = "zboxapi.main:launch"
```

### Comparing `zboxapi-0.0.5/src/zboxapi/main.py` & `zboxapi-0.0.6/src/zboxapi/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,38 +45,40 @@
 
 def get_hosts_lines(hosts_fo: IO) -> list[dict[str, str]]:
     lines = []
     for line in hosts_fo.read().splitlines():
         line = line.strip()
         if not line or line.startswith("#"):
             continue
-        line_ip, *line_fqdns = line.split()
+        line_ip, *line_hostnames = line.split()
         lines.extend(
-            {"ip": IPv4Address(line_ip), "fqdn": line_fqdn} for line_fqdn in line_fqdns
+            {"ip": IPv4Address(line_ip), "hostname": line_hostname}
+            for line_hostname in line_hostnames
         )
     return sorted(lines, key=sort_hosts_lines)
 
 
 def filter_hosts_file(
     lines: list[dict[str, str]],
     ip: IPv4Address | None = None,
-    fqdn: str | None = None,
+    hostname: str | None = None,
 ):
     return [
         line
         for line in lines
-        if (not ip or ip == line["ip"]) and (not fqdn or fqdn == line["fqdn"])
+        if (not ip or ip == line["ip"])
+        and (not hostname or hostname == line["hostname"])
     ]
 
 
 def write_hosts_file(hosts_fo: IO, lines: list[dict[str, str]]):
     lines.sort(key=sort_hosts_lines)
     hosts_fo.seek(0)
     hosts_fo.truncate()
-    hosts_fo.writelines([f"{line['ip']}\t{line['fqdn']}\n" for line in lines])
+    hosts_fo.writelines([f"{line['ip']}\t{line['hostname']}\n" for line in lines])
 
 
 def validate_api_key(api_key: Annotated[APIKey, Security(api_key_header)]):
     if api_key != ZPOD_PASSWORD:
         raise HTTPException(
             status_code=status.HTTP_403_FORBIDDEN,
             detail="Invalid access_token",
@@ -97,162 +99,151 @@
 
 def dnsmasq_sighup():
     print("Send SIGHUP to dnsmasq...")
     subprocess.call(["pkill", "-SIGHUP", "dnsmasq"])
 
 
 def sort_hosts_lines(item: dict):
-    """Sort list by loopback first, ip second, fqdn third"""
+    """Sort list by loopback first, ip second, hostname third"""
     return (
         not item["ip"].is_loopback,
         socket.inet_aton(str(item["ip"])),
-        item["fqdn"],
+        item["hostname"],
     )
 
 
 def simplify_operation_ids(api: FastAPI) -> None:
     """
     Update operation IDs so that generated API clients have simpler function
     names.
     """
     for route in api.routes:
         if isinstance(route, APIRoute) and not route.operation_id:
             tag = route.tags[0] if route.tags else "default"
             route.operation_id = f"{tag}_{route.name}"
 
 
-def RecordNotFound(ip, fqdn):
+def RecordNotFound(ip, hostname):
     return HTTPException(
         status_code=status.HTTP_404_NOT_FOUND,
-        detail=f"DNS record not found: ip={ip}, fqdn={fqdn}",
+        detail=f"DNS record not found: ip={ip}, hostname={hostname}",
     )
 
 
-def RecordAlreadyPresent(ip, fqdn):
+def RecordAlreadyPresent(ip, hostname):
     return HTTPException(
         status_code=status.HTTP_406_NOT_ACCEPTABLE,
-        detail=f"DNS record already present: ip={ip}, fqdn={fqdn}",
+        detail=f"DNS record already present: ip={ip}, hostname={hostname}",
     )
 
 
-def validate_fqdn(value: str):
-    """
-    https://en.m.wikipedia.org/wiki/Fully_qualified_domain_name
-    """
-
-    if not 1 < len(value) < 253:
-        raise PydanticCustomError("value_error", "Invalid fqdn length")
-
-    # Remove trailing dot
-    if value[-1] == ".":
-        value = value[:-1]
-
-    #  Split hostname into list of DNS labels
-    labels = value.split(".")
+def validate_hostname(value: str):
+    if not 1 < len(value) < 64:
+        raise PydanticCustomError("value_error", "Invalid hostname length")
 
     #  Define pattern of DNS label
     #  Can begin and end with a number or letter only
     #  Can contain hyphens, a-z, A-Z, 0-9
     #  1 - 63 chars allowed
-    fqdn = re.compile(r"^[a-z0-9]([a-z-0-9-]{0,61}[a-z0-9])?$", re.IGNORECASE)
+    hostname_re = re.compile(r"^[a-z0-9]([a-z-0-9-]{0,61}[a-z0-9])?$", re.IGNORECASE)
 
     # Check that all labels match that pattern.
-    if not all(fqdn.match(label) for label in labels):
-        raise PydanticCustomError("value_error", "Invalid fqdn")
+    if not hostname_re.match(value):
+        raise PydanticCustomError("value_error", "Invalid hostname")
     return value
 
 
-FQDN = Annotated[str, AfterValidator(validate_fqdn)]
+HOSTNAME = Annotated[str, AfterValidator(validate_hostname)]
 
 
 class DnsCreate(BaseModel):
     ip: IPv4Address
-    fqdn: FQDN
+    hostname: HOSTNAME
 
 
 class DnsDelete(BaseModel):
     ip: IPv4Address
-    fqdn: FQDN
+    hostname: HOSTNAME
 
 
 class DnsUpdate(BaseModel):
     ip: IPv4Address
-    fqdn: FQDN
+    hostname: HOSTNAME
 
 
 class DnsView(BaseModel):
     ip: IPv4Address
-    fqdn: str
+    hostname: str
 
 
 dns_router = APIRouter(prefix="/dns", tags=["dns"])
 
 
 @dns_router.get("")
 def dns_get_all() -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
     return hosts_lines
 
 
-@dns_router.get("/{ip}/{fqdn}")
+@dns_router.get("/{ip}/{hostname}")
 def dns_get(
     ip: IPv4Address,
-    fqdn: FQDN,
+    hostname: HOSTNAME,
 ) -> DnsView:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        hosts_lines = filter_hosts_file(hosts_lines, ip, fqdn)
+        hosts_lines = filter_hosts_file(hosts_lines, ip, hostname)
     if not hosts_lines:
-        raise RecordNotFound(ip, fqdn)
+        raise RecordNotFound(ip, hostname)
     return hosts_lines[0]
 
 
 @dns_router.post("")
 def dns_add(
     dns_in: DnsCreate,
 ) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        if filter_hosts_file(hosts_lines, dns_in.ip, dns_in.fqdn):
-            raise RecordAlreadyPresent(dns_in.ip, dns_in.fqdn)
-        hosts_lines.append({"ip": dns_in.ip, "fqdn": dns_in.fqdn})
+        if filter_hosts_file(hosts_lines, dns_in.ip, dns_in.hostname):
+            raise RecordAlreadyPresent(dns_in.ip, dns_in.hostname)
+        hosts_lines.append({"ip": dns_in.ip, "hostname": dns_in.hostname})
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
-@dns_router.put("/{ip}/{fqdn}")
+@dns_router.put("/{ip}/{hostname}")
 def dns_update(
     ip: IPv4Address,
-    fqdn: FQDN,
+    hostname: HOSTNAME,
     dns_in: DnsUpdate,
 ) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        key = {"ip": ip, "fqdn": fqdn}
+        key = {"ip": ip, "hostname": hostname}
         if key not in hosts_lines:
-            raise RecordNotFound(ip, fqdn)
+            raise RecordNotFound(ip, hostname)
         ix = hosts_lines.index(key)
-        hosts_lines[ix] = {"ip": dns_in.ip, "fqdn": dns_in.fqdn}
+        hosts_lines[ix] = {"ip": dns_in.ip, "hostname": dns_in.hostname}
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
-@dns_router.delete("/{ip}/{fqdn}")
+@dns_router.delete("/{ip}/{hostname}")
 def dns_delete(
     ip: IPv4Address,
-    fqdn: FQDN,
+    hostname: HOSTNAME,
 ) -> list[DnsView]:
     with get_hosts_file_object() as hosts_fo:
         hosts_lines = get_hosts_lines(hosts_fo)
-        key = {"ip": ip, "fqdn": fqdn}
+        key = {"ip": ip, "hostname": hostname}
         if key not in hosts_lines:
-            raise RecordNotFound(ip, fqdn)
+            raise RecordNotFound(ip, hostname)
         hosts_lines.remove(key)
         write_hosts_file(hosts_fo, hosts_lines)
     dnsmasq_sighup()
     return hosts_lines
 
 
 zboxapi_root_path = os.getenv("ZBOXAPI_ROOT_PATH", None)
```

### Comparing `zboxapi-0.0.5/PKG-INFO` & `zboxapi-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zboxapi
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: Kelby Valenti
 Author-email: kelby.valenti@gmail.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

