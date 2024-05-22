# Comparing `tmp/randombetter-1.0.1.tar.gz` & `tmp/randombetter-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randombetter-1.0.1.tar", last modified: Tue May 21 16:06:17 2024, max compression
+gzip compressed data, was "randombetter-1.0.2.tar", last modified: Wed May 22 18:41:17 2024, max compression
```

## Comparing `randombetter-1.0.1.tar` & `randombetter-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:06:17.777547 randombetter-1.0.1/
--rw-rw-rw-   0        0        0      312 2024-05-21 16:06:17.775548 randombetter-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 16:06:17.757548 randombetter-1.0.1/randombetter/
--rw-rw-rw-   0        0        0      819 2024-05-21 15:38:42.000000 randombetter-1.0.1/randombetter/__init__.py
--rw-rw-rw-   0        0        0     2565 2024-05-21 16:05:33.000000 randombetter-1.0.1/randombetter/randomness.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:06:17.774546 randombetter-1.0.1/randombetter.egg-info/
--rw-rw-rw-   0        0        0      312 2024-05-21 16:06:17.000000 randombetter-1.0.1/randombetter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2024-05-21 16:06:17.000000 randombetter-1.0.1/randombetter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:06:17.000000 randombetter-1.0.1/randombetter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-21 16:06:17.000000 randombetter-1.0.1/randombetter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 16:06:17.777547 randombetter-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      440 2024-05-21 16:06:12.000000 randombetter-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.424404 randombetter-1.0.2/
+-rw-rw-rw-   0        0        0      338 2024-05-22 18:41:17.423404 randombetter-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.405396 randombetter-1.0.2/randombetter/
+-rw-rw-rw-   0        0        0      930 2024-05-22 18:37:40.000000 randombetter-1.0.2/randombetter/__init__.py
+-rw-rw-rw-   0        0        0     3044 2024-05-22 18:38:42.000000 randombetter-1.0.2/randombetter/randomness.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:17.422402 randombetter-1.0.2/randombetter.egg-info/
+-rw-rw-rw-   0        0        0      338 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 18:41:17.000000 randombetter-1.0.2/randombetter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:41:17.424404 randombetter-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-22 18:39:58.000000 randombetter-1.0.2/setup.py
```

### Comparing `randombetter-1.0.1/randombetter/__init__.py` & `randombetter-1.0.2/randombetter/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,10 +18,14 @@
     res = randomness.normalize_weights(weights)
     return res
 
 def shuffle(seed, list_to_shuffle: list) -> list:
     res = randomness.shuffle(seed, list_to_shuffle)
     return res
 
+def maxsplit_sort(list_to_sort: list) -> list:
+    res = randomness.maxisort(list_to_sort)
+    return res
+
 def random_seed() -> int:
     res = randomness.random_seed()
     return res
```

### Comparing `randombetter-1.0.1/randombetter/randomness.py` & `randombetter-1.0.2/randombetter/randomness.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time
+import string
 
 def random_int(seed: int, min_val, max_val) -> int:
     # Get the current time in milliseconds
     if not isinstance(max_val, int) and not isinstance(max_val, float):
         raise ValueError("max_val must be an integer or float")
     if not isinstance(min_val, int) and not isinstance(min_val, float):
         raise ValueError("min_val must be an integer or float")
@@ -59,14 +60,28 @@
     shuffled_list = lts.copy()
     n = len(shuffled_list)
     for i in range(n - 1, 0, -1):
         j = random_int(seed, 0, i)
         shuffled_list[i], shuffled_list[j] = shuffled_list[j], shuffled_list[i]
     return shuffled_list
 
+def maxisort(list_to_sort: list) -> list:
+    sorted = []
+    while list_to_sort:
+        maxnum = max(list_to_sort)
+        sorted.append(maxnum)
+        list_to_sort.remove(maxnum)
+    sorted.reverse()
+    return sorted
+
+def random_password(seed: int, length: int) -> str:
+    characters = string.ascii_letters + string.digits + string.punctuation
+    password = ''.join(random_choice(seed, characters) for _ in range(length))
+    return password
+
 def random_seed() -> int:
     seed = ""
     current_time = time.time()
     current_ms = int((current_time - int(current_time)) * 1000)
     for _ in range(200):
         check = random_int(current_ms, 0, 9)
         seed += str(check)
```

