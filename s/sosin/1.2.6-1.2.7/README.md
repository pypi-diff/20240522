# Comparing `tmp/sosin-1.2.6.tar.gz` & `tmp/sosin-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.2.6.tar", last modified: Fri May 17 13:31:51 2024, max compression
+gzip compressed data, was "sosin-1.2.7.tar", last modified: Wed May 22 12:39:29 2024, max compression
```

## Comparing `sosin-1.2.6.tar` & `sosin-1.2.7.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.578196 sosin-1.2.6/
--rw-rw-rw-   0        0        0     1083 2024-05-17 13:30:25.000000 sosin-1.2.6/LICENSE
--rw-rw-rw-   0        0        0     1269 2024-05-17 13:31:51.577110 sosin-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      863 2024-05-17 13:30:25.000000 sosin-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-17 13:31:51.578196 sosin-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      985 2024-05-17 13:31:12.000000 sosin-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.538398 sosin-1.2.6/sosin/
--rw-rw-rw-   0        0        0      302 2024-05-17 13:31:04.000000 sosin-1.2.6/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.561913 sosin-1.2.6/sosin/databases/
--rw-rw-rw-   0        0        0    13404 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.564954 sosin-1.2.6/sosin/rpa/
--rw-rw-rw-   0        0        0    12041 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.569529 sosin-1.2.6/sosin/utils/
--rw-rw-rw-   0        0        0     1797 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      422 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.572792 sosin-1.2.6/sosin/web/
--rw-rw-rw-   0        0        0     1055 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/content.py
--rw-rw-rw-   0        0        0     6138 2024-05-17 13:30:49.000000 sosin-1.2.6/sosin/web/session.py
--rw-rw-rw-   0        0        0     1051 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4580 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.560408 sosin-1.2.6/sosin.egg-info/
--rw-rw-rw-   0        0        0     1269 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.603343 sosin-1.2.7/
+-rw-rw-rw-   0        0        0     1062 2024-05-22 04:37:09.000000 sosin-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     1269 2024-05-22 12:39:29.602655 sosin-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      839 2024-05-22 04:37:09.000000 sosin-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:39:29.603343 sosin-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      985 2024-05-22 04:41:04.000000 sosin-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.569091 sosin-1.2.7/sosin/
+-rw-rw-rw-   0        0        0      354 2024-05-22 04:40:15.000000 sosin-1.2.7/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.590350 sosin-1.2.7/sosin/databases/
+-rw-rw-rw-   0        0        0    13404 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.592834 sosin-1.2.7/sosin/rpa/
+-rw-rw-rw-   0        0        0    12041 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3573 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.596619 sosin-1.2.7/sosin/utils/
+-rw-rw-rw-   0        0        0     1752 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      294 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      511 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      422 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      856 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.601614 sosin-1.2.7/sosin/web/
+-rw-rw-rw-   0        0        0     1018 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/web/content.py
+-rw-rw-rw-   0        0        0     6138 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/web/session.py
+-rw-rw-rw-   0        0        0     6156 2024-05-22 04:39:56.000000 sosin-1.2.7/sosin/web/session_async.py
+-rw-rw-rw-   0        0        0     1020 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4580 2024-05-22 04:37:09.000000 sosin-1.2.7/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:39:29.589324 sosin-1.2.7/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1269 2024-05-22 12:39:29.000000 sosin-1.2.7/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-05-22 12:39:29.000000 sosin-1.2.7/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:39:29.000000 sosin-1.2.7/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-22 12:39:29.000000 sosin-1.2.7/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 12:39:29.000000 sosin-1.2.7/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.2.6/LICENSE` & `sosin-1.2.7/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 sosin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 sosin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sosin-1.2.6/PKG-INFO` & `sosin-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: sosincomp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sosin-1.2.6/README.md` & `sosin-1.2.7/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
```

### Comparing `sosin-1.2.6/setup.py` & `sosin-1.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.2.6",
+    version                             = "1.2.7",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "sosincomp@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
```

### Comparing `sosin-1.2.6/sosin/databases/rdb.py` & `sosin-1.2.7/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.6/sosin/rpa/email_mgr.py` & `sosin-1.2.7/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.6/sosin/rpa/sms_mgr.py` & `sosin-1.2.7/sosin/rpa/sms_mgr.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import requests
-
-class AligoManager:
-    """
-    Aligo Messages API
-
-    https://smartsms.aligo.in/
-    """
-
-    def __init__(self, key, user_id, sender_phone, is_test) -> None:
-        """
-        Aligo configs
-        key = API Key
-        user_id = User ID
-        sender_phone = phone number
-        is_test = test Y/N
-        """
-        self.key = key 
-        self.user_id = user_id 
-        self.sender_phone = sender_phone 
-        self.is_test = is_test 
-
-    def send_sms(self, rec_list:list, msg_list:list, msg_type='LMS') -> int:
-        """
-        send messages (text)
-
-        * required
-        rec_list (receiver phone numbers)
-        msg_list (messages)
-        """
-        mass_send_url = 'https://apis.aligo.in/send_mass/' 
-        cnt = len(rec_list)
-        data = {
-            'key': self.key, 
-            'userid': self.user_id, 
-            'sender': self.sender_phone, 
-            'cnt' : cnt, # 메세지 전송건수(번호,메세지 매칭건수)
-            'msg_type' : msg_type, 
-            'testmode_yn' : self.is_test
-        }
-        for i in range(1, cnt+1):
-            data[f'rec_{i}'] = rec_list[i-1]
-            data[f'msg_{i}'] = msg_list[i-1]
-
-        return requests.post(mass_send_url, data=data).json()['success_cnt']
-    
-    def send_mms(self, rec:str, msg:str, image_path:str) -> int:
-        """
-        send messages (image)
-
-        * required
-        rec (receiver phone number)
-        msg (message)
-        image_path (image file)
-        """
-        send_url = 'https://apis.aligo.in/send/'
-        data = {
-            'key': self.key,
-            'userid': self.user_id,
-            'sender': self.sender_phone,
-            'receiver': rec, # 수신번호 (,활용하여 1000명까지 추가 가능)
-            'msg': msg, 
-            'msg_type' : 'MMS',
-            'testmode_yn' : self.is_test 
-        }
-        image_file = {'image' : open(image_path, 'rb')}
-
-        return requests.post(send_url, data=data, files=image_file).json()['success_cnt']
-
-
-class TwilioManager:
-    """
-    Twilio Manager
-
-    """
-
-    def __init__(self, account_sid:str, auth_token:str, from_number:str) -> None:
-        """
-        twilio config
-        account_sid ACcff1...
-        auth_token e1a1...
-        from_number +1534...
-        """
-        try:
-            from twilio.rest import Client
-        except:
-            raise ImportError('twilio module not found.\nplease enter pip install twilio')
-            
-        self.client = Client(account_sid, auth_token)
-
-        self.from_ = from_number
-        pass
-
-    def send_sms(self, to:str, msg:str):
-        """
-        send_message
-        to - receiver (+4478600..)
-        msg - message
-        """
-        message = self.client.messages.create(
-            from_ = self.from_,
-            body = msg,
-            to = to,
-        )
-
-        return message.sid
-
-if __name__ == '__main__':
-    config = {
-        'ALIGO_KEY': 'aligo-api-key',
-        'ALIGO_ID': 'aligo-user-id',
-        'ALIGO_HP': 'aligo-phone-number',
-        'ALIGO_TEST': 'Y/N'
-    }
-    aligo_mgr = AligoManager(key=config['ALIGO_KEY'], user_id=config['ALIGO_ID'], 
-                             sender_phone=config['ALIGO_HP'], is_test=config['ALIGO_TEST'])
-    
-    receiver_list = ['00012345678', '00023456789']
-    message_list = ['Test 1', 'Test 2']
-    success_count = aligo_mgr.send_sms(receiver_list, message_list)
-    print('success: %d'%success_count)
-
-    success_count = aligo_mgr.send_mms('00012345678', 'Test Image', './image.jpg')
-    print('success: %d'%success_count)
-
+import requests
+
+class AligoManager:
+    """
+    Aligo Messages API
+
+    https://smartsms.aligo.in/
+    """
+
+    def __init__(self, key, user_id, sender_phone, is_test) -> None:
+        """
+        Aligo configs
+        key = API Key
+        user_id = User ID
+        sender_phone = phone number
+        is_test = test Y/N
+        """
+        self.key = key 
+        self.user_id = user_id 
+        self.sender_phone = sender_phone 
+        self.is_test = is_test 
+
+    def send_sms(self, rec_list:list, msg_list:list, msg_type='LMS') -> int:
+        """
+        send messages (text)
+
+        * required
+        rec_list (receiver phone numbers)
+        msg_list (messages)
+        """
+        mass_send_url = 'https://apis.aligo.in/send_mass/' 
+        cnt = len(rec_list)
+        data = {
+            'key': self.key, 
+            'userid': self.user_id, 
+            'sender': self.sender_phone, 
+            'cnt' : cnt, # 메세지 전송건수(번호,메세지 매칭건수)
+            'msg_type' : msg_type, 
+            'testmode_yn' : self.is_test
+        }
+        for i in range(1, cnt+1):
+            data[f'rec_{i}'] = rec_list[i-1]
+            data[f'msg_{i}'] = msg_list[i-1]
+
+        return requests.post(mass_send_url, data=data).json()['success_cnt']
+    
+    def send_mms(self, rec:str, msg:str, image_path:str) -> int:
+        """
+        send messages (image)
+
+        * required
+        rec (receiver phone number)
+        msg (message)
+        image_path (image file)
+        """
+        send_url = 'https://apis.aligo.in/send/'
+        data = {
+            'key': self.key,
+            'userid': self.user_id,
+            'sender': self.sender_phone,
+            'receiver': rec, # 수신번호 (,활용하여 1000명까지 추가 가능)
+            'msg': msg, 
+            'msg_type' : 'MMS',
+            'testmode_yn' : self.is_test 
+        }
+        image_file = {'image' : open(image_path, 'rb')}
+
+        return requests.post(send_url, data=data, files=image_file).json()['success_cnt']
+
+
+class TwilioManager:
+    """
+    Twilio Manager
+
+    """
+
+    def __init__(self, account_sid:str, auth_token:str, from_number:str) -> None:
+        """
+        twilio config
+        account_sid ACcff1...
+        auth_token e1a1...
+        from_number +1534...
+        """
+        try:
+            from twilio.rest import Client
+        except:
+            raise ImportError('twilio module not found.\nplease enter pip install twilio')
+            
+        self.client = Client(account_sid, auth_token)
+
+        self.from_ = from_number
+        pass
+
+    def send_sms(self, to:str, msg:str):
+        """
+        send_message
+        to - receiver (+4478600..)
+        msg - message
+        """
+        message = self.client.messages.create(
+            from_ = self.from_,
+            body = msg,
+            to = to,
+        )
+
+        return message.sid
+
+if __name__ == '__main__':
+    config = {
+        'ALIGO_KEY': 'aligo-api-key',
+        'ALIGO_ID': 'aligo-user-id',
+        'ALIGO_HP': 'aligo-phone-number',
+        'ALIGO_TEST': 'Y/N'
+    }
+    aligo_mgr = AligoManager(key=config['ALIGO_KEY'], user_id=config['ALIGO_ID'], 
+                             sender_phone=config['ALIGO_HP'], is_test=config['ALIGO_TEST'])
+    
+    receiver_list = ['00012345678', '00023456789']
+    message_list = ['Test 1', 'Test 2']
+    success_count = aligo_mgr.send_sms(receiver_list, message_list)
+    print('success: %d'%success_count)
+
+    success_count = aligo_mgr.send_mms('00012345678', 'Test Image', './image.jpg')
+    print('success: %d'%success_count)
+
```

### Comparing `sosin-1.2.6/sosin/utils/currency.py` & `sosin-1.2.7/sosin/utils/currency.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import requests
-try:
-    from bs4 import BeautifulSoup
-except:
-    print('you need to install BeautifulSoup4\n$ : python -m pip install BeautifulSoup4')
-
-country_list = [
-    '미국', '유럽연합', '일본', '중국', '홍콩', '대만', '영국', '오만', '캐나다', 
-    '스위스', '스웨덴', '호주', '뉴질랜드', '체코', '칠레', '터키', '몽골', '이스라엘', 
-    '덴마크', '노르웨이', '사우디아라비아', '쿠웨이트', '바레인', '아랍에미리트', '요르단', 
-    '이집트', '태국', '싱가포르', '말레이시아', '인도네시아', '카타르', '카자흐스탄', '브루나이', 
-    '인도', '파키스탄', '방글라데시', '필리핀', '멕시코', '브라질', '베트남', '남아프리카', 
-    '러시아', '헝가리', '폴란드', '스리랑카', '알제리', '케냐', '콜롬비아', '탄자니아', 
-    '네팔', '루마니아', '리비아', '마카오', '미얀마', '에티오피아', '우즈베키스탄', '캄보디아', '피지'
-]
-
-symbols = [
-'AUD',
-'USD',
-'JPY',
-]
-
-symbol_to_name = {
-    'AUD': '호주',
-    'USD': '미국',
-    'JPY': '일본',
-}
-name_to_symbol = {
-    v: k
-    for k, v in symbol_to_name.items()
-}
-
-def get_currency(symbol):
-    symbol = symbol.upper()
-    if symbol == 'KRW'or symbol =='한국':
-        return 1.0
-    assert symbol in symbol_to_name or symbol in name_to_symbol, '유효하지 않은 symbol 입니다.'
-
-    if symbol in symbol_to_name:
-        name = symbol_to_name[symbol]
-    else:
-        name = name_to_symbol[symbol]
-    r = requests.get(f'https://www.google.com/search?q={name}환율')
-    sp = BeautifulSoup(r.text, 'html.parser')
-    return float(sp.select_one('.BNeawe.iBp4i.AP7Wnd').text.split()[0].replace(',', ''))
+import requests
+try:
+    from bs4 import BeautifulSoup
+except:
+    print('you need to install BeautifulSoup4\n$ : python -m pip install BeautifulSoup4')
+
+country_list = [
+    '미국', '유럽연합', '일본', '중국', '홍콩', '대만', '영국', '오만', '캐나다', 
+    '스위스', '스웨덴', '호주', '뉴질랜드', '체코', '칠레', '터키', '몽골', '이스라엘', 
+    '덴마크', '노르웨이', '사우디아라비아', '쿠웨이트', '바레인', '아랍에미리트', '요르단', 
+    '이집트', '태국', '싱가포르', '말레이시아', '인도네시아', '카타르', '카자흐스탄', '브루나이', 
+    '인도', '파키스탄', '방글라데시', '필리핀', '멕시코', '브라질', '베트남', '남아프리카', 
+    '러시아', '헝가리', '폴란드', '스리랑카', '알제리', '케냐', '콜롬비아', '탄자니아', 
+    '네팔', '루마니아', '리비아', '마카오', '미얀마', '에티오피아', '우즈베키스탄', '캄보디아', '피지'
+]
+
+symbols = [
+'AUD',
+'USD',
+'JPY',
+]
+
+symbol_to_name = {
+    'AUD': '호주',
+    'USD': '미국',
+    'JPY': '일본',
+}
+name_to_symbol = {
+    v: k
+    for k, v in symbol_to_name.items()
+}
+
+def get_currency(symbol):
+    symbol = symbol.upper()
+    if symbol == 'KRW'or symbol =='한국':
+        return 1.0
+    assert symbol in symbol_to_name or symbol in name_to_symbol, '유효하지 않은 symbol 입니다.'
+
+    if symbol in symbol_to_name:
+        name = symbol_to_name[symbol]
+    else:
+        name = name_to_symbol[symbol]
+    r = requests.get(f'https://www.google.com/search?q={name}환율')
+    sp = BeautifulSoup(r.text, 'html.parser')
+    return float(sp.select_one('.BNeawe.iBp4i.AP7Wnd').text.split()[0].replace(',', ''))
```

### Comparing `sosin-1.2.6/sosin/web/session.py` & `sosin-1.2.7/sosin/web/session.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.6/sosin/web/translate.py` & `sosin-1.2.7/sosin/web/translate.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import time
-try:
-    from sosin.web.virtual import VirtualDriver, By, WebDriverWait, EC
-except:
-    pass
-
-def papago(txts:list[str]) -> list[str]:
-    
-    """
-    파파고 번역기
-    """
-    webdriver = VirtualDriver()
-    webdriver.set_argument()
-    driver = webdriver.get_driver()
-    driver.execute_script("window.open('https://papago.naver.com/')")
-    time.sleep(1)
-    driver.switch_to.window(driver.window_handles[-1])
-    result = []
-    for txt in txts:
-        WebDriverWait(driver,5).until(EC.presence_of_element_located((By.ID, 'txtSource'))).send_keys(txt)
-        target_text = ''
-        while True:
-            # 충분히 번역할때까지 재확인
-            time.sleep(2)
-            if target_text == driver.find_element(By.ID, 'txtTarget').text:
-                result.append(target_text)
-                driver.find_element(By.ID, 'txtSource').clear()
-                break
-            target_text = driver.find_element(By.ID, 'txtTarget').text
-        
-    driver.quit()
+import time
+try:
+    from sosin.web.virtual import VirtualDriver, By, WebDriverWait, EC
+except:
+    pass
+
+def papago(txts:list[str]) -> list[str]:
+    
+    """
+    파파고 번역기
+    """
+    webdriver = VirtualDriver()
+    webdriver.set_argument()
+    driver = webdriver.get_driver()
+    driver.execute_script("window.open('https://papago.naver.com/')")
+    time.sleep(1)
+    driver.switch_to.window(driver.window_handles[-1])
+    result = []
+    for txt in txts:
+        WebDriverWait(driver,5).until(EC.presence_of_element_located((By.ID, 'txtSource'))).send_keys(txt)
+        target_text = ''
+        while True:
+            # 충분히 번역할때까지 재확인
+            time.sleep(2)
+            if target_text == driver.find_element(By.ID, 'txtTarget').text:
+                result.append(target_text)
+                driver.find_element(By.ID, 'txtSource').clear()
+                break
+            target_text = driver.find_element(By.ID, 'txtTarget').text
+        
+    driver.quit()
     return result
```

### Comparing `sosin-1.2.6/sosin/web/virtual.py` & `sosin-1.2.7/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.6/sosin.egg-info/PKG-INFO` & `sosin-1.2.7/sosin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.2.6
+Version: 1.2.7
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: sosincomp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

