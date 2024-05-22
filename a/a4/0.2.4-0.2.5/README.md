# Comparing `tmp/a4-0.2.4-py3-none-any.whl.zip` & `tmp/a4-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7622 bytes, number of entries: 8
+Zip file size: 7632 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx     8491 b- defN 23-Dec-18 11:01 a4/__init__.py
--rw-rw-r--  2.0 unx     4704 b- defN 23-Dec-18 11:03 a4/app.py
+-rw-rw-r--  2.0 unx     4718 b- defN 24-May-22 08:17 a4/app.py
 -rw-rw-r--  2.0 unx     1871 b- defN 24-Jan-30 06:32 a4/log.py
--rw-rw-r--  2.0 unx     1068 b- defN 24-Jan-30 06:36 a4-0.2.4.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1856 b- defN 24-Jan-30 06:36 a4-0.2.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Jan-30 06:36 a4-0.2.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 24-Jan-30 06:36 a4-0.2.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-Jan-30 06:36 a4-0.2.4.dist-info/RECORD
-8 files, 18648 bytes uncompressed, 6660 bytes compressed:  64.3%
+-rw-rw-r--  2.0 unx     1068 b- defN 24-May-22 08:18 a4-0.2.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1856 b- defN 24-May-22 08:18 a4-0.2.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-22 08:18 a4-0.2.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 24-May-22 08:18 a4-0.2.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 24-May-22 08:18 a4-0.2.5.dist-info/RECORD
+8 files, 18662 bytes uncompressed, 6670 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: a4/app.py
 Comment: 
 
 Filename: a4/log.py
 Comment: 
 
-Filename: a4-0.2.4.dist-info/LICENSE
+Filename: a4-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: a4-0.2.4.dist-info/METADATA
+Filename: a4-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: a4-0.2.4.dist-info/WHEEL
+Filename: a4-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: a4-0.2.4.dist-info/top_level.txt
+Filename: a4-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: a4-0.2.4.dist-info/RECORD
+Filename: a4-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## a4/app.py

```diff
@@ -90,15 +90,15 @@
                       '\n\n       help <command> --- print help for command'
                       '\n\n       ')
             usage += '\n       '.join(map(self.getdoc, self.cmds))
             print(usage, file=sys.stderr)
 
 
         def run(self):
-            (opts, args) = get_opts('nvV')
+            (opts, args) = get_opts('nvV', greedy=False)
             if len(args) < 1:
                 self._print_global_usage()
                 sys.exit(0)
 
             self.app.dry = opts['n']
             self.app.debug = opts['V']
             self.app.verbose = self.app.debug or opts['v']
```

## Comparing `a4-0.2.4.dist-info/LICENSE` & `a4-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `a4-0.2.4.dist-info/METADATA` & `a4-0.2.5.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a4
-Version: 0.2.4
+Version: 0.2.5
 Summary: Minimal library for command-line applications.
 Author-email: Sun Yijiang <sunyijiang@gmail.com>
 Project-URL: Homepage, https://github.com/sunyj/a4
 Project-URL: Bug Tracker, https://github.com/sunyj/a4/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

