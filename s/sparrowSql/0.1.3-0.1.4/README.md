# Comparing `tmp/sparrowSql-0.1.3.tar.gz` & `tmp/sparrowSql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrowSql-0.1.3.tar", last modified: Tue Apr 16 06:46:04 2024, max compression
+gzip compressed data, was "sparrowSql-0.1.4.tar", last modified: Wed May 22 01:10:14 2024, max compression
```

## Comparing `sparrowSql-0.1.3.tar` & `sparrowSql-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 06:46:04.960078 sparrowSql-0.1.3/
--rw-rw-rw-   0        0        0      231 2024-04-16 06:46:04.958578 sparrowSql-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-16 06:46:04.960577 sparrowSql-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      309 2024-04-16 06:45:59.000000 sparrowSql-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:46:04.946635 sparrowSql-0.1.3/sparrowSql/
--rw-rw-rw-   0        0        0      156 2024-04-15 07:10:45.000000 sparrowSql-0.1.3/sparrowSql/__init__.py
--rw-rw-rw-   0        0        0    20750 2024-04-16 06:40:48.000000 sparrowSql-0.1.3/sparrowSql/mariaDB.py
--rw-rw-rw-   0        0        0    20892 2024-04-16 06:43:06.000000 sparrowSql-0.1.3/sparrowSql/mysql.py
--rw-rw-rw-   0        0        0    21513 2024-04-16 06:45:28.000000 sparrowSql-0.1.3/sparrowSql/postgresql.py
--rw-rw-rw-   0        0        0      745 2024-04-12 06:04:46.000000 sparrowSql-0.1.3/sparrowSql/sparrow.py
--rw-rw-rw-   0        0        0    19319 2024-04-16 06:44:57.000000 sparrowSql-0.1.3/sparrowSql/sqLite.py
-drwxrwxrwx   0        0        0        0 2024-04-16 06:46:04.956579 sparrowSql-0.1.3/sparrowSql.egg-info/
--rw-rw-rw-   0        0        0      231 2024-04-16 06:46:04.000000 sparrowSql-0.1.3/sparrowSql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-16 06:46:04.000000 sparrowSql-0.1.3/sparrowSql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 06:46:04.000000 sparrowSql-0.1.3/sparrowSql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-16 06:46:04.000000 sparrowSql-0.1.3/sparrowSql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-16 06:46:04.000000 sparrowSql-0.1.3/sparrowSql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 01:10:14.065719 sparrowSql-0.1.4/
+-rw-rw-rw-   0        0        0      231 2024-05-22 01:10:14.064718 sparrowSql-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:10:14.066718 sparrowSql-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      309 2024-05-22 01:10:00.000000 sparrowSql-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:10:14.055719 sparrowSql-0.1.4/sparrowSql/
+-rw-rw-rw-   0        0        0      202 2024-04-16 07:14:23.000000 sparrowSql-0.1.4/sparrowSql/__init__.py
+-rw-rw-rw-   0        0        0    20750 2024-04-16 06:40:48.000000 sparrowSql-0.1.4/sparrowSql/mariaDB.py
+-rw-rw-rw-   0        0        0    21068 2024-05-22 01:09:37.000000 sparrowSql-0.1.4/sparrowSql/mysql.py
+-rw-rw-rw-   0        0        0    21513 2024-04-16 06:45:28.000000 sparrowSql-0.1.4/sparrowSql/postgresql.py
+-rw-rw-rw-   0        0        0     6068 2024-05-07 10:05:13.000000 sparrowSql-0.1.4/sparrowSql/sparrow.py
+-rw-rw-rw-   0        0        0    19319 2024-04-16 06:44:57.000000 sparrowSql-0.1.4/sparrowSql/sqLite.py
+-rw-rw-rw-   0        0        0    14746 2024-04-17 06:25:08.000000 sparrowSql-0.1.4/sparrowSql/sqlserver.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:10:14.063715 sparrowSql-0.1.4/sparrowSql.egg-info/
+-rw-rw-rw-   0        0        0      231 2024-05-22 01:10:13.000000 sparrowSql-0.1.4/sparrowSql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-05-22 01:10:13.000000 sparrowSql-0.1.4/sparrowSql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:10:13.000000 sparrowSql-0.1.4/sparrowSql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-05-22 01:10:13.000000 sparrowSql-0.1.4/sparrowSql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 01:10:13.000000 sparrowSql-0.1.4/sparrowSql.egg-info/top_level.txt
```

### Comparing `sparrowSql-0.1.3/sparrowSql/mariaDB.py` & `sparrowSql-0.1.4/sparrowSql/mariaDB.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1.3/sparrowSql/mysql.py` & `sparrowSql-0.1.4/sparrowSql/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,16 +201,15 @@
                 sql += f" order by {sort_column} desc"
         sql += ";"
         self._cursor_.execute(sql, params)
         row = self._cursor_.fetchall()
         return row
 
     def select_page(self, table: str, conditions: dict = None, columns: list = None, page_size: int = 20,
-                    page_index: int = 0,
-                    sort_column: str = None, sort_method: str = ""):
+                    page_index: int = 0, sort_column: str = None, sort_method: str = "asc"):
         """
         分页查询
         :param table: 表名
         :param conditions: 查询参数。默认为全部
         :param columns: 字段名，默认为全部
         :param page_size: 分页大小，默认20
         :param page_index: 当前页码，默认为0
@@ -554,15 +553,15 @@
         self._cursor_.execute(sql)
 
     def start_transaction(self):
         """
         开始事务
         :return:
         """
-        sql = "BEGIN TRANSACTION;"
+        sql = "BEGIN WORK;"
         self._cursor_.execute(sql)
         print("事务开启...")
 
     def rollback_transaction(self):
         """
         回滚事务
         :return:
@@ -576,12 +575,24 @@
         提交事务
         :return:
         """
         sql = "COMMIT;"
         self._cursor_.execute(sql)
         print("事务提交...")
 
+    def get_cursor(self):
+        """
+        返回游标
+        :return:
+        """
+        return self._cursor_
+
+    def get_connection(self):
+        """
+        返回连接
+        :return:
+        """
+        return self._connect_
 
 
 if __name__ == '__main__':
     run = MySQL("192.168.233.131", 3306, "root", "123456")
-    run.create_index("test", "name", "name_index")
```

### Comparing `sparrowSql-0.1.3/sparrowSql/postgresql.py` & `sparrowSql-0.1.4/sparrowSql/postgresql.py`

 * *Files identical despite different names*

### Comparing `sparrowSql-0.1.3/sparrowSql/sqLite.py` & `sparrowSql-0.1.4/sparrowSql/sqLite.py`

 * *Files identical despite different names*

