# Comparing `tmp/unittestreport_yami-0.0.2.tar.gz` & `tmp/unittestreport_yami-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.0.2.tar", last modified: Fri Apr  5 02:19:59 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.0.tar", last modified: Wed May 22 03:19:30 2024, max compression
```

## Comparing `unittestreport_yami-0.0.2.tar` & `unittestreport_yami-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 02:19:59.712477 unittestreport_yami-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2097 2024-04-05 02:19:59.710477 unittestreport_yami-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-04-05 01:17:01.000000 unittestreport_yami-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-05 02:19:59.713477 unittestreport_yami-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-04-05 02:17:19.000000 unittestreport_yami-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:19:59.652476 unittestreport_yami-0.0.2/unittestreport/
--rw-rw-rw-   0        0        0      554 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:19:59.666475 unittestreport_yami-0.0.2/unittestreport/core/
--rw-rw-rw-   0        0        0      189 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/parameterized.py
--rw-rw-rw-   0        0        0     1204 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/reRun.py
--rw-rw-rw-   0        0        0     5156 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/resultPush.py
--rw-rw-rw-   0        0        0     2675 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/core/sendEmail.py
--rw-rw-rw-   0        0        0     6945 2024-04-05 02:14:29.000000 unittestreport_yami-0.0.2/unittestreport/core/testResult.py
--rw-rw-rw-   0        0        0    12803 2024-04-03 07:20:27.000000 unittestreport_yami-0.0.2/unittestreport/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-04-05 02:19:59.676474 unittestreport_yami-0.0.2/unittestreport/templates/
--rw-rw-rw-   0        0        0      189 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/templates/dingtalk.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 02:16:12.000000 unittestreport_yami-0.0.2/unittestreport/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-03 07:19:10.000000 unittestreport_yami-0.0.2/unittestreport/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-04-05 02:19:59.708472 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2097 2024-04-05 02:19:59.000000 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2024-04-05 02:19:59.000000 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 02:19:59.000000 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-04-05 02:19:59.000000 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-05 02:19:59.000000 unittestreport_yami-0.0.2/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.715623 unittestreport_yami-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-22 03:19:30.713615 unittestreport_yami-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:19:30.716618 unittestreport_yami-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-22 03:19:15.000000 unittestreport_yami-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.659612 unittestreport_yami-0.1.0/unittestreport_yami/
+-rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.0/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.699616 unittestreport_yami-0.1.0/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     7090 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    12904 2024-05-22 02:30:51.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.709611 unittestreport_yami-0.1.0/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.683613 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.0.2/LICENSE` & `unittestreport_yami-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/PKG-INFO` & `unittestreport_yami-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.0.2
+Version: 0.1.0
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2==3.0.3
 Requires-Dist: PyYAML==5.3.1
-Requires-Dist: requests==2.24.0
+Requires-Dist: requests==2.32.2
 
 # unittestreport介绍
 
 ## 说明
 本项目是在unittestreport的基础上增加了截图功能。在生成的最终的报告中可以看到截图，并支持多图切换。原项目地址：https://github.com/musen123/UnitTestReport
 ![sceen shot button](docs/img/screen-shot-1.png)
 ![view sceen shot](docs/img/screen-shot-2.png)
```

### Comparing `unittestreport_yami-0.0.2/README.md` & `unittestreport_yami-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/setup.py` & `unittestreport_yami-0.1.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-"""
-============================
-Author:Ethan
-============================
-"""
 from setuptools import setup, find_packages
 
-with open("readme.md", "r", encoding='utf8') as fh:
+with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
-    name='unittestreport_yami',
-    version='0.0.2',
-    author='Ethan',
-    author_email='ethan.liu@yamibuy.com',
-    url='https://github.com/EthanLiuInyami/UnitTestReport',
+    name="unittestreport_yami",
+    version="0.1.0",
+    author="Ethan",
+    author_email="ethan.liu@yamibuy.com",
+    url="https://github.com/EthanLiuInyami/UnitTestReport",
+    license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["Jinja2==3.0.3", "PyYAML==5.3.1","requests==2.24.0"],
+    install_requires=["Jinja2==3.0.3", "PyYAML==5.3.1", "requests==2.32.2"],
     packages=find_packages(),
     package_data={
-        "": ["*.html",'*.md'],
+        "": ["*.html", "*.md"],
     },
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
 )
-
```

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/dataDriver.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/parameterized.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/resultPush.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/resultPush.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-============================
-Author:柠檬班-木森
-Time:2020/11/25  14:14
-E-mail:3247119728@qq.com
-Company:湖南零檬信息技术有限公司
-============================
-"""
 import hmac
 import hashlib
 import base64
 import urllib.parse
 import requests
 import os
 import smtplib
@@ -34,15 +26,17 @@
         else:
             self.smtp = smtplib.SMTP(host=host, port=port)
         self.smtp.ehlo()
 
         self.smtp.login(user=user, password=password)
         self.user = user
 
-    def send_email(self, subject="test report", content=None, filename=None, to_addrs=None):
+    def send_email(
+        self, subject="test report", content=None, filename=None, to_addrs=None
+    ):
         """
         :param subject:Email subject
         :param content: Email content
         :param filename: Attachment document
         :param to_addrs: Addressee's address
         :type to_addrs: str or list
         :return:
@@ -62,15 +56,15 @@
             with open(filename, "rb") as f:
                 content = f.read()
             try:
                 report = MIMEApplication(content, _subtype=None)
             except:
                 report = MIMEApplication(content)
             name = os.path.split(filename)[1]
-            report.add_header('content-disposition', 'attachment', filename=name)
+            report.add_header("content-disposition", "attachment", filename=name)
             msg.attach(report)
         try:
             self.smtp.send_message(msg, from_addr=self.user, to_addrs=to_addrs)
         except Exception as e:
             print("Failed to send test report")
             raise e
         else:
@@ -89,18 +83,20 @@
         self.url = url
         self.data = data
         self.secret = secret
 
     def get_stamp(self):
         """Countersign"""
         timestamp = str(round(time.time() * 1000))
-        secret_enc = self.secret.encode('utf-8')
-        string_to_sign = '{}\n{}'.format(timestamp, self.secret)
-        string_to_sign_enc = string_to_sign.encode('utf-8')
-        hmac_code = hmac.new(secret_enc, string_to_sign_enc, digestmod=hashlib.sha256).digest()
+        secret_enc = self.secret.encode("utf-8")
+        string_to_sign = "{}\n{}".format(timestamp, self.secret)
+        string_to_sign_enc = string_to_sign.encode("utf-8")
+        hmac_code = hmac.new(
+            secret_enc, string_to_sign_enc, digestmod=hashlib.sha256
+        ).digest()
         sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
         return {"sign": sign, "timestamp": timestamp}
 
     def send_info(self):
         """send info"""
         if self.secret:
             params = self.get_stamp()
@@ -110,43 +106,40 @@
         return response
 
 
 class WeiXin:
     """
     Enterprise wechat group notice
     """
+
     base_url = "https://qyapi.weixin.qq.com/cgi-bin/appchat/send?access_token="
 
     def __init__(self, access_token=None, corpid=None, corpsecret=None):
         """
         :param corpid:wechat corpid
         :param corpsecret:Applied credential key
         """
         self.corpid = corpid
         self.corpsecret = corpsecret
         if access_token:
             self.access_token = access_token
         elif corpid and corpsecret:
             self.access_token = self.get_access_token()
         else:
-            raise ValueError("access_token and [corpid, corpsecret] cannot both be empty. At least one of them must be passed in")
+            raise ValueError(
+                "access_token and [corpid, corpsecret] cannot both be empty. At least one of them must be passed in"
+            )
 
     def get_access_token(self):
         """get access_token"""
         url = "https://qyapi.weixin.qq.com/cgi-bin/gettoken"
-        params = {
-            "corpid": self.corpid,
-            "corpsecret": self.corpsecret
-        }
+        params = {"corpid": self.corpid, "corpsecret": self.corpsecret}
         result = requests.get(url=url, params=params).json()
-        if result['errcode'] != 0:
+        if result["errcode"] != 0:
             raise ValueError(result["errmsg"])
         return result["access_token"]
 
     def send_info(self, data):
         """send info"""
         url = self.base_url + self.access_token
         response = requests.post(url=url, json=data)
         return response
-
-
-
```

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/sendEmail.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/sendEmail.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-"""
-============================
-Author:柠檬班-木森
-Time:2020/8/31   14:48
-E-mail:3247119728@qq.com
-Company:湖南零檬信息技术有限公司
-============================
-"""
 import os
 import smtplib
 import time
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 
@@ -30,15 +22,17 @@
         :param user: 邮箱账号
         :param password: 邮箱的smtp服务授权码
         """
         self.smtp = smtplib.SMTP_SSL(host=host, port=port)
         self.smtp.login(user=user, password=password)
         self.user = user
 
-    def send_email(self, subject="测试报告", content=None, filename=None, to_addrs=None):
+    def send_email(
+        self, subject="测试报告", content=None, filename=None, to_addrs=None
+    ):
         """
         发送邮件
         :param subject: 邮件主题
         :param content: 邮件内容
         :param filename: 报告文件的完整路径
         :param to_addrs: 收件人地址
         :type to_addrs: str or list
@@ -59,15 +53,15 @@
         msg.attach(text)
         # 判断是否要发送附件
         if filename and os.path.isfile(filename):
             with open(filename, "rb") as f:
                 content = f.read()
             report = MIMEApplication(content, _subtype=None)
             name = os.path.split(filename)[1]
-            report.add_header('content-disposition', 'attachment', filename=name)
+            report.add_header("content-disposition", "attachment", filename=name)
             msg.attach(report)
         # 第三步：发送邮件
         try:
             self.smtp.send_message(msg, from_addr=self.user, to_addrs=to_addrs)
         except Exception as e:
             print("--------测试报告发送失败------")
             raise e
```

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/testResult.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/testResult.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,27 @@
-"""
-============================
-Author:柠檬班-木森
-Time:2020/8/26   11:25
-E-mail:3247119728@qq.com
-Company:湖南零檬信息技术有限公司
-============================
-"""
 import re
 import traceback
 import unittest
 import sys
 import time
 from io import StringIO
 
 origin_stdout = sys.stdout
 
 
 def output2console(s):
     """Output stdout content to console"""
     tmp_stdout = sys.stdout
     sys.stdout = origin_stdout
-    print(s, end='')
+    print(s, end="")
     sys.stdout = tmp_stdout
 
 
 class OutputRedirector(object):
-    """ Wrapper to redirect stdout or stderr """
+    """Wrapper to redirect stdout or stderr"""
 
     def __init__(self, fp):
         self.fp = fp
 
     def write(self, s):
         self.fp.write(s)
         origin_stdout.write(str(s))
@@ -53,15 +45,15 @@
             "success": 0,
             "all": 0,
             "fail": 0,
             "skip": 0,
             "error": 0,
             "begin_time": "",
             "results": [],
-            "testClass": set()
+            "testClass": set(),
         }
         self.sys_stdout = None
         self.sys_stderr = None
         self.outputBuffer = None
 
     def startTest(self, test):
         super().startTest(test)
@@ -79,74 +71,91 @@
             sys.stdout = self.sys_stdout
             sys.stderr = self.sys_stderr
             self.sys_stdout = None
             self.sys_stderr = None
         return self.outputBuffer.getvalue()
 
     def stopTest(self, test):
-        test.run_time = '{:.3}s'.format((time.time() - self.start_time))
+        test.run_time = "{:.3}s".format((time.time() - self.start_time))
         test.class_name = test.__class__.__qualname__
-        test.method_name = test.__dict__['_testMethodName']
+        test.method_name = test.__dict__["_testMethodName"]
         test.method_doc = test.shortDescription()
-        self.fields['results'].append(test)
+        self.fields["results"].append(test)
         self.fields["testClass"].add(test.class_name)
         self.complete_output()
 
     def stopTestRun(self, title=None):
-        self.fields['fail'] = len(self.failures)
-        self.fields['error'] = len(self.errors)
-        self.fields['skip'] = len(self.skipped)
-        self.fields['all'] = sum(
-            [self.fields['fail'], self.fields['error'], self.fields['skip'], self.fields['success']])
-        self.fields['testClass'] = list(self.fields['testClass'])
+        self.fields["fail"] = len(self.failures)
+        self.fields["error"] = len(self.errors)
+        self.fields["skip"] = len(self.skipped)
+        self.fields["all"] = sum(
+            [
+                self.fields["fail"],
+                self.fields["error"],
+                self.fields["skip"],
+                self.fields["success"],
+            ]
+        )
+        self.fields["testClass"] = list(self.fields["testClass"])
 
     def addSuccess(self, test):
         self.fields["success"] += 1
-        test.state = '成功'
+        test.state = "成功"
         sys.stdout.write("{}执行——>【通过】\n".format(test))
         logs = []
         output = self.complete_output()
         logs.append(output)
         test.run_info = logs
+        self._add_screen_shot_in_test(test)
 
     def addFailure(self, test, err):
         super().addFailure(test, err)
         logs = []
-        test.state = '失败'
+        test.state = "失败"
         sys.stderr.write("{}执行——>【失败】\n".format(test))
         output = self.complete_output()
         logs.append(output)
         logs.extend(traceback.format_exception(*err))
         test.run_info = logs
+        self._add_screen_shot_in_test(test)
 
     def addSkip(self, test, reason):
         super().addSkip(test, reason)
-        test.state = '跳过'
+        test.state = "跳过"
         sys.stdout.write("{}执行--【跳过Skip】\n".format(test))
         logs = [reason]
         test.run_info = logs
 
     def addError(self, test, err):
         super().addError(test, err)
-        test.state = '错误'
+        test.state = "错误"
         sys.stderr.write("{}执行——>【错误Error】\n".format(test))
         logs = []
         logs.extend(traceback.format_exception(*err))
         test.run_info = logs
-        if test.__class__.__qualname__ == '_ErrorHolder':
+        if test.__class__.__qualname__ == "_ErrorHolder":
             test.run_time = 0
-            res = re.search(r'(.*)\(.*\.(.*)\)', test.description)
+            res = re.search(r"(.*)\(.*\.(.*)\)", test.description)
             test.class_name = res.group(2)
             test.method_name = res.group(1)
             test.method_doc = test.shortDescription()
-            self.fields['results'].append(test)
+            self.fields["results"].append(test)
             self.fields["testClass"].add(test.class_name)
         else:
             output = self.complete_output()
             logs.append(output)
+        self._add_screen_shot_in_test(test)
+
+    def _add_screen_shot_in_test(self, test):
+        if type(getattr(test, "driver", "")).__name__ == "WebDriver":
+            driver = getattr(test, "driver")
+            try:
+                test.images.append(driver.get_screenshot_as_base64())
+            except BaseException as e:
+                print(e)
 
 
 class ReRunResult(TestResult):
 
     def __init__(self, count, interval):
         super().__init__()
         self.count = count
@@ -160,48 +169,48 @@
 
     def stopTest(self, test):
         if test not in self.run_cases:
             self.run_cases.append(test)
             super().stopTest(test)
 
     def addFailure(self, test, err):
-        if not hasattr(test, 'count'):
+        if not hasattr(test, "count"):
             test.count = 0
         if test.count < self.count:
             test.count += 1
             sys.stderr.write("{}执行——>【失败Failure】\n".format(test))
             for string in traceback.format_exception(*err):
                 sys.stderr.write(string)
-            sys.stderr.write("================{}重运行第{}次================\n".format(test, test.count))
+            sys.stderr.write(
+                f"================{test}重运行第{test.count}次================\n"
+            )
 
             time.sleep(self.interval)
             test.run(self)
         else:
             super().addFailure(test, err)
             if test.count != 0:
-                sys.stderr.write("================重运行{}次完毕================\n".format(test.count))
+                sys.stderr.write(
+                    f"================重运行{test.count}次完毕================\n"
+                )
         self._add_screen_shot_in_test(test)
 
     def addError(self, test, err):
-        if not hasattr(test, 'count'):
+        if not hasattr(test, "count"):
             test.count = 0
         if test.count < self.count:
             test.count += 1
             sys.stderr.write("{}执行——>【错误Error】\n".format(test))
             for string in traceback.format_exception(*err):
                 sys.stderr.write(string)
-            sys.stderr.write("================{}重运行第{}次================\n".format(test, test.count))
+            sys.stderr.write(
+                f"================{test}重运行第{test.count}次================\n"
+            )
             time.sleep(self.interval)
             test.run(self)
         else:
             super().addError(test, err)
             if test.count != 0:
-                sys.stderr.write("================重运行{}次完毕================\n".format(test.count))
+                sys.stderr.write(
+                    f"================重运行{test.count}次完毕================\n"
+                )
         self._add_screen_shot_in_test(test)
-
-    def _add_screen_shot_in_test(self, test):
-        if type(getattr(test, "driver", "")).__name__ == 'WebDriver':
-            driver = getattr(test, "driver")
-            try:
-                test.images.append(driver.get_screenshot_as_base64())
-            except BaseException as e:
-                print(e)
```

### Comparing `unittestreport_yami-0.0.2/unittestreport/core/testRunner.py` & `unittestreport_yami-0.1.0/unittestreport_yami/core/testRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 # encoding=utf-8
-"""
-============================
-Author:柠檬班-木森
-Time:2020/7/7   14:47
-E-mail:3247119728@qq.com
-Company:湖南零檬信息技术有限公司
-============================
-"""
+
 import json
 import os
 import unittest
 import time
 from concurrent.futures.thread import ThreadPoolExecutor
 from ..core.testResult import TestResult, ReRunResult
 from ..core.resultPush import DingTalk, WeiXin, SendEmail
@@ -37,24 +30,27 @@
         </div>
         <div class="img-circle"></div>
     </div>
     </div>
 </div>
 """
 
-class TestRunner():
 
-    def __init__(self, suite: unittest.TestSuite,
-                 filename="report.html",
-                 report_dir="./reports",
-                 title='测试报告',
-                 tester='测试员',
-                 desc="XX项目测试生成的报告",
-                 templates=1
-                 ):
+class TestRunner:
+
+    def __init__(
+        self,
+        suite: unittest.TestSuite,
+        filename="report.html",
+        report_dir="./reports",
+        title="测试报告",
+        tester="测试员",
+        desc="XX项目测试生成的报告",
+        templates=1,
+    ):
         """
         :param suites: test suite
         :param filename: Report file name
         :param report_dir:The path to the report file
         :param title:Test suite title
         :param templates: You can specify the style template for the report by parameter value 1 or 2. Currently, there are only two templates
         :param tester:Tester
@@ -100,103 +96,119 @@
             "results": [],
             "testClass": [],
         }
         for res in self.result:
             for item in test_result:
                 test_result[item] += res.fields[item]
 
-        test_result['runtime'] = '{:.2f} S'.format(time.time() - self.starttime)
-        test_result["begin_time"] = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(self.starttime))
+        test_result["runtime"] = "{:.2f} S".format(time.time() - self.starttime)
+        test_result["begin_time"] = time.strftime(
+            "%Y-%m-%d %H:%M:%S", time.localtime(self.starttime)
+        )
         test_result["title"] = self.title
         test_result["tester"] = self.tester
-        test_result['desc'] = self.desc
-        if test_result['all'] != 0:
-            test_result['pass_rate'] = '{:.2f}'.format(test_result['success'] / test_result['all'] * 100)
+        test_result["desc"] = self.desc
+        if test_result["all"] != 0:
+            test_result["pass_rate"] = "{:.2f}".format(
+                test_result["success"] / test_result["all"] * 100
+            )
         else:
-            test_result['pass_rate'] = 0
-        for res in test_result['results']:
-            if getattr(res, 'images', []):
+            test_result["pass_rate"] = 0
+        for res in test_result["results"]:
+            if getattr(res, "images", []):
                 tmp = ""
                 for i, img in enumerate(res.images):
                     if i == 0:
-                        tmp += """<img src="data:image/jpg;base64,{}" style="display: block;" class="img"/>\n""".format(img)
+                        tmp += """<img src="data:image/jpg;base64,{}" style="display: block;" class="img"/>\n""".format(
+                            img
+                        )
                     else:
-                        tmp += """<img src="data:image/jpg;base64,{}" style="display: none;" class="img"/>\n""".format(img)
+                        tmp += """<img src="data:image/jpg;base64,{}" style="display: none;" class="img"/>\n""".format(
+                            img
+                        )
                 screenshots_html = IMG_TMPL.format(images=tmp)
                 setattr(res, "screenshots_html", screenshots_html)
         # 判断是否要生产测试报告
         if os.path.isdir(self.report_dir):
             pass
         else:
             os.mkdir(self.report_dir)
         # 获取历史执行数据
-        test_result['history'] = self.__handle_history_data(test_result)
+        test_result["history"] = self.__handle_history_data(test_result)
 
-        template_path = os.path.join(os.path.dirname(__file__), '../templates')
+        template_path = os.path.join(os.path.dirname(__file__), "../templates")
         env = Environment(loader=FileSystemLoader(template_path))
         if self.templates == 2:
-            template = env.get_template('templates2.html')
+            template = env.get_template("templates2.html")
         elif self.templates == 3:
-            template = env.get_template('templates3.html')
+            template = env.get_template("templates3.html")
         else:
-            template = env.get_template('templates.html')
+            template = env.get_template("templates.html")
         file_path = os.path.join(self.report_dir, self.filename)
         res = template.render(test_result)
-        with open(file_path, 'wb') as f:
-            f.write(res.encode('utf8'))
+        with open(file_path, "wb") as f:
+            f.write(res.encode("utf8"))
         print("测试报告已经生成，报告路径为:{}".format(file_path))
-        self.email_conent = {"file": os.path.abspath(file_path),
-                             "content": env.get_template('templates03.html').render(test_result)
-                             }
+        self.email_conent = {
+            "file": os.path.abspath(file_path),
+            "content": env.get_template("templates03.html").render(test_result),
+        }
         self.test_result = test_result
         return test_result
 
     def __handle_history_data(self, test_result):
         """
         处理历史数据
         :return:
         """
         try:
-            with open(os.path.join(self.report_dir, 'history.json'), 'r', encoding='utf-8') as f:
+            with open(
+                os.path.join(self.report_dir, "history.json"), "r", encoding="utf-8"
+            ) as f:
                 history = json.load(f)
         except FileNotFoundError as e:
             history = []
-        history.append({'success': test_result['success'],
-                        'all': test_result['all'],
-                        'fail': test_result['fail'],
-                        'skip': test_result['skip'],
-                        'error': test_result['error'],
-                        'runtime': test_result['runtime'],
-                        'begin_time': test_result['begin_time'],
-                        'pass_rate': test_result['pass_rate'],
-                        })
+        history.append(
+            {
+                "success": test_result["success"],
+                "all": test_result["all"],
+                "fail": test_result["fail"],
+                "skip": test_result["skip"],
+                "error": test_result["error"],
+                "runtime": test_result["runtime"],
+                "begin_time": test_result["begin_time"],
+                "pass_rate": test_result["pass_rate"],
+            }
+        )
 
-        with open(os.path.join(self.report_dir, 'history.json'), 'w', encoding='utf-8') as f:
+        with open(
+            os.path.join(self.report_dir, "history.json"), "w", encoding="utf-8"
+        ) as f:
             json.dump(history, f, ensure_ascii=True)
         return history
 
     def __get_notice_content(self):
         """获取通知的内容"""
-        template_path = os.path.join(os.path.dirname(__file__), '../templates')
+        template_path = os.path.join(os.path.dirname(__file__), "../templates")
         env = Environment(loader=FileSystemLoader(template_path))
-        res_text = env.get_template('dingtalk.md').render(self.test_result)
+        res_text = env.get_template("dingtalk.md").render(self.test_result)
         return res_text
 
     def run(self, thread_count=1, count=0, interval=2):
         """
         The entrance to running tests
         Note: if multiple test classes share a global variable, errors may occur due to resource competition
         :param thread_count:Number of threads. default 1
         :param count: Rerun times,  default 0
         :param interval: Rerun interval, default 2
         :return: Test run results
         """
         suites = self.__classification_suite()
 
-        if thread_count>1:
+        if thread_count > 1:
             with ThreadPoolExecutor(max_workers=thread_count) as ts:
                 for i in suites:
                     res = ReRunResult(count=count, interval=interval)
                     self.result.append(res)
                     ts.submit(i.run, result=res).add_done_callback(res.stopTestRun)
         else:
             res = ReRunResult(count=count, interval=interval)
@@ -218,15 +230,17 @@
         suites = self.__classification_suite()
         for case_ in suites:
             case_.run(res)
         res.stopTestRun()
         res = self.__get_reports()
         return res
 
-    def send_email(self, host: str, port: int, user: str, password: str, to_addrs, is_file=True):
+    def send_email(
+        self, host: str, port: int, user: str, password: str, to_addrs, is_file=True
+    ):
         """
         The occurrence report is attached to the mailbox
         :param host: SMTP server address
         :param port: SMTP server port
         :param user: Email account number
         :param password: SMTP service authorization code of mailbox
         :param to_addrs: Addressee's address str or list
@@ -235,59 +249,71 @@
         sm = SendEmail(host=host, port=port, user=user, password=password)
         if is_file:
             filename = self.email_conent["file"]
         else:
             filename = None
         content = self.email_conent["content"]
 
-        sm.send_email(subject=self.title, content=content, filename=filename, to_addrs=to_addrs)
+        sm.send_email(
+            subject=self.title, content=content, filename=filename, to_addrs=to_addrs
+        )
 
     def get_except_info(self):
         """Get error reporting information for error cases and failure cases"""
         except_info = []
         num = 0
         for i in self.result:
             for texts in i.failures:
                 t, content = texts
                 num += 1
-                except_info.append("*{}、用例【{}】执行失败*，\n失败信息如下：".format(num, t._testMethodDoc))
+                except_info.append(
+                    "*{}、用例【{}】执行失败*，\n失败信息如下：".format(
+                        num, t._testMethodDoc
+                    )
+                )
                 except_info.append(content)
             for texts in i.errors:
                 num += 1
                 t, content = texts
-                except_info.append("*{}、用例【{}】执行错误*，\n错误信息如下：".format(num, t._testMethodDoc))
+                except_info.append(
+                    "*{}、用例【{}】执行错误*，\n错误信息如下：".format(
+                        num, t._testMethodDoc
+                    )
+                )
                 except_info.append(content)
         except_str = "\n".join(except_info)
         return except_str
 
-    def dingtalk_notice(self, url, key=None, secret=None, atMobiles=None, isatall=False, except_info=False):
+    def dingtalk_notice(
+        self,
+        url,
+        key=None,
+        secret=None,
+        atMobiles=None,
+        isatall=False,
+        except_info=False,
+    ):
         """
         :param url: 钉钉机器人的Webhook地址
         :param key: （非必传：str类型）如果钉钉机器人安全设置了关键字，则需要传入对应的关键字
         :param secret:（非必传:str类型）如果钉钉机器人安全设置了签名，则需要传入对应的密钥
         :param atMobiles: （非必传，list类型）发送通知钉钉中要@人的手机号列表，如：[137xxx,188xxx]
         :param isatall: 是否@所有人，默认为False,设为True则会@所有人
         :param except_info:是否发送未通过用例的详细信息，默认为False，设为True则会发送失败用例的详细信息
         :return:  发送成功返回 {"errcode":0,"errmsg":"ok"}  发送失败返回 {"errcode":错误码,"errmsg":"失败原因"}
         """
 
         res_text = self.__get_notice_content()
         if except_info:
-            res_text += '\n ### 未通过用例详情：\n'
+            res_text += "\n ### 未通过用例详情：\n"
             res_text += self.get_except_info()
         data = {
             "msgtype": "markdown",
-            "markdown": {
-                "title": '{}({})'.format(self.title, key),
-                "text": res_text
-            },
-            "at": {
-                "atMobiles": atMobiles,
-                "isAtAll": isatall
-            }
+            "markdown": {"title": "{}({})".format(self.title, key), "text": res_text},
+            "at": {"atMobiles": atMobiles, "isAtAll": isatall},
         }
         ding = DingTalk(url=url, data=data, secret=secret)
         response = ding.send_info()
         return response.json()
 
     def weixin_notice(self, chatid, access_token=None, corpid=None, corpsecret=None):
         """
@@ -300,14 +326,12 @@
         :return:
         """
         # 获取通知结果
         res_text = self.__get_notice_content()
         data = {
             "chatid": chatid,
             "msgtype": "markdown",
-            "markdown": {
-                "content": res_text
-            }
+            "markdown": {"content": res_text},
         }
         wx = WeiXin(access_token=access_token, corpid=corpid, corpsecret=corpsecret)
         response = wx.send_info(data=data)
         return response
```

### Comparing `unittestreport_yami-0.0.2/unittestreport/templates/templates.html` & `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport/templates/templates03.html` & `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport/templates/templates2.html` & `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport/templates/templates3.html` & `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.0.2/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.0/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.0.2
+Version: 0.1.0
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
+License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Jinja2==3.0.3
 Requires-Dist: PyYAML==5.3.1
-Requires-Dist: requests==2.24.0
+Requires-Dist: requests==2.32.2
 
 # unittestreport介绍
 
 ## 说明
 本项目是在unittestreport的基础上增加了截图功能。在生成的最终的报告中可以看到截图，并支持多图切换。原项目地址：https://github.com/musen123/UnitTestReport
 ![sceen shot button](docs/img/screen-shot-1.png)
 ![view sceen shot](docs/img/screen-shot-2.png)
```

