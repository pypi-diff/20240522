# Comparing `tmp/zaku-0.0.8rc1-py3-none-any.whl.zip` & `tmp/zaku-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12816 bytes, number of entries: 12
+Zip file size: 12794 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       59 b- defN 24-Apr-15 02:31 zaku/__init__.py
 -rw-r--r--  2.0 unx     3780 b- defN 24-Apr-20 20:02 zaku/base.py
--rw-r--r--  2.0 unx     6382 b- defN 24-May-12 20:47 zaku/client.py
+-rw-r--r--  2.0 unx     6469 b- defN 24-May-13 10:43 zaku/client.py
 -rw-r--r--  2.0 unx     8743 b- defN 24-Apr-19 06:33 zaku/interfaces.py
 -rw-r--r--  2.0 unx     1678 b- defN 24-Apr-14 19:38 zaku/job_queue.py
 -rw-r--r--  2.0 unx     5982 b- defN 24-Apr-18 05:38 zaku/server.py
--rw-r--r--  2.0 unx     1064 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4263 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      911 b- defN 24-May-12 20:48 zaku-0.0.8rc1.dist-info/RECORD
-12 files, 33008 bytes uncompressed, 11302 bytes compressed:  65.8%
+-rw-r--r--  2.0 unx     1064 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4260 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      893 b- defN 24-May-13 10:50 zaku-0.0.9.dist-info/RECORD
+12 files, 33074 bytes uncompressed, 11316 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: zaku/job_queue.py
 Comment: 
 
 Filename: zaku/server.py
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/LICENSE
+Filename: zaku-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/METADATA
+Filename: zaku-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/WHEEL
+Filename: zaku-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/entry_points.txt
+Filename: zaku-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/top_level.txt
+Filename: zaku-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: zaku-0.0.8rc1.dist-info/RECORD
+Filename: zaku-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zaku/client.py

```diff
@@ -199,14 +199,17 @@
         if not job_tuple:
             yield None
             return
 
         job_id, job = job_tuple
         try:
             yield job
+        except SystemExit as e:
+            self.mark_done(job_id)
+            raise e
         except Exception as e:
             self.mark_reset(job_id)
             raise e
 
         self.mark_done(job_id)
 
     def clear_queue(self):
```

## Comparing `zaku-0.0.8rc1.dist-info/LICENSE` & `zaku-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `zaku-0.0.8rc1.dist-info/METADATA` & `zaku-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zaku
-Version: 0.0.8rc1
+Version: 0.0.9
 Summary: Zaku Task Queue is for distributed ML-workloads.
 Home-page: https://github.com/geyang/zaku
 Author: Ge Yang<ge.ike.yang@gmail.com>
 Author-email: ge.ike.yang@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

## Comparing `zaku-0.0.8rc1.dist-info/RECORD` & `zaku-0.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 zaku/__init__.py,sha256=dVBFG2RyfsJ9Yf3OgSN49X6Tpk7RgfdFHyFYgs1vvjs,59
 zaku/base.py,sha256=7jgQ1Rcz6eDLNjkryDXLC9QrDWcct9fdixwHPjXd59g,3780
-zaku/client.py,sha256=muJqHpC8HBTuP6P94tlbJqN-Mw7s-FGA3EsBlLk83jM,6382
+zaku/client.py,sha256=mtc_vXUw5vxGHSIQk9BQF7DeGokNemh58d53VnXR6ss,6469
 zaku/interfaces.py,sha256=QL4_WVWMFXV3WxiBCIpEpry0Rr47RZEmnuOxanlXeus,8743
 zaku/job_queue.py,sha256=rClaiGYU6ZDSi-ehPtKbZfJcYxZaOr3DHMPfRq9jl4o,1678
 zaku/server.py,sha256=G91fCTGtwaaQiuRlpFPV7_aJq_gc0lTWTLFeCDNTeS4,5982
-zaku-0.0.8rc1.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
-zaku-0.0.8rc1.dist-info/METADATA,sha256=aoYzPfNwds5ACaInQT3ABzLginbPrQcqGB1BPBIWd6A,4263
-zaku-0.0.8rc1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-zaku-0.0.8rc1.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
-zaku-0.0.8rc1.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
-zaku-0.0.8rc1.dist-info/RECORD,,
+zaku-0.0.9.dist-info/LICENSE,sha256=ViVJUWot4p3kmGwzBBRu6vqoBFQuLFKyGIR3jzh4X_A,1064
+zaku-0.0.9.dist-info/METADATA,sha256=jY6r1owEOX88p90n4QyUbSLZ38WfKX7LrPSvB8TODYY,4260
+zaku-0.0.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+zaku-0.0.9.dist-info/entry_points.txt,sha256=OQmjyBNrqRKNAK7zutZ83SXuKvH6EURf28dG8-nPtdE,49
+zaku-0.0.9.dist-info/top_level.txt,sha256=NOH9JyYZg-VCpceLmApF5Rx3njTGe8RjuRaQsTc5k4o,5
+zaku-0.0.9.dist-info/RECORD,,
```

