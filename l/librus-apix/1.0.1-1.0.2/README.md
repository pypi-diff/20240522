# Comparing `tmp/librus_apix-1.0.1.tar.gz` & `tmp/librus_apix-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librus_apix-1.0.1.tar", last modified: Mon May 20 16:33:59 2024, max compression
+gzip compressed data, was "librus_apix-1.0.2.tar", last modified: Wed May 22 19:08:23 2024, max compression
```

## Comparing `librus_apix-1.0.1.tar` & `librus_apix-1.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 16:33:53.000000 librus_apix-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 16:33:59.734650 librus_apix-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-20 16:33:53.000000 librus_apix-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/librus_apix/
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/announcements.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/attendance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/completed_lessons.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/grades.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/homework.py
--rw-r--r--   0 runner    (1001) docker     (127)    12374 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/student_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/timetable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-20 16:33:53.000000 librus_apix-1.0.1/librus_apix/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 16:33:59.734650 librus_apix-1.0.1/librus_apix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 16:33:59.000000 librus_apix-1.0.1/librus_apix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-20 16:33:53.000000 librus_apix-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 16:33:59.734650 librus_apix-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 16:33:53.000000 librus_apix-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:08:23.305204 librus_apix-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 19:08:20.000000 librus_apix-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 19:08:23.305204 librus_apix-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-22 19:08:20.000000 librus_apix-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:08:23.301203 librus_apix-1.0.2/librus_apix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/announcements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/attendance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/completed_lessons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/grades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/homework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12404 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/student_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6757 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/timetable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-05-22 19:08:20.000000 librus_apix-1.0.2/librus_apix/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:08:23.305204 librus_apix-1.0.2/librus_apix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 19:08:23.000000 librus_apix-1.0.2/librus_apix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-22 19:08:23.000000 librus_apix-1.0.2/librus_apix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:08:23.000000 librus_apix-1.0.2/librus_apix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 19:08:23.000000 librus_apix-1.0.2/librus_apix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:08:23.000000 librus_apix-1.0.2/librus_apix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-22 19:08:20.000000 librus_apix-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-22 19:08:23.305204 librus_apix-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:08:20.000000 librus_apix-1.0.2/setup.py
```

### Comparing `librus_apix-1.0.1/LICENSE` & `librus_apix-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/README.md` & `librus_apix-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,17 @@
   print("Sent!")
 else:
   print("Error sending a message!")
 ```
 
 ### Getting the Messages
 ```py
-from librus_apix.messages import get_recieved, message_content
+from librus_apix.messages import get_received, message_content
 
-messages = get_recieved(client, page=1)
+messages = get_received(client, page=1)
 for message in messages:
   print(message.title)
   href = message.href
   print(message_content(client, href))
 
 ```
```

### Comparing `librus_apix-1.0.1/librus_apix/__init__.py` & `librus_apix-1.0.2/librus_apix/__init__.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/announcements.py` & `librus_apix-1.0.2/librus_apix/announcements.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/attendance.py` & `librus_apix-1.0.2/librus_apix/attendance.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/client.py` & `librus_apix-1.0.2/librus_apix/client.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/completed_lessons.py` & `librus_apix-1.0.2/librus_apix/completed_lessons.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/exceptions.py` & `librus_apix-1.0.2/librus_apix/exceptions.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/grades.py` & `librus_apix-1.0.2/librus_apix/grades.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/helpers.py` & `librus_apix-1.0.2/librus_apix/helpers.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/homework.py` & `librus_apix-1.0.2/librus_apix/homework.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/messages.py` & `librus_apix-1.0.2/librus_apix/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
         # Send a message
         title = "Test Message"
         content = "This is a test message."
         recipient_ids = list(recipients.values())
         success, result_message = send_message(client, title, content, recipient_ids)
 
-        # Get recieved/sent messages
+        # Get received/sent messages
         messages = get_sent(client, page=1)
-        messages = get_recieved(client, page=1)
+        messages = get_received(client, page=1)
         ...
         # Retrieve content of a message
         for message in messages:
             content = message_content(client, message.href)
             ...
     ```
 """
@@ -303,15 +303,15 @@
         message_data: List[Tag] = td.find_all("td")
         if len(message_data) < 6:
             raise ParseError("Message data has less than 6 elements")
         _tick, attachment, author, title, date, _trash = message_data[:6]
         if attachment.find("img"):
             hasAttachment = True
         style = title.get("style")
-        if not isinstance(style, List):
+        if not isinstance(style, List) or not isinstance(style, str):
             style = []
         if "font-weight: bold" in style:
             unread = True
 
         author_a = author.find("a")
         href = ""
         if isinstance(author_a, Tag):
@@ -347,15 +347,15 @@
             return 0
         max_pages_number = int(max_pages_re.group(0).replace("z", ""))
     except:
         raise ParseError("Error while trying to get max page number.")
     return max_pages_number - 1
 
 
-def get_recieved(client: Client, page: int) -> List[Message]:
+def get_received(client: Client, page: int) -> List[Message]:
     """
     Retrieves received messages from a specific page.
 
     Args:
         client (Client): The client object for making HTTP requests.
         page (int): The page number of messages to retrieve.
 
@@ -364,16 +364,16 @@
     """
     payload = {
         "numer_strony105": page,
         "porcjowanie_pojemnik105": "105",
     }
     response = client.post(client.MESSAGE_URL, data=payload)
     soup = no_access_check(BeautifulSoup(response.text, "lxml"))
-    recieved_msgs = parse(soup)
-    return recieved_msgs
+    received_msgs = parse(soup)
+    return received_msgs
 
 
 def get_sent(client: Client, page: int) -> List[Message]:
     """
     Retrieves sent messages from a specific page.
 
     Args:
@@ -385,9 +385,9 @@
     """
     payload = {
         "numer_strony105": page,
         "porcjowanie_pojemnik105": "105",
     }
     response = client.post(client.SEND_MESSAGE_URL, data=payload)
     soup = no_access_check(BeautifulSoup(response.text, "lxml"))
-    recieved_msgs = parse_sent(soup)
-    return recieved_msgs
+    received_msgs = parse_sent(soup)
+    return received_msgs
```

### Comparing `librus_apix-1.0.1/librus_apix/notifications.py` & `librus_apix-1.0.2/librus_apix/notifications.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/schedule.py` & `librus_apix-1.0.2/librus_apix/schedule.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/student_information.py` & `librus_apix-1.0.2/librus_apix/student_information.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/timetable.py` & `librus_apix-1.0.2/librus_apix/timetable.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix/urls.py` & `librus_apix-1.0.2/librus_apix/urls.py`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/librus_apix.egg-info/SOURCES.txt` & `librus_apix-1.0.2/librus_apix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librus_apix-1.0.1/setup.cfg` & `librus_apix-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [darglint]
 strictness = long
 docstring_style = google
 
 [metadata]
 name = librus_apix
-version = v1.0.1
+version = v1.0.2
 license = MIT
 description = Web Scraper for Librus Synergia
 long_description = ""
 author = Pascal Jodłowski
 url = https://github.com/poroknights/librus-apix
 keywords = librus, scraper, api, synergia
 classifiers =
```

