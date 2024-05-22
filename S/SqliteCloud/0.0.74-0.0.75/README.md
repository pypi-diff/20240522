# Comparing `tmp/sqlitecloud-0.0.74.tar.gz` & `tmp/sqlitecloud-0.0.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlitecloud-0.0.74.tar", last modified: Thu May 16 16:04:41 2024, max compression
+gzip compressed data, was "sqlitecloud-0.0.75.tar", last modified: Wed May 22 13:34:25 2024, max compression
```

## Comparing `sqlitecloud-0.0.74.tar` & `sqlitecloud-0.0.75.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/README-PYPI.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/SqliteCloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 16:04:41.000000 sqlitecloud-0.0.74/SqliteCloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 16:04:38.000000 sqlitecloud-0.0.74/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/sqlitecloud/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/conn_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/resultset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/sqlitecloud/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:41.335042 sqlitecloud-0.0.74/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22271 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-16 16:04:37.000000 sqlitecloud-0.0.74/tests/integration/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/README-PYPI.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/SqliteCloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 13:34:25.000000 sqlitecloud-0.0.75/SqliteCloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 13:34:22.000000 sqlitecloud-0.0.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/sqlitecloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/conn_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/resultset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/sqlitecloud/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:25.108926 sqlitecloud-0.0.75/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23341 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-22 13:34:20.000000 sqlitecloud-0.0.75/tests/integration/test_upload.py
```

### Comparing `sqlitecloud-0.0.74/README-PYPI.md` & `sqlitecloud-0.0.75/README-PYPI.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,23 +9,20 @@
 
 You can install SqliteCloud Package using Python Package Index (PYPI):
 
 ```bash
 $ pip install SqliteCloud
 ```
 
-- Follow the instructions reported here https://github.com/sqlitecloud/sdk/tree/master/C to build the driver.
-
-- Set SQLITECLOUD_DRIVER_PATH environment variable to the path of the driver file build.
-
 ## Usage
 <hr>
 
 ```python
-from sqlitecloud.client import SqliteCloudClient, SqliteCloudAccount
+from sqlitecloud.client import SqliteCloudClient
+from sqlitecloud.types import SqliteCloudAccount
 ```
 
 ### _Init a connection_
 
 #### Using explicit configuration
 
 ```python
@@ -41,17 +38,16 @@
 client = SqliteCloudClient(cloud_account=account)
 conn = client.open_connection()
 ```
 
 ### _Execute a query_
 You can bind values to parametric queries: you can pass parameters as positional values in an array
 ```python
-result = client.exec_statement(
-    "SELECT * FROM table_name WHERE id = ?",
-    [1],
+result = client.exec_query(
+    "SELECT * FROM table_name WHERE id = 1"
     conn=conn
 )
 ```
 
 ### _Iterate result_
 result is an iterable object
 ```python
```

### Comparing `sqlitecloud-0.0.74/setup.py` & `sqlitecloud-0.0.75/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,31 +14,31 @@
         full_path = os.path.join(base_path, f'../{filename}')
         with io.open(full_path, encoding='utf-8') as file:
             return file.read()
 
 
 setup(
     name='SqliteCloud',
-    version='0.0.74',
-    author='Sam Reghenzi & Matteo Fredi',
+    version='0.0.75',
+    author='sqlitecloud.io',
     description='A Python package for working with SQLite databases in the cloud.',
     long_description=read_file('README-PYPI.md'),
     long_description_content_type='text/markdown',
     url="https://github.com/sqlitecloud/python",
     packages=find_packages(),
     install_requires=[
-        'mypy == 1.6.1',
-        'mypy-extensions == 1.0.0',
-        'typing-extensions == 4.8.0',
-        'black == 23.7.0',
-        'python-dotenv == 1.0.0',
+        'lz4 == 3.1.10',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     license='MIT',
 )
```

### Comparing `sqlitecloud-0.0.74/sqlitecloud/client.py` & `sqlitecloud-0.0.75/sqlitecloud/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,23 +21,24 @@
 
     SQLITE_DEFAULT_PORT = 8860
 
     def __init__(
         self,
         cloud_account: Optional[SqliteCloudAccount] = None,
         connection_str: Optional[str] = None,
-        # pub_subs: SQCloudPubSubCallback = [],
     ) -> None:
         """Initializes a new instance of the class with connection information.
 
         Args:
-            connection_str (str): The connection string for the database.
+            cloud_account (SqliteCloudAccount): The account information for the SQlite Cloud database.
+            connection_str (str): The connection string for the SQlite Cloud database.
+                Eg: sqlitecloud://user:pass@host.com:port/dbname?timeout=10&apikey=abcd123
 
         """
-        self.driver = Driver()
+        self._driver = Driver()
 
         self.config = SQCloudConfig()
 
         if connection_str:
             self.config = self._parse_connection_string(connection_str)
         elif cloud_account:
             self.config.account = cloud_account
@@ -49,54 +50,61 @@
 
         Returns:
             SQCloudConnect: An instance of the SQCloudConnect class representing the connection to the SQCloud server.
 
         Raises:
             SQCloudException: If an error occurs while opening the connection.
         """
-        connection = self.driver.connect(
+        connection = self._driver.connect(
             self.config.account.hostname, self.config.account.port, self.config
         )
 
         return connection
 
     def disconnect(self, conn: SQCloudConnect) -> None:
         """Close the connection to the database."""
-        self.driver.disconnect(conn)
+        self._driver.disconnect(conn)
+
+    def is_connected(self, conn: SQCloudConnect) -> bool:
+        """Check if the connection is still open.
+
+        Args:
+            conn (SQCloudConnect): The connection to the database.
+
+        Returns:
+            bool: True if the connection is open, False otherwise.
+        """
+        return self._driver.is_connected(conn)
 
     def exec_query(
-        self, query: str, conn: SQCloudConnect = None
+        self, query: str, conn: SQCloudConnect
     ) -> SqliteCloudResultSet:
         """Executes a SQL query on the SQLite Cloud database.
 
         Args:
             query (str): The SQL query to be executed.
 
         Returns:
             SqliteCloudResultSet: The result set of the executed query.
-        """
-        provided_connection = conn is not None
-        if not provided_connection:
-            conn = self.open_connection()
-
-        result = self.driver.execute(query, conn)
 
-        if not provided_connection:
-            self.disconnect(conn)
+        Raises:
+            SQCloudException: If an error occurs while executing the query.
+        """
+        result = self._driver.execute(query, conn)
 
         return SqliteCloudResultSet(result)
 
     def sendblob(self, blob: bytes, conn: SQCloudConnect) -> SqliteCloudResultSet:
         """Sends a blob to the SQLite database.
 
         Args:
             blob (bytes): The blob to be sent to the database.
             conn (SQCloudConnect): The connection to the database.
         """
-        return self.driver.sendblob(blob, conn)
+        return self._driver.send_blob(blob, conn)
 
     def _parse_connection_string(self, connection_string) -> SQCloudConfig:
         # URL STRING FORMAT
         # sqlitecloud://user:pass@host.com:port/dbname?timeout=10&key2=value2&key3=value3
         # or sqlitecloud://host.sqlite.cloud:8860/dbname?apikey=zIiAARzKm9XBVllbAzkB1wqrgijJ3Gx0X5z1A4m4xBA
 
         config = SQCloudConfig()
```

### Comparing `sqlitecloud-0.0.74/sqlitecloud/driver.py` & `sqlitecloud-0.0.75/sqlitecloud/driver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,124 @@
+from io import BufferedReader, BufferedWriter
+import logging
+import select
 import ssl
-from typing import Optional, Union
+import threading
+from typing import Callable, Optional, Union
 import lz4.block
-from sqlitecloud.resultset import SQCloudResult
+from sqlitecloud.resultset import SQCloudResult, SqliteCloudResultSet
 from sqlitecloud.types import (
     SQCLOUD_CMD,
+    SQCLOUD_DEFAULT,
     SQCLOUD_INTERNAL_ERRCODE,
+    SQCLOUD_RESULT_TYPE,
     SQCLOUD_ROWSET,
     SQCloudConfig,
     SQCloudConnect,
     SQCloudException,
     SQCloudNumber,
     SQCloudRowsetSignature,
     SQCloudValue,
 )
 import socket
 
 
 class Driver:
+    SQCLOUD_DEFAULT_UPLOAD_SIZE = 512 * 1024
+
     def __init__(self) -> None:
         # Used while parsing chunked rowset
         self._rowset: SQCloudResult = None
 
     def connect(
         self, hostname: str, port: int, config: SQCloudConfig
     ) -> SQCloudConnect:
         """
-        Connects to the SQLite Cloud server.
+        Connect to the SQLite Cloud server.
 
         Args:
             hostname (str): The hostname of the server.
             port (int): The port number of the server.
             config (SQCloudConfig): The configuration for the connection.
 
         Returns:
             SQCloudConnect: The connection object.
 
         Raises:
-            SQCloudException: If an error occurs while initializing the socket.
+            SQCloudException: If an error occurs while connecting the socket.
+        """
+        sock = self._internal_connect(hostname, port, config)
+
+        connection = SQCloudConnect()
+        connection.config = config
+        connection.socket = sock
+
+        self._internal_config_apply(connection, config)
+
+        return connection
+
+    def disconnect(self, conn: SQCloudConnect, only_main_socket: bool = False) -> None:
+        """
+        Disconnect from the SQLite Cloud server.
+        """
+        try:
+            if conn.socket:
+                conn.socket.close()
+            if not only_main_socket and conn.pubsub_socket:
+                conn.pubsub_socket.close()
+        except Exception:
+            pass
+        finally:
+            conn.socket = None
+            if not only_main_socket:
+                conn.pubsub_socket = None
+
+    def execute(self, command: str, connection: SQCloudConnect) -> SQCloudResult:
+        """
+        Execute a query on the SQLite Cloud server.
+        """
+        return self._internal_run_command(connection, command)
+
+    def send_blob(self, blob: bytes, conn: SQCloudConnect) -> SQCloudResult:
+        """
+        Send a blob to the SQLite Cloud server.
+        """
+        try:
+            conn.isblob = True
+            return self._internal_run_command(conn, blob)
+        finally:
+            conn.isblob = False
+
+    def is_connected(
+        self, connection: SQCloudConnect, main_socket: bool = True
+    ) -> bool:
+        """
+        Check if the connection is still open.
+        """
+        sock = connection.socket if main_socket else connection.pubsub_socket
+
+        if not sock:
+            return False
+        try:
+            sock.sendall(b"")
+        except OSError:
+            return False
+
+        return True
+
+    def _internal_connect(
+        self, hostname: str, port: int, config: SQCloudConfig
+    ) -> socket:
+        """
+        Create a socket connection to the SQLite Cloud server.
         """
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.settimeout(config.connect_timeout)
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
+        sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if not config.insecure:
             context = ssl.create_default_context(cafile=config.root_certificate)
             if config.certificate:
                 context.load_cert_chain(
                     certfile=config.certificate, keyfile=config.certificate_key
                 )
@@ -55,44 +130,251 @@
 
         try:
             sock.connect((hostname, port))
         except Exception as e:
             errmsg = f"An error occurred while initializing the socket."
             raise SQCloudException(errmsg) from e
 
-        connection = SQCloudConnect()
-        connection.socket = sock
-        connection.config = config
+        return sock
 
-        self._internal_config_apply(connection, config)
+    def _internal_reconnect(self, buffer: bytes) -> bool:
+        return True
 
-        return connection
+    def _internal_setup_pubsub(self, connection: SQCloudConnect, buffer: bytes) -> bool:
+        """
+        Prepare the connection for PubSub.
+        Opens a new specific socket and starts the thread to listen for incoming messages.
+        """
+        if self.is_connected(connection, False):
+            return True
+
+        if connection.pubsub_callback is None:
+            raise SQCloudException(
+                "A callback function must be provided to setup the PubSub connection."
+            )
+
+        connection.pubsub_socket = self._internal_connect(
+            connection.config.account.hostname,
+            connection.config.account.port,
+            connection.config,
+        )
+
+        self._internal_run_command(connection, buffer, False)
+        thread = threading.Thread(
+            target=self._internal_pubsub_thread, args=(connection,)
+        )
+        # kill the thread when the main one is terminated
+        thread.daemon = True
+        thread.start()
+        connection.pubsub_thread = thread
+
+        return True
+
+    def _internal_pubsub_thread(self, connection: SQCloudConnect) -> None:
+        blen = 2048
+        buffer: bytes = b""
 
-    def disconnect(self, conn: SQCloudConnect):
         try:
-            if conn.socket:
-                conn.socket.close()
+            while True:
+                tread = 0
+
+                try:
+                    if not connection.pubsub_socket:
+                        logging.info("PubSub socket dismissed.")
+                        break
+
+                    # wait for the socket to be readable (no timeout)
+                    ready_to_read, _, errors = select.select(
+                        [connection.pubsub_socket], [], []
+                    )
+                    # eg, no data to read
+                    if len(ready_to_read) == 0:
+                        continue
+                    # eg, if the socket is closed
+                    if len(errors) > 0:
+                        break
+
+                    data = connection.pubsub_socket.recv(blen)
+                    if not data:
+                        logging.info("PubSub connection closed.")
+                        break
+                except Exception as e:
+                    logging.error(
+                        f"An error occurred while reading data: {SQCLOUD_INTERNAL_ERRCODE.NETWORK.value} ({e})."
+                    )
+                    break
+
+                nread = len(data)
+                tread += nread
+                blen -= nread
+                buffer += data
+
+                sqcloud_number = self._internal_parse_number(buffer)
+                clen = sqcloud_number.value
+                if clen == 0:
+                    continue
+
+                # check if read is complete
+                # clen is the lenght parsed in the buffer
+                # cstart is the index of the first space
+                cstart = sqcloud_number.cstart
+                if clen + cstart != tread:
+                    continue
+
+                result = self._internal_parse_buffer(connection, buffer, tread)
+                if result.tag == SQCLOUD_RESULT_TYPE.RESULT_STRING:
+                    result.tag = SQCLOUD_RESULT_TYPE.RESULT_JSON
+
+                connection.pubsub_callback(
+                    connection, SqliteCloudResultSet(result), connection.pubsub_data
+                )
+        except Exception as e:
+            logging.error(f"An error occurred while parsing data: {e}.")
+
         finally:
-            conn.socket = None
+            connection.pubsub_callback(connection, None, connection.pubsub_data)
 
-    def execute(self, command: str, connection: SQCloudConnect) -> SQCloudResult:
-        return self._internal_run_command(connection, command)
+    def upload_database(
+        self,
+        connection: SQCloudConnect,
+        dbname: str,
+        key: Optional[str],
+        is_file_transfer: bool,
+        snapshot_id: int,
+        is_internal_db: bool,
+        fd: BufferedReader,
+        dbsize: int,
+        xCallback: Callable[[BufferedReader, int, int, int], bytes],
+    ) -> None:
+        """
+        Uploads a database to the server.
 
-    def sendblob(self, blob: bytes, conn: SQCloudConnect) -> SQCloudResult:
+        Args:
+            connection (SQCloudConnect): The connection object to the SQLite Cloud server.
+            dbname (str): The name of the database to upload.
+            key (Optional[str]): The encryption key for the database, if applicable.
+            is_file_transfer (bool): Indicates whether the database is being transferred as a file.
+            snapshot_id (int): The ID of the snapshot to upload.
+            is_internal_db (bool): Indicates whether the database is an internal database.
+            fd (BufferedReader): The file descriptor of the database file.
+            dbsize (int): The size of the database file.
+            xCallback (Callable[[BufferedReader, int, int, int], bytes]): The callback function to read the buffer.
+
+        Raises:
+            SQCloudException: If an error occurs during the upload process.
+
+        """
+        keyarg = "KEY " if key else ""
+        keyvalue = key if key else ""
+
+        # prepare command to execute
+        command = ""
+        if is_file_transfer:
+            internalarg = "INTERNAL" if is_internal_db else ""
+            command = f"TRANSFER DATABASE '{dbname}' {keyarg}{keyvalue} SNAPSHOT {snapshot_id} {internalarg}"
+        else:
+            command = f"UPLOAD DATABASE '{dbname}' {keyarg}{keyvalue}"
+
+        # execute command on server side
+        result = self._internal_run_command(connection, command)
+        if not result.data[0]:
+            raise SQCloudException(
+                "An error occurred while initializing the upload of the database."
+            )
+
+        buffer: bytes = b""
+        blen = 0
+        nprogress = 0
         try:
-            conn.isblob = True
-            return self._internal_run_command(conn, blob)
-        finally:
-            conn.isblob = False
+            while True:
+                # execute callback to read buffer
+                blen = SQCLOUD_DEFAULT.UPLOAD_SIZE.value
+                try:
+                    buffer = xCallback(fd, blen, dbsize, nprogress)
+                    blen = len(buffer)
+                except Exception as e:
+                    raise SQCloudException(
+                        "An error occurred while reading the file."
+                    ) from e
+
+                try:
+                    # send also the final confirmation blob of zero bytes
+                    self.send_blob(buffer, connection)
+                except Exception as e:
+                    raise SQCloudException(
+                        "An error occurred while uploading the file."
+                    ) from e
+
+                # update progress
+                nprogress += blen
+
+                if blen == 0:
+                    # Upload completed
+                    break
+        except Exception as e:
+            self._internal_run_command(connection, "UPLOAD ABORT")
+            raise e
 
-    def _internal_reconnect(self, buffer: bytes) -> bool:
-        return True
+    def download_database(
+        self,
+        connection: SQCloudConnect,
+        dbname: str,
+        fd: BufferedWriter,
+        xCallback: Callable[[BufferedWriter, int, int, int], bytes],
+        if_exists: bool,
+    ) -> None:
+        """
+        Downloads a database from the SQLite Cloud service.
 
-    def _internal_setup_pubsub(self, buffer: bytes) -> bool:
-        return True
+        Args:
+            connection (SQCloudConnect): The connection object used to communicate with the SQLite Cloud service.
+            dbname (str): The name of the database to download.
+            fd (BufferedWriter): The file descriptor to write the downloaded data to.
+            xCallback (Callable[[BufferedWriter, int, int, int], bytes]): A callback function to write downloaded data with the download progress information.
+            if_exists (bool): If True, the download won't rise an exception if database is missing.
+
+        Raises:
+            SQCloudException: If an error occurs while downloading the database.
+
+        """
+        exists_cmd = " IF EXISTS" if if_exists else ""
+        result = self._internal_run_command(
+            connection, f"DOWNLOAD DATABASE {dbname}{exists_cmd};"
+        )
+
+        if result.nrows == 0:
+            raise SQCloudException(
+                "An error occurred while initializing the download of the database."
+            )
+
+        # result is an ARRAY (database size, number of pages, raft_index)
+        download_info = result.data[0]
+        db_size = int(download_info[0])
+
+        # loop to download
+        progress_size = 0
+
+        try:
+            while progress_size < db_size:
+                result = self._internal_run_command(connection, "DOWNLOAD STEP")
+
+                # res is BLOB, decode it
+                data = result.data[0]
+                data_len = len(data)
+
+                # execute callback (with progress_size updated)
+                progress_size += data_len
+                xCallback(fd, data, data_len, db_size, progress_size)
+
+                # check exit condition
+                if data_len == 0:
+                    break
+        except Exception as e:
+            self._internal_run_command(connection, "DOWNLOAD ABORT")
+            raise e
 
     def _internal_config_apply(
         self, connection: SQCloudConnect, config: SQCloudConfig
     ) -> None:
         if config.timeout > 0:
             connection.socket.settimeout(config.timeout)
 
@@ -131,70 +413,82 @@
         if config.maxrowset:
             buffer += f"SET CLIENT KEY MAXROWSET TO {config.maxrowset};"
 
         if len(buffer) > 0:
             self._internal_run_command(connection, buffer)
 
     def _internal_run_command(
-        self, connection: SQCloudConnect, command: Union[str, bytes]
-    ) -> None:
-        self._internal_socket_write(connection, command)
-        return self._internal_socket_read(connection)
+        self,
+        connection: SQCloudConnect,
+        command: Union[str, bytes],
+        main_socket: bool = True,
+    ) -> SQCloudResult:
+        self._internal_socket_write(connection, command, main_socket)
+        return self._internal_socket_read(connection, main_socket)
 
     def _internal_socket_write(
-        self, connection: SQCloudConnect, command: Union[str, bytes]
+        self,
+        connection: SQCloudConnect,
+        command: Union[str, bytes],
+        main_socket: bool = True,
     ) -> None:
         # compute header
         delimit = "$" if connection.isblob else "+"
         buffer = command.encode() if isinstance(command, str) else command
         buffer_len = len(buffer)
         header = f"{delimit}{buffer_len} "
 
+        sock = connection.socket if main_socket else connection.pubsub_socket
+
         # write header
         try:
-            connection.socket.sendall(header.encode())
+            sock.sendall(header.encode())
         except Exception as exc:
             raise SQCloudException(
                 "An error occurred while writing header data.",
-                SQCLOUD_INTERNAL_ERRCODE.INTERNAL_ERRCODE_NETWORK,
+                SQCLOUD_INTERNAL_ERRCODE.NETWORK,
             ) from exc
 
         # write buffer
         if buffer_len == 0:
             return
         try:
-            connection.socket.sendall(buffer)
+            sock.sendall(buffer)
         except Exception as exc:
             raise SQCloudException(
                 "An error occurred while writing data.",
-                SQCLOUD_INTERNAL_ERRCODE.INTERNAL_ERRCODE_NETWORK,
+                SQCLOUD_INTERNAL_ERRCODE.NETWORK,
             ) from exc
 
-    def _internal_socket_read(self, connection: SQCloudConnect) -> SQCloudResult:
+    def _internal_socket_read(
+        self, connection: SQCloudConnect, main_socket: bool = True
+    ) -> SQCloudResult:
         """
         Read from the socket and parse the response.
 
         The buffer is stored as a string of bytes without decoding it with UTF-8.
         The dimensions (LEN) specified in the SCSP protocol are in bytes, while
         Python counts decoded strings in characters. This can cause issues when
         slicing the buffer into parts if there are special characters like "ò".
         """
         buffer = b""
         buffer_size = 8192
         nread = 0
 
+        sock = connection.socket if main_socket else connection.pubsub_socket
+
         while True:
             try:
-                data = connection.socket.recv(buffer_size)
+                data = sock.recv(buffer_size)
                 if not data:
                     raise SQCloudException("Incomplete response from server.")
             except Exception as exc:
                 raise SQCloudException(
                     "An error occurred while reading data from the socket.",
-                    SQCLOUD_INTERNAL_ERRCODE.INTERNAL_ERRCODE_NETWORK,
+                    SQCLOUD_INTERNAL_ERRCODE.NETWORK,
                 ) from exc
 
             # the expected data length to read
             # matches the string size before decoding it
             nread += len(data)
             # update buffers
             buffer += data
@@ -271,15 +565,15 @@
         # string
         # list
         # object
         # None
 
         # check OK value
         if buffer == b"+2 OK":
-            return SQCloudResult(True)
+            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_OK, True)
 
         cmd = chr(buffer[0])
 
         # check for compressed result
         if cmd == SQCLOUD_CMD.COMPRESSED.value:
             buffer = self._internal_uncompress_data(buffer)
             if buffer is None:
@@ -302,31 +596,46 @@
             SQCLOUD_CMD.BLOB.value,
             SQCLOUD_CMD.JSON.value,
         ]:
             sqlite_number = self._internal_parse_number(buffer)
             len_ = sqlite_number.value
             cstart = sqlite_number.cstart
             if len_ == 0:
-                return SQCloudResult("")
+                return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_STRING, "")
+
+            tag = (
+                SQCLOUD_RESULT_TYPE.RESULT_JSON
+                if cmd == SQCLOUD_CMD.JSON.value
+                else SQCLOUD_RESULT_TYPE.RESULT_STRING
+            )
 
             if cmd == SQCLOUD_CMD.ZEROSTRING.value:
                 len_ -= 1
             clone = buffer[cstart : cstart + len_]
 
             if cmd == SQCLOUD_CMD.COMMAND.value:
                 return self._internal_run_command(connection, clone)
             elif cmd == SQCLOUD_CMD.PUBSUB.value:
-                return SQCloudResult(self._internal_setup_pubsub(clone))
+                return SQCloudResult(
+                    SQCLOUD_RESULT_TYPE.RESULT_OK,
+                    self._internal_setup_pubsub(connection, clone),
+                )
             elif cmd == SQCLOUD_CMD.RECONNECT.value:
-                return SQCloudResult(self._internal_reconnect(clone))
+                return SQCloudResult(
+                    SQCLOUD_RESULT_TYPE.RESULT_OK, self._internal_reconnect(clone)
+                )
             elif cmd == SQCLOUD_CMD.ARRAY.value:
-                return SQCloudResult(self._internal_parse_array(clone))
+                return SQCloudResult(
+                    SQCLOUD_RESULT_TYPE.RESULT_ARRAY, self._internal_parse_array(clone)
+                )
+            elif cmd == SQCLOUD_CMD.BLOB.value:
+                tag = SQCLOUD_RESULT_TYPE.RESULT_BLOB
 
             clone = clone.decode() if cmd != SQCLOUD_CMD.BLOB.value else clone
-            return SQCloudResult(clone)
+            return SQCloudResult(tag, clone)
 
         elif cmd == SQCLOUD_CMD.ERROR.value:
             # -LEN ERRCODE:EXTCODE ERRMSG
             sqlite_number = self._internal_parse_number(buffer)
             len_ = sqlite_number.value
             cstart = sqlite_number.cstart
             clone = buffer[cstart:]
@@ -372,33 +681,37 @@
             buffer = buffer[sign_len + len(f"/{sign_len} ") :]
             if cmd == SQCLOUD_CMD.ROWSET_CHUNK.value and buffer:
                 return self._internal_parse_buffer(connection, buffer, len(buffer))
 
             return rowset
 
         elif cmd == SQCLOUD_CMD.NULL.value:
-            return None
+            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
 
         elif cmd in [SQCLOUD_CMD.INT.value, SQCLOUD_CMD.FLOAT.value]:
             sqcloud_value = self._internal_parse_value(buffer)
             clone = sqcloud_value.value
 
+            tag = (
+                SQCLOUD_RESULT_TYPE.RESULT_INTEGER
+                if cmd == SQCLOUD_CMD.INT.value
+                else SQCLOUD_RESULT_TYPE.RESULT_FLOAT
+            )
+
             if clone is None:
-                return SQCloudResult(0)
+                return SQCloudResult(tag, 0)
 
             if cmd == SQCLOUD_CMD.INT.value:
-                return SQCloudResult(int(clone))
-            return SQCloudResult(float(clone))
+                return SQCloudResult(tag, int(clone))
+            return SQCloudResult(tag, float(clone))
 
         elif cmd == SQCLOUD_CMD.RAWJSON.value:
-            # TODO: isn't implemented in C?
-            return SQCloudResult(None)
+            return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
 
-        # TODO: exception here?
-        return SQCloudResult(None)
+        return SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_NONE, None)
 
     def _internal_uncompress_data(self, buffer: bytes) -> Optional[bytes]:
         """
         %LEN COMPRESSED UNCOMPRESSED BUFFER
 
         Args:
             buffer (str): The compressed data buffer.
@@ -541,15 +854,15 @@
         n = start
         ischunk = chr(buffer[0]) == SQCLOUD_CMD.ROWSET_CHUNK.value
 
         # idx == 0 means first (and only) chunk for rowset
         # idx == 1 means first chunk for chunked rowset
         first_chunk = (ischunk and idx == 1) or (not ischunk and idx == 0)
         if first_chunk:
-            rowset = SQCloudResult()
+            rowset = SQCloudResult(SQCLOUD_RESULT_TYPE.RESULT_ROWSET)
             rowset.nrows = nrows
             rowset.ncols = ncols
             rowset.version = version
             rowset.data = []
             if ischunk:
                 self._rowset = rowset
             n = self._internal_parse_rowset_header(rowset, buffer, start)
```

### Comparing `sqlitecloud-0.0.74/sqlitecloud/resultset.py` & `sqlitecloud-0.0.75/sqlitecloud/resultset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from typing import Any, Dict, List, Optional
 
+from sqlitecloud.types import SQCLOUD_RESULT_TYPE
+
 
 class SQCloudResult:
-    def __init__(self, result: Optional[any] = None) -> None:
+    def __init__(self, tag: SQCLOUD_RESULT_TYPE, result: Optional[any] = None) -> None:
+        self.tag: SQCLOUD_RESULT_TYPE = tag
         self.nrows: int = 0
         self.ncols: int = 0
         self.version: int = 0
         # table values are stored in 1-dimensional array
         self.data: List[Any] = []
         self.colname: List[str] = []
         self.decltype: List[str] = []
@@ -30,15 +33,15 @@
 
 
 class SqliteCloudResultSet:
     def __init__(self, result: SQCloudResult) -> None:
         self._iter_row: int = 0
         self._result: SQCloudResult = result
 
-    def __getattr__(self, attr: str) -> Any:
+    def __getattr__(self, attr: str) -> Optional[Any]:
         return getattr(self._result, attr)
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self._result.data and self._iter_row < self._result.nrows:
```

### Comparing `sqlitecloud-0.0.74/tests/integration/test_client.py` & `sqlitecloud-0.0.75/tests/integration/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,33 @@
 import json
+from multiprocessing import connection
 import os
 import sqlite3
 import tempfile
 import time
 
 import pytest
 from sqlitecloud.client import SqliteCloudClient
 from sqlitecloud.types import (
-    SQCLOUD_CLOUD_ERRCODE,
+    SQCLOUD_ERRCODE,
     SQCLOUD_INTERNAL_ERRCODE,
+    SQCLOUD_RESULT_TYPE,
     SQCloudConnect,
     SQCloudException,
     SqliteCloudAccount,
 )
 
 
 class TestClient:
     # Will warn if a query or other basic operation is slower than this
     WARN_SPEED_MS = 500
 
     # Will except queries to be quicker than this
     EXPECT_SPEED_MS = 6 * 1000
 
-    @pytest.fixture()
-    def sqlitecloud_connection(self):
-        account = SqliteCloudAccount()
-        account.username = os.getenv("SQLITE_USER")
-        account.password = os.getenv("SQLITE_PASSWORD")
-        account.dbname = os.getenv("SQLITE_DB")
-        account.hostname = os.getenv("SQLITE_HOST")
-        account.port = 8860
-
-        client = SqliteCloudClient(cloud_account=account)
-
-        connection = client.open_connection()
-        assert isinstance(connection, SQCloudConnect)
-
-        yield (connection, client)
-
-        client.disconnect(connection)
-
     def test_connection_with_credentials(self):
         account = SqliteCloudAccount()
         account.username = os.getenv("SQLITE_USER")
         account.password = os.getenv("SQLITE_PASSWORD")
         account.dbname = os.getenv("SQLITE_DB")
         account.hostname = os.getenv("SQLITE_HOST")
         account.port = 8860
@@ -93,14 +77,47 @@
         client = SqliteCloudClient(connection_str=connection_string)
 
         conn = client.open_connection()
         assert isinstance(conn, SQCloudConnect)
 
         client.disconnect(conn)
 
+    def test_is_connected(self):
+        account = SqliteCloudAccount()
+        account.username = os.getenv("SQLITE_API_KEY")
+        account.hostname = os.getenv("SQLITE_HOST")
+        account.port = 8860
+
+        client = SqliteCloudClient(cloud_account=account)
+
+        conn = client.open_connection()
+        assert client.is_connected(conn) == True
+
+        client.disconnect(conn)
+        assert client.is_connected(conn) == False
+
+    def test_disconnect(self):
+        account = SqliteCloudAccount()
+        account.username = os.getenv("SQLITE_API_KEY")
+        account.hostname = os.getenv("SQLITE_HOST")
+        account.port = 8860
+
+        client = SqliteCloudClient(cloud_account=account)
+
+        conn = client.open_connection()
+        assert client.is_connected(conn) == True
+
+        client.disconnect(conn)
+        assert client.is_connected(conn) == False
+        assert conn.socket is None
+        assert conn.pubsub_socket is None
+
+        # disconnecting a second time should not raise an exception
+        client.disconnect(conn)
+
     def test_select(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         result = client.exec_query("SELECT 'Hello'", connection)
 
         assert False == result.is_result
         assert 1 == result.nrows
@@ -115,14 +132,15 @@
         assert e.value.errcode == 1
         assert e.value.errmsg == "no such column: not_a_column"
 
     def test_rowset_data(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("SELECT AlbumId FROM albums LIMIT 2", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
         assert 2 == result.nrows
         assert 1 == result.ncols
         assert 2 == result.version
 
     def test_get_value(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("SELECT * FROM albums", connection)
@@ -174,52 +192,58 @@
         assert "VALUE" == rowset.get_name(0)
         assert value == rowset.get_value(0, 0)
 
     def test_integer(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST INTEGER", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_INTEGER == result.tag
         assert 123456 == result.get_result()
 
     def test_float(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST FLOAT", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_FLOAT == result.tag
         assert 3.1415926 == result.get_result()
 
     def test_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST STRING", connection)
 
-        assert "Hello World, this is a test string." == result.get_result()
+        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert result.get_result() == "Hello World, this is a test string."
 
     def test_zero_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ZERO_STRING", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
         assert (
-            "Hello World, this is a zero-terminated test string." == result.get_result()
+            result.get_result() == "Hello World, this is a zero-terminated test string."
         )
 
     def test_empty_string(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST STRING0", connection)
 
-        assert "" == result.get_result()
+        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert result.get_result() == ""
 
     def test_command(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST COMMAND", connection)
 
         assert "PONG" == result.get_result()
 
     def test_json(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST JSON", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_JSON == result.tag 
         assert {
             "msg-from": {"class": "soldier", "name": "Wixilav"},
             "msg-to": {"class": "supreme-commander", "name": "[Redacted]"},
             "msg-type": ["0xdeadbeef", "irc log"],
             "msg-log": [
                 "soldier: Boss there is a slight problem with the piece offering to humans",
                 "supreme-commander: Explain yourself soldier!",
@@ -228,60 +252,65 @@
             ],
         } == json.loads(result.get_result())
 
     def test_blob(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST BLOB", connection)
 
-        assert 1000 == len(result.get_result())
+        assert SQCLOUD_RESULT_TYPE.RESULT_BLOB == result.tag
+        assert len(result.get_result()) == 1000
 
     def test_blob0(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST BLOB0", connection)
 
-        assert 0 == len(result.get_result())
+        assert SQCLOUD_RESULT_TYPE.RESULT_STRING == result.tag
+        assert len(result.get_result()) == 0
 
     def test_error(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         with pytest.raises(SQCloudException) as e:
             client.exec_query("TEST ERROR", connection)
 
-        assert 66666 == e.value.errcode
-        assert "This is a test error message with a devil error code." == e.value.errmsg
+        assert e.value.errcode == 66666
+        assert e.value.errmsg == "This is a test error message with a devil error code."
 
     def test_ext_error(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         with pytest.raises(SQCloudException) as e:
             client.exec_query("TEST EXTERROR", connection)
 
-        assert 66666 == e.value.errcode
-        assert 333 == e.value.xerrcode
+        assert e.value.errcode == 66666
+        assert e.value.xerrcode == 333
         assert (
-            "This is a test error message with an extcode and a devil error code."
-            == e.value.errmsg
+            e.value.errmsg
+            == "This is a test error message with an extcode and a devil error code."
         )
 
     def test_array(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ARRAY", connection)
 
         result_array = result.get_result()
+        
+        assert SQCLOUD_RESULT_TYPE.RESULT_ARRAY == result.tag
         assert isinstance(result_array, list)
         assert len(result_array) == 5
         assert result_array[0] == "Hello World"
         assert result_array[1] == "123456"
         assert result_array[2] == "3.1415"
         assert result_array[3] is None
 
     def test_rowset(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         result = client.exec_query("TEST ROWSET", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == result.tag
         assert result.nrows >= 30
         assert result.ncols == 2
         assert result.version in [1, 2]
         assert result.get_name(0) == "key"
         assert result.get_name(1) == "value"
 
     def test_max_rows_option(self):
@@ -289,53 +318,68 @@
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.maxrows = 1
 
-        rowset = client.exec_query("TEST ROWSET_CHUNK")
+        connection = client.open_connection()
+
+        rowset = client.exec_query("TEST ROWSET_CHUNK", connection)
+
+        client.disconnect(connection)
 
         # maxrows cannot be tested at this level.
         # just expect everything is ok
         assert rowset.nrows > 100
 
+
     def test_max_rowset_option_to_fail_when_rowset_is_bigger(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.maxrowset = 1024
 
+        connection = client.open_connection()
+
         with pytest.raises(SQCloudException) as e:
-            client.exec_query("SELECT * FROM albums")
+            client.exec_query("SELECT * FROM albums", connection)
 
-        assert SQCLOUD_CLOUD_ERRCODE.CLOUD_ERRCODE_INTERNAL.value == e.value.errcode
+        client.disconnect(connection)
+
+        assert SQCLOUD_ERRCODE.INTERNAL.value == e.value.errcode
         assert "RowSet too big to be sent (limit set to 1024 bytes)." == e.value.errmsg
 
+
     def test_max_rowset_option_to_succeed_when_rowset_is_lighter(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.maxrowset = 1024
 
-        rowset = client.exec_query("SELECT 'hello world'")
+        connection = client.open_connection()
+
+        rowset = client.exec_query("SELECT 'hello world'", connection)
+
+        client.disconnect(connection)
 
         assert 1 == rowset.nrows
 
     def test_chunked_rowset(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         rowset = client.exec_query("TEST ROWSET_CHUNK", connection)
 
+        assert SQCLOUD_RESULT_TYPE.RESULT_ROWSET == rowset.tag
         assert 147 == rowset.nrows
         assert 1 == rowset.ncols
         assert 147 == len(rowset.data)
         assert "key" == rowset.get_name(0)
 
     def test_chunked_rowset_twice(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
@@ -377,29 +421,34 @@
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = os.getenv("SQLITE_DB")
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.timeout = 1  # 1 sec
 
+        connection = client.open_connection()
+
         # this operation should take more than 1 sec
         with pytest.raises(SQCloudException) as e:
             # just a long running query
             client.exec_query(
                 """
                 WITH RECURSIVE r(i) AS (
                     VALUES(0)
                     UNION ALL
                     SELECT i FROM r
                     LIMIT 10000000
                 )
-                SELECT i FROM r WHERE i = 1;"""
+                SELECT i FROM r WHERE i = 1;""",
+                connection
             )
 
-        assert e.value.errcode == SQCLOUD_INTERNAL_ERRCODE.INTERNAL_ERRCODE_NETWORK
+        client.disconnect(connection)
+
+        assert e.value.errcode == SQCLOUD_INTERNAL_ERRCODE.NETWORK
         assert e.value.errmsg == "An error occurred while reading data from the socket."
 
     def test_XXL_query(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
 
         xxl_query = 300000
         long_sql = ""
@@ -466,15 +515,19 @@
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.dbname = ""
         account.apikey = os.getenv("SQLITE_API_KEY")
 
         client = SqliteCloudClient(cloud_account=account)
 
-        rowset = client.exec_query("USE DATABASE chinook.sqlite")
+        connection = client.open_connection()
+
+        rowset = client.exec_query("USE DATABASE chinook.sqlite", connection)
+
+        client.disconnect(connection)
 
         assert rowset.get_result()
 
     def test_select_tracks_without_limit(self, sqlitecloud_connection):
         connection, client = sqlitecloud_connection
         rowset = client.exec_query("SELECT * FROM tracks", connection)
 
@@ -550,75 +603,53 @@
             if completed >= num_queries:
                 query_ms = round((time.time() - start_time) * 1000 / num_queries)
                 if query_ms > self.WARN_SPEED_MS:
                     assert (
                         query_ms < self.EXPECT_SPEED_MS
                     ), f"{num_queries}x batched selects, {query_ms}ms per query"
 
-    def test_download_database(self, sqlitecloud_connection):
-        connection, client = sqlitecloud_connection
-
-        rowset = client.exec_query(
-            "DOWNLOAD DATABASE " + os.getenv("SQLITE_DB"), connection
-        )
-
-        result_array = rowset.get_result()
-
-        db_size = int(result_array[0])
-
-        tot_read = 0
-        data: bytes = b""
-        while tot_read < db_size:
-            result = client.exec_query("DOWNLOAD STEP;", connection)
-
-            data += result.get_result()
-            tot_read += len(data)
-
-        temp_file = tempfile.mkstemp(prefix="chinook")[1]
-        with open(temp_file, "wb") as f:
-            f.write(data)
-
-        db = sqlite3.connect(temp_file)
-        cursor = db.execute("SELECT * FROM albums")
-        rowset = cursor.fetchall()
-
-        assert cursor.description[0][0] == "AlbumId"
-        assert cursor.description[1][0] == "Title"
-
     def test_compression_single_column(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.apikey = os.getenv("SQLITE_API_KEY")
         account.dbname = os.getenv("SQLITE_DB")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.compression = True
 
+        connection = client.open_connection()
+
         # min compression size for rowset set by default to 20400 bytes
         blob_size = 20 * 1024
         # rowset = client.exec_query("SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId")
         rowset = client.exec_query(
-            f"SELECT hex(randomblob({blob_size})) AS 'someColumnName'"
+            f"SELECT hex(randomblob({blob_size})) AS 'someColumnName'", connection
         )
 
+        client.disconnect(connection)
+
         assert rowset.nrows == 1
         assert rowset.ncols == 1
         assert rowset.get_name(0) == "someColumnName"
         assert len(rowset.get_value(0, 0)) == blob_size * 2
 
     def test_compression_multiple_columns(self):
         account = SqliteCloudAccount()
         account.hostname = os.getenv("SQLITE_HOST")
         account.apikey = os.getenv("SQLITE_API_KEY")
         account.dbname = os.getenv("SQLITE_DB")
 
         client = SqliteCloudClient(cloud_account=account)
         client.config.compression = True
 
+        connection = client.open_connection()
+
         # min compression size for rowset set by default to 20400 bytes
         rowset = client.exec_query(
-            "SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId"
+            "SELECT * from albums inner join albums a2 on albums.AlbumId = a2.AlbumId", connection
         )
 
+        client.disconnect(connection)
+
         assert rowset.nrows > 0
         assert rowset.ncols > 0
         assert rowset.get_name(0) == "AlbumId"
```

