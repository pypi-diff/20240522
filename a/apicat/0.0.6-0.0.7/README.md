# Comparing `tmp/apicat-0.0.6.tar.gz` & `tmp/apicat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apicat-0.0.6.tar", max compression
+gzip compressed data, was "apicat-0.0.7.tar", max compression
```

## Comparing `apicat-0.0.6.tar` & `apicat-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     2857 2024-05-12 05:41:33.063108 apicat-0.0.6/apicat/__init__.py
--rw-r--r--   0        0        0     1125 2024-05-12 05:48:09.499077 apicat-0.0.6/apicat/config.py
--rw-r--r--   0        0        0      578 2024-05-11 13:16:00.298607 apicat-0.0.6/apicat/core.py
--rw-r--r--   0        0        0      412 2024-05-12 05:59:48.227460 apicat-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-10 09:24:50.379838 apicat-0.0.6/README.md
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 apicat-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2566 2024-05-22 10:16:06.846622 apicat-0.0.7/apicat/__init__.py
+-rw-r--r--   0        0        0     2007 2024-05-22 15:22:09.417958 apicat-0.0.7/apicat/cli.py
+-rw-r--r--   0        0        0     1144 2024-05-22 11:11:24.195221 apicat-0.0.7/apicat/config.py
+-rw-r--r--   0        0        0      873 2024-05-22 11:07:59.126979 apicat-0.0.7/apicat/core.py
+-rw-r--r--   0        0        0      484 2024-05-22 11:12:07.003182 apicat-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      574 2024-05-22 15:26:21.639531 apicat-0.0.7/README.md
+-rw-r--r--   0        0        0     1332 1970-01-01 00:00:00.000000 apicat-0.0.7/PKG-INFO
```

### Comparing `apicat-0.0.6/apicat/__init__.py` & `apicat-0.0.7/apicat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,14 +99,7 @@
             padding: 10px;
         }
     }
 </style>
         </html>
         """
     return render_template_string(combined_html)
-
-def start(plugin_list: list):
-    log.info("欢迎使用 ApiCat🎉")
-    log.info("开发团队: 星海码队")
-    log.info("项目地址: https://github.com/xinghai-osc/apicat")
-    core.register_plugins(plugin_list, app)
-    app.run(port=config.get_port(), host=config.get_host())
```

#### html2text {}

```diff
@@ -8,12 +8,8 @@
 æ²¡æææ¡£ã") combined_html = f"""
 ************ {{ccoonnffiigg..ggeett__wweebbssiittee__nnaammee(())}} ************
 """ for plugin_name, docs_func in plugin_docs.items(): docs_str = docs_func()
 if callable(docs_func) else str(docs_func) combined_html += f"""
 {docs_str}
 """ combined_html += """
 Powered by _A_p_i_C_a_t
-""" return render_template_string(combined_html) def start(plugin_list: list):
-log.info("æ¬¢è¿ä½¿ç¨ ApiCatð") log.info("å¼åå¢é: ææµ·ç é")
-log.info("é¡¹ç®å°å: https://github.com/xinghai-osc/apicat")
-core.register_plugins(plugin_list, app) app.run(port=config.get_port(),
-host=config.get_host())
+""" return render_template_string(combined_html)
```

### Comparing `apicat-0.0.6/apicat/config.py` & `apicat-0.0.7/apicat/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import toml
+import toml,os
 
-path = "config.toml"
+path = os.getcwd() + "\\config.toml"
 
 def get_port():
     """获取端口，若不存在则返回80"""
     try:
         config = toml.load(path)
         return config['website']['port']
     except KeyError:
```

