# Comparing `tmp/tools_hjh-2.6.3.tar.gz` & `tmp/tools_hjh-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.6.3.tar", last modified: Wed Apr 24 01:51:43 2024, max compression
+gzip compressed data, was "dist\tools_hjh-2.6.4.tar", last modified: Wed May 22 16:14:07 2024, max compression
```

## Comparing `tools_hjh-2.6.3.tar` & `tools_hjh-2.6.4.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.3/LICENSE
--rw-rw-rw-   0        0        0      207 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-04-24 01:51:25.000000 tools_hjh-2.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 01:51:42.000000 tools_hjh-2.6.3/tools_hjh/
--rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.3/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.3/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.3/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.3/tools_hjh/HTTPRequest2.py
--rw-rw-rw-   0        0        0     9183 2024-03-13 12:45:59.000000 tools_hjh-2.6.3/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.3/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.3/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.3/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.3/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     2092 2024-03-13 06:16:36.000000 tools_hjh-2.6.3/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     7061 2024-04-22 05:04:03.000000 tools_hjh-2.6.3/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.3/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 01:51:43.000000 tools_hjh-2.6.3/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      479 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 01:51:40.000000 tools_hjh-2.6.3/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.4/LICENSE
+-rw-rw-rw-   0        0        0      207 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-05-22 16:13:40.000000 tools_hjh-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:14:05.000000 tools_hjh-2.6.4/tools_hjh/
+-rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.4/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.4/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.4/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.4/tools_hjh/HTTPRequest2.py
+-rw-rw-rw-   0        0        0     8808 2024-04-29 21:48:40.000000 tools_hjh-2.6.4/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.4/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.4/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.4/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.4/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     3263 2024-05-22 16:13:25.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     3051 2024-05-15 16:00:45.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool_back.py
+-rw-rw-rw-   0        0        0     3104 2024-05-15 23:30:29.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool原版.py
+-rw-rw-rw-   0        0        0     3392 2024-05-22 13:14:41.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool新版.py
+-rw-rw-rw-   0        0        0     7766 2024-05-22 13:57:46.000000 tools_hjh-2.6.4/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.4/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      568 2024-05-22 16:13:57.000000 tools_hjh-2.6.4/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 16:13:56.000000 tools_hjh-2.6.4/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.6.3/tools_hjh/Chrome.py` & `tools_hjh-2.6.4/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/DBConn.py` & `tools_hjh-2.6.4/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/HTTPRequest.py` & `tools_hjh-2.6.4/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/HTTPRequest2.py` & `tools_hjh-2.6.4/tools_hjh/HTTPRequest2.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/HTTPTools.py` & `tools_hjh-2.6.4/tools_hjh/HTTPTools.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from tools_hjh.Tools import mkdir, rm
 from tools_hjh.ThreadPool import ThreadPool
 import os
 
     
 def main():
     headers = {
-        'cookie':'_pk_id.1.88f4=e133b997b9baa0a0.1699604120.; _pk_ref.1.88f4=%5B%22%22%2C%22%22%2C1705329658%2C%22https%3A%2F%2Facg1.xyz%2F%22%5D; b2_token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJodHRwczpcL1wvZmgteHkubmV0IiwiaWF0IjoxNzA1ODE0NzQ3LCJuYmYiOjE3MDU4MTQ3NDcsImV4cCI6MTcwNzcxNTU0NywiZGF0YSI6eyJ1c2VyIjp7ImlkIjoiMzAyMiJ9fX0.UX60IEj7dLZZmGUFdqL5A-J1DfOgFEiqHiiwCRK7dKs; cf_clearance=rwsFkkA7UMCeLWtw1e2CDky77adK7RvN4E5t5SYFTJQ-1705861563-1-AfyTd9qCAJdI1zqAkvgIWkarB52DdHDcB5GqtEIMbmSeJUe4GD4tGGpcLNuFAaK5FYZ9ElYhUaDA/EtGdDXPuHA=; b2_back_url=https://fh-xy.net/gold',
+        'cookie':'cf_clearance=ZyXhlDX.MEsAT8edtS9fzDZpnwDpDBgN8jzhq4uzQHY-1714422048-1.0.1.1-gMVkjl718OqgU4CMIWop9tl4WCWpgYdT3aizn70Z0z905jYV.zSYdAwMg1OScze8BsMUQtkcdNJ3GtfT0m3ZMA; csrftoken=ZgclpVKZTiRpWHRhF0OOeTdSlU5odAJsyWq2a37iNNizZykV4w2XAhL9VOWW7hIT',
         'accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
         'accept-language': 'zh-CN,zh;q=0.9',
         'cache-control': 'no-cache',
         'cookie':'',
         'dnt': '1',
         'pragma': 'no-cache',
         'sec-ch-ua': '".Not/A)Brand";v="99", "Google Chrome";v="103", "Chromium";v="103"',
         'sec-ch-ua-mobile': '?0',
         'sec-ch-ua-platform': '"Windows"',
         'Referer': 'https://avbebe.com/',
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/103.0.0.0 Safari/537.36'
     }
     # size = HTTPTools.get_size(url='https://v.avgigi.com/acg/watch/198910.mp4', headers=headers)
     # size = HTTPTools.download(url='https://www.bixiashuku.com/modules/article/txtarticle.php?id=87850', filepath='D:/1.txt', headers=headers, retry_until_success=True)
-    size = HTTPTools.get_size(url='https://www.bixiashuku.com/modules/article/txtarticle.php?id=87850')
+    size = HTTPTools.get(url='https://nhentai.net/')
     print(size)
 
 
 class HTTPTools():
     
     @staticmethod
     def get_page(url, headers=None, data=None, proxies=None, encoding='UTF-8', timeout=None, stream=True, allow_redirects=True, verify=False, retry_until_success=False):
```

### Comparing `tools_hjh-2.6.3/tools_hjh/Log.py` & `tools_hjh-2.6.4/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/MemoryDB.py` & `tools_hjh-2.6.4/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/OracleTools.py` & `tools_hjh-2.6.4/tools_hjh/OracleTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/SSHConn.py` & `tools_hjh-2.6.4/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.3/tools_hjh/ThreadPool.py` & `tools_hjh-2.6.4/tools_hjh/ThreadPool原版.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,99 @@
 # coding:utf-8
 import time
 import threading
 from uuid import uuid1
+import eventlet
+
+
+def one(name):
+    print(name, 'begin')
+    time.sleep(10)
+    print(name, 'end')
+
+
+def main():
+    tp = ThreadPool(2)
+    tp.run(one, ('1',))
+    tp.run(one, ('2',))
+    tp.run(one, ('3',))
+    # tp.wait()
 
 
 class ThreadPool():
     """ 维护一个线程池 """
     
-    def __init__(self, size, save_result=False):
+    def __init__(self, size, save_result=False, while_wait_time=0.5, report=False):
         self.size = size
+        self.thread_pool = []
         self.pool_status = [0]
         self.result_map = {}
         self.save_result = save_result
+        self.while_wait_time = while_wait_time
+        self.report = report
         
     def clear(self):
         self.pool_status = [0]
         self.result_map = {}
 
-    def run(self, func, args, kwargs={}):
+    def run(self, func, args, kwargs={}, time_out=None):
         """ 主线程命令当前线程池从空闲线程中取一个线程执行给入的方法，如果池满，则主线程等待 """
         if self.pool_status[0] < self.size:
             thread_id = uuid1()
-            t = myThread(func, args=args, kwargs=kwargs, thread_id=thread_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result)
+            t = myThread(func, args=args, kwargs=kwargs, thread_id=thread_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result, time_out=time_out)
             t.start()
+            self.thread_pool.append(t)
             return thread_id
         else:
             while self.pool_status[0] >= self.size:
-                time.sleep(0.5)
+                time.sleep(self.while_wait_time)
             return self.run(func, args, kwargs)
 
     def get_results(self):
         return self.result_map
     
     def get_result(self, num):
         return self.result_map[num]
     
     def clear_result(self):
         self.result_map = {}
 
     def wait(self):
         """ 主线程等待，直到线程池不存在活动线程 """
         while self.pool_status[0] > 0:
-            time.sleep(0.5)
+            time.sleep(self.while_wait_time)
+    
+    def get_running_num(self):
+        return self.pool_status[0]
 
 
 class myThread (threading.Thread):
 
-    def __init__(self, func, args, kwargs, thread_id, pool_status, result_map, save_result):
+    def __init__(self, func, args, kwargs, thread_id, pool_status, result_map, save_result, time_out):
         threading.Thread.__init__(self)
+        threading.Thread.daemon = True
         self.func = func
         self.args = args
         self.kwargs = kwargs
         self.thread_id = thread_id
         self.pool_status = pool_status
         self.result_map = result_map
         self.save_result = save_result
+        self.time_out = time_out
 
     def run(self):
         self.pool_status[0] = self.pool_status[0] + 1
-        result = self.func(*self.args, **self.kwargs)
-        if self.save_result:
-            self.result_map[self.thread_id] = result
+        if self.time_out is None:
+            result = self.func(*self.args, **self.kwargs)
+            if self.save_result:
+                self.result_map[self.thread_id] = result
+        else:
+            eventlet.monkey_patch()
+            with eventlet.Timeout(self.time_out, False):
+                result = self.func(*self.args, **self.kwargs)
+                if self.save_result:
+                    self.result_map[self.thread_id] = result
         self.pool_status[0] = self.pool_status[0] - 1
 
+
+if __name__ == '__main__':
+    main()
```

### Comparing `tools_hjh-2.6.3/tools_hjh/Tools.py` & `tools_hjh-2.6.4/tools_hjh/Tools.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # coding:utf-8
 import time
 import os
+import cv2
 
 
 def main():
-    pass
+    get_pic_by_text(r'U:\1.png', 'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA')
+
+
+def get_pic_by_text(file_path, text, pic_size=(500, 500), color='white'):
+    from PIL import Image
+    img = Image.new('RGB', pic_size, color=color)
+    img.save(file_path)
+    img.close()
 
 
 def locattime():
     """ 返回当前时间，格式%Y-%m-%d %H:%M:%S """
     return time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
 
 
@@ -125,15 +133,15 @@
 def zip_folder(zip_folder_path, out_file_path):
     """ 压缩指定文件夹
     :param zip_folder_path: 目标文件夹路径
     :param out_file_path: 压缩文件保存路径+xxxx.zip
     :return: 无
     """
     import zipfile
-    zip_ = zipfile.ZipFile(out_file_path, "w", zipfile.ZIP_DEFLATED)
+    zip_ = zipfile.ZipFile(out_file_path, mode="w", compression=zipfile.ZIP_DEFLATED, allowZip64=True)
     for path, _, filenames in os.walk(zip_folder_path):
         # 去掉目标跟路径，只对目标文件夹下边的文件及文件夹进行压缩
         fpath = path.replace(zip_folder_path, '')
 
         for filename in filenames:
             zip_.write(os.path.join(path, filename), os.path.join(fpath, filename))
     zip_.close()
@@ -170,14 +178,16 @@
         else:
             str_ = str_ + str1 + ' ' * (strlennum - len(str1) + 1) + str2 + '\n'
     return str_.strip()
 
 
 def pictures_folder_2_pdf(source_path, target_pdf):
     from PIL import Image
+    from PIL import ImageFile
+    ImageFile.LOAD_TRUNCATED_IMAGES = True
     files = os.listdir(source_path)
     pic_files = []
     for file in files:
         if file.endswith('.jpg') or file.endswith('.png'):
             file = source_path + '/' + file
             pic_files.append(file)
     pic_files.sort()
@@ -186,18 +196,27 @@
     sources = []
     for file in pic_files:
         png_file = Image.open(file)
         if png_file.mode != "RGB":
             png_file = png_file.convert("RGB")
         sources.append(png_file)    
         
-    outFDF.save(target_pdf, "pdf", save_all=True, append_images=sources)
+    outFDF.save(target_pdf, "pdf", save_all=True, append_images=sources, optimize=True, progressive=True)
     sources.clear()
 
 
+def repair_img(root_path):
+    import cv2
+    for fileName in os.listdir(root_path):
+        file_path = os.path.join(root_path, fileName)
+        img = cv2.imread(file_path)
+        new_path = os.path.join(root_path, fileName)
+        cv2.imwrite(new_path, img)
+
+
 def remove_leading_space(str1):
     """ 每行去掉首尾的空格换行等字符后，再接回去 """
     str2 = ''
     for line in str1.split('\n'):
         str2 = str2 + line.strip() + '\n'
     return str2.strip('\n')
```

### Comparing `tools_hjh-2.6.3/tools_hjh/__init__.py` & `tools_hjh-2.6.4/tools_hjh/__init__.py`

 * *Files identical despite different names*

