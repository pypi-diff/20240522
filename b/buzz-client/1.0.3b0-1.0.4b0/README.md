# Comparing `tmp/buzz_client-1.0.3b0.tar.gz` & `tmp/buzz_client-1.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.0.3b0.tar", max compression
+gzip compressed data, was "buzz_client-1.0.4b0.tar", max compression
```

## Comparing `buzz_client-1.0.3b0.tar` & `buzz_client-1.0.4b0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.3b0/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.3b0/buzz_client/__init__.py
--rwxr-xr-x   0        0        0     4262 2024-05-20 13:31:49.929211 buzz_client-1.0.3b0/buzz_client/cli.py
--rw-r--r--   0        0        0     2592 2024-05-20 13:55:38.284805 buzz_client-1.0.3b0/buzz_client/client.py
--rw-r--r--   0        0        0      452 2024-05-20 13:55:28.866559 buzz_client-1.0.3b0/pyproject.toml
--rw-r--r--   0        0        0     2821 1970-01-01 00:00:00.000000 buzz_client-1.0.3b0/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-21 10:16:10.377792 buzz_client-1.0.4b0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.4b0/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     5050 2024-05-21 10:35:55.428345 buzz_client-1.0.4b0/buzz_client/cli.py
+-rw-r--r--   0        0        0     2617 2024-05-21 09:18:17.969995 buzz_client-1.0.4b0/buzz_client/client.py
+-rw-r--r--   0        0        0      452 2024-05-21 10:36:04.365363 buzz_client-1.0.4b0/pyproject.toml
+-rw-r--r--   0        0        0     2935 1970-01-01 00:00:00.000000 buzz_client-1.0.4b0/PKG-INFO
```

### Comparing `buzz_client-1.0.3b0/README.md` & `buzz_client-1.0.4b0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -10,39 +10,47 @@
 
 ```
 Buzz client
 
 Usage:
     buzz [options] list
     buzz [options] version
-    buzz [options] send <notifier> --recipient <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
+    buzz [options] send <notifier> <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
     buzz --version
 
 
 Options:
+    <notifier>                   the notifier you want to use,
+                                 you can see the available notifiers using `list` command
+
+    <recipient>                  the recipient of the notification,
+                                 must be valid for the notifier chosen
+
     -h  --help                   show this help message and exit
+
     -v --version                 show version and exit
-    -s URL --server=URL          API URL
-    -t TOKEN --token=TOKEN       API Auth token
 
-    --recipient <recipient>      the recipient of the notification,
-                                 must be valid for the notifier chosen
+    -a URL --api=URL             API URL
+
     --title <title>              the title of the notification. [default: You received a buzz]
     --severity <severity>        the severity of the message. [default: info]
                                  One of: 'info', 'success', 'warning', 'failure'
     --attach <file>              a file you want to attach to the notification
 
-    <notifier>                   the notifier you want to use,
-                                 you can see the available notifiers using `list` command
+    --format <format>            format of the message text [default: text]
+                                 One of: 'text', 'markdown', 'html'
+
 
     <body>                       Content of the notification,
                                  if not specified read from stdin
 Environment variables:
-    - BC_API         API URL, overrides command line argument
-    - BC_TOKEN       API token, overrides command line argument
+    - BUZZ_API         API URL, overrides command line argument
+
+API URL format is `http(s)://auth-token@server`
+Example: http://sesame@localhost:8000
 ```
 
 - URL is the URL of the buzzAPI, for example https://buzz.domain.com/
 - TOKEN is the authentication token of the buzzAPI instance.
 
 The other arguments are quite self explicative, but you have to bear in mind that the body of the notification:
```

#### html2text {}

```diff
@@ -1,25 +1,25 @@
 # buzz_client A client for buzzAPI ## Intro `buzz` is a client for [buzzAPI]
 (https://git.arr.lan/gitroot/devops/apps/buzz-api), a tool to send
 notifications to several services, like email, pushover, slack, teams... Syntax
 is: ``` Buzz client Usage: buzz [options] list buzz [options] version buzz
-[options] send --recipient [--title
+[options] send [--title
  ] [--attach ] [
-...] buzz --version Options: -h --help show this help message and exit -v --
-version show version and exit -s URL --server=URL API URL -t TOKEN --
-token=TOKEN API Auth token --recipient the recipient of the notification, must
-be valid for the notifier chosen --title
+...] buzz --version Options: the notifier you want to use, you can see the
+available notifiers using `list` command the recipient of the notification,
+must be valid for the notifier chosen -h --help show this help message and exit
+-v --version show version and exit -a URL --api=URL API URL --title
  the severity of the message. [default: info] One of: 'info', 'success',
-'warning', 'failure' --attach a file you want to attach to the notification the
-notifier you want to use, you can see the available notifiers using `list`
-command
+'warning', 'failure' --attach a file you want to attach to the notification --
+format format of the message text [default: text] One of: 'text', 'markdown',
+'html'
 Content of the notification, if not specified read from stdin Environment
-variables: - BC_API API URL, overrides command line argument - BC_TOKEN API
-token, overrides command line argument ``` - URL is the URL of the buzzAPI, for
-example https://buzz.domain.com/ - TOKEN is the authentication token of the
-buzzAPI instance. The other arguments are quite self explicative, but you have
-to bear in mind that the body of the notification: - can be passed on the
-command line of `buzz` like ``` buzz send email --recipient me@domain.com This
-is the content of the notification ``` - if not passed as an argument of
-`buzz`, then the content of the notification is read from standard input, for
-example ``` echo "Content of directory"; ls | buzz send --recipient
-me@domain.com ```
+variables: - BUZZ_API API URL, overrides command line argument API URL format
+is `http(s)://auth-token@server` Example: http://sesame@localhost:8000 ``` -
+URL is the URL of the buzzAPI, for example https://buzz.domain.com/ - TOKEN is
+the authentication token of the buzzAPI instance. The other arguments are quite
+self explicative, but you have to bear in mind that the body of the
+notification: - can be passed on the command line of `buzz` like ``` buzz send
+email --recipient me@domain.com This is the content of the notification ``` -
+if not passed as an argument of `buzz`, then the content of the notification is
+read from standard input, for example ``` echo "Content of directory"; ls |
+buzz send --recipient me@domain.com ```
```

### Comparing `buzz_client-1.0.3b0/buzz_client/cli.py` & `buzz_client-1.0.4b0/buzz_client/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,54 +3,54 @@
 """
 
 Buzz client
 
 Usage:
     buzz [options] list
     buzz [options] version
-    buzz [options] send <notifier> --recipient <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
+    buzz [options] send <notifier> <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
     buzz --version
 
+Arguments:
+    <notifier>                   the notifier you want to use, you can see the available notifiers using `list` command
+    <recipient>                  the recipient of the notification, must be valid for the notifier chosen
+    <body>                       Content of the notification, if not specified read from stdin
 
 Options:
+
     -h  --help                   show this help message and exit
-    -d
-    -q
 
     -v --version                 show version and exit
 
     -a URL --api=URL             API URL
-    -t TOKEN --token=TOKEN       API Auth token
 
-    --recipient <recipient>      the recipient of the notification,
-                                 must be valid for the notifier chosen
     --title <title>              the title of the notification. [default: You received a buzz]
     --severity <severity>        the severity of the message. [default: info]
                                  One of: 'info', 'success', 'warning', 'failure'
     --attach <file>              a file you want to attach to the notification
+    --format <format>            format of the message text [default: text]
+                                 One of: 'text', 'markdown', 'html'
 
-    <notifier>                   the notifier you want to use,
-                                 you can see the available notifiers using `list` command
-
-    <body>                       Content of the notification,
-                                 if not specified read from stdin
 Environment variables:
     - BUZZ_API         API URL, overrides command line argument
-    - BUZZ_TOKEN       API token, overrides command line argument
+                       API URL format is `http(s)://auth-token@server`
+                       Example: http://sesame@localhost:8000
+
 """
 import sys
 import signal
+import time
 from docopt import docopt
 from buzz_client.client import BuzzClient
 from scriptonite.configuration import Configuration
 from scriptonite.logging import Logger
 
 log = Logger(level="INFO")
 
-VERSION = "1.0.3b"
+VERSION = "1.0.4"
 
 
 def shutdown(sig, frame):
     print("\nAye, aye! See you...")
     sys.exit(0)
 
 
@@ -69,75 +69,100 @@
 
     print(header)
     print("\n".join(banner))
     print(header)
     print()
 
 
+def parse_settings(settings):
+    url = settings.api
+
+    if url:
+        scheme, rest = url.split(':', 1)
+        dirty_token, host = rest.split('@', 1)
+        token = dirty_token.replace('/', '')
+        return (token, f"{scheme}://{host}")
+    else:
+        return (None, None)
+
+
 def main():
     arguments = docopt(__doc__, version=VERSION)
 
-    if (arguments.get('--debug')):
-        print(">> arguments")
-        for k, v in arguments.items():
-            print(f"{k:15}: {str(v):20}")
-        print("")
-
     client_configuration = Configuration()
+    # Pass the `--api` argument
     client_configuration.from_mapping(
-        dict(api=arguments.get('--api'), token=arguments.get('--token')))
+        dict(api=arguments.get('--api')))
+    # Read environment variables
+    # We check if we have an `BUZZ_API` env var defined
+    # This can override the `--api` value
     client_configuration.from_environ(prefix="BUZZ")
 
-    client = BuzzClient(client_configuration)
+    # Extract token and URL from the API value
+    token, url = parse_settings(client_configuration)
 
-    if client.api is None or client.settings.token is None:
+    # Bail out on missing parameters
+    if url is None or token is None:
         print("\n** Missing values for API URL or TOKEN")
         sys.exit(2)
 
+    # Create the client
+    client = BuzzClient(url, token)
+
     # Check connection
+    # Measure round trip time
+    start = time.time()
     check = client.check()
+    rtt = int((time.time() - start) * 1000)  # in milliseconds
+
     if not check.get('api_ok'):
         print(f"\nERROR: connection to '{client.api}' failed.\n")
         sys.exit(2)
+
     if not check.get('token_ok'):
-        print(f"\nERROR: authentication failed while connecting to '{
-              client.api}'\n")
+        print(f"\nERROR: authentication failed connecting to '{client.api}'\n")
         sys.exit(3)
 
+    print(f"Connection ok [{rtt}ms]\n")
+
     if arguments.version:
+        # Show banner
         banner(client)
         sys.exit(0)
 
     if arguments.list:
+        # Show available notifiers
         print("Available notifiers")
         print("-" * len("Available notifiers"))
         for notifier in client.notifiers:
             print(notifier)
         sys.exit(0)
 
     if arguments.send:
+        # Send message
         if arguments.get('<body>'):
             body = [" ".join(arguments.get('<body>'))]  # type: ignore
         else:
             body = []
+            print("Type your message, <Ctrl-D> to end, <Ctrl-C> to send\n")
             for line in sys.stdin:
                 body.append(line)
 
         if len(body) == 0:
             print("ERROR: refusing to send an empty message\n")
             sys.exit(2)
 
         r = client.send(notifier=arguments.get('<notifier>'),  # type: ignore
-                        title=arguments.get('--title'),  # type: ignore
-                        recipient=arguments.get(
-            '--recipient'),  # type: ignore
-            body="".join(body),
-            severity=arguments.get('--severity'),  # type: ignore
-            attach=arguments.get('--attach')  # type: ignore
-        )
+                        title=arguments.get('--title'),
+                        recipient=arguments.get('<recipient>'),  # type: ignore
+                        body="".join(body),
+                        severity=arguments.get('--severity'),
+                        attach=arguments.get('--attach'),
+                        format_=arguments.get('--format')
+                        )
         print(f"{r.json().get('detail')} [{r.status_code}]")
 
-        sys.exit(int(not (r)))
+        sys.exit(int(not (r.ok)))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `buzz_client-1.0.3b0/buzz_client/client.py` & `buzz_client-1.0.4b0/buzz_client/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from functools import cached_property
 import requests
 import logging
-from scriptonite.configuration import Configuration, yaml_load
-from scriptonite.utilities import dictObj
+from scriptonite.configuration import Configuration
 from scriptonite.logging import Logger
+from typing import Union
 
 
 log = Logger(level=logging.DEBUG)
 
 
 class BuzzClient:
 
-    settings: dictObj
-
-    def __init__(self, settings) -> None:
-
-        # Load config
-        self.settings = settings
-        self.api = settings.api
-        self.headers = {'x-auth-token': self.settings.token}
+    def __init__(self, api_url: str, token: str) -> None:
+        self.api = api_url
+        self.token = token
+        self.headers = {'x-auth-token': self.token}
 
     def get(self, endpoint: str):
         response = requests.get(f"{self.api}{endpoint}",
                                 headers=self.headers)
         return response
 
     def check(self):
@@ -60,30 +56,32 @@
             return response.json().get(
                 'notifiers')
         else:
             return []
 
     def send(self, notifier: str,
              recipient: str,
-             body: str = "The body",
-             title: str = "You got a buzz",
-             severity: str = "info",
-             attach: str = ''):
+             body: str,
+             title: Union[str, None] = "You got a buzz",
+             severity: Union[str, None] = "info",
+             attach: Union[str, None] = '',
+             format_: Union[str, None] = 'text'):
 
         data = dict(recipient=recipient,
                     body=body,
                     title=title,
-                    severity=severity)
+                    severity=severity,
+                    format_=format_)
         files = {}
         if attach:
             log.debug(f"attaching {attach}...")
             files = {'attach': open(attach, 'rb')}
 
         response = requests.post(
-            f"{self.settings.api}{self.api_path}/send/{notifier}",
+            f"{self.api}{self.api_path}/send/{notifier}",
             data=data,
             files=files,
             headers=self.headers)
 
         # response.raise_for_status()
         return response
```

### Comparing `buzz_client-1.0.3b0/PKG-INFO` & `buzz_client-1.0.4b0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.0.3b0
+Version: 1.0.4b0
 Summary: A client for Buzz API
 License: GPL
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -29,39 +29,47 @@
 
 ```
 Buzz client
 
 Usage:
     buzz [options] list
     buzz [options] version
-    buzz [options] send <notifier> --recipient <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
+    buzz [options] send <notifier> <recipient> [--title <title>] [--severity <severity>] [--attach <file>] [<body>...]
     buzz --version
 
 
 Options:
+    <notifier>                   the notifier you want to use,
+                                 you can see the available notifiers using `list` command
+
+    <recipient>                  the recipient of the notification,
+                                 must be valid for the notifier chosen
+
     -h  --help                   show this help message and exit
+
     -v --version                 show version and exit
-    -s URL --server=URL          API URL
-    -t TOKEN --token=TOKEN       API Auth token
 
-    --recipient <recipient>      the recipient of the notification,
-                                 must be valid for the notifier chosen
+    -a URL --api=URL             API URL
+
     --title <title>              the title of the notification. [default: You received a buzz]
     --severity <severity>        the severity of the message. [default: info]
                                  One of: 'info', 'success', 'warning', 'failure'
     --attach <file>              a file you want to attach to the notification
 
-    <notifier>                   the notifier you want to use,
-                                 you can see the available notifiers using `list` command
+    --format <format>            format of the message text [default: text]
+                                 One of: 'text', 'markdown', 'html'
+
 
     <body>                       Content of the notification,
                                  if not specified read from stdin
 Environment variables:
-    - BC_API         API URL, overrides command line argument
-    - BC_TOKEN       API token, overrides command line argument
+    - BUZZ_API         API URL, overrides command line argument
+
+API URL format is `http(s)://auth-token@server`
+Example: http://sesame@localhost:8000
 ```
 
 - URL is the URL of the buzzAPI, for example https://buzz.domain.com/
 - TOKEN is the authentication token of the buzzAPI instance.
 
 The other arguments are quite self explicative, but you have to bear in mind that the body of the notification:
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: buzz-client Version: 1.0.3b0 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.0.4b0 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt-ng
 (>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: scriptonite (>=1.0.3,<2.0.0)
 Description-Content-Type: text/markdown # buzz_client A client for buzzAPI ##
 Intro `buzz` is a client for [buzzAPI](https://git.arr.lan/gitroot/devops/apps/
 buzz-api), a tool to send notifications to several services, like email,
 pushover, slack, teams... Syntax is: ``` Buzz client Usage: buzz [options] list
-buzz [options] version buzz [options] send --recipient [--title
+buzz [options] version buzz [options] send [--title
  ] [--attach ] [
-...] buzz --version Options: -h --help show this help message and exit -v --
-version show version and exit -s URL --server=URL API URL -t TOKEN --
-token=TOKEN API Auth token --recipient the recipient of the notification, must
-be valid for the notifier chosen --title
+...] buzz --version Options: the notifier you want to use, you can see the
+available notifiers using `list` command the recipient of the notification,
+must be valid for the notifier chosen -h --help show this help message and exit
+-v --version show version and exit -a URL --api=URL API URL --title
  the severity of the message. [default: info] One of: 'info', 'success',
-'warning', 'failure' --attach a file you want to attach to the notification the
-notifier you want to use, you can see the available notifiers using `list`
-command
+'warning', 'failure' --attach a file you want to attach to the notification --
+format format of the message text [default: text] One of: 'text', 'markdown',
+'html'
 Content of the notification, if not specified read from stdin Environment
-variables: - BC_API API URL, overrides command line argument - BC_TOKEN API
-token, overrides command line argument ``` - URL is the URL of the buzzAPI, for
-example https://buzz.domain.com/ - TOKEN is the authentication token of the
-buzzAPI instance. The other arguments are quite self explicative, but you have
-to bear in mind that the body of the notification: - can be passed on the
-command line of `buzz` like ``` buzz send email --recipient me@domain.com This
-is the content of the notification ``` - if not passed as an argument of
-`buzz`, then the content of the notification is read from standard input, for
-example ``` echo "Content of directory"; ls | buzz send --recipient
-me@domain.com ```
+variables: - BUZZ_API API URL, overrides command line argument API URL format
+is `http(s)://auth-token@server` Example: http://sesame@localhost:8000 ``` -
+URL is the URL of the buzzAPI, for example https://buzz.domain.com/ - TOKEN is
+the authentication token of the buzzAPI instance. The other arguments are quite
+self explicative, but you have to bear in mind that the body of the
+notification: - can be passed on the command line of `buzz` like ``` buzz send
+email --recipient me@domain.com This is the content of the notification ``` -
+if not passed as an argument of `buzz`, then the content of the notification is
+read from standard input, for example ``` echo "Content of directory"; ls |
+buzz send --recipient me@domain.com ```
```

