# Comparing `tmp/tools_hjh-2.6.4.tar.gz` & `tmp/tools_hjh-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\tools_hjh-2.6.4.tar", last modified: Wed May 22 16:14:07 2024, max compression
+gzip compressed data, was "dist\tools_hjh-2.6.5.tar", last modified: Wed May 22 20:37:26 2024, max compression
```

## Comparing `tools_hjh-2.6.4.tar` & `tools_hjh-2.6.5.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/
--rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.4/LICENSE
--rw-rw-rw-   0        0        0      207 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/setup.cfg
--rw-rw-rw-   0        0        0      417 2024-05-22 16:13:40.000000 tools_hjh-2.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:14:05.000000 tools_hjh-2.6.4/tools_hjh/
--rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.4/tools_hjh/Chrome.py
--rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.4/tools_hjh/DBConn.py
--rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.4/tools_hjh/HTTPRequest.py
--rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.4/tools_hjh/HTTPRequest2.py
--rw-rw-rw-   0        0        0     8808 2024-04-29 21:48:40.000000 tools_hjh-2.6.4/tools_hjh/HTTPTools.py
--rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.4/tools_hjh/Log.py
--rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.4/tools_hjh/MemoryDB.py
--rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.4/tools_hjh/OracleTools.py
--rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.4/tools_hjh/SSHConn.py
--rw-rw-rw-   0        0        0     3263 2024-05-22 16:13:25.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool.py
--rw-rw-rw-   0        0        0     3051 2024-05-15 16:00:45.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool_back.py
--rw-rw-rw-   0        0        0     3104 2024-05-15 23:30:29.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool原版.py
--rw-rw-rw-   0        0        0     3392 2024-05-22 13:14:41.000000 tools_hjh-2.6.4/tools_hjh/ThreadPool新版.py
--rw-rw-rw-   0        0        0     7766 2024-05-22 13:57:46.000000 tools_hjh-2.6.4/tools_hjh/Tools.py
--rw-rw-rw-   0        0        0      539 2024-01-30 07:55:42.000000 tools_hjh-2.6.4/tools_hjh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:14:07.000000 tools_hjh-2.6.4/tools_hjh.egg-info/
--rw-rw-rw-   0        0        0        1 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-05-22 16:13:55.000000 tools_hjh-2.6.4/tools_hjh.egg-info/requires.txt
--rw-rw-rw-   0        0        0      568 2024-05-22 16:13:57.000000 tools_hjh-2.6.4/tools_hjh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 16:13:56.000000 tools_hjh-2.6.4/tools_hjh.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:37:25.000000 tools_hjh-2.6.5/
+-rw-rw-rw-   0        0        0        0 2022-05-25 02:55:28.000000 tools_hjh-2.6.5/LICENSE
+-rw-rw-rw-   0        0        0      207 2024-05-22 20:37:25.000000 tools_hjh-2.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      154 2022-11-23 09:57:04.000000 tools_hjh-2.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:37:25.000000 tools_hjh-2.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      417 2024-05-22 20:37:13.000000 tools_hjh-2.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:37:25.000000 tools_hjh-2.6.5/tools_hjh/
+-rw-rw-rw-   0        0        0     4066 2024-04-22 08:48:58.000000 tools_hjh-2.6.5/tools_hjh/Chrome.py
+-rw-rw-rw-   0        0        0     9415 2023-11-14 06:43:07.000000 tools_hjh-2.6.5/tools_hjh/DBConn.py
+-rw-rw-rw-   0        0        0     3601 2024-03-07 02:36:55.000000 tools_hjh-2.6.5/tools_hjh/HTTPRequest.py
+-rw-rw-rw-   0        0        0     3662 2024-03-13 07:44:41.000000 tools_hjh-2.6.5/tools_hjh/HTTPRequest2.py
+-rw-rw-rw-   0        0        0     8808 2024-04-29 21:48:40.000000 tools_hjh-2.6.5/tools_hjh/HTTPTools.py
+-rw-rw-rw-   0        0        0      640 2022-12-27 02:25:42.000000 tools_hjh-2.6.5/tools_hjh/Log.py
+-rw-rw-rw-   0        0        0     1536 2022-11-18 09:52:05.000000 tools_hjh-2.6.5/tools_hjh/MemoryDB.py
+-rw-rw-rw-   0        0        0    46268 2024-04-24 01:40:14.000000 tools_hjh-2.6.5/tools_hjh/OracleTools.py
+-rw-rw-rw-   0        0        0     3178 2024-05-22 20:29:34.000000 tools_hjh-2.6.5/tools_hjh/ProcessPool.py
+-rw-rw-rw-   0        0        0     2966 2023-04-07 22:41:22.000000 tools_hjh-2.6.5/tools_hjh/SSHConn.py
+-rw-rw-rw-   0        0        0     3228 2024-05-22 20:20:44.000000 tools_hjh-2.6.5/tools_hjh/ThreadPool.py
+-rw-rw-rw-   0        0        0     7766 2024-05-22 13:57:46.000000 tools_hjh-2.6.5/tools_hjh/Tools.py
+-rw-rw-rw-   0        0        0      586 2024-05-22 20:30:47.000000 tools_hjh-2.6.5/tools_hjh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:37:25.000000 tools_hjh-2.6.5/tools_hjh.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:37:22.000000 tools_hjh-2.6.5/tools_hjh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-05-22 20:37:22.000000 tools_hjh-2.6.5/tools_hjh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-05-22 20:37:22.000000 tools_hjh-2.6.5/tools_hjh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      504 2024-05-22 20:37:22.000000 tools_hjh-2.6.5/tools_hjh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 20:37:22.000000 tools_hjh-2.6.5/tools_hjh.egg-info/top_level.txt
```

### Comparing `tools_hjh-2.6.4/tools_hjh/Chrome.py` & `tools_hjh-2.6.5/tools_hjh/Chrome.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/DBConn.py` & `tools_hjh-2.6.5/tools_hjh/DBConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/HTTPRequest.py` & `tools_hjh-2.6.5/tools_hjh/HTTPRequest.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/HTTPRequest2.py` & `tools_hjh-2.6.5/tools_hjh/HTTPRequest2.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/HTTPTools.py` & `tools_hjh-2.6.5/tools_hjh/HTTPTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/Log.py` & `tools_hjh-2.6.5/tools_hjh/Log.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/MemoryDB.py` & `tools_hjh-2.6.5/tools_hjh/MemoryDB.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/OracleTools.py` & `tools_hjh-2.6.5/tools_hjh/OracleTools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/SSHConn.py` & `tools_hjh-2.6.5/tools_hjh/SSHConn.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/ThreadPool.py` & `tools_hjh-2.6.5/tools_hjh/ThreadPool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # coding:utf-8
 import time
 import threading
 from uuid import uuid1
 import eventlet
-from test.support import time_out
 
 
 def one(name):
     print(name, 'begin')
     time.sleep(3)
     print(name, 'end')
```

### Comparing `tools_hjh-2.6.4/tools_hjh/ThreadPool_back.py` & `tools_hjh-2.6.5/tools_hjh/ProcessPool.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 # coding:utf-8
 import time
 import threading
 from uuid import uuid1
-import datetime
+import eventlet
+from multiprocessing import Process
 
 
 def one(name):
     print(name, 'begin')
-    time.sleep(10)
+    time.sleep(3)
     print(name, 'end')
 
 
 def main():
-    tp = ThreadPool(2)
+    tp = ProcessPool(2)
     tp.run(one, ('1',))
     tp.run(one, ('2',))
-    tp.run(one, ('3',))
-    # tp.wait()
+    tp.wait()
 
 
-class ThreadPool():
+class ProcessPool():
     """ 维护一个线程池 """
     
     def __init__(self, size, save_result=False, while_wait_time=0.5, report=False):
         self.size = size
-        self.thread_pool = []
+        self.process_pool = []
         self.pool_status = [0]
         self.result_map = {}
         self.save_result = save_result
         self.while_wait_time = while_wait_time
         self.report = report
         
     def clear(self):
         self.pool_status = [0]
         self.result_map = {}
 
-    def run(self, func, args, kwargs={}):
+    def run(self, func, args, kwargs={}, time_out=None):
         """ 主线程命令当前线程池从空闲线程中取一个线程执行给入的方法，如果池满，则主线程等待 """
         if self.pool_status[0] < self.size:
-            thread_id = uuid1()
-            t = myThread(func, args=args, kwargs=kwargs, thread_id=thread_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result)
+            process_id = uuid1()
+            t = myProcess(func, args=args, kwargs=kwargs, process_id=process_id, pool_status=self.pool_status, result_map=self.result_map, save_result=self.save_result, time_out=time_out)
             t.start()
-            self.thread_pool.append(t)
-            return thread_id
+            self.process_pool.append(t)
+            return process_id
         else:
             while self.pool_status[0] >= self.size:
                 time.sleep(self.while_wait_time)
             return self.run(func, args, kwargs)
 
     def get_results(self):
         return self.result_map
@@ -55,46 +55,47 @@
         return self.result_map[num]
     
     def clear_result(self):
         self.result_map = {}
 
     def wait(self):
         """ 主线程等待，直到线程池不存在活动线程 """
-        '''
         while self.pool_status[0] > 0:
-            if self.report:
-                print('ThreadPool running thread num is ' + str(self.pool_status[0]))
             time.sleep(self.while_wait_time)
-        '''
-        for t in self.thread_pool:
-            if t.isAlive():
-                run_time = t.get_run_time()
-                print(run_time)
-                t.join()
+    
+    def get_running_num(self):
+        return self.pool_status[0]
 
 
-class myThread (threading.Thread):
+class myProcess (Process):
 
-    def __init__(self, func, args, kwargs, thread_id, pool_status, result_map, save_result):
-        threading.Thread.__init__(self)
+    def __init__(self, func, args, kwargs, process_id, pool_status, result_map, save_result, time_out):
+        super().__init__()
         self.func = func
         self.args = args
         self.kwargs = kwargs
-        self.thread_id = thread_id
+        self.process_id = process_id
         self.pool_status = pool_status
         self.result_map = result_map
         self.save_result = save_result
-        self.begin_time = datetime.datetime.now()
+        self.time_out = time_out
 
     def run(self):
         self.pool_status[0] = self.pool_status[0] + 1
-        result = self.func(*self.args, **self.kwargs)
-        if self.save_result:
-            self.result_map[self.thread_id] = result
-        self.pool_status[0] = self.pool_status[0] - 1
-        
-    def get_run_time(self):
-        return datetime.datetime.now() - self.begin_time
+        try:
+            if self.time_out is None:
+                result = self.func(*self.args, **self.kwargs)
+                if self.save_result:
+                    self.result_map[self.thread_id] = result
+            else:
+                # 实测效率很低
+                eventlet.monkey_patch()
+                with eventlet.Timeout(self.time_out, False):
+                    result = self.func(*self.args, **self.kwargs)
+                    if self.save_result:
+                        self.result_map[self.thread_id] = result
+        finally:
+            self.pool_status[0] = self.pool_status[0] - 1
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `tools_hjh-2.6.4/tools_hjh/Tools.py` & `tools_hjh-2.6.5/tools_hjh/Tools.py`

 * *Files identical despite different names*

### Comparing `tools_hjh-2.6.4/tools_hjh/__init__.py` & `tools_hjh-2.6.5/tools_hjh/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from tools_hjh.DBConn import QueryResults
 from tools_hjh.OracleTools import OracleTools
 from tools_hjh.MemoryDB import MemoryDB
 
 from tools_hjh.SSHConn import SSHConn
 
 from tools_hjh.ThreadPool import ThreadPool
+from tools_hjh.ProcessPool import ProcessPool
 
 from tools_hjh.HTTPRequest import HTTPRequest
 from tools_hjh.HTTPTools import HTTPTools
 
 from tools_hjh.Chrome import Chrome
 from tools_hjh.Chrome import ChromePool
 from tools_hjh.HTTPRequest2 import HTTPRequestPool
```

