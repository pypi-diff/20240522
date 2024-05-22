# Comparing `tmp/PFlowC-2.3.0.tar.gz` & `tmp/PFlowC-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-2.3.0.tar", last modified: Fri May 10 05:04:32 2024, max compression
+gzip compressed data, was "PFlowC-2.4.0.tar", last modified: Mon May 20 02:52:30 2024, max compression
```

## Comparing `PFlowC-2.3.0.tar` & `PFlowC-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.462128 PFlowC-2.3.0/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.433350 PFlowC-2.3.0/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 05:03:01.000000 PFlowC-2.3.0/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3055 2024-05-10 05:00:52.000000 PFlowC-2.3.0/PFlowC/geo_proxy.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7872 2024-04-29 09:28:01.000000 PFlowC-2.3.0/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.3.0/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.434858 PFlowC-2.3.0/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.3.0/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.3.0/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.458067 PFlowC-2.3.0/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.3.0/PFlowC/utils/Country.mmdb
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.3.0/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.3.0/PFlowC/utils/logger.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3324 2024-05-10 05:00:58.000000 PFlowC-2.3.0/PFlowC/utils/net.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.434491 PFlowC-2.3.0/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      641 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       64 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-10 05:04:31.000000 PFlowC-2.3.0/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-10 05:04:32.461909 PFlowC-2.3.0/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1831 2024-05-10 05:03:18.000000 PFlowC-2.3.0/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-10 05:04:32.462206 PFlowC-2.3.0/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1778 2024-05-10 05:03:23.000000 PFlowC-2.3.0/setup.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-10 05:04:32.461374 PFlowC-2.3.0/tests/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.3.0/tests/test-agent-service.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.3.0/tests/test-api.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.3.0/tests/test-banner.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.3.0/tests/test-dns-socket.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.3.0/tests/test-dnspython.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      370 2024-05-10 04:38:13.000000 PFlowC-2.3.0/tests/test-file-path.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      532 2024-05-10 02:34:13.000000 PFlowC-2.3.0/tests/test-filter-domains.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.3.0/tests/test-json-dump.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.3.0/tests/test-salary.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.574532 PFlowC-2.4.0/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.556575 PFlowC-2.4.0/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-20 02:51:10.000000 PFlowC-2.4.0/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3219 2024-05-10 11:06:42.000000 PFlowC-2.4.0/PFlowC/geo_proxy.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     8010 2024-05-10 11:13:02.000000 PFlowC-2.4.0/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-2.4.0/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.557889 PFlowC-2.4.0/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      859 2024-04-29 09:50:09.000000 PFlowC-2.4.0/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     7391 2024-04-29 09:49:45.000000 PFlowC-2.4.0/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.570463 PFlowC-2.4.0/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)  6381855 2024-04-29 05:46:08.000000 PFlowC-2.4.0/PFlowC/utils/Country.mmdb
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-2.4.0/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-2.4.0/PFlowC/utils/logger.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3379 2024-05-20 02:50:44.000000 PFlowC-2.4.0/PFlowC/utils/net.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.557309 PFlowC-2.4.0/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      641 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       64 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-05-20 02:52:29.000000 PFlowC-2.4.0/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2885 2024-05-20 02:52:30.574301 PFlowC-2.4.0/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1831 2024-05-20 02:52:26.000000 PFlowC-2.4.0/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-05-20 02:52:30.574709 PFlowC-2.4.0/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1778 2024-05-20 02:51:18.000000 PFlowC-2.4.0/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-05-20 02:52:30.573845 PFlowC-2.4.0/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     3532 2024-04-29 07:46:42.000000 PFlowC-2.4.0/tests/test-agent-service.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      416 2024-04-29 02:59:48.000000 PFlowC-2.4.0/tests/test-api.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-2.4.0/tests/test-banner.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      824 2024-04-30 04:51:51.000000 PFlowC-2.4.0/tests/test-dns-socket.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      858 2024-04-30 08:11:38.000000 PFlowC-2.4.0/tests/test-dnspython.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      370 2024-05-10 04:38:13.000000 PFlowC-2.4.0/tests/test-file-path.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      585 2024-05-10 06:02:56.000000 PFlowC-2.4.0/tests/test-filter-domains.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      566 2024-04-29 10:14:26.000000 PFlowC-2.4.0/tests/test-json-dump.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1313 2024-04-30 06:00:45.000000 PFlowC-2.4.0/tests/test-salary.py
```

### Comparing `PFlowC-2.3.0/PFlowC/geo_proxy.py` & `PFlowC-2.4.0/PFlowC/geo_proxy.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,85 +7,90 @@
 @disc:
 ======================================="""
 import json
 import logging
 import os
 import socket
 
-import geoip2.database
 from mitmproxy import http
 
 from PFlowC.proxy_helper import set_bypass_domains
-from PFlowC.utils.net import is_domestic2, geoip_db
-
+from PFlowC.utils.net import is_domestic2
 
 # 本地区域的国家代码，例如'CN'为中国
 LOCAL_REGION_CODE = 'CN'
 DEFAULT_BYPASS_DOMAINS = [
+    # LOCAL Address
     "127.0.0.1",
     "192.168.0.0/16",
     "172.16.0.0/16",
     "10.0.0.0/8",
+    # DNS
     '223.5.5.5',
     '119.29.29.29',
     'doh.pub',
     'dns.alidns.com',
-    "218.31.113.0/24"
 ]
-AGENT_DOMAINS = {
+DOMAINS = {
     "CN": [
+        # TODO:不要用记下IP地址, 因为GeoIP就能够分辨IP地址的区域划分.
+        "218.31.113.0/24"
+    ],
+    "US": [
         "github.com",
         "api.github.com"
     ]
 }
 
 home_dir = os.path.expanduser("~/.PFlowC")
 bypass_domains_fp = os.path.join(home_dir, "bypass_domains.json")
 bypass_domains = set()
 if not os.path.isfile(bypass_domains_fp):
-    logging.warning("bypass domains cache file[{}] does not exist.".format(bypass_domains_fp))
+    print("bypass domains cache file[{}] does not exist.".format(bypass_domains_fp))
 else:
     try:
         bypass_domains = set(json.load(open(bypass_domains_fp)))
         # TODO: 加载时对在PROXY规则里, 但是由于时间关系, 之前被加入到DIRECT里的域名都要提取出来
         # TODO: 用户个人的BypassDomains列表也要进行汇入.
     except json.decoder.JSONDecodeError as e:
-        logging.warning("BypassDomains缓存列表解析异常")
+        print("BypassDomains缓存列表解析异常")
 
 
 def save_bypass_domains():
     with open(bypass_domains_fp, "w") as bypass_domains_file:
         json.dump(list(bypass_domains), bypass_domains_file, indent=4, ensure_ascii=False)
 
 
 for item in DEFAULT_BYPASS_DOMAINS:
     bypass_domains.add(item)
-    set_bypass_domains(bypass_domains)
+for domain in DOMAINS[LOCAL_REGION_CODE]:
+    bypass_domains.add(domain)
+set_bypass_domains(bypass_domains)
 
 
-def is_local_region(ip):
-    try:
-        response = geoip_db.country(ip)
-        return response.country.iso_code == LOCAL_REGION_CODE
-    except geoip2.errors.AddressNotFoundError:
-        return False
+def is_exact_other_region(host):
+    for country_code, domains in DOMAINS.items():
+        if country_code != LOCAL_REGION_CODE:
+            if host in domains:
+                return True
+    return False
 
 
 def request(flow: http.HTTPFlow) -> None:
     # 获取请求的目标IP地址
     # 这里通过域名服务获取IP地址的方法要改成从特定的DNS获取, 直接从socket获取可能会因为不同的本地环境而导致出现异常.
     # 判断是否属于本地区域
     ip = socket.gethostbyname(flow.request.pretty_host)
     _type = "PROXY"
-    if flow.request.pretty_host in AGENT_DOMAINS[LOCAL_REGION_CODE]:
+    if is_exact_other_region(flow.request.pretty_host):
         _type = "PROXY"
     else:
         # 直接访问，不走上游代理
-        _type = "DIRECT"
         if is_domestic2(flow.request.pretty_host, target_country_code=LOCAL_REGION_CODE):
+            _type = "PROXY =2=> DIRECT"
             # 需要更新一下bypass_domains列表
             # TODO: 部分特殊域名要存在于官网规则中, 对他们进行过滤单独分离出来
             bypass_domains.add(flow.request.pretty_host)
             set_bypass_domains(bypass_domains)
             save_bypass_domains()
             # TODO: 收集到中央服务方便以后成为按地区分布代理流量控制缓存.
-    print(f"[{flow.timestamp_start}][{flow.type}][mode:{flow.mode}][{_type}][{ip} - {flow.request.pretty_host}]")
+    logging.info(f"[{flow.timestamp_start}][{flow.type}][mode:{flow.mode}][{_type}][{ip} - {flow.request.pretty_host}]")
```

### Comparing `PFlowC-2.3.0/PFlowC/main.py` & `PFlowC-2.4.0/PFlowC/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 @Software: PyCharm
 @disc:
 ======================================="""
 import json
 import logging
 import os
 import subprocess
+import sys
 from pathlib import Path
-
 import click
 
 from PFlowC import get_version
 from PFlowC.proxy_helper import set_all_proxy, clear_all_proxy
 from PFlowC.utils import logger
 
 home_dir = os.path.expanduser("~/.PFlowC")
@@ -144,20 +144,21 @@
     proxy_config = config.get_proxy_config()
     set_all_proxy(*proxy_config)
     upstream_proxy_address = config.get_upstream_proxy_address()
     fp = os.path.join(Path(__file__).parent, "geo_proxy.py")
     cmd = [
         "mitmdump", "--listen-port", str(proxy_config[1]), "--mode", f"upstream:{upstream_proxy_address}",
         "-s", fp, ]
-    print("CMD:", cmd)
+    logging.debug("CMD:%s" % cmd)
     try:
         p = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
-        print("Server is now on!")
+        logging.info("Server is now on!")
         # 循环读取输出并打印
         for line in iter(p.stdout.readline, b''):
-            print(line.decode(), end='')
+            sys.stdout.write(line.decode())
+            sys.stdout.flush()  # 刷新缓冲区以立即显示内容
     except subprocess.CalledProcessError as e:
-        print(e.stderr)
+        logging.error("CallSubprocessFailed:%s" % e.stderr)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `PFlowC-2.3.0/PFlowC/proxy.py` & `PFlowC-2.4.0/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PFlowC/proxy_helper/__init__.py` & `PFlowC-2.4.0/PFlowC/proxy_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PFlowC/proxy_helper/macosx.py` & `PFlowC-2.4.0/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PFlowC/utils/Country.mmdb` & `PFlowC-2.4.0/PFlowC/utils/Country.mmdb`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PFlowC/utils/logger.py` & `PFlowC-2.4.0/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PFlowC/utils/net.py` & `PFlowC-2.4.0/PFlowC/utils/net.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,23 @@
             with tempfile.NamedTemporaryFile(delete=False) as tmpfile:
                 tmpfile.write(data)
                 GEOIP_DB_PATH = tmpfile.name
         else:
             raise ImportError("无法加载资源文件 'Country.mmdb'")
 
 # 确保GEOIP_DB_PATH有有效的值后再使用
-if GEOIP_DB_PATH:
+if not GEOIP_DB_PATH:
     raise FileNotFoundError("未能找到或创建GeoIP数据库文件的路径")
 
 # 继续使用GEOIP_DB_PATH
 # 初始化GeoIP数据库
 geoip_db = geoip2.database.Reader(GEOIP_DB_PATH)
 
 # 初始化DNS解析器
-resolver = dns.resolver.Resolver()
+resolver = dns.resolver.Resolver(configure=False)
 resolver.nameservers = ['223.5.5.5', '119.29.29.29', 'https://doh.pub/dns-query',
                         'https://dns.alidns.com/dns-query']
 
 
 def resolve(domain_name: str, max_count: int = 20):
     ips = {}
     for i in range(max_count):
@@ -77,14 +77,15 @@
         if result[ip] == target_country_code:
             count += 1
     score = count / len(result.keys())
     return score > 0.5
 
 
 def is_domestic2(domain_name: str, max_try=10, target_country_code: str = "CN"):
+    # FIXME:区分是否是IP地址
     for i in range(max_try):
         answers = resolver.resolve(domain_name, 'A')
         for rdata in answers:
             try:
                 response = geoip_db.country(rdata.address)
                 if response.country.iso_code == target_country_code:
                     pass
```

### Comparing `PFlowC-2.3.0/PFlowC.egg-info/PKG-INFO` & `PFlowC-2.4.0/PFlowC.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.3.0
+Version: 2.4.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,15 +41,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.3.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.4.0                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.3.0/PFlowC.egg-info/SOURCES.txt` & `PFlowC-2.4.0/PFlowC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/PKG-INFO` & `PFlowC-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PFlowC
-Version: 2.3.0
+Version: 2.4.0
 Summary: https://github.com/Haoke98/FlowPilot/README.md
 Home-page: https://github.com/Haoke98/FlowPilot
 Author: Haoke98
 Author-email: BlackHaoke<Haoke98@outlook.com>
 License: MIT
 Keywords: proxy flow control
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,15 +41,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.3.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.4.0                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.3.0/README.rst` & `PFlowC-2.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     ██╔══██╗██╔════╝██║     ██╔═══██╗██║    ██║██╔════╝
     ██████╔╝█████╗  ██║     ██║   ██║██║ █╗ ██║██║
     ██╔═══╝ ██╔══╝  ██║     ██║   ██║██║███╗██║██║
     ██║     ██║     ███████╗╚██████╔╝╚███╔███╔╝╚██████╗
     ╚═╝     ╚═╝     ╚══════╝ ╚═════╝  ╚══╝╚══╝  ╚═════╝
 
     Command line interface for Proxy Flow Controller with basic auto configurations.
-    Version: 2.3.0                    By: BlackHaoke<Haoke98@outlook.com>
+    Version: 2.4.0                    By: BlackHaoke<Haoke98@outlook.com>
     Usage: pflow-cli [OPTIONS] COMMAND [ARGS]...
 
     Options:
       --help  Show this message and exit.
 
     Commands:
       off      Set off and clear all proxy config.
```

### Comparing `PFlowC-2.3.0/setup.py` & `PFlowC-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst', encoding='utf-8').read()
 
 setup(
     name='PFlowC',
-    version='2.3.0',
+    version='2.4.0',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=['colorlog', 'click', 'mitmproxy>=10.3.0', 'geoip2>=4.8.0', 'dnspython>=2.6.1'],
```

### Comparing `PFlowC-2.3.0/tests/test-agent-service.py` & `PFlowC-2.4.0/tests/test-agent-service.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/tests/test-banner.py` & `PFlowC-2.4.0/tests/test-banner.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/tests/test-dns-socket.py` & `PFlowC-2.4.0/tests/test-dns-socket.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/tests/test-dnspython.py` & `PFlowC-2.4.0/tests/test-dnspython.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/tests/test-json-dump.py` & `PFlowC-2.4.0/tests/test-json-dump.py`

 * *Files identical despite different names*

### Comparing `PFlowC-2.3.0/tests/test-salary.py` & `PFlowC-2.4.0/tests/test-salary.py`

 * *Files identical despite different names*

