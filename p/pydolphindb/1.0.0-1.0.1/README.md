# Comparing `tmp/pydolphindb-1.0.0-py3-none-any.whl.zip` & `tmp/pydolphindb-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 18094 bytes, number of entries: 14
--rw-r--r--  2.0 unx      446 b- defN 23-Mar-08 01:46 pydolphindb/__init__.py
--rw-r--r--  2.0 unx     3395 b- defN 23-Mar-27 02:08 pydolphindb/connection.py
--rw-r--r--  2.0 unx     7402 b- defN 23-Mar-01 22:31 pydolphindb/cursor.py
--rw-r--r--  2.0 unx     1024 b- defN 23-Mar-01 22:31 pydolphindb/exceptions.py
--rw-r--r--  2.0 unx       74 b- defN 23-Mar-01 22:31 pydolphindb/sqlalchemy/__init__.py
--rw-r--r--  2.0 unx    29586 b- defN 23-Mar-01 22:31 pydolphindb/sqlalchemy/compiler.py
--rw-r--r--  2.0 unx     7047 b- defN 23-Mar-01 22:31 pydolphindb/sqlalchemy/dialect.py
--rw-r--r--  2.0 unx      163 b- defN 23-Mar-01 22:31 pydolphindb/sqlalchemy/sa_version.py
--rw-r--r--  2.0 unx      326 b- defN 23-Mar-01 22:31 pydolphindb/sqlalchemy/types.py
--rw-r--r--  2.0 unx     7260 b- defN 23-Mar-28 09:41 pydolphindb-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 09:41 pydolphindb-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-28 09:41 pydolphindb-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 23-Mar-28 09:41 pydolphindb-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1184 b- defN 23-Mar-28 09:41 pydolphindb-1.0.0.dist-info/RECORD
-14 files, 58075 bytes uncompressed, 16108 bytes compressed:  72.3%
+Zip file size: 22426 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      462 b- defN 24-May-20 03:18 pydolphindb/__init__.py
+-rw-rw-rw-  2.0 fat     3495 b- defN 24-May-15 09:23 pydolphindb/connection.py
+-rw-rw-rw-  2.0 fat     7650 b- defN 24-May-15 09:23 pydolphindb/cursor.py
+-rw-rw-rw-  2.0 fat     1082 b- defN 24-May-15 09:23 pydolphindb/exceptions.py
+-rw-rw-rw-  2.0 fat       78 b- defN 24-May-15 09:23 pydolphindb/sqlalchemy/__init__.py
+-rw-rw-rw-  2.0 fat    30416 b- defN 24-May-15 09:23 pydolphindb/sqlalchemy/compiler.py
+-rw-rw-rw-  2.0 fat     7268 b- defN 24-May-15 09:23 pydolphindb/sqlalchemy/dialect.py
+-rw-rw-rw-  2.0 fat      170 b- defN 24-May-15 09:23 pydolphindb/sqlalchemy/sa_version.py
+-rw-rw-rw-  2.0 fat      336 b- defN 24-May-15 09:23 pydolphindb/sqlalchemy/types.py
+-rw-rw-rw-  2.0 fat    11596 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7429 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       63 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1277 b- defN 24-May-20 03:27 pydolphindb-1.0.1.dist-info/RECORD
+15 files, 71426 bytes uncompressed, 20294 bytes compressed:  71.6%
```

## zipnote {}

```diff
@@ -21,23 +21,26 @@
 
 Filename: pydolphindb/sqlalchemy/sa_version.py
 Comment: 
 
 Filename: pydolphindb/sqlalchemy/types.py
 Comment: 
 
-Filename: pydolphindb-1.0.0.dist-info/METADATA
+Filename: pydolphindb-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: pydolphindb-1.0.0.dist-info/WHEEL
+Filename: pydolphindb-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pydolphindb-1.0.0.dist-info/entry_points.txt
+Filename: pydolphindb-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pydolphindb-1.0.0.dist-info/top_level.txt
+Filename: pydolphindb-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: pydolphindb-1.0.0.dist-info/RECORD
+Filename: pydolphindb-1.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: pydolphindb-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pydolphindb/__init__.py

```diff
@@ -1,16 +1,16 @@
-from .connection import Connection as connect
-from .exceptions import Error
-from .sqlalchemy import DolphinDBDialect
-# from .enginespec import DolphinDBEngineSpec
-
-__all__ = [
-    connect,
-    Error,
-    DolphinDBDialect,
-]
-
-__version__ = "1.0.0"       # pydolphindb version
-
-apilevel = "2.0"            # DBapi2.0
-threadsafety = 0            # thread safety level, need to check & modify
-paramstyle = "qmark"        # param style for Engine URL
+from .connection import Connection as connect
+from .exceptions import Error
+from .sqlalchemy import DolphinDBDialect
+# from .enginespec import DolphinDBEngineSpec
+
+__all__ = [
+    connect,
+    Error,
+    DolphinDBDialect,
+]
+
+__version__ = "1.0.1"       # pydolphindb version
+
+apilevel = "2.0"            # DBapi2.0
+threadsafety = 0            # thread safety level, need to check & modify
+paramstyle = "qmark"        # param style for Engine URL
```

## pydolphindb/connection.py

 * *Ordering differences only*

```diff
@@ -1,100 +1,100 @@
-from .cursor import Cursor
-import dolphindb as ddb
-from .exceptions import ProgrammingError
-from typing import Optional, List
-
-class Connection(object):
-    """This is the object you use to connect with the database.
-
-    See `Connection <https://www.python.org/dev/peps/pep-0249/#connection-objects>`_ in
-    the specification.
-
-    Attributes: 
-        session:Session is the connection object to execute scripts.
-
-    """
-    def __init__(self,
-                 host: str,
-                 port: int,
-                 username: str = "",
-                 password: str = "",
-                 enableSSL:bool=False, 
-                 enableASYNC:bool=False,
-                 keepAliveTime:int=30, 
-                 enableChunkGranularityConfig:bool=False, 
-                 compress:bool=False,
-                 enablePickle:bool=True, 
-                 protocol:int=0,
-                 python:bool=False,
-                 startup:str=None,
-                 highAvailability:bool=False,
-                 highAvailabilitySites:Optional[List[str]]=None,
-                 reconnect:bool=False,
-                 enableEncryption:bool=True
-                 ):
-        self.session = ddb.session(enableSSL=enableSSL, enableASYNC=enableASYNC, enableChunkGranularityConfig=enableChunkGranularityConfig, compress=compress, enablePickle=enablePickle, protocol=protocol, python=python)
-        self.isConnected = self.session.connect(host=host, port=port, startup=startup, highAvailability=highAvailability, highAvailabilitySites=highAvailabilitySites, keepAliveTime=keepAliveTime, reconnect=reconnect)
-        if not self.isConnected:
-            raise RuntimeError("<Exception>:Failed to connect to the server {host}:{port}".format(host=host, port=port))
-        self.session.login(userid=username, password=password, enableEncryption=enableEncryption)
-        self._closed = False 
-        self._result = None
-    
-    def cursor(self):
-        """Get a cursor to interact with the DolphinDB by connection object.
-
-        Returns:
-            Specify cursor object
-            
-        """
-        if not self._closed:
-            return Cursor(self)
-        else:
-            raise ProgrammingError("Connection closed")
-
-    def run(self, script: str, *args, **kwargs):
-        """Execute script.
-
-        Args:
-            script (str): DolphinDB script to be executed. 
-            *args: Arguments to be passed to the function.
-
-        Note:
-            Args is only required when script is the function name.
-
-        Kwargs:
-            See the DolphinDB parameter list for details.
-
-        Returns:
-            Execution result.
-            
-        """
-        self._result = self.session.run(script, *args, **kwargs)
-        return self._result
-
-    def close(self):
-        """ Close session connection. """
-        self._closed = True
-        self.session.close()
-
-    def commit(self):
-        """ Not Supported. """
-        pass
-        # raise RuntimeError("This method is not supported for DolphinDB.")
-
-    def rollback(self):
-        """ Not Supported. """
-        pass
-        # raise RuntimeError("This method is not supported for DolphinDB.")
-    
-    def __repr__(self):
-        return '<Connection {0}>'.format(repr(self.session))
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *exc_info):
-        del exc_info
-        self.close()
-
-connect = Connection
+from .cursor import Cursor
+import dolphindb as ddb
+from .exceptions import ProgrammingError
+from typing import Optional, List
+
+class Connection(object):
+    """This is the object you use to connect with the database.
+
+    See `Connection <https://www.python.org/dev/peps/pep-0249/#connection-objects>`_ in
+    the specification.
+
+    Attributes: 
+        session:Session is the connection object to execute scripts.
+
+    """
+    def __init__(self,
+                 host: str,
+                 port: int,
+                 username: str = "",
+                 password: str = "",
+                 enableSSL:bool=False, 
+                 enableASYNC:bool=False,
+                 keepAliveTime:int=30, 
+                 enableChunkGranularityConfig:bool=False, 
+                 compress:bool=False,
+                 enablePickle:bool=True, 
+                 protocol:int=0,
+                 python:bool=False,
+                 startup:str=None,
+                 highAvailability:bool=False,
+                 highAvailabilitySites:Optional[List[str]]=None,
+                 reconnect:bool=False,
+                 enableEncryption:bool=True
+                 ):
+        self.session = ddb.session(enableSSL=enableSSL, enableASYNC=enableASYNC, enableChunkGranularityConfig=enableChunkGranularityConfig, compress=compress, enablePickle=enablePickle, protocol=protocol, python=python)
+        self.isConnected = self.session.connect(host=host, port=port, startup=startup, highAvailability=highAvailability, highAvailabilitySites=highAvailabilitySites, keepAliveTime=keepAliveTime, reconnect=reconnect)
+        if not self.isConnected:
+            raise RuntimeError("<Exception>:Failed to connect to the server {host}:{port}".format(host=host, port=port))
+        self.session.login(userid=username, password=password, enableEncryption=enableEncryption)
+        self._closed = False 
+        self._result = None
+    
+    def cursor(self):
+        """Get a cursor to interact with the DolphinDB by connection object.
+
+        Returns:
+            Specify cursor object
+            
+        """
+        if not self._closed:
+            return Cursor(self)
+        else:
+            raise ProgrammingError("Connection closed")
+
+    def run(self, script: str, *args, **kwargs):
+        """Execute script.
+
+        Args:
+            script (str): DolphinDB script to be executed. 
+            *args: Arguments to be passed to the function.
+
+        Note:
+            Args is only required when script is the function name.
+
+        Kwargs:
+            See the DolphinDB parameter list for details.
+
+        Returns:
+            Execution result.
+            
+        """
+        self._result = self.session.run(script, *args, **kwargs)
+        return self._result
+
+    def close(self):
+        """ Close session connection. """
+        self._closed = True
+        self.session.close()
+
+    def commit(self):
+        """ Not Supported. """
+        pass
+        # raise RuntimeError("This method is not supported for DolphinDB.")
+
+    def rollback(self):
+        """ Not Supported. """
+        pass
+        # raise RuntimeError("This method is not supported for DolphinDB.")
+    
+    def __repr__(self):
+        return '<Connection {0}>'.format(repr(self.session))
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_info):
+        del exc_info
+        self.close()
+
+connect = Connection
```

## pydolphindb/cursor.py

 * *Ordering differences only*

```diff
@@ -1,248 +1,248 @@
-from pandas import DataFrame
-from .exceptions import ProgrammingError
-import warnings
-import pandas as pd
-from numpy import ndarray
-import numpy as np
-import decimal
-from typing import Optional, Tuple, List
-
-class Cursor(object):
-    """
-    This is the object you use to interact with the database.
-
-    Do not create an instance of a Cursor yourself. Call
-    connections.Connection.cursor().
-
-    See `Cursor <https://www.python.org/dev/peps/pep-0249/#cursor-objects>`_ in
-    the specification.
-
-    """
-
-    def __init__(self, connection):
-        self.connection = connection
-        self.description: Optional[Tuple] = None
-        self.rowcount: int = -1
-        self.arraysize: int = 1
-        self.rownumber:int = 0 
-        self._executed: Optional[str] = None
-
-        self._result: Optional[List]= None
-        self._rows:List = []
-
-    def close(self):
-        """Close the cursor. No further scripts will be possible."""
-        try:
-            if self.connection is None:
-                return
-        finally:
-            self.connection = None
-            self._result = None
-
-    def _check_executed(self):
-        if not self._executed:
-            raise ProgrammingError("execute() first")
-
-    def fetchone(self):
-        """Fetches a single row from the cursor. None indicates that
-        no more rows are available.
-
-        Returns:
-            One result. 
-            
-        """
-        self._check_executed()
-        if self.rownumber >= len(self._rows):
-            return None
-        result = self._rows[self.rownumber]
-        self.rownumber = self.rownumber + 1
-        return result
-
-    def fetchmany(self, size: Optional[int] = None):
-        """Fetch up to size rows from the cursor. Result set may be smaller
-        than size. If size is not defined, cursor.arraysize(by default is 1) is used.
-
-        Args:
-            size (int): Feche size.
-
-        Returns:
-            Size length result set.
-            
-        """
-        self._check_executed()
-        end = self.rownumber + (size or self.arraysize)
-        result = self._rows[self.rownumber : end]
-        self.rownumber = min(end, len(self._rows))
-        return result
-
-    def fetchall(self):
-        """Fetches all available rows from the cursor.
-
-        Returns:
-            All available result set.
-            
-        """
-        self._check_executed()
-        if self.rownumber:
-            result = self._rows[self.rownumber :]
-        else:
-            result = self._rows
-        self.rownumber = len(self._rows)
-        return result
-
-    def _get_db(self):
-        con = self.connection
-        if con is None:
-            raise ProgrammingError("cursor closed")
-        return con
-
-    def _run(self, script, db, *args, **kwargs):
-        self._result = None
-        self._do_get_result(script, db, *args, **kwargs)
-        self._post_get_result()
-        self._executed = script
-        return self.rowcount
-
-    def _get_result(self, script, db, *args, **kwargs):
-        return db.run(script, *args, **kwargs)
-
-    def _do_get_result(self, script, db, *args, **kwargs):
-        self._result = self._get_result(script, db, *args, **kwargs)
-        if self._result is None:
-            self.description = tuple()
-        else:
-            description = []
-            if(isinstance(self._result, DataFrame)):
-                for col in self._result.columns:
-                    description.append((
-                        col,
-                        None,
-                        None,
-                        None,
-                        None,
-                        None,
-                        None,
-                        ))
-            else:
-                description.append((
-                    "string",
-                    None,
-                    None,
-                    None,
-                    None,
-                    None,
-                    None))
-            self.description = tuple(description)
-
-        self.rownumber = 0
-
-    def _DataFrame_to_list(self, df):
-        result = []
-        for _, row in df.iterrows():
-            newrow = []
-            for item in row:
-                if isinstance(item, ndarray):
-                    item = [x if not pd.isna(x) else None for x in list(item)]
-                else:
-                    if pd.isna(item):
-                        item = None
-                newrow.append(item)
-            result.append(newrow)
-        return result
-
-    def _post_get_result(self):
-        if(isinstance(self._result, DataFrame)):
-            self._rows = self._DataFrame_to_list(self._result)
-        elif(isinstance(self._result, list)):
-            self._rows = self._result
-        elif(isinstance(self._result, ndarray)):
-            self._rows = [x if not pd.isna(x) else None for x in list(self._result)]
-        elif(isinstance(self._result, type(None))):
-            self._rows = []
-        else:
-            self._rows = [self._result]
-        self.rowcount = len(self._rows)
-        self._result = None
-
-    def execute(self, script: str, parameters=None, *args, **kwargs) -> int:
-        """Execute a script.
-
-        Args:
-            script: DolphinDB script to be executed.  
-            parameters: parameter to replace %s in script. 
-
-        Note: If args is a tuple, then %s must be used as the
-        parameter placeholder in the query. If a mapping is used,
-
-        Args:
-            *args: See the DolphinDB parameter list for details.
-            **kwargs: See the DolphinDB parameter list for details.
-
-        Returns:
-            Integer represents rows affected, if any.
-
-        """
-        db = self._get_db()
-
-        if(script == "select 1"):
-            script = "1+1"
-
-        if parameters is not None:
-            parameters = tuple(parameters)
-            try:
-                script = script % parameters
-            except TypeError as m:
-                raise ProgrammingError(str(m))
-
-        assert isinstance(script, str)
-        rowcount = self._run(script, db, *args, **kwargs)
-        return rowcount
-            
-    def executemany(self, script: str, seq_of_parameters: List) -> int:
-        """Execute a multi-row script.
-
-        Args:
-            script: DolphinDB script to be executed.
-            seq_of_parameters: It is used as parameter.
-
-        Returns:
-            Number of rows affected, if any.
-
-        Note:
-            This method improves performance on multiple-row INSERT and
-            REPLACE. Otherwise it is equivalent to looping over args with
-            execute().
-
-        """
-        if not seq_of_parameters:
-            raise ProgrammingError("need two parameter")
-
-        self.rowcount = sum(self.execute(script, arg) for arg in seq_of_parameters)
-        return self.rowcount
-
-    def __iter__(self):
-        warnings.warn("DB-API extension cursor.__iter__() used")
-        return self
-
-    def setinputsizes(self):
-        """Not supported"""
-        raise RuntimeError("This method is not supported for DolphinDB.")
-
-    def setoutputsize(self):
-        """Not supported"""
-        raise RuntimeError("This method is not supported for DolphinDB.")
-
-    def next(self):
-        """Get next result set, Similar with fetchone.
-
-        Returns:
-            One row result.
-            
-        """
-        row = self.fetchone()
-        if row is None:
-            raise StopIteration
-        return row
-
-    __next__ = next
-
+from pandas import DataFrame
+from .exceptions import ProgrammingError
+import warnings
+import pandas as pd
+from numpy import ndarray
+import numpy as np
+import decimal
+from typing import Optional, Tuple, List
+
+class Cursor(object):
+    """
+    This is the object you use to interact with the database.
+
+    Do not create an instance of a Cursor yourself. Call
+    connections.Connection.cursor().
+
+    See `Cursor <https://www.python.org/dev/peps/pep-0249/#cursor-objects>`_ in
+    the specification.
+
+    """
+
+    def __init__(self, connection):
+        self.connection = connection
+        self.description: Optional[Tuple] = None
+        self.rowcount: int = -1
+        self.arraysize: int = 1
+        self.rownumber:int = 0 
+        self._executed: Optional[str] = None
+
+        self._result: Optional[List]= None
+        self._rows:List = []
+
+    def close(self):
+        """Close the cursor. No further scripts will be possible."""
+        try:
+            if self.connection is None:
+                return
+        finally:
+            self.connection = None
+            self._result = None
+
+    def _check_executed(self):
+        if not self._executed:
+            raise ProgrammingError("execute() first")
+
+    def fetchone(self):
+        """Fetches a single row from the cursor. None indicates that
+        no more rows are available.
+
+        Returns:
+            One result. 
+            
+        """
+        self._check_executed()
+        if self.rownumber >= len(self._rows):
+            return None
+        result = self._rows[self.rownumber]
+        self.rownumber = self.rownumber + 1
+        return result
+
+    def fetchmany(self, size: Optional[int] = None):
+        """Fetch up to size rows from the cursor. Result set may be smaller
+        than size. If size is not defined, cursor.arraysize(by default is 1) is used.
+
+        Args:
+            size (int): Feche size.
+
+        Returns:
+            Size length result set.
+            
+        """
+        self._check_executed()
+        end = self.rownumber + (size or self.arraysize)
+        result = self._rows[self.rownumber : end]
+        self.rownumber = min(end, len(self._rows))
+        return result
+
+    def fetchall(self):
+        """Fetches all available rows from the cursor.
+
+        Returns:
+            All available result set.
+            
+        """
+        self._check_executed()
+        if self.rownumber:
+            result = self._rows[self.rownumber :]
+        else:
+            result = self._rows
+        self.rownumber = len(self._rows)
+        return result
+
+    def _get_db(self):
+        con = self.connection
+        if con is None:
+            raise ProgrammingError("cursor closed")
+        return con
+
+    def _run(self, script, db, *args, **kwargs):
+        self._result = None
+        self._do_get_result(script, db, *args, **kwargs)
+        self._post_get_result()
+        self._executed = script
+        return self.rowcount
+
+    def _get_result(self, script, db, *args, **kwargs):
+        return db.run(script, *args, **kwargs)
+
+    def _do_get_result(self, script, db, *args, **kwargs):
+        self._result = self._get_result(script, db, *args, **kwargs)
+        if self._result is None:
+            self.description = tuple()
+        else:
+            description = []
+            if(isinstance(self._result, DataFrame)):
+                for col in self._result.columns:
+                    description.append((
+                        col,
+                        None,
+                        None,
+                        None,
+                        None,
+                        None,
+                        None,
+                        ))
+            else:
+                description.append((
+                    "string",
+                    None,
+                    None,
+                    None,
+                    None,
+                    None,
+                    None))
+            self.description = tuple(description)
+
+        self.rownumber = 0
+
+    def _DataFrame_to_list(self, df):
+        result = []
+        for _, row in df.iterrows():
+            newrow = []
+            for item in row:
+                if isinstance(item, ndarray):
+                    item = [x if not pd.isna(x) else None for x in list(item)]
+                else:
+                    if pd.isna(item):
+                        item = None
+                newrow.append(item)
+            result.append(newrow)
+        return result
+
+    def _post_get_result(self):
+        if(isinstance(self._result, DataFrame)):
+            self._rows = self._DataFrame_to_list(self._result)
+        elif(isinstance(self._result, list)):
+            self._rows = self._result
+        elif(isinstance(self._result, ndarray)):
+            self._rows = [x if not pd.isna(x) else None for x in list(self._result)]
+        elif(isinstance(self._result, type(None))):
+            self._rows = []
+        else:
+            self._rows = [self._result]
+        self.rowcount = len(self._rows)
+        self._result = None
+
+    def execute(self, script: str, parameters=None, *args, **kwargs) -> int:
+        """Execute a script.
+
+        Args:
+            script: DolphinDB script to be executed.  
+            parameters: parameter to replace %s in script. 
+
+        Note: If args is a tuple, then %s must be used as the
+        parameter placeholder in the query. If a mapping is used,
+
+        Args:
+            *args: See the DolphinDB parameter list for details.
+            **kwargs: See the DolphinDB parameter list for details.
+
+        Returns:
+            Integer represents rows affected, if any.
+
+        """
+        db = self._get_db()
+
+        if(script == "select 1"):
+            script = "1+1"
+
+        if parameters is not None:
+            parameters = tuple(parameters)
+            try:
+                script = script % parameters
+            except TypeError as m:
+                raise ProgrammingError(str(m))
+
+        assert isinstance(script, str)
+        rowcount = self._run(script, db, *args, **kwargs)
+        return rowcount
+            
+    def executemany(self, script: str, seq_of_parameters: List) -> int:
+        """Execute a multi-row script.
+
+        Args:
+            script: DolphinDB script to be executed.
+            seq_of_parameters: It is used as parameter.
+
+        Returns:
+            Number of rows affected, if any.
+
+        Note:
+            This method improves performance on multiple-row INSERT and
+            REPLACE. Otherwise it is equivalent to looping over args with
+            execute().
+
+        """
+        if not seq_of_parameters:
+            raise ProgrammingError("need two parameter")
+
+        self.rowcount = sum(self.execute(script, arg) for arg in seq_of_parameters)
+        return self.rowcount
+
+    def __iter__(self):
+        warnings.warn("DB-API extension cursor.__iter__() used")
+        return self
+
+    def setinputsizes(self):
+        """Not supported"""
+        raise RuntimeError("This method is not supported for DolphinDB.")
+
+    def setoutputsize(self):
+        """Not supported"""
+        raise RuntimeError("This method is not supported for DolphinDB.")
+
+    def next(self):
+        """Get next result set, Similar with fetchone.
+
+        Returns:
+            One row result.
+            
+        """
+        row = self.fetchone()
+        if row is None:
+            raise StopIteration
+        return row
+
+    __next__ = next
+
```

## pydolphindb/exceptions.py

 * *Ordering differences only*

```diff
@@ -1,58 +1,58 @@
-class Error(Exception):
-    
-    def __init__(self, msg=None, error_trace=None):
-        # for compatibility reasons we want to keep the exception message
-        # attribute because clients may depend on it
-        if msg:
-            self.message = msg
-        super(Error, self).__init__(msg)
-        self.error_trace = error_trace
-
-
-class Warning(Exception):
-    pass
-
-class InterfaceError(Error):
-    pass
-
-class DatabaseError(Error):
-    pass
-
-class InternalError(DatabaseError):
-    pass
-
-class OperationalError(DatabaseError):
-    pass
-
-class ProgrammingError(DatabaseError):
-    pass
-
-class IntegrityError(DatabaseError):
-    pass
-
-class DataError(DatabaseError):
-    pass
-
-class NotSupportedError(DatabaseError):
-    pass
-
-
-# exceptions not in db api
-class ConnectionError(OperationalError):
-    pass
-
-
-class BlobException(Exception):
-    pass
-
-
-class DigestNotFoundException(BlobException):
-    pass
-
-
-class BlobLocationNotFoundException(BlobException):
-    pass
-
-
-class TimezoneUnawareException(Error):
-    pass
+class Error(Exception):
+    
+    def __init__(self, msg=None, error_trace=None):
+        # for compatibility reasons we want to keep the exception message
+        # attribute because clients may depend on it
+        if msg:
+            self.message = msg
+        super(Error, self).__init__(msg)
+        self.error_trace = error_trace
+
+
+class Warning(Exception):
+    pass
+
+class InterfaceError(Error):
+    pass
+
+class DatabaseError(Error):
+    pass
+
+class InternalError(DatabaseError):
+    pass
+
+class OperationalError(DatabaseError):
+    pass
+
+class ProgrammingError(DatabaseError):
+    pass
+
+class IntegrityError(DatabaseError):
+    pass
+
+class DataError(DatabaseError):
+    pass
+
+class NotSupportedError(DatabaseError):
+    pass
+
+
+# exceptions not in db api
+class ConnectionError(OperationalError):
+    pass
+
+
+class BlobException(Exception):
+    pass
+
+
+class DigestNotFoundException(BlobException):
+    pass
+
+
+class BlobLocationNotFoundException(BlobException):
+    pass
+
+
+class TimezoneUnawareException(Error):
+    pass
```

## pydolphindb/sqlalchemy/__init__.py

 * *Ordering differences only*

```diff
@@ -1,5 +1,5 @@
-from .dialect import DolphinDBDialect
-
-__all__ = [
-    DolphinDBDialect,
+from .dialect import DolphinDBDialect
+
+__all__ = [
+    DolphinDBDialect,
 ]
```

## pydolphindb/sqlalchemy/compiler.py

 * *Ordering differences only*

```diff
@@ -1,830 +1,830 @@
-import re
-from sqlalchemy.sql import compiler
-from sqlalchemy import exc
-from sqlalchemy import sql
-from sqlalchemy import types as sqltypes
-from sqlalchemy import util
-from sqlalchemy.sql import compiler
-from sqlalchemy.sql import operators
-from sqlalchemy.sql import elements
-
-
-RE_DATETIME_PATTERN = r"'(?P<Y>\d{4})-(?P<M>\d{2})-(?P<D>\d{2}) (?P<H>\d{2}):(?P<m>\d{2}):(?P<s>\d{2}).(?P<ms>\d{6})'"
-def _datetime_replace(matched):
-    matched_dict = matched.groupdict()
-    Y_ = matched_dict['Y']
-    M_ = matched_dict['M']
-    D_ = matched_dict['D']
-    H_ = matched_dict['H']
-    m_ = matched_dict['m']
-    s_ = matched_dict['s']
-    ms_ = matched_dict['ms']
-    return "{}.{}.{}T{}:{}:{}.{}".format(Y_, M_, D_, H_, m_, s_, ms_)
-
-RE_JOIN_AS = r"as (?P<name>\w*)__"
-def _join_as_replace(matched):
-    matched_dict = matched.groupdict()
-    name_ = matched_dict['name']
-    if name_ == "mme_inner":
-        return "as {}__".format(name_)
-    else:
-        return "as {}".format(name_)
-
-RE_JOIN_ON = r"(?P<name1>\w*) = (?P<name2>\w*)__"
-def _join_on_replace(matched):
-    matched_dict = matched.groupdict()
-    name1_ = matched_dict['name1']
-    name2_ = matched_dict['name2']
-    if name1_ == name2_:
-        return "{}".format(name1_)
-    else:
-        return "{} = {}__".format(name1_, name2_)
-
-OPERATORS = {
-    # binary
-    operators.and_: " && ",         # sqlparse will detect "and"/"AND" and add '\n' to sql string    refine link:sqlparse.__init__.format -> ReindentFilter._next_token
-    operators.or_: " || ",
-    operators.add: " + ",
-    operators.mul: " * ",
-    operators.sub: " - ",
-    operators.div: " / ",
-    operators.mod: " % ",
-    operators.truediv: " / ",
-    operators.neg: "-",
-    operators.lt: " < ",
-    operators.le: " <= ",
-    operators.ne: " != ",
-    operators.gt: " > ",
-    operators.ge: " >= ",
-    operators.eq: " = ",
-    operators.is_distinct_from: " IS DISTINCT FROM ",
-    operators.isnot_distinct_from: " IS NOT DISTINCT FROM ",
-    operators.concat_op: " || ",
-    operators.match_op: " MATCH ",
-    operators.notmatch_op: " NOT MATCH ",
-    operators.in_op: " in ",
-    operators.notin_op: " not in ",
-    operators.comma_op: ", ",
-    operators.from_: " from ",
-    operators.as_: " as ",
-    operators.is_: " IS ",
-    operators.isnot: " IS NOT ",
-    operators.collate: " COLLATE ",
-    # unary
-    operators.exists: "EXISTS ",
-    operators.distinct_op: "DISTINCT ",
-    operators.inv: "NOT ",
-    operators.any_op: "ANY ",
-    operators.all_op: "ALL ",
-    # modifiers
-    operators.desc_op: " desc",
-    operators.asc_op: " asc",
-    operators.nullsfirst_op: " NULLS FIRST",
-    operators.nullslast_op: " NULLS LAST",
-}
-
-## Preparer for sql string
-class DDBIdentifierPreparer(sql.compiler.IdentifierPreparer):
-    def __init__(self, dialect):
-        # here changed the initial_quote to "TMP_"
-        super(DDBIdentifierPreparer, self).__init__(dialect, omit_schema=True, initial_quote="")
-
-    # TODO: delete
-    def format_label(self, label, name=None):
-        # print("MLOG [format_label] label=", label, " name=", name)
-        return self.quote(name or label.name)
-
-    # TODO: delete
-    def quote(self, ident, force=None):
-        """Conditionally quote an identfier.
-
-        The identifier is quoted if it is a reserved word, contains
-        quote-necessary characters, or is an instance of
-        :class:`.quoted_name` which includes ``quote`` set to ``True``.
-
-        Subclasses can override this to provide database-dependent
-        quoting behavior for identifier names.
-
-        :param ident: string identifier
-        :param force: unused
-
-            .. deprecated:: 0.9
-
-                The :paramref:`.IdentifierPreparer.quote.force`
-                parameter is deprecated and will be removed in a future
-                release.  This flag has no effect on the behavior of the
-                :meth:`.IdentifierPreparer.quote` method; please refer to
-                :class:`.quoted_name`.
-
-        """
-        if force is not None:
-            # not using the util.deprecated_params() decorator in this
-            # case because of the additional function call overhead on this
-            # very performance-critical spot.
-            util.warn_deprecated(
-                "The IdentifierPreparer.quote.force parameter is "
-                "deprecated and will be removed in a future release.  This "
-                "flag has no effect on the behavior of the "
-                "IdentifierPreparer.quote method; please refer to "
-                "quoted_name()."
-            )
-
-        force = getattr(ident, "quote", None)
-
-        if force is None:
-            if ident in self._strings:
-                return self._strings[ident]
-            else:
-                if self._requires_quotes(ident):
-                    self._strings[ident] = self.quote_identifier(ident)
-                else:
-                    self._strings[ident] = ident
-                return self._strings[ident]
-        elif force:
-            return self.quote_identifier(ident)
-        else:
-            return ident
-        
-    # TODO: delete
-    def quote_identifier(self, value):
-        """Quote an identifier.
-
-        Subclasses should override this to provide database-dependent
-        quoting behavior.
-        """
-
-        return (
-            self.initial_quote
-            + self._escape_identifier(value)
-            + self.final_quote
-        )
-
-## SQLAlchemy types to DolphinDB types
-class DDBTypeCompiler(compiler.GenericTypeCompiler):
-    def visit_String(self, type_, **kw):
-        return 'STRING'
-    
-    def visit_DECIMAL(self, type_, **kw):
-        return 'DOUBLE'
-
-    def visit_VARCHAR(self, type_, **kw):
-        return 'STRING'
-
-    def visit_unicode_text(self, type_, **kw):
-        return 'STRING'
-
-## SQLAlchemy SQL to DolphinDB SQL
-class DDBCompiler(compiler.SQLCompiler):
-    OPERATORS = OPERATORS
-
-    ansi_bind_rules = True
-    def visit_cast(self, cast, **kwargs):
-        # print("cast: ", cast)
-        # print(type(cast))
-        # print("kwargs: ", kwargs)
-        return "cast(%s, %s)" % (
-            cast.clause._compiler_dispatch(self, **kwargs),
-            cast.typeclause._compiler_dispatch(self, **kwargs),
-        )
-
-    def visit_label(
-        self,
-        label,
-        add_to_result_map=None,
-        within_label_clause=False,
-        within_columns_clause=False,
-        render_label_as_label=None,
-        **kw
-    ):
-        # only render labels within the columns clause
-        # or ORDER BY clause of a select.  dialect-specific compilers
-        # can modify this behavior.
-        render_label_with_as = (
-            within_columns_clause and not within_label_clause
-        )
-        render_label_only = render_label_as_label is label
-        # print("pre labelname: ", label.name, type(label))
-        labelname = ""
-        if render_label_only or render_label_with_as:
-            if isinstance(label.name, elements._truncated_label):
-                labelname = self._truncated_identifier("colident", label.name)
-            else:
-                labelname = label.name
-        ## labelname has `(` and `)`.
-        #  replace them with `TMP_`.
-        if labelname.find('(')!=-1 and labelname.find(')')!=-1:
-            labelname = labelname.replace('(', "TMP_")
-            labelname = labelname.replace(')', "TMP_")
-
-        # print("format_label:", label, "|", labelname)
-        if render_label_with_as:
-            if add_to_result_map is not None:
-                add_to_result_map(
-                    labelname,
-                    label.name,
-                    (label, labelname) + label._alt_names,
-                    label.type,
-                )
-            # print("ffff", self.preparer.format_label(label, labelname))
-            pretmp = label.element._compiler_dispatch(
-                    self,
-                    within_columns_clause=True,
-                    within_label_clause=True,
-                    **kw
-                )
-            tmp =  (
-                pretmp
-                + OPERATORS[operators.as_]
-                + self.preparer.format_label(label, labelname)
-            )
-            ## replace keywords
-            if tmp.find("AVG(") != -1:
-                tmp = tmp.replace("AVG(", "avg(")
-            if tmp.find("COUNT(*)") != -1:
-                tmp = tmp.replace("COUNT(*)", "count(*)")
-            if tmp.find("count(DISTINCT ") != -1:
-                tmp = tmp.replace("count(DISTINCT ", "(tmp_->count(distinct(tmp_)))(")
-            if tmp.find("__timestamp") != -1:
-                return pretmp
-                tmp = tmp.replace("__timestamp", pretmp)
-            # print("render_label_with_as: ", tmp)
-            return tmp
-        elif render_label_only:
-
-            tmp = self.preparer.format_label(label, labelname)
-            # print("render_label_only: ", tmp)
-            return tmp
-        else:
-            tmp = label.element._compiler_dispatch(
-                self, within_columns_clause=False, **kw
-            )
-            # print("else: ", tmp)
-            return tmp
-
-    def get_render_as_alias_suffix(self, alias_name_text):
-        return " as " + alias_name_text
-
-    def group_by_clause(self, select, **kw):
-        """allow dialects to customize how GROUP BY is rendered."""
-
-        group_by = select._group_by_clause._compiler_dispatch(self, **kw)
-        if group_by:
-            return " group by " + group_by
-        else:
-            return ""
-
-    def order_by_clause(self, select, **kw):
-        """allow dialects to customize how ORDER BY is rendered."""
-
-        order_by = select._order_by_clause._compiler_dispatch(self, **kw)
-        if order_by:
-            return " order by " + order_by
-        else:
-            return ""
-
-    def visit_table(
-        self,
-        table,
-        asfrom=False,
-        iscrud=False,
-        ashint=False,
-        fromhints=None,
-        use_schema=True,
-        **kwargs
-    ):
-        if asfrom or ashint:
-            effective_schema = self.preparer.schema_for_object(table)
-
-            if use_schema and effective_schema:
-                if(effective_schema=="shared_table"):
-                    ret = (self.preparer.quote(table.name))
-                else:
-                    ret = 'loadTable("{}", "{}")'.format(effective_schema, table.name)
-            else:
-                ret = self.preparer.quote(table.name)
-            if fromhints and table in fromhints:
-                ret = self.format_from_hint_text(
-                    ret, table, fromhints[table], iscrud
-                )
-            return ret
-        else:
-            return ""
-
-    # TODO: need to complete [full join] and [outer join]
-    #       and to check [join]
-    def visit_join(self, join, asfrom=False, **kwargs):
-        if join.full:
-            return "[TODO LIST]"
-        elif join.isouter:
-            return "[TODO LIST]"
-        else:
-            str_l = join.left._compiler_dispatch(self, asfrom=True, **kwargs)
-            str_r = join.right._compiler_dispatch(self, asfrom=True, **kwargs)
-            str_r = re.sub(RE_JOIN_AS, _join_as_replace, str_r)
-            str_e = join.onclause._compiler_dispatch(self, **kwargs)
-            str_o = re.sub(RE_JOIN_ON, _join_on_replace, str_e)
-            if str_e != str_o:
-                return "ej((" + str_l + "), (" + str_r + "), `" + str_o + ")"
-            else:
-                return "ej((" + str_l + "), (" + str_r + "), `" + str_o + ", `" + str_e + ")"
-    
-    # not use
-    # now using `top_clause` instead
-    def limit_clause(self, select, **kw):
-        text = ""
-        # TODO: need to support group by + limit and offset has problem
-        if select._limit_clause is not None:
-            a = self.process(select._limit_clause, **kw)
-            # print("MLOG limit process: ", a, type(a))
-            text += " limit " + self.process(select._limit_clause, **kw)
-        if select._offset_clause is not None:
-            if select._limit_clause is None:
-                text += " limit -1"
-            text += " offset " + self.process(select._offset_clause, **kw)
-        return text
-    
-    def top_clause(self, select, **kw):
-        text = " top "
-        if select._limit_clause is not None and select._offset_clause is None:
-            text += "0:" + self.process(select._limit_clause, **kw) + " "
-        if select._limit_clause is not None and select._offset_clause is not None:
-            limitnum = (int)(self.process(select._limit_clause, **kw))
-            offsetnum = (int)(self.process(select._offset_clause, **kw))
-            text += (str)(offsetnum) + ":" + (str)(offsetnum + limitnum) + " "
-        if select._limit_clause is None and select._offset_clause is not None:
-            text += self.process(select._offset_clause, **kw) + ":50000 "
-        # if select._limit_clause is None and select._offset_clause is None:
-        #     text += "0:50000"
-        return text
-
-    def _compose_select_body(
-        self, text, select, inner_columns, froms, byfrom, kwargs
-    ):
-        # if (
-        #     select._limit_clause is not None
-        #     or select._offset_clause is not None
-        # ):
-            # TODO: need to support group by + limit
-            # text = "select * from (" + text + ") "
-        toptext = self.top_clause(select, **kwargs)
-        text += ", ".join(inner_columns)
-        if froms:
-            text += " from "
-            if select._hints:
-                text += ", ".join(
-                    [
-                        f._compiler_dispatch(
-                            self, asfrom=True, fromhints=byfrom, **kwargs
-                        )
-                        for f in froms
-                    ]
-                )
-            else:
-                text += ", ".join(
-                    [
-                        f._compiler_dispatch(self, asfrom=True, **kwargs)
-                        for f in froms
-                    ]
-                )
-        else:
-            text += self.default_from()
-        # print("MLOG: Start whereclause")
-        if select._whereclause is not None:
-            # print("**kwargs: ", kwargs)
-            t = select._whereclause._compiler_dispatch(self, **kwargs)
-            ## TableColumn.dttm_sql_literal "%Y-%m-%d %H:%M:%S.%f"
-            t = re.sub(RE_DATETIME_PATTERN, _datetime_replace, t)
-            if t:
-                text += " where " + t
-        # print("MLOG: End whereclause")
-
-        if select._group_by_clause.clauses:
-            text += self.group_by_clause(select, **kwargs)
-
-        if select._having is not None:
-            t = select._having._compiler_dispatch(self, **kwargs)
-            if t:
-                text += " having " + t
-
-        if select._order_by_clause.clauses:
-            text += self.order_by_clause(select, **kwargs)
-        
-        if select._for_update_arg is not None:
-            text += self.for_update_clause(select, **kwargs)
-
-        if (
-            select._limit_clause is not None
-            or select._offset_clause is not None
-        ):
-            text = "select " + toptext + " * from (" + text + ")"
-
-        return text
-
-    # for OPERATORS changes
-    # visit_OPERATORS 
-    def visit_clauselist(self, clauselist, **kw):
-        sep = clauselist.operator
-        if sep is None:
-            sep = " "
-        else:
-            sep = OPERATORS[clauselist.operator]
-            # print("OPERATORS: ", sep)
-
-        text = sep.join(
-            s
-            for s in (
-                c._compiler_dispatch(self, **kw) for c in clauselist.clauses
-            )
-            if s
-        )
-        # TODO: "insert value"
-        if clauselist._tuple_values and self.dialect.tuple_in_values:
-            text = "VALUES " + text
-        # print("MOG: visit_clauselist: ", text)
-        return text
-
-    # for OPERATORS change
-    def visit_unary(self, unary, **kw):
-        if unary.operator:
-            if unary.modifier:
-                raise exc.CompileError(
-                    "Unary expression does not support operator "
-                    "and modifier simultaneously"
-                )
-            disp = self._get_operator_dispatch(
-                unary.operator, "unary", "operator"
-            )
-            if disp:
-                return disp(unary, unary.operator, **kw)
-            else:
-                return self._generate_generic_unary_operator(
-                    unary, OPERATORS[unary.operator], **kw
-                )
-        elif unary.modifier:
-            disp = self._get_operator_dispatch(
-                unary.modifier, "unary", "modifier"
-            )
-            if disp:
-                return disp(unary, unary.modifier, **kw)
-            else:
-                return self._generate_generic_unary_modifier(
-                    unary, OPERATORS[unary.modifier], **kw
-                )
-        else:
-            raise exc.CompileError(
-                "Unary expression has no operator or modifier"
-            )
-
-    # get operators
-    def visit_binary(
-        self, binary, override_operator=None, eager_grouping=False, **kw
-    ):
-
-        # don't allow "? = ?" to render
-        if (
-            self.ansi_bind_rules
-            and isinstance(binary.left, elements.BindParameter)
-            and isinstance(binary.right, elements.BindParameter)
-        ):
-            kw["literal_binds"] = True
-
-        operator_ = override_operator or binary.operator
-        # print("MLOG: operator_: ", operator_)
-        disp = self._get_operator_dispatch(operator_, "binary", None)
-        if disp:
-            return disp(binary, operator_, **kw)
-        else:
-            try:
-                opstring = OPERATORS[operator_]
-                # print("MLOG: opstring: ", opstring)
-            except KeyError as err:
-                util.raise_(
-                    exc.UnsupportedCompilationError(self, operator_),
-                    replace_context=err,
-                )
-            else:
-                return self._generate_generic_binary(binary, opstring, **kw)
-    
-    def _generate_generic_binary(
-        self, binary, opstring, eager_grouping=False, **kw
-    ):
-
-        _in_binary = kw.get("_in_binary", False)
-
-        kw["_in_binary"] = True
-        # print("---------")
-        leftstr = binary.left._compiler_dispatch(
-            self, eager_grouping=eager_grouping, **kw
-        )
-        rightstr = binary.right._compiler_dispatch(
-            self, eager_grouping=eager_grouping, **kw
-        )
-
-        if opstring == OPERATORS[operators.is_]:
-            if rightstr == "NULL":
-                text = " isNull(" + leftstr + ")"
-            else:
-                text = leftstr + opstring + rightstr
-        elif opstring == OPERATORS[operators.isnot]:
-            if rightstr == "NULL":
-                text = " !isNull(" + leftstr + ")"
-            else:
-                text = leftstr + opstring + rightstr
-        elif opstring == OPERATORS[operators.notin_op]:
-            text = "not " + leftstr + " in " + rightstr
-        else:
-            text = leftstr + opstring + rightstr
-        # print("MLOG: generate_binary: ", text, type(binary.right))
-
-        if _in_binary and eager_grouping:
-            text = "(%s)" % text
-        # print("_generate_generic_binary: ", text)
-        return text
-    
-    def visit_like_op_binary(self, binary, operator, **kw):
-        escape = binary.modifiers.get("escape", None)
-
-        # TODO: use ternary here, not "and"/ "or"
-        return "%s like %s" % (
-            binary.left._compiler_dispatch(self, **kw),
-            binary.right._compiler_dispatch(self, **kw),
-        ) + (
-            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
-            if escape
-            else ""
-        )
-
-    def visit_notlike_op_binary(self, binary, operator, **kw):
-        escape = binary.modifiers.get("escape", None)
-        return "%s not like %s" % (
-            binary.left._compiler_dispatch(self, **kw),
-            binary.right._compiler_dispatch(self, **kw),
-        ) + (
-            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
-            if escape
-            else ""
-        )
-
-    def visit_ilike_op_binary(self, binary, operator, **kw):
-        escape = binary.modifiers.get("escape", None)
-        return "lower(%s) like lower(%s)" % (
-            binary.left._compiler_dispatch(self, **kw),
-            binary.right._compiler_dispatch(self, **kw)
-        ) + (
-            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
-            if escape
-            else ""
-        )
-    
-    def visit_notilike_op_binary(self, binary, operator, **kw):
-        escape = binary.modifiers.get("escape", None)
-        return "lower(%s) not like lower(%s)" % (
-            binary.left._compiler_dispatch(self, **kw),
-            binary.right._compiler_dispatch(self, **kw),
-        ) + (
-            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
-            if escape
-            else ""
-        )
-
-    def render_literal_bindparam(self, bindparam, **kw):
-        value = bindparam.effective_value
-        # print("type: ", bindparam.type)
-        renderstr = self.render_literal_value(value, bindparam.type)
-        # print("render_literal_bindparam: value: ", value, "renderstr: ", renderstr)
-        return renderstr
-
-    def visit_bindparam(
-        self,
-        bindparam,
-        within_columns_clause=False,
-        literal_binds=False,
-        skip_bind_expression=False,
-        **kwargs
-    ):
-        # print("visit_bindparam1:")
-        if not skip_bind_expression:
-            impl = bindparam.type.dialect_impl(self.dialect)
-            if impl._has_bind_expression:
-                bind_expression = impl.bind_expression(bindparam)
-                return self.process(
-                    bind_expression,
-                    skip_bind_expression=True,
-                    within_columns_clause=within_columns_clause,
-                    literal_binds=literal_binds,
-                    **kwargs
-                )
-        # print("visit_bindparam2:")
-        if literal_binds or (within_columns_clause and self.ansi_bind_rules):
-            if bindparam.value is None and bindparam.callable is None:
-                raise exc.CompileError(
-                    "Bind parameter '%s' without a "
-                    "renderable value not allowed here." % bindparam.key
-                )
-            return self.render_literal_bindparam(
-                bindparam, within_columns_clause=True, **kwargs
-            )
-
-        name = self._truncate_bindparam(bindparam)
-
-        if name in self.binds:
-            existing = self.binds[name]
-            if existing is not bindparam:
-                if (
-                    existing.unique or bindparam.unique
-                ) and not existing.proxy_set.intersection(bindparam.proxy_set):
-                    raise exc.CompileError(
-                        "Bind parameter '%s' conflicts with "
-                        "unique bind parameter of the same name"
-                        % bindparam.key
-                    )
-                elif existing._is_crud or bindparam._is_crud:
-                    raise exc.CompileError(
-                        "bindparam() name '%s' is reserved "
-                        "for automatic usage in the VALUES or SET "
-                        "clause of this "
-                        "insert/update statement.   Please use a "
-                        "name other than column name when using bindparam() "
-                        "with insert() or update() (for example, 'b_%s')."
-                        % (bindparam.key, bindparam.key)
-                    )
-
-        self.binds[bindparam.key] = self.binds[name] = bindparam
-        # print("visit_bindparam3:")
-        return self.bindparam_string(
-            name, expanding=bindparam.expanding, **kwargs
-        )
-
-    def visit_select(
-        self,
-        select,
-        asfrom=False,
-        parens=True,
-        fromhints=None,
-        compound_index=0,
-        nested_join_translation=False,
-        select_wraps_for=None,
-        lateral=False,
-        **kwargs
-    ):
-        # print("here here here")
-        needs_nested_translation = (
-            select.use_labels
-            and not nested_join_translation
-            and not self.stack
-            and not self.dialect.supports_right_nested_joins
-        )
-
-        if needs_nested_translation:
-            transformed_select = self._transform_select_for_nested_joins(
-                select
-            )
-            text = self.visit_select(
-                transformed_select,
-                asfrom=asfrom,
-                parens=parens,
-                fromhints=fromhints,
-                compound_index=compound_index,
-                nested_join_translation=True,
-                **kwargs
-            )
-
-        toplevel = not self.stack
-        entry = self._default_stack_entry if toplevel else self.stack[-1]
-
-        populate_result_map = need_column_expressions = (
-            toplevel
-            or entry.get("need_result_map_for_compound", False)
-            or entry.get("need_result_map_for_nested", False)
-        )
-
-        if compound_index > 0:
-            populate_result_map = False
-
-        # this was first proposed as part of #3372; however, it is not
-        # reached in current tests and could possibly be an assertion
-        # instead.
-        if not populate_result_map and "add_to_result_map" in kwargs:
-            del kwargs["add_to_result_map"]
-
-        if needs_nested_translation:
-            if populate_result_map:
-                self._transform_result_map_for_nested_joins(
-                    select, transformed_select
-                )
-            return text
-
-        froms = self._setup_select_stack(select, entry, asfrom, lateral)
-
-        column_clause_args = kwargs.copy()
-        column_clause_args.update(
-            {"within_label_clause": False, "within_columns_clause": False}
-        )
-
-        text = "select "  # we're off to a good start !
-        # print("text01 >  ", text, select._whereclause)
-        if select._hints:
-            hint_text, byfrom = self._setup_select_hints(select)
-            if hint_text:
-                text += hint_text + " "
-        else:
-            byfrom = None
-        # print("text02 >  ", text, select._whereclause)
-        if select._prefixes:
-            text += self._generate_prefixes(select, select._prefixes, **kwargs)
-        # print("text03 >  ", text, select._whereclause)
-        text += self.get_select_precolumns(select, **kwargs)
-        # print("text04 >  ", text, select._whereclause)
-        # the actual list of columns to print in the SELECT column list.
-        inner_columns = [
-            c
-            for c in [
-                self._label_select_column(
-                    select,
-                    column,
-                    populate_result_map,
-                    asfrom,
-                    column_clause_args,
-                    name=name,
-                    need_column_expressions=need_column_expressions,
-                )
-                for name, column in select._columns_plus_names
-            ]
-            if c is not None
-        ]
-
-        if populate_result_map and select_wraps_for is not None:
-            # if this select is a compiler-generated wrapper,
-            # rewrite the targeted columns in the result map
-
-            translate = dict(
-                zip(
-                    [name for (key, name) in select._columns_plus_names],
-                    [
-                        name
-                        for (key, name) in select_wraps_for._columns_plus_names
-                    ],
-                )
-            )
-
-            self._result_columns = [
-                (key, name, tuple(translate.get(o, o) for o in obj), type_)
-                for key, name, obj, type_ in self._result_columns
-            ]
-
-        text = self._compose_select_body(
-            text, select, inner_columns, froms, byfrom, kwargs
-        )
-        # print("text05 >  ", text, select._whereclause)
-        if select._statement_hints:
-            per_dialect = [
-                ht
-                for (dialect_name, ht) in select._statement_hints
-                if dialect_name in ("*", self.dialect.name)
-            ]
-            if per_dialect:
-                text += " " + self.get_statement_hint_text(per_dialect)
-        # print("text06 >  ", text)
-        if self.ctes and toplevel:
-            text = self._render_cte_clause() + text
-        # print("text07 >  ", text)
-        if select._suffixes:
-            text += " " + self._generate_prefixes(
-                select, select._suffixes, **kwargs
-            )
-        # print("text08 >  ", text)
-        self.stack.pop(-1)
-
-        if (asfrom or lateral) and parens:
-            return "(" + text + ")"
-        else:
-            return text
-
-
-
-class DDBDDLCompiler(sql.compiler.DDLCompiler):
-    pass
-
-
-
-# class DDBExecutionContext(default.DefaultExecutionContext):
-#     def fire_sequence(self, seq, type_):
-#         """Get the next value from the sequence using ``gen_id()``."""
-
-#         return self._execute_scalar(
-#             "SELECT gen_id(%s, 1) FROM rdb$database"
-#             % self.identifier_preparer.format_sequence(seq),
-#             type_,
-#         )
-
-# class DDBExecutionContext_kinterbasdb(DDBExecutionContext):
-#     @property
-#     def rowcount(self):
-#         if self.execution_options.get(
-#             "enable_rowcount", self.dialect.enable_rowcount
-#         ):
-#             return self.cursor.rowcount
-#         else:
-#             return -1
-    
-
+import re
+from sqlalchemy.sql import compiler
+from sqlalchemy import exc
+from sqlalchemy import sql
+from sqlalchemy import types as sqltypes
+from sqlalchemy import util
+from sqlalchemy.sql import compiler
+from sqlalchemy.sql import operators
+from sqlalchemy.sql import elements
+
+
+RE_DATETIME_PATTERN = r"'(?P<Y>\d{4})-(?P<M>\d{2})-(?P<D>\d{2}) (?P<H>\d{2}):(?P<m>\d{2}):(?P<s>\d{2}).(?P<ms>\d{6})'"
+def _datetime_replace(matched):
+    matched_dict = matched.groupdict()
+    Y_ = matched_dict['Y']
+    M_ = matched_dict['M']
+    D_ = matched_dict['D']
+    H_ = matched_dict['H']
+    m_ = matched_dict['m']
+    s_ = matched_dict['s']
+    ms_ = matched_dict['ms']
+    return "{}.{}.{}T{}:{}:{}.{}".format(Y_, M_, D_, H_, m_, s_, ms_)
+
+RE_JOIN_AS = r"as (?P<name>\w*)__"
+def _join_as_replace(matched):
+    matched_dict = matched.groupdict()
+    name_ = matched_dict['name']
+    if name_ == "mme_inner":
+        return "as {}__".format(name_)
+    else:
+        return "as {}".format(name_)
+
+RE_JOIN_ON = r"(?P<name1>\w*) = (?P<name2>\w*)__"
+def _join_on_replace(matched):
+    matched_dict = matched.groupdict()
+    name1_ = matched_dict['name1']
+    name2_ = matched_dict['name2']
+    if name1_ == name2_:
+        return "{}".format(name1_)
+    else:
+        return "{} = {}__".format(name1_, name2_)
+
+OPERATORS = {
+    # binary
+    operators.and_: " && ",         # sqlparse will detect "and"/"AND" and add '\n' to sql string    refine link:sqlparse.__init__.format -> ReindentFilter._next_token
+    operators.or_: " || ",
+    operators.add: " + ",
+    operators.mul: " * ",
+    operators.sub: " - ",
+    operators.div: " / ",
+    operators.mod: " % ",
+    operators.truediv: " / ",
+    operators.neg: "-",
+    operators.lt: " < ",
+    operators.le: " <= ",
+    operators.ne: " != ",
+    operators.gt: " > ",
+    operators.ge: " >= ",
+    operators.eq: " = ",
+    operators.is_distinct_from: " IS DISTINCT FROM ",
+    operators.isnot_distinct_from: " IS NOT DISTINCT FROM ",
+    operators.concat_op: " || ",
+    operators.match_op: " MATCH ",
+    operators.notmatch_op: " NOT MATCH ",
+    operators.in_op: " in ",
+    operators.notin_op: " not in ",
+    operators.comma_op: ", ",
+    operators.from_: " from ",
+    operators.as_: " as ",
+    operators.is_: " IS ",
+    operators.isnot: " IS NOT ",
+    operators.collate: " COLLATE ",
+    # unary
+    operators.exists: "EXISTS ",
+    operators.distinct_op: "DISTINCT ",
+    operators.inv: "NOT ",
+    operators.any_op: "ANY ",
+    operators.all_op: "ALL ",
+    # modifiers
+    operators.desc_op: " desc",
+    operators.asc_op: " asc",
+    operators.nullsfirst_op: " NULLS FIRST",
+    operators.nullslast_op: " NULLS LAST",
+}
+
+## Preparer for sql string
+class DDBIdentifierPreparer(sql.compiler.IdentifierPreparer):
+    def __init__(self, dialect):
+        # here changed the initial_quote to "TMP_"
+        super(DDBIdentifierPreparer, self).__init__(dialect, omit_schema=True, initial_quote="")
+
+    # TODO: delete
+    def format_label(self, label, name=None):
+        # print("MLOG [format_label] label=", label, " name=", name)
+        return self.quote(name or label.name)
+
+    # TODO: delete
+    def quote(self, ident, force=None):
+        """Conditionally quote an identfier.
+
+        The identifier is quoted if it is a reserved word, contains
+        quote-necessary characters, or is an instance of
+        :class:`.quoted_name` which includes ``quote`` set to ``True``.
+
+        Subclasses can override this to provide database-dependent
+        quoting behavior for identifier names.
+
+        :param ident: string identifier
+        :param force: unused
+
+            .. deprecated:: 0.9
+
+                The :paramref:`.IdentifierPreparer.quote.force`
+                parameter is deprecated and will be removed in a future
+                release.  This flag has no effect on the behavior of the
+                :meth:`.IdentifierPreparer.quote` method; please refer to
+                :class:`.quoted_name`.
+
+        """
+        if force is not None:
+            # not using the util.deprecated_params() decorator in this
+            # case because of the additional function call overhead on this
+            # very performance-critical spot.
+            util.warn_deprecated(
+                "The IdentifierPreparer.quote.force parameter is "
+                "deprecated and will be removed in a future release.  This "
+                "flag has no effect on the behavior of the "
+                "IdentifierPreparer.quote method; please refer to "
+                "quoted_name()."
+            )
+
+        force = getattr(ident, "quote", None)
+
+        if force is None:
+            if ident in self._strings:
+                return self._strings[ident]
+            else:
+                if self._requires_quotes(ident):
+                    self._strings[ident] = self.quote_identifier(ident)
+                else:
+                    self._strings[ident] = ident
+                return self._strings[ident]
+        elif force:
+            return self.quote_identifier(ident)
+        else:
+            return ident
+        
+    # TODO: delete
+    def quote_identifier(self, value):
+        """Quote an identifier.
+
+        Subclasses should override this to provide database-dependent
+        quoting behavior.
+        """
+
+        return (
+            self.initial_quote
+            + self._escape_identifier(value)
+            + self.final_quote
+        )
+
+## SQLAlchemy types to DolphinDB types
+class DDBTypeCompiler(compiler.GenericTypeCompiler):
+    def visit_String(self, type_, **kw):
+        return 'STRING'
+    
+    def visit_DECIMAL(self, type_, **kw):
+        return 'DOUBLE'
+
+    def visit_VARCHAR(self, type_, **kw):
+        return 'STRING'
+
+    def visit_unicode_text(self, type_, **kw):
+        return 'STRING'
+
+## SQLAlchemy SQL to DolphinDB SQL
+class DDBCompiler(compiler.SQLCompiler):
+    OPERATORS = OPERATORS
+
+    ansi_bind_rules = True
+    def visit_cast(self, cast, **kwargs):
+        # print("cast: ", cast)
+        # print(type(cast))
+        # print("kwargs: ", kwargs)
+        return "cast(%s, %s)" % (
+            cast.clause._compiler_dispatch(self, **kwargs),
+            cast.typeclause._compiler_dispatch(self, **kwargs),
+        )
+
+    def visit_label(
+        self,
+        label,
+        add_to_result_map=None,
+        within_label_clause=False,
+        within_columns_clause=False,
+        render_label_as_label=None,
+        **kw
+    ):
+        # only render labels within the columns clause
+        # or ORDER BY clause of a select.  dialect-specific compilers
+        # can modify this behavior.
+        render_label_with_as = (
+            within_columns_clause and not within_label_clause
+        )
+        render_label_only = render_label_as_label is label
+        # print("pre labelname: ", label.name, type(label))
+        labelname = ""
+        if render_label_only or render_label_with_as:
+            if isinstance(label.name, elements._truncated_label):
+                labelname = self._truncated_identifier("colident", label.name)
+            else:
+                labelname = label.name
+        ## labelname has `(` and `)`.
+        #  replace them with `TMP_`.
+        if labelname.find('(')!=-1 and labelname.find(')')!=-1:
+            labelname = labelname.replace('(', "TMP_")
+            labelname = labelname.replace(')', "TMP_")
+
+        # print("format_label:", label, "|", labelname)
+        if render_label_with_as:
+            if add_to_result_map is not None:
+                add_to_result_map(
+                    labelname,
+                    label.name,
+                    (label, labelname) + label._alt_names,
+                    label.type,
+                )
+            # print("ffff", self.preparer.format_label(label, labelname))
+            pretmp = label.element._compiler_dispatch(
+                    self,
+                    within_columns_clause=True,
+                    within_label_clause=True,
+                    **kw
+                )
+            tmp =  (
+                pretmp
+                + OPERATORS[operators.as_]
+                + self.preparer.format_label(label, labelname)
+            )
+            ## replace keywords
+            if tmp.find("AVG(") != -1:
+                tmp = tmp.replace("AVG(", "avg(")
+            if tmp.find("COUNT(*)") != -1:
+                tmp = tmp.replace("COUNT(*)", "count(*)")
+            if tmp.find("count(DISTINCT ") != -1:
+                tmp = tmp.replace("count(DISTINCT ", "(tmp_->count(distinct(tmp_)))(")
+            if tmp.find("__timestamp") != -1:
+                return pretmp
+                tmp = tmp.replace("__timestamp", pretmp)
+            # print("render_label_with_as: ", tmp)
+            return tmp
+        elif render_label_only:
+
+            tmp = self.preparer.format_label(label, labelname)
+            # print("render_label_only: ", tmp)
+            return tmp
+        else:
+            tmp = label.element._compiler_dispatch(
+                self, within_columns_clause=False, **kw
+            )
+            # print("else: ", tmp)
+            return tmp
+
+    def get_render_as_alias_suffix(self, alias_name_text):
+        return " as " + alias_name_text
+
+    def group_by_clause(self, select, **kw):
+        """allow dialects to customize how GROUP BY is rendered."""
+
+        group_by = select._group_by_clause._compiler_dispatch(self, **kw)
+        if group_by:
+            return " group by " + group_by
+        else:
+            return ""
+
+    def order_by_clause(self, select, **kw):
+        """allow dialects to customize how ORDER BY is rendered."""
+
+        order_by = select._order_by_clause._compiler_dispatch(self, **kw)
+        if order_by:
+            return " order by " + order_by
+        else:
+            return ""
+
+    def visit_table(
+        self,
+        table,
+        asfrom=False,
+        iscrud=False,
+        ashint=False,
+        fromhints=None,
+        use_schema=True,
+        **kwargs
+    ):
+        if asfrom or ashint:
+            effective_schema = self.preparer.schema_for_object(table)
+
+            if use_schema and effective_schema:
+                if(effective_schema=="shared_table"):
+                    ret = (self.preparer.quote(table.name))
+                else:
+                    ret = 'loadTable("{}", "{}")'.format(effective_schema, table.name)
+            else:
+                ret = self.preparer.quote(table.name)
+            if fromhints and table in fromhints:
+                ret = self.format_from_hint_text(
+                    ret, table, fromhints[table], iscrud
+                )
+            return ret
+        else:
+            return ""
+
+    # TODO: need to complete [full join] and [outer join]
+    #       and to check [join]
+    def visit_join(self, join, asfrom=False, **kwargs):
+        if join.full:
+            return "[TODO LIST]"
+        elif join.isouter:
+            return "[TODO LIST]"
+        else:
+            str_l = join.left._compiler_dispatch(self, asfrom=True, **kwargs)
+            str_r = join.right._compiler_dispatch(self, asfrom=True, **kwargs)
+            str_r = re.sub(RE_JOIN_AS, _join_as_replace, str_r)
+            str_e = join.onclause._compiler_dispatch(self, **kwargs)
+            str_o = re.sub(RE_JOIN_ON, _join_on_replace, str_e)
+            if str_e != str_o:
+                return "ej((" + str_l + "), (" + str_r + "), `" + str_o + ")"
+            else:
+                return "ej((" + str_l + "), (" + str_r + "), `" + str_o + ", `" + str_e + ")"
+    
+    # not use
+    # now using `top_clause` instead
+    def limit_clause(self, select, **kw):
+        text = ""
+        # TODO: need to support group by + limit and offset has problem
+        if select._limit_clause is not None:
+            a = self.process(select._limit_clause, **kw)
+            # print("MLOG limit process: ", a, type(a))
+            text += " limit " + self.process(select._limit_clause, **kw)
+        if select._offset_clause is not None:
+            if select._limit_clause is None:
+                text += " limit -1"
+            text += " offset " + self.process(select._offset_clause, **kw)
+        return text
+    
+    def top_clause(self, select, **kw):
+        text = " top "
+        if select._limit_clause is not None and select._offset_clause is None:
+            text += "0:" + self.process(select._limit_clause, **kw) + " "
+        if select._limit_clause is not None and select._offset_clause is not None:
+            limitnum = (int)(self.process(select._limit_clause, **kw))
+            offsetnum = (int)(self.process(select._offset_clause, **kw))
+            text += (str)(offsetnum) + ":" + (str)(offsetnum + limitnum) + " "
+        if select._limit_clause is None and select._offset_clause is not None:
+            text += self.process(select._offset_clause, **kw) + ":50000 "
+        # if select._limit_clause is None and select._offset_clause is None:
+        #     text += "0:50000"
+        return text
+
+    def _compose_select_body(
+        self, text, select, inner_columns, froms, byfrom, kwargs
+    ):
+        # if (
+        #     select._limit_clause is not None
+        #     or select._offset_clause is not None
+        # ):
+            # TODO: need to support group by + limit
+            # text = "select * from (" + text + ") "
+        toptext = self.top_clause(select, **kwargs)
+        text += ", ".join(inner_columns)
+        if froms:
+            text += " from "
+            if select._hints:
+                text += ", ".join(
+                    [
+                        f._compiler_dispatch(
+                            self, asfrom=True, fromhints=byfrom, **kwargs
+                        )
+                        for f in froms
+                    ]
+                )
+            else:
+                text += ", ".join(
+                    [
+                        f._compiler_dispatch(self, asfrom=True, **kwargs)
+                        for f in froms
+                    ]
+                )
+        else:
+            text += self.default_from()
+        # print("MLOG: Start whereclause")
+        if select._whereclause is not None:
+            # print("**kwargs: ", kwargs)
+            t = select._whereclause._compiler_dispatch(self, **kwargs)
+            ## TableColumn.dttm_sql_literal "%Y-%m-%d %H:%M:%S.%f"
+            t = re.sub(RE_DATETIME_PATTERN, _datetime_replace, t)
+            if t:
+                text += " where " + t
+        # print("MLOG: End whereclause")
+
+        if select._group_by_clause.clauses:
+            text += self.group_by_clause(select, **kwargs)
+
+        if select._having is not None:
+            t = select._having._compiler_dispatch(self, **kwargs)
+            if t:
+                text += " having " + t
+
+        if select._order_by_clause.clauses:
+            text += self.order_by_clause(select, **kwargs)
+        
+        if select._for_update_arg is not None:
+            text += self.for_update_clause(select, **kwargs)
+
+        if (
+            select._limit_clause is not None
+            or select._offset_clause is not None
+        ):
+            text = "select " + toptext + " * from (" + text + ")"
+
+        return text
+
+    # for OPERATORS changes
+    # visit_OPERATORS 
+    def visit_clauselist(self, clauselist, **kw):
+        sep = clauselist.operator
+        if sep is None:
+            sep = " "
+        else:
+            sep = OPERATORS[clauselist.operator]
+            # print("OPERATORS: ", sep)
+
+        text = sep.join(
+            s
+            for s in (
+                c._compiler_dispatch(self, **kw) for c in clauselist.clauses
+            )
+            if s
+        )
+        # TODO: "insert value"
+        if clauselist._tuple_values and self.dialect.tuple_in_values:
+            text = "VALUES " + text
+        # print("MOG: visit_clauselist: ", text)
+        return text
+
+    # for OPERATORS change
+    def visit_unary(self, unary, **kw):
+        if unary.operator:
+            if unary.modifier:
+                raise exc.CompileError(
+                    "Unary expression does not support operator "
+                    "and modifier simultaneously"
+                )
+            disp = self._get_operator_dispatch(
+                unary.operator, "unary", "operator"
+            )
+            if disp:
+                return disp(unary, unary.operator, **kw)
+            else:
+                return self._generate_generic_unary_operator(
+                    unary, OPERATORS[unary.operator], **kw
+                )
+        elif unary.modifier:
+            disp = self._get_operator_dispatch(
+                unary.modifier, "unary", "modifier"
+            )
+            if disp:
+                return disp(unary, unary.modifier, **kw)
+            else:
+                return self._generate_generic_unary_modifier(
+                    unary, OPERATORS[unary.modifier], **kw
+                )
+        else:
+            raise exc.CompileError(
+                "Unary expression has no operator or modifier"
+            )
+
+    # get operators
+    def visit_binary(
+        self, binary, override_operator=None, eager_grouping=False, **kw
+    ):
+
+        # don't allow "? = ?" to render
+        if (
+            self.ansi_bind_rules
+            and isinstance(binary.left, elements.BindParameter)
+            and isinstance(binary.right, elements.BindParameter)
+        ):
+            kw["literal_binds"] = True
+
+        operator_ = override_operator or binary.operator
+        # print("MLOG: operator_: ", operator_)
+        disp = self._get_operator_dispatch(operator_, "binary", None)
+        if disp:
+            return disp(binary, operator_, **kw)
+        else:
+            try:
+                opstring = OPERATORS[operator_]
+                # print("MLOG: opstring: ", opstring)
+            except KeyError as err:
+                util.raise_(
+                    exc.UnsupportedCompilationError(self, operator_),
+                    replace_context=err,
+                )
+            else:
+                return self._generate_generic_binary(binary, opstring, **kw)
+    
+    def _generate_generic_binary(
+        self, binary, opstring, eager_grouping=False, **kw
+    ):
+
+        _in_binary = kw.get("_in_binary", False)
+
+        kw["_in_binary"] = True
+        # print("---------")
+        leftstr = binary.left._compiler_dispatch(
+            self, eager_grouping=eager_grouping, **kw
+        )
+        rightstr = binary.right._compiler_dispatch(
+            self, eager_grouping=eager_grouping, **kw
+        )
+
+        if opstring == OPERATORS[operators.is_]:
+            if rightstr == "NULL":
+                text = " isNull(" + leftstr + ")"
+            else:
+                text = leftstr + opstring + rightstr
+        elif opstring == OPERATORS[operators.isnot]:
+            if rightstr == "NULL":
+                text = " !isNull(" + leftstr + ")"
+            else:
+                text = leftstr + opstring + rightstr
+        elif opstring == OPERATORS[operators.notin_op]:
+            text = "not " + leftstr + " in " + rightstr
+        else:
+            text = leftstr + opstring + rightstr
+        # print("MLOG: generate_binary: ", text, type(binary.right))
+
+        if _in_binary and eager_grouping:
+            text = "(%s)" % text
+        # print("_generate_generic_binary: ", text)
+        return text
+    
+    def visit_like_op_binary(self, binary, operator, **kw):
+        escape = binary.modifiers.get("escape", None)
+
+        # TODO: use ternary here, not "and"/ "or"
+        return "%s like %s" % (
+            binary.left._compiler_dispatch(self, **kw),
+            binary.right._compiler_dispatch(self, **kw),
+        ) + (
+            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
+            if escape
+            else ""
+        )
+
+    def visit_notlike_op_binary(self, binary, operator, **kw):
+        escape = binary.modifiers.get("escape", None)
+        return "%s not like %s" % (
+            binary.left._compiler_dispatch(self, **kw),
+            binary.right._compiler_dispatch(self, **kw),
+        ) + (
+            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
+            if escape
+            else ""
+        )
+
+    def visit_ilike_op_binary(self, binary, operator, **kw):
+        escape = binary.modifiers.get("escape", None)
+        return "lower(%s) like lower(%s)" % (
+            binary.left._compiler_dispatch(self, **kw),
+            binary.right._compiler_dispatch(self, **kw)
+        ) + (
+            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
+            if escape
+            else ""
+        )
+    
+    def visit_notilike_op_binary(self, binary, operator, **kw):
+        escape = binary.modifiers.get("escape", None)
+        return "lower(%s) not like lower(%s)" % (
+            binary.left._compiler_dispatch(self, **kw),
+            binary.right._compiler_dispatch(self, **kw),
+        ) + (
+            " ESCAPE " + self.render_literal_value(escape, sqltypes.STRINGTYPE)
+            if escape
+            else ""
+        )
+
+    def render_literal_bindparam(self, bindparam, **kw):
+        value = bindparam.effective_value
+        # print("type: ", bindparam.type)
+        renderstr = self.render_literal_value(value, bindparam.type)
+        # print("render_literal_bindparam: value: ", value, "renderstr: ", renderstr)
+        return renderstr
+
+    def visit_bindparam(
+        self,
+        bindparam,
+        within_columns_clause=False,
+        literal_binds=False,
+        skip_bind_expression=False,
+        **kwargs
+    ):
+        # print("visit_bindparam1:")
+        if not skip_bind_expression:
+            impl = bindparam.type.dialect_impl(self.dialect)
+            if impl._has_bind_expression:
+                bind_expression = impl.bind_expression(bindparam)
+                return self.process(
+                    bind_expression,
+                    skip_bind_expression=True,
+                    within_columns_clause=within_columns_clause,
+                    literal_binds=literal_binds,
+                    **kwargs
+                )
+        # print("visit_bindparam2:")
+        if literal_binds or (within_columns_clause and self.ansi_bind_rules):
+            if bindparam.value is None and bindparam.callable is None:
+                raise exc.CompileError(
+                    "Bind parameter '%s' without a "
+                    "renderable value not allowed here." % bindparam.key
+                )
+            return self.render_literal_bindparam(
+                bindparam, within_columns_clause=True, **kwargs
+            )
+
+        name = self._truncate_bindparam(bindparam)
+
+        if name in self.binds:
+            existing = self.binds[name]
+            if existing is not bindparam:
+                if (
+                    existing.unique or bindparam.unique
+                ) and not existing.proxy_set.intersection(bindparam.proxy_set):
+                    raise exc.CompileError(
+                        "Bind parameter '%s' conflicts with "
+                        "unique bind parameter of the same name"
+                        % bindparam.key
+                    )
+                elif existing._is_crud or bindparam._is_crud:
+                    raise exc.CompileError(
+                        "bindparam() name '%s' is reserved "
+                        "for automatic usage in the VALUES or SET "
+                        "clause of this "
+                        "insert/update statement.   Please use a "
+                        "name other than column name when using bindparam() "
+                        "with insert() or update() (for example, 'b_%s')."
+                        % (bindparam.key, bindparam.key)
+                    )
+
+        self.binds[bindparam.key] = self.binds[name] = bindparam
+        # print("visit_bindparam3:")
+        return self.bindparam_string(
+            name, expanding=bindparam.expanding, **kwargs
+        )
+
+    def visit_select(
+        self,
+        select,
+        asfrom=False,
+        parens=True,
+        fromhints=None,
+        compound_index=0,
+        nested_join_translation=False,
+        select_wraps_for=None,
+        lateral=False,
+        **kwargs
+    ):
+        # print("here here here")
+        needs_nested_translation = (
+            select.use_labels
+            and not nested_join_translation
+            and not self.stack
+            and not self.dialect.supports_right_nested_joins
+        )
+
+        if needs_nested_translation:
+            transformed_select = self._transform_select_for_nested_joins(
+                select
+            )
+            text = self.visit_select(
+                transformed_select,
+                asfrom=asfrom,
+                parens=parens,
+                fromhints=fromhints,
+                compound_index=compound_index,
+                nested_join_translation=True,
+                **kwargs
+            )
+
+        toplevel = not self.stack
+        entry = self._default_stack_entry if toplevel else self.stack[-1]
+
+        populate_result_map = need_column_expressions = (
+            toplevel
+            or entry.get("need_result_map_for_compound", False)
+            or entry.get("need_result_map_for_nested", False)
+        )
+
+        if compound_index > 0:
+            populate_result_map = False
+
+        # this was first proposed as part of #3372; however, it is not
+        # reached in current tests and could possibly be an assertion
+        # instead.
+        if not populate_result_map and "add_to_result_map" in kwargs:
+            del kwargs["add_to_result_map"]
+
+        if needs_nested_translation:
+            if populate_result_map:
+                self._transform_result_map_for_nested_joins(
+                    select, transformed_select
+                )
+            return text
+
+        froms = self._setup_select_stack(select, entry, asfrom, lateral)
+
+        column_clause_args = kwargs.copy()
+        column_clause_args.update(
+            {"within_label_clause": False, "within_columns_clause": False}
+        )
+
+        text = "select "  # we're off to a good start !
+        # print("text01 >  ", text, select._whereclause)
+        if select._hints:
+            hint_text, byfrom = self._setup_select_hints(select)
+            if hint_text:
+                text += hint_text + " "
+        else:
+            byfrom = None
+        # print("text02 >  ", text, select._whereclause)
+        if select._prefixes:
+            text += self._generate_prefixes(select, select._prefixes, **kwargs)
+        # print("text03 >  ", text, select._whereclause)
+        text += self.get_select_precolumns(select, **kwargs)
+        # print("text04 >  ", text, select._whereclause)
+        # the actual list of columns to print in the SELECT column list.
+        inner_columns = [
+            c
+            for c in [
+                self._label_select_column(
+                    select,
+                    column,
+                    populate_result_map,
+                    asfrom,
+                    column_clause_args,
+                    name=name,
+                    need_column_expressions=need_column_expressions,
+                )
+                for name, column in select._columns_plus_names
+            ]
+            if c is not None
+        ]
+
+        if populate_result_map and select_wraps_for is not None:
+            # if this select is a compiler-generated wrapper,
+            # rewrite the targeted columns in the result map
+
+            translate = dict(
+                zip(
+                    [name for (key, name) in select._columns_plus_names],
+                    [
+                        name
+                        for (key, name) in select_wraps_for._columns_plus_names
+                    ],
+                )
+            )
+
+            self._result_columns = [
+                (key, name, tuple(translate.get(o, o) for o in obj), type_)
+                for key, name, obj, type_ in self._result_columns
+            ]
+
+        text = self._compose_select_body(
+            text, select, inner_columns, froms, byfrom, kwargs
+        )
+        # print("text05 >  ", text, select._whereclause)
+        if select._statement_hints:
+            per_dialect = [
+                ht
+                for (dialect_name, ht) in select._statement_hints
+                if dialect_name in ("*", self.dialect.name)
+            ]
+            if per_dialect:
+                text += " " + self.get_statement_hint_text(per_dialect)
+        # print("text06 >  ", text)
+        if self.ctes and toplevel:
+            text = self._render_cte_clause() + text
+        # print("text07 >  ", text)
+        if select._suffixes:
+            text += " " + self._generate_prefixes(
+                select, select._suffixes, **kwargs
+            )
+        # print("text08 >  ", text)
+        self.stack.pop(-1)
+
+        if (asfrom or lateral) and parens:
+            return "(" + text + ")"
+        else:
+            return text
+
+
+
+class DDBDDLCompiler(sql.compiler.DDLCompiler):
+    pass
+
+
+
+# class DDBExecutionContext(default.DefaultExecutionContext):
+#     def fire_sequence(self, seq, type_):
+#         """Get the next value from the sequence using ``gen_id()``."""
+
+#         return self._execute_scalar(
+#             "SELECT gen_id(%s, 1) FROM rdb$database"
+#             % self.identifier_preparer.format_sequence(seq),
+#             type_,
+#         )
+
+# class DDBExecutionContext_kinterbasdb(DDBExecutionContext):
+#     @property
+#     def rowcount(self):
+#         if self.execution_options.get(
+#             "enable_rowcount", self.dialect.enable_rowcount
+#         ):
+#             return self.cursor.rowcount
+#         else:
+#             return -1
+    
+
```

## pydolphindb/sqlalchemy/dialect.py

 * *Ordering differences only*

```diff
@@ -1,221 +1,221 @@
-from sqlalchemy import  types as sqltypes
-from sqlalchemy.engine import default, reflection
-from sqlalchemy import util
-
-from .compiler import(
-    DDBCompiler,
-    DDBDDLCompiler,
-    DDBTypeCompiler,
-    DDBIdentifierPreparer,
-    # DDBExecutionContext,
-)
-from .types import(
-    DDBString,
-)
-
-ischema_names = {
-    "BOOL":     sqltypes.BOOLEAN,       # bool
-    "CHAR":     sqltypes.CHAR,          # int8
-    "SHORT":    sqltypes.SMALLINT,      # int16
-    "INT":      sqltypes.INTEGER,       # int32
-    "LONG":     sqltypes.NUMERIC,       # int64
-    "DATE":     sqltypes.TIMESTAMP,      # DATE
-    "MONTH":    sqltypes.DATETIME,      
-    "TIME":     sqltypes.TIME,
-    "MINUTE":   sqltypes.TIME,
-    "SECOND":   sqltypes.TIME,
-    "DATETIME": sqltypes.DATETIME,
-    "TIMESTAMP":    sqltypes.TIMESTAMP,
-    "NANOTIME":     sqltypes.TIME,
-    "NANOTIMESTAMP":sqltypes.TIMESTAMP,
-    "FLOAT":    sqltypes.FLOAT,         # float32   # precision problem
-    "DOUBLE":   sqltypes.DECIMAL,       # float64
-    "SYMBOL":   DDBString,      # symbol
-    "STRING":   DDBString,      # string
-}
-
-colspecs = {
-    sqltypes.TEXT:          DDBString,
-    sqltypes.UnicodeText:   DDBString,
-    sqltypes.VARCHAR:       DDBString,
-    sqltypes.Unicode:       DDBString,
-}
-
-class DolphinDBDialect(default.DefaultDialect):
-    name = "dolphindb"
-    statement_compiler = DDBCompiler
-    ddl_compiler = DDBDDLCompiler
-    preparer = DDBIdentifierPreparer
-    type_compiler = DDBTypeCompiler
-
-    driver = "pydolphindb"
-    supports_sane_rowcount = False
-    supports_sane_multi_rowcount = False
-    supports_native_decimal = True
-
-    ischema_names = ischema_names
-    colspecs = colspecs
-
-    def __init__(self, **kwargs):
-        default.DefaultDialect.__init__(self, **kwargs)
-
-    def do_execute(self, cursor, statement, parameters, context=None):
-        # print("do execute >>>>>>>>>>")
-        # print("statement: ", statement)
-        # print("parameters: ", parameters)
-        statement = statement.replace("?", "%s")
-        # print("statement: ", statement)
-        # print("parameters: ", parameters)
-        cursor.execute(statement, parameters)
-
-    # def do_execute(self, cursor, sql, *args, **kwargs):
-    #     print("here>>>>>>>>>>")
-    #     print("sql: ", sql)
-    #     print("args: ", args)
-    #     print("kwargs: ", kwargs)
-    #     cursor.execute(sql, *args, **kwargs)
-
-    @classmethod
-    def dbapi(cls):
-        return __import__("pydolphindb")
-        
-    # TODO: need server support `select 1` clause
-    def has_table(self, connection, table_name, schema=None):
-        """Return ``True`` if the given table exists"""
-        if schema is not None:
-            current_schema = schema
-        else:
-            current_schema = self.default_schema_name
-        if current_schema == "shared_table":
-            # tblqry = """
-            #     select 1 as has_table from {}
-            # """.format(table_name)
-            tblqry = """
-                select name from objs(shared=true) where shared=true && name=`{}
-            """.format(table_name)
-            result = connection.execute(tblqry)
-            b = result.fetchone()
-            # print("has_table: ", b)
-            return b is not None
-        else:
-            tblqry = """
-                existsTable("{}", `{})
-            """.format(current_schema, table_name)
-            result = connection.execute(tblqry)
-            a = result.fetchone()
-            # print("has_table: ", a)
-            return a[0]
-
-    @reflection.cache
-    def get_table_names(self, connection, schema=None, **kw):
-        # print(">>>>>>> ")
-        if schema is not None:
-            current_schema = schema
-        else:
-            current_schema = self.default_schema_name
-
-        
-
-        # charset = self._connection_charset
-        # print("charset: ", charset)
-        # print("schema: ", current_schema)
-
-        if(current_schema=="shared_table"):
-            script = """
-                select name from objs(shared=true) where shared=true
-            """
-        else:
-            script = """
-                select * from (
-                    select distinct(tableName) 
-                    from getTabletsMeta("{}/%", "%", top=-1)
-                ) order by distinct_tableName
-                """.format(current_schema[5:])
-
-        # print("script: ", script)
-
-        rp = connection.execute(script)
-        return [r[0] for r in rp]
-
-    @reflection.cache
-    def get_pk_constraint(self, connection, table_name, schema=None, **kw):
-        return []
-
-    @reflection.cache
-    def get_foreign_keys(self, connection, table_name, schema=None, **kw):
-        return []
-
-    @reflection.cache
-    def get_unique_constraints(self, connection, table_name,
-                                schema=None, **kw):
-        return []
-
-    @reflection.cache
-    def get_indexes(self, connection, table_name, schema=None, **kw):
-        return []
-
-    @reflection.cache
-    def get_schema_names(self, connection, **kw):
-        # cursor = connection.execute(
-        #     """
-        #     select * from (
-        #         select distinct(tableName) 
-        #         from getTabletsMeta("/%", "%", top=-1)
-        #     ) order by distinct_tableName
-        #     """
-        # )
-        cursor = connection.execute(
-            """
-            schema = getDFSDatabases()
-            select * from table(schema) order by schema asc
-            """
-        )
-        return ["shared_table"] + [r[0] for r in cursor]
-
-    @reflection.cache
-    def get_columns(self, connection, table_name, schema=None, **kw):
-        # Query to extract the details of all the fields of the given table
-        if schema is not None:
-            current_schema = schema
-        else:
-            current_schema = self.default_schema_name
-        if(current_schema == "shared_table"):
-            tblqry = """
-                schema({})['colDefs']
-            """.format(table_name)
-        else:
-            tblqry = """
-                schema(loadTable("{}", "{}"))['colDefs']
-            """.format(current_schema, table_name)
-        result = connection.execute(tblqry)
-        cols = []
-        while True:
-            row = result.fetchone()
-            if row is None:
-                break
-            name = row['name']
-            typestr = row['typeString']
-            coltype = self.ischema_names.get(typestr)
-            if coltype is None:
-                util.warn(
-                    "Did not recognize type '%s' of column '%s'"
-                    % (typestr, name)
-                )
-                coltype = sqltypes.NULLTYPE
-            else:
-                coltype = coltype()
-            
-            # define value of this type
-            defvalue = None
-
-            col_d = {
-                "name": name,
-                "type": coltype,
-                "nullable": False,
-                "default": defvalue,
-                "autoincrement": "auto",
-            }
-
-            cols.append(col_d)
-        # print("get_columns: ", cols)
-        return cols
+from sqlalchemy import  types as sqltypes
+from sqlalchemy.engine import default, reflection
+from sqlalchemy import util
+
+from .compiler import(
+    DDBCompiler,
+    DDBDDLCompiler,
+    DDBTypeCompiler,
+    DDBIdentifierPreparer,
+    # DDBExecutionContext,
+)
+from .types import(
+    DDBString,
+)
+
+ischema_names = {
+    "BOOL":     sqltypes.BOOLEAN,       # bool
+    "CHAR":     sqltypes.CHAR,          # int8
+    "SHORT":    sqltypes.SMALLINT,      # int16
+    "INT":      sqltypes.INTEGER,       # int32
+    "LONG":     sqltypes.NUMERIC,       # int64
+    "DATE":     sqltypes.TIMESTAMP,      # DATE
+    "MONTH":    sqltypes.DATETIME,      
+    "TIME":     sqltypes.TIME,
+    "MINUTE":   sqltypes.TIME,
+    "SECOND":   sqltypes.TIME,
+    "DATETIME": sqltypes.DATETIME,
+    "TIMESTAMP":    sqltypes.TIMESTAMP,
+    "NANOTIME":     sqltypes.TIME,
+    "NANOTIMESTAMP":sqltypes.TIMESTAMP,
+    "FLOAT":    sqltypes.FLOAT,         # float32   # precision problem
+    "DOUBLE":   sqltypes.DECIMAL,       # float64
+    "SYMBOL":   DDBString,      # symbol
+    "STRING":   DDBString,      # string
+}
+
+colspecs = {
+    sqltypes.TEXT:          DDBString,
+    sqltypes.UnicodeText:   DDBString,
+    sqltypes.VARCHAR:       DDBString,
+    sqltypes.Unicode:       DDBString,
+}
+
+class DolphinDBDialect(default.DefaultDialect):
+    name = "dolphindb"
+    statement_compiler = DDBCompiler
+    ddl_compiler = DDBDDLCompiler
+    preparer = DDBIdentifierPreparer
+    type_compiler = DDBTypeCompiler
+
+    driver = "pydolphindb"
+    supports_sane_rowcount = False
+    supports_sane_multi_rowcount = False
+    supports_native_decimal = True
+
+    ischema_names = ischema_names
+    colspecs = colspecs
+
+    def __init__(self, **kwargs):
+        default.DefaultDialect.__init__(self, **kwargs)
+
+    def do_execute(self, cursor, statement, parameters, context=None):
+        # print("do execute >>>>>>>>>>")
+        # print("statement: ", statement)
+        # print("parameters: ", parameters)
+        statement = statement.replace("?", "%s")
+        # print("statement: ", statement)
+        # print("parameters: ", parameters)
+        cursor.execute(statement, parameters)
+
+    # def do_execute(self, cursor, sql, *args, **kwargs):
+    #     print("here>>>>>>>>>>")
+    #     print("sql: ", sql)
+    #     print("args: ", args)
+    #     print("kwargs: ", kwargs)
+    #     cursor.execute(sql, *args, **kwargs)
+
+    @classmethod
+    def dbapi(cls):
+        return __import__("pydolphindb")
+        
+    # TODO: need server support `select 1` clause
+    def has_table(self, connection, table_name, schema=None):
+        """Return ``True`` if the given table exists"""
+        if schema is not None:
+            current_schema = schema
+        else:
+            current_schema = self.default_schema_name
+        if current_schema == "shared_table":
+            # tblqry = """
+            #     select 1 as has_table from {}
+            # """.format(table_name)
+            tblqry = """
+                select name from objs(shared=true) where shared=true && name=`{}
+            """.format(table_name)
+            result = connection.execute(tblqry)
+            b = result.fetchone()
+            # print("has_table: ", b)
+            return b is not None
+        else:
+            tblqry = """
+                existsTable("{}", `{})
+            """.format(current_schema, table_name)
+            result = connection.execute(tblqry)
+            a = result.fetchone()
+            # print("has_table: ", a)
+            return a[0]
+
+    @reflection.cache
+    def get_table_names(self, connection, schema=None, **kw):
+        # print(">>>>>>> ")
+        if schema is not None:
+            current_schema = schema
+        else:
+            current_schema = self.default_schema_name
+
+        
+
+        # charset = self._connection_charset
+        # print("charset: ", charset)
+        # print("schema: ", current_schema)
+
+        if(current_schema=="shared_table"):
+            script = """
+                select name from objs(shared=true) where shared=true
+            """
+        else:
+            script = """
+                select * from (
+                    select distinct(tableName) 
+                    from getTabletsMeta("{}/%", "%", top=-1)
+                ) order by distinct_tableName
+                """.format(current_schema[5:])
+
+        # print("script: ", script)
+
+        rp = connection.execute(script)
+        return [r[0] for r in rp]
+
+    @reflection.cache
+    def get_pk_constraint(self, connection, table_name, schema=None, **kw):
+        return []
+
+    @reflection.cache
+    def get_foreign_keys(self, connection, table_name, schema=None, **kw):
+        return []
+
+    @reflection.cache
+    def get_unique_constraints(self, connection, table_name,
+                                schema=None, **kw):
+        return []
+
+    @reflection.cache
+    def get_indexes(self, connection, table_name, schema=None, **kw):
+        return []
+
+    @reflection.cache
+    def get_schema_names(self, connection, **kw):
+        # cursor = connection.execute(
+        #     """
+        #     select * from (
+        #         select distinct(tableName) 
+        #         from getTabletsMeta("/%", "%", top=-1)
+        #     ) order by distinct_tableName
+        #     """
+        # )
+        cursor = connection.execute(
+            """
+            schema = getDFSDatabases()
+            select * from table(schema) order by schema asc
+            """
+        )
+        return ["shared_table"] + [r[0] for r in cursor]
+
+    @reflection.cache
+    def get_columns(self, connection, table_name, schema=None, **kw):
+        # Query to extract the details of all the fields of the given table
+        if schema is not None:
+            current_schema = schema
+        else:
+            current_schema = self.default_schema_name
+        if(current_schema == "shared_table"):
+            tblqry = """
+                schema({})['colDefs']
+            """.format(table_name)
+        else:
+            tblqry = """
+                schema(loadTable("{}", "{}"))['colDefs']
+            """.format(current_schema, table_name)
+        result = connection.execute(tblqry)
+        cols = []
+        while True:
+            row = result.fetchone()
+            if row is None:
+                break
+            name = row['name']
+            typestr = row['typeString']
+            coltype = self.ischema_names.get(typestr)
+            if coltype is None:
+                util.warn(
+                    "Did not recognize type '%s' of column '%s'"
+                    % (typestr, name)
+                )
+                coltype = sqltypes.NULLTYPE
+            else:
+                coltype = coltype()
+            
+            # define value of this type
+            defvalue = None
+
+            col_d = {
+                "name": name,
+                "type": coltype,
+                "nullable": False,
+                "default": defvalue,
+                "autoincrement": "auto",
+            }
+
+            cols.append(col_d)
+        # print("get_columns: ", cols)
+        return cols
```

## pydolphindb/sqlalchemy/sa_version.py

 * *Ordering differences only*

```diff
@@ -1,7 +1,7 @@
-import sqlalchemy as sa
-from distutils.version import StrictVersion as V
-# from packaging import version as V
-
-SA_VERSION = V(sa.__version__)
-
-SA_1_1 = V('1.1a0')
+import sqlalchemy as sa
+from distutils.version import StrictVersion as V
+# from packaging import version as V
+
+SA_VERSION = V(sa.__version__)
+
+SA_1_1 = V('1.1a0')
```

## pydolphindb/sqlalchemy/types.py

 * *Ordering differences only*

```diff
@@ -1,11 +1,11 @@
-import sqlalchemy.types as sqltypes
-from sqlalchemy.sql import operators, expression
-from sqlalchemy.sql import default_comparator
-
-class DDBString(sqltypes.String):
-    __visit_name__ = "DDBString"
-    def literal_processor(self, dialect):
-        def process(value):
-            return '"%s"' % value
-
+import sqlalchemy.types as sqltypes
+from sqlalchemy.sql import operators, expression
+from sqlalchemy.sql import default_comparator
+
+class DDBString(sqltypes.String):
+    __visit_name__ = "DDBString"
+    def literal_processor(self, dialect):
+        def process(value):
+            return '"%s"' % value
+
         return process
```

## Comparing `pydolphindb-1.0.0.dist-info/METADATA` & `pydolphindb-1.0.1.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,160 +1,159 @@
-Metadata-Version: 2.1
-Name: pydolphindb
-Version: 1.0.0
-Summary: A python DolphinDB API based on DBAPI2.0 Specification
-Home-page: https://www.dolphindb.com
-Author: DolphinDB, Inc.
-Author-email: support@dolphindb.com
-License: DolphinDB
-Platform: any
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: dolphindb (>=1.30.21.1)
-Requires-Dist: sqlalchemy (<2.0,>=1.4)
-Requires-Dist: importlib-metadata (<=6.0.0,>=0.23)
-
-# pydolphindb
-
-- [pydolphindb](#pydolphindb)
-  - [1. Installing pydolphindb](#1-installing-pydolphindb)
-    - [1.1 Prerequisites](#11-prerequisites)
-    - [1.2 Installation](#12-installation)
-  - [2. Functions](#2-functions)
-    - [2.1 Function Reference](#21-function-reference)
-    - [2.2 Sample Code](#22-sample-code)
-  - [3. Connecting to DolphinDB Using SQLAlchemy](#3-connecting-to-dolphindb-using-sqlalchemy)
-  - [Related Links](#related-links)
-
-
-*pydolphindb* is a library that enables you to connect to the DolphinDB server in Python. It implements the classes and methods as defined in the [DolphinDB Python API specification](https://github.com/dolphindb/api_python3/blob/master/README.md) and is compliant with the Python Database API v2.0 specification ([PEP-249](https://www.python.org/dev/peps/pep-0249/)). *pydolphindb* contains a Python DolphinDB client library and supports connecting to DolphinDB using [SQLAlchemy](https://www.sqlalchemy.org/). 
-
-## 1. Installing pydolphindb
-
-### 1.1 Prerequisites
-
-Make sure you use:
-
-- Python 3.7 or higher
-- DolphinDB 1.30.21 or higher can also 2.00.9 or higher
-
-Install the following libraries:
-
-- dolphindb 1.30.21.1 or higher
-- sqlalchemy 1.4 or higher while lower than 2.0 
-
-### 1.2 Installation 
-
-Execute the following `pip` command:
-
-```
-pip install pydolphindb
-```
-
-## 2. Functions
-
-### 2.1 Function Reference
-
-| **Function**                                         | **Parameters**                                               | **Description**                                              |
-| :--------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
-| `pydolphindb.connect(host, port username, password)` | host (*string*) - hostname of the server to connect to.port (*integer*) *-* port number of the server to connect to.username (*string*) - username for login.password (*string*) - password for login. | Connect to database.                                         |
-| `connection.cursor()`                                | -                                                            | Create a cursor object.                                      |
-| `cursor.execute(script,Parameters = None)`           | script (*string*) - script to execute.parameters (*tuple, list or dictionary*) - Optional. Parameters used with script. | Execute script.If *parameters* is a list or tuple, use `%s` as a placeholder in the script. If *parameters* is a dict, use `%(name)s` as a placeholder in the script. |
-| `cursor.executemany(script,seq_of_parameters)`       | script (*string*) - script to execute.seq_of_parameters (*list* or *tuple*) - a sequence (list or tuple) of lists or tuples used with script. | Execute the script against all parameter sequences specified in `seq_of_parameters`. Use this function for a batch insert operation. |
-| `cursor.fetchone()`                                  | -                                                            | Fetch the next record.                                       |
-| `cursor.fetchmany(size)`                             | size (*integer*) - number of records to fetch.               | Fetch multiple (as specified by *size*) records.             |
-| `cursor.fetchall()`                                  | -                                                            | Fetch all records.                                           |
-
-Note: *pydolphindb* does not support functions to *commit* or *rollback* a transaction.
-
-### 2.2 Sample Code
-
-In this example, we import *pydolphindb* with the `import` command, then connect to DolphinDB with the `connect` function. Functions `execute` and `executemany` are called to create and write to a database, respectively, through the specified DolphinDB script. Functions `fetchone`, `fetchmany`, and `fetchall` are called to fetch data from the database. The connection is closed with the `close` function.
-
-```
-import pydolphindb
-
-# connect to database server
-db = pydolphindb.connect(host='localhost',
-                         port='8848',
-                         username='testuser',
-                         password='test123')
-
-# create a cursor object
-cursor = db.cursor()
-
-# DolphinDB script for creating a database
-script = """
-        dbPath = "dfs://valuedb"
-        if(existsDatabase(dbPath))
-            dropDatabase(dbPath)
-        t = table(100:100,`id`time`vol,[SYMBOL,DATE, INT])
-        db=database(dbPath,VALUE, `APPL`IBM`AMZN)
-        pt = db.createPartitionedTable(t, `pt, `id)
-"""
-
-# execute DolphinDB script with execute()
-cursor.execute(script)
-
-# execute DolphinDB script with executemany()
-cursor.executemany('insert into t values(%d, `%s, %.2f)',[(2,'b',3.5239),(3,'c',-0.93154)])
-
-# get the next record with fetchone()
-data = cursor.fetchone()
-
-# the result is None
-print ("Result:" + data)
-
-# get the next two records with fetchmany()
-data = cursor.fetchmany(size = 2)
-
-# get all records with fetchall()
-data = cursor.fetchall()
-
-# close connection
-db.close()
-```
-
-## 3. Connecting to DolphinDB Using SQLAlchemy
-
-[SQLAlchemy](https://www.sqlalchemy.org/) is a Python SQL toolkit and Object Relational Mapper which is designed for efficient database access. *pydolphindb* is a Python [DB API 2.0 (PEP 249)](https://peps.python.org/pep-0249/) client for DolphinDB. The DolphinDB SQLAlchemy dialect is supported so you can connect to the DolphinDB databases through a SQLAlchemy engine.
-
-The following script shows how to connect to and interact with DolphinDB through SQLAlchemy in Python:
-
-```
-from sqlalchemy import create_engine
-
-# create an engine for connection
-engine = create_engine("dolphindb://testuser:test123@localhost:8848")
-
-# DolphinDB script for a database query
-script = """
-    pt = loadTable("dfs://valuedb", "pt")
-    select * from pt
-"""
-
-# run script with execute()
-result = engine.execute(script)
-
-# print all results
-print(result.all())
-```
-
-Note:
-
-- The DolphinDB SQLAlchemy currently does not support ORM (object-relational mapping).
-- When creating engine, pass the DolphinDB database URL to `create_engine` as a string in the following pattern: `dolphindb://{user}:{password}@{host}:{port}`
-
-## Related Links
-
-- [DB API 2.0 (PEP 249)](https://peps.python.org/pep-0249/)
-- [DolphinDB Manual](https://dolphindb.com/help200/index.html)
-- [DolphinDB Python API](https://github.com/dolphindb/api_python3) 
-
-
+Metadata-Version: 2.1
+Name: pydolphindb
+Version: 1.0.1
+Summary: A python DolphinDB API based on DBAPI2.0 Specification
+Home-page: https://www.dolphindb.com
+Author: DolphinDB, Inc.
+Author-email: support@dolphindb.com
+License: DolphinDB
+Platform: any
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: dolphindb >=1.30.21.1
+Requires-Dist: sqlalchemy <2.0,>=1.4
+Requires-Dist: importlib-metadata >=0.23
+
+# pydolphindb
+
+- [pydolphindb](#pydolphindb)
+  - [1. Installing pydolphindb](#1-installing-pydolphindb)
+    - [1.1 Prerequisites](#11-prerequisites)
+    - [1.2 Installation](#12-installation)
+  - [2. Functions](#2-functions)
+    - [2.1 Function Reference](#21-function-reference)
+    - [2.2 Sample Code](#22-sample-code)
+  - [3. Connecting to DolphinDB Using SQLAlchemy](#3-connecting-to-dolphindb-using-sqlalchemy)
+  - [Related Links](#related-links)
+
+
+*pydolphindb* is a library that enables you to connect to the DolphinDB server in Python. It implements the classes and methods as defined in the [DolphinDB Python API specification](https://github.com/dolphindb/api_python3/blob/master/README.md) and is compliant with the Python Database API v2.0 specification ([PEP-249](https://www.python.org/dev/peps/pep-0249/)). *pydolphindb* contains a Python DolphinDB client library and supports connecting to DolphinDB using [SQLAlchemy](https://www.sqlalchemy.org/). 
+
+## 1. Installing pydolphindb
+
+### 1.1 Prerequisites
+
+Make sure you use:
+
+- Python 3.7 or higher
+- DolphinDB 1.30.21 or higher can also 2.00.9 or higher
+
+Install the following libraries:
+
+- dolphindb 1.30.21.1 or higher
+- sqlalchemy 1.4 or higher while lower than 2.0 
+
+### 1.2 Installation 
+
+Execute the following `pip` command:
+
+```
+pip install pydolphindb
+```
+
+## 2. Functions
+
+### 2.1 Function Reference
+
+| **Function**                                         | **Parameters**                                               | **Description**                                              |
+| :--------------------------------------------------- | :----------------------------------------------------------- | :----------------------------------------------------------- |
+| `pydolphindb.connect(host, port username, password)` | host (*string*) - hostname of the server to connect to.port (*integer*) *-* port number of the server to connect to.username (*string*) - username for login.password (*string*) - password for login. | Connect to database.                                         |
+| `connection.cursor()`                                | -                                                            | Create a cursor object.                                      |
+| `cursor.execute(script,Parameters = None)`           | script (*string*) - script to execute.parameters (*tuple, list or dictionary*) - Optional. Parameters used with script. | Execute script.If *parameters* is a list or tuple, use `%s` as a placeholder in the script. If *parameters* is a dict, use `%(name)s` as a placeholder in the script. |
+| `cursor.executemany(script,seq_of_parameters)`       | script (*string*) - script to execute.seq_of_parameters (*list* or *tuple*) - a sequence (list or tuple) of lists or tuples used with script. | Execute the script against all parameter sequences specified in `seq_of_parameters`. Use this function for a batch insert operation. |
+| `cursor.fetchone()`                                  | -                                                            | Fetch the next record.                                       |
+| `cursor.fetchmany(size)`                             | size (*integer*) - number of records to fetch.               | Fetch multiple (as specified by *size*) records.             |
+| `cursor.fetchall()`                                  | -                                                            | Fetch all records.                                           |
+
+Note: *pydolphindb* does not support functions to *commit* or *rollback* a transaction.
+
+### 2.2 Sample Code
+
+In this example, we import *pydolphindb* with the `import` command, then connect to DolphinDB with the `connect` function. Functions `execute` and `executemany` are called to create and write to a database, respectively, through the specified DolphinDB script. Functions `fetchone`, `fetchmany`, and `fetchall` are called to fetch data from the database. The connection is closed with the `close` function.
+
+```
+import pydolphindb
+ 
+# connect to database server
+db = pydolphindb.connect(host='localhost',
+                         port='8848',
+                         username='testuser',
+                         password='test123')
+ 
+# create a cursor object
+cursor = db.cursor()
+ 
+# DolphinDB script for creating a database
+script = """
+        dbPath = "dfs://valuedb"
+        if(existsDatabase(dbPath))
+            dropDatabase(dbPath)
+        t = table(100:100,`id`time`vol,[SYMBOL,DATE, INT])
+        db=database(dbPath,VALUE, `APPL`IBM`AMZN)
+        pt = db.createPartitionedTable(t, `pt, `id)
+"""
+
+# execute DolphinDB script with execute()
+cursor.execute(script)
+ 
+# execute DolphinDB script with executemany()
+cursor.executemany('insert into t values(%d, `%s, %.2f)',[(2,'b',3.5239),(3,'c',-0.93154)])
+
+# get the next record with fetchone()
+data = cursor.fetchone()
+
+# the result is None
+print ("Result:" + data)
+
+# get the next two records with fetchmany()
+data = cursor.fetchmany(size = 2)
+
+# get all records with fetchall()
+data = cursor.fetchall()
+
+# close connection
+db.close()
+```
+
+## 3. Connecting to DolphinDB Using SQLAlchemy
+
+[SQLAlchemy](https://www.sqlalchemy.org/) is a Python SQL toolkit and Object Relational Mapper which is designed for efficient database access. *pydolphindb* is a Python [DB API 2.0 (PEP 249)](https://peps.python.org/pep-0249/) client for DolphinDB. The DolphinDB SQLAlchemy dialect is supported so you can connect to the DolphinDB databases through a SQLAlchemy engine.
+
+The following script shows how to connect to and interact with DolphinDB through SQLAlchemy in Python:
+
+```
+from sqlalchemy import create_engine
+
+# create an engine for connection
+engine = create_engine("dolphindb://testuser:test123@localhost:8848")
+
+# DolphinDB script for a database query
+script = """
+    pt = loadTable("dfs://valuedb", "pt")
+    select * from pt
+"""
+
+# run script with execute()
+result = engine.execute(script)
+
+# print all results
+print(result.all())
+```
+
+Note:
+
+- The DolphinDB SQLAlchemy currently does not support ORM (object-relational mapping).
+- When creating engine, pass the DolphinDB database URL to `create_engine` as a string in the following pattern: `dolphindb://{user}:{password}@{host}:{port}`
+
+## Related Links
+
+- [DB API 2.0 (PEP 249)](https://peps.python.org/pep-0249/)
+- [DolphinDB Manual](https://dolphindb.com/help200/index.html)
+- [DolphinDB Python API](https://github.com/dolphindb/api_python3)
```

## Comparing `pydolphindb-1.0.0.dist-info/RECORD` & `pydolphindb-1.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-pydolphindb/__init__.py,sha256=Q2JZ4Bw73pp2kDuJDTho4hcfnrPWlz6f-NvBUqjaW1Y,446
-pydolphindb/connection.py,sha256=Ashs_QSroBIHrasyIbjbYqltVW_8YndFHYVYJaJPgKE,3395
-pydolphindb/cursor.py,sha256=A8YK51NZaIHYrb9yT4apGR-wkv-cwJDAmlIUKSx2Rls,7402
-pydolphindb/exceptions.py,sha256=yw2L2guIyvSjvU6IAj2Ty74xWSr4TyERPDeZ2UJ9Mtw,1024
-pydolphindb/sqlalchemy/__init__.py,sha256=Xs8rzq17yloEUtDJD3NF-F73XLfNkgcl0_f1dO3w-OA,74
-pydolphindb/sqlalchemy/compiler.py,sha256=66zzlnFd7H_7XUJYG_pmJ6iN8i5Ah3uwmHvCyvdTQUE,29586
-pydolphindb/sqlalchemy/dialect.py,sha256=d2jLzduQlPwve41ckkecIUJqWprxaIEXm4Do-1epToA,7047
-pydolphindb/sqlalchemy/sa_version.py,sha256=8a6RVQVmYLraEFygftSHcls3nCa6_bnfsZeOLG9Hpg4,163
-pydolphindb/sqlalchemy/types.py,sha256=58D1_o8L_RAb397fraBgfRQFe6BxLXxhWin-WSEbIsc,326
-pydolphindb-1.0.0.dist-info/METADATA,sha256=fs-gp3fWfkTHnGKRBTja1YZPDBSJaKf0SVjZjfUgyPY,7260
-pydolphindb-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pydolphindb-1.0.0.dist-info/entry_points.txt,sha256=n8ZNLQGX87qUL276Av6HJYkXHyk1VfE1yQWjjcMVZ8c,64
-pydolphindb-1.0.0.dist-info/top_level.txt,sha256=Asovb3GamqmEnpvO9aoMIlLskjJFxtzgmByOETfMx-s,12
-pydolphindb-1.0.0.dist-info/RECORD,,
+pydolphindb/__init__.py,sha256=ddCNBgHpRtUCBI9PjBTTItZxXszBhEL0T8SvbZtXRqM,462
+pydolphindb/connection.py,sha256=7Lov-rH5yuS-UzkWGHuWybzm8PaQ6KQW-Fh9Xr1vGSM,3495
+pydolphindb/cursor.py,sha256=yXQ7H64is3D1Qw9vRTxAbs5Wd3P0gEYosvkCOD99CZw,7650
+pydolphindb/exceptions.py,sha256=jBHKzqwHu7fPgFJUU4Fu2PF2YGZH96NdGwquOFYBF0Y,1082
+pydolphindb/sqlalchemy/__init__.py,sha256=POHG351v6fgTjoSd6pMbpO5xKBiNslkAtiniPMzrtGw,78
+pydolphindb/sqlalchemy/compiler.py,sha256=s6mfIj6W_j7TQX9JkOKKTClHa9fODWI2w80JEjU624Q,30416
+pydolphindb/sqlalchemy/dialect.py,sha256=bunnWcUBy98FWrGApoLOBhNJTHOLReosGUtdBVVWkc8,7268
+pydolphindb/sqlalchemy/sa_version.py,sha256=Fh-xwpkmjAVI2H2XLeYPeXUd_WoC4ZeEmC71VvziX6g,170
+pydolphindb/sqlalchemy/types.py,sha256=jJVOxPsgEyqxb6MYOJ-PFPemRQC61laUdI-ljaVEas8,336
+pydolphindb-1.0.1.dist-info/LICENSE,sha256=3G-4_VJXNLVIIF3fWcAOpS4EBGoZm2Y78XVyaHTnD68,11596
+pydolphindb-1.0.1.dist-info/METADATA,sha256=7BF1UraOXzaM_OkzZ3CxG9nZRWsZVgIcJiK6QYv12ic,7429
+pydolphindb-1.0.1.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+pydolphindb-1.0.1.dist-info/entry_points.txt,sha256=zuX8ICiZyq9a47iVhJSgF2nJhThuOPRqcwFrfAUk1ac,63
+pydolphindb-1.0.1.dist-info/top_level.txt,sha256=Asovb3GamqmEnpvO9aoMIlLskjJFxtzgmByOETfMx-s,12
+pydolphindb-1.0.1.dist-info/RECORD,,
```

