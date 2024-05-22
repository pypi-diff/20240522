# Comparing `tmp/randombetter-1.0.2.tar.gz` & `tmp/randombetter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randombetter-1.0.2.tar", last modified: Wed May 22 18:41:17 2024, max compression
+gzip compressed data, was "randombetter-1.0.3.tar", last modified: Wed May 22 18:52:30 2024, max compression
```

## Comparing `randombetter-1.0.2.tar` & `randombetter-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.424404 randombetter-1.0.2/
--rw-rw-rw-   0        0        0      338 2024-05-22 18:41:17.423404 randombetter-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.405396 randombetter-1.0.2/randombetter/
--rw-rw-rw-   0        0        0      930 2024-05-22 18:37:40.000000 randombetter-1.0.2/randombetter/__init__.py
--rw-rw-rw-   0        0        0     3044 2024-05-22 18:38:42.000000 randombetter-1.0.2/randombetter/randomness.py
-drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.422402 randombetter-1.0.2/randombetter.egg-info/
--rw-rw-rw-   0        0        0      338 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 18:41:17.424404 randombetter-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-22 18:39:58.000000 randombetter-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:30.680082 randombetter-1.0.3/
+-rw-rw-rw-   0        0        0      338 2024-05-22 18:52:30.679082 randombetter-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:30.664923 randombetter-1.0.3/randombetter/
+-rw-rw-rw-   0        0        0      930 2024-05-22 18:37:40.000000 randombetter-1.0.3/randombetter/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-05-22 18:50:16.000000 randombetter-1.0.3/randombetter/randomness.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:52:30.678082 randombetter-1.0.3/randombetter.egg-info/
+-rw-rw-rw-   0        0        0      338 2024-05-22 18:52:30.000000 randombetter-1.0.3/randombetter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-22 18:52:30.000000 randombetter-1.0.3/randombetter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:52:30.000000 randombetter-1.0.3/randombetter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 18:52:30.000000 randombetter-1.0.3/randombetter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:52:30.680082 randombetter-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-22 18:52:26.000000 randombetter-1.0.3/setup.py
```

### Comparing `randombetter-1.0.2/randombetter/__init__.py` & `randombetter-1.0.3/randombetter/__init__.py`

 * *Files identical despite different names*

### Comparing `randombetter-1.0.2/randombetter/randomness.py` & `randombetter-1.0.3/randombetter/randomness.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         sorted.append(maxnum)
         list_to_sort.remove(maxnum)
     sorted.reverse()
     return sorted
 
 def random_password(seed: int, length: int) -> str:
     characters = string.ascii_letters + string.digits + string.punctuation
-    password = ''.join(random_choice(seed, characters) for _ in range(length))
+    password = ''.join(random_choice(seed + i, characters) for i in range(length))
     return password
 
 def random_seed() -> int:
     seed = ""
     current_time = time.time()
     current_ms = int((current_time - int(current_time)) * 1000)
     for _ in range(200):
```

