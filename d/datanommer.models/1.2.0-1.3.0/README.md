# Comparing `tmp/datanommer_models-1.2.0.tar.gz` & `tmp/datanommer_models-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanommer_models-1.2.0.tar", max compression
+gzip compressed data, was "datanommer_models-1.3.0.tar", max compression
```

## Comparing `datanommer_models-1.2.0.tar` & `datanommer_models-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_models-1.2.0/LICENSE
--rw-r--r--   0        0        0     1614 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/NEWS.rst
--rw-r--r--   0        0        0      302 2022-01-17 12:04:04.000000 datanommer_models-1.2.0/README.rst
--rw-r--r--   0        0        0      916 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/alembic.ini
--rw-r--r--   0        0        0    11002 2024-04-11 07:27:40.911012 datanommer_models-1.2.0/coverage.xml
--rw-r--r--   0        0        0    16874 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/datanommer/models/__init__.py
--rw-r--r--   0        0        0     2793 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/env.py
--rw-r--r--   0        0        0      412 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/script.py.mako
--rw-r--r--   0        0        0      249 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/versions/5db25abc63be_init.py
--rw-r--r--   0        0        0      843 2022-07-06 08:10:03.000000 datanommer_models-1.2.0/datanommer/models/alembic/versions/951c40020acc_unique.py
--rw-r--r--   0        0        0     1453 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/datanommer/models/testing/__init__.py
--rw-r--r--   0        0        0     4279 2024-04-15 09:57:21.428639 datanommer_models-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_models-1.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1882 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tests/test_jsonencodeddict.py
--rw-r--r--   0        0        0    20108 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tests/test_model.py
--rw-r--r--   0        0        0      543 2024-04-15 09:57:21.429639 datanommer_models-1.2.0/tox.ini
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 datanommer_models-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_models-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2412 2024-05-22 17:03:32.326278 datanommer_models-1.3.0/NEWS.rst
+-rw-r--r--   0        0        0      302 2022-01-17 12:04:04.000000 datanommer_models-1.3.0/README.rst
+-rw-r--r--   0        0        0      916 2022-07-06 08:10:03.000000 datanommer_models-1.3.0/alembic.ini
+-rw-r--r--   0        0        0    11747 2024-05-22 12:55:32.460810 datanommer_models-1.3.0/coverage.xml
+-rw-r--r--   0        0        0    18628 2024-05-22 12:50:38.985339 datanommer_models-1.3.0/datanommer/models/__init__.py
+-rw-r--r--   0        0        0     2793 2022-07-06 08:10:03.000000 datanommer_models-1.3.0/datanommer/models/alembic/env.py
+-rw-r--r--   0        0        0      412 2022-07-06 08:10:03.000000 datanommer_models-1.3.0/datanommer/models/alembic/script.py.mako
+-rw-r--r--   0        0        0      249 2022-07-06 08:10:03.000000 datanommer_models-1.3.0/datanommer/models/alembic/versions/5db25abc63be_init.py
+-rw-r--r--   0        0        0      843 2022-07-06 08:10:03.000000 datanommer_models-1.3.0/datanommer/models/alembic/versions/951c40020acc_unique.py
+-rw-r--r--   0        0        0     1693 2024-05-22 12:53:27.465722 datanommer_models-1.3.0/datanommer/models/testing/__init__.py
+-rw-r--r--   0        0        0     4365 2024-05-22 16:48:36.950003 datanommer_models-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_models-1.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1884 2024-05-06 16:09:12.240921 datanommer_models-1.3.0/tests/test_jsonencodeddict.py
+-rw-r--r--   0        0        0    21042 2024-05-20 09:41:48.376185 datanommer_models-1.3.0/tests/test_model.py
+-rw-r--r--   0        0        0      543 2024-04-15 09:57:21.429639 datanommer_models-1.3.0/tox.ini
+-rw-r--r--   0        0        0     2561 1970-01-01 00:00:00.000000 datanommer_models-1.3.0/PKG-INFO
```

### Comparing `datanommer_models-1.2.0/LICENSE` & `datanommer_models-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.2.0/alembic.ini` & `datanommer_models-1.3.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.2.0/coverage.xml` & `datanommer_models-1.3.0/coverage.xml`

 * *Files 2% similar despite different names*

#### Comparing `datanommer_models-1.2.0/coverage.xml` & `datanommer_models-1.3.0/coverage.xml`

```diff
@@ -1,18 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
-<coverage version="7.4.4" timestamp="1712820460896" lines-valid="220" lines-covered="217" line-rate="0.9864" branches-valid="100" branches-covered="100" branch-rate="1" complexity="0">
-  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.4.4 -->
+<coverage version="7.5.1" timestamp="1716382532447" lines-valid="236" lines-covered="236" line-rate="1" branches-valid="108" branches-covered="108" branch-rate="1" complexity="0">
+  <!-- Generated by coverage.py: https://coverage.readthedocs.io/en/7.5.1 -->
   <!-- Based on https://raw.githubusercontent.com/cobertura/web/master/htdocs/xml/coverage-04.dtd -->
   <sources>
     <source>/home/abompard/Fedora/apps/datanommer/datanommer.models/datanommer</source>
   </sources>
   <packages>
-    <package name="models" line-rate="0.9864" branch-rate="1" complexity="0">
+    <package name="models" line-rate="1" branch-rate="1" complexity="0">
       <classes>
-        <class name="__init__.py" filename="models/__init__.py" complexity="0" line-rate="0.9864" branch-rate="1">
+        <class name="__init__.py" filename="models/__init__.py" complexity="0" line-rate="1" branch-rate="1">
           <methods/>
           <lines>
             <line number="16" hits="1"/>
             <line number="17" hits="1"/>
             <line number="18" hits="1"/>
             <line number="19" hits="1"/>
             <line number="20" hits="1"/>
@@ -57,17 +57,17 @@
             <line number="127" hits="1"/>
             <line number="128" hits="1"/>
             <line number="129" hits="1"/>
             <line number="130" hits="1"/>
             <line number="132" hits="1"/>
             <line number="135" hits="1"/>
             <line number="136" hits="1"/>
-            <line number="137" hits="0"/>
-            <line number="138" hits="0"/>
-            <line number="143" hits="0"/>
+            <line number="137" hits="1"/>
+            <line number="138" hits="1"/>
+            <line number="143" hits="1"/>
             <line number="144" hits="1"/>
             <line number="145" hits="1"/>
             <line number="146" hits="1"/>
             <line number="147" hits="1"/>
             <line number="152" hits="1"/>
             <line number="154" hits="1"/>
             <line number="165" hits="1"/>
@@ -156,84 +156,100 @@
             <line number="342" hits="1"/>
             <line number="343" hits="1"/>
             <line number="352" hits="1"/>
             <line number="353" hits="1"/>
             <line number="359" hits="1"/>
             <line number="361" hits="1"/>
             <line number="362" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="414" hits="1"/>
+            <line number="405" hits="1"/>
+            <line number="406" hits="1"/>
+            <line number="407" hits="1"/>
+            <line number="408" hits="1"/>
+            <line number="409" hits="1"/>
+            <line number="410" hits="1"/>
+            <line number="411" hits="1"/>
+            <line number="412" hits="1"/>
+            <line number="413" hits="1"/>
             <line number="415" hits="1"/>
             <line number="416" hits="1"/>
-            <line number="417" hits="1"/>
-            <line number="418" hits="1"/>
-            <line number="419" hits="1"/>
-            <line number="420" hits="1"/>
+            <line number="420" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="421" hits="1"/>
-            <line number="422" hits="1"/>
-            <line number="424" hits="1"/>
-            <line number="425" hits="1"/>
-            <line number="429" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="430" hits="1"/>
-            <line number="434" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="435" hits="1"/>
-            <line number="437" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="438" hits="1"/>
+            <line number="425" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="426" hits="1"/>
+            <line number="428" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="429" hits="1"/>
+            <line number="432" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="433" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="435" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="436" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="438" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="439" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="441" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="442" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="444" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="445" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="447" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="448" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="450" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="449" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="451" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="453" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="454" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="452" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="456" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="457" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="458" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="459" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="460" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="461" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="462" hits="1"/>
+            <line number="464" hits="1"/>
             <line number="465" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="466" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="468" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="469" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="472" hits="1"/>
-            <line number="473" hits="1"/>
-            <line number="475" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="476" hits="1"/>
-            <line number="478" hits="1"/>
-            <line number="479" hits="1"/>
-            <line number="481" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="482" hits="1"/>
-            <line number="485" hits="1"/>
-            <line number="486" hits="1"/>
-            <line number="489" hits="1"/>
-            <line number="490" hits="1"/>
-            <line number="491" hits="1"/>
-            <line number="493" hits="1"/>
-            <line number="494" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="500" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="503" hits="1"/>
-            <line number="504" hits="1"/>
-            <line number="505" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="506" hits="1"/>
-            <line number="507" hits="1"/>
-            <line number="508" hits="1"/>
-            <line number="509" hits="1"/>
-            <line number="510" hits="1"/>
-            <line number="512" hits="1"/>
-            <line number="513" hits="1" branch="true" condition-coverage="100% (2/2)"/>
-            <line number="514" hits="1"/>
+            <line number="511" hits="1"/>
+            <line number="513" hits="1"/>
+            <line number="515" hits="1"/>
+            <line number="516" hits="1"/>
             <line number="517" hits="1"/>
-            <line number="518" hits="1"/>
-            <line number="519" hits="1"/>
+            <line number="519" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="520" hits="1"/>
             <line number="522" hits="1"/>
             <line number="523" hits="1"/>
             <line number="524" hits="1"/>
-            <line number="527" hits="1"/>
+            <line number="526" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="527" hits="1" branch="true" condition-coverage="100% (2/2)"/>
             <line number="528" hits="1"/>
+            <line number="529" hits="1"/>
+            <line number="532" hits="1"/>
+            <line number="533" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="534" hits="1"/>
             <line number="535" hits="1"/>
+            <line number="537" hits="1"/>
+            <line number="538" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="540" hits="1"/>
+            <line number="541" hits="1"/>
+            <line number="542" hits="1"/>
+            <line number="545" hits="1"/>
+            <line number="546" hits="1"/>
+            <line number="547" hits="1"/>
+            <line number="549" hits="1"/>
+            <line number="550" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="556" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="559" hits="1"/>
+            <line number="560" hits="1"/>
+            <line number="561" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="562" hits="1"/>
+            <line number="563" hits="1"/>
+            <line number="564" hits="1"/>
+            <line number="565" hits="1"/>
+            <line number="566" hits="1"/>
+            <line number="568" hits="1"/>
+            <line number="569" hits="1" branch="true" condition-coverage="100% (2/2)"/>
+            <line number="570" hits="1"/>
+            <line number="573" hits="1"/>
+            <line number="574" hits="1"/>
+            <line number="575" hits="1"/>
+            <line number="578" hits="1"/>
+            <line number="579" hits="1"/>
+            <line number="580" hits="1"/>
+            <line number="583" hits="1"/>
+            <line number="584" hits="1"/>
+            <line number="591" hits="1"/>
           </lines>
         </class>
       </classes>
     </package>
   </packages>
 </coverage>
```

### Comparing `datanommer_models-1.2.0/datanommer/models/__init__.py` & `datanommer_models-1.3.0/datanommer/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     session.commit()
 
 
 # https://docs.sqlalchemy.org/en/14/core/custom_types.html#marshal-json-strings
 
 
-class JSONEncodedDict(TypeDecorator):
+class _JSONEncodedDict(TypeDecorator):
     """Represents an immutable structure as a json-encoded string."""
 
     impl = UnicodeText
 
     cache_ok = True
 
     def process_bind_param(self, value, dialect):
@@ -223,15 +223,15 @@
     certificate = Column(UnicodeText)
     signature = Column(UnicodeText)
     category = Column(Unicode, nullable=False, index=True)
     username = Column(Unicode)
     crypto = Column(UnicodeText)
     source_name = Column(Unicode, default="datanommer")
     source_version = Column(Unicode, default=lambda context: __version__)
-    msg = Column(JSONEncodedDict, nullable=False)
+    msg = Column(_JSONEncodedDict, nullable=False)
     headers = Column(postgresql.JSONB(none_as_null=True))
     users = relationship(
         "User",
         secondary=users_assoc_table,
         backref="messages",
         primaryjoin=lambda: and_(
             Message.id == users_assoc_table.c.msg_id,
@@ -355,32 +355,28 @@
             "in the next major version",
             DeprecationWarning,
             stacklevel=2,
         )
         return self.as_dict(request)
 
     @classmethod
-    def grep(
+    def make_query(
         cls,
         start=None,
         end=None,
-        page=1,
-        rows_per_page=100,
-        order="asc",
         msg_id=None,
         users=None,
         not_users=None,
         packages=None,
         not_packages=None,
         categories=None,
         not_categories=None,
         topics=None,
         not_topics=None,
         contains=None,
-        defer=False,
     ):
         """Flexible query interface for messages.
 
         Arguments are filters.  start and end should be :mod:`datetime` objs.
 
         Other filters should be lists of strings.  They are applied in a
         conjunctive-normal-form (CNF) kind of way
@@ -400,19 +396,14 @@
             users = ['ralph']
             not_categories = ['bodhi', 'wiki']
 
         should return messages where
 
             (user == 'ralph') AND
             NOT (category == 'bodhi' OR category == 'wiki')
-
-        ----
-
-        If the `defer` argument evaluates to True, the query won't actually
-        be executed, but a SQLAlchemy query object returned instead.
         """
 
         users = users or []
         not_users = not_users or []
         packages = packages or []
         not_packs = not_packages or []
         categories = categories or []
@@ -464,31 +455,96 @@
 
         if not_cats:
             query = query.where(not_(or_(*(Message.category == category for category in not_cats))))
 
         if not_topics:
             query = query.where(not_(or_(*(Message.topic == topic for topic in not_topics))))
 
+        return query
+
+    @classmethod
+    def grep(
+        cls,
+        *,
+        page=1,
+        rows_per_page=100,
+        order="asc",
+        defer=False,
+        **kwargs,
+    ):
+        """Flexible query interface for messages.
+
+        Arguments are filters.  start and end should be :mod:`datetime` objs.
+
+        Other filters should be lists of strings.  They are applied in a
+        conjunctive-normal-form (CNF) kind of way
+
+        for example, the following::
+
+          users = ['ralph', 'lmacken']
+          categories = ['bodhi', 'wiki']
+
+        should return messages where
+
+          (user=='ralph' OR user=='lmacken') AND
+          (category=='bodhi' OR category=='wiki')
+
+        Furthermore, you can use a negative version of each argument.
+
+            users = ['ralph']
+            not_categories = ['bodhi', 'wiki']
+
+        should return messages where
+
+            (user == 'ralph') AND
+            NOT (category == 'bodhi' OR category == 'wiki')
+
+        ----
+
+        The ``jsons`` argument is a list of jsonpath filters, please refer to
+        `PostgreSQL's documentation
+        <https://www.postgresql.org/docs/current/functions-json.html#FUNCTIONS-SQLJSON-PATH>`_
+        on the matter to learn how to build the jsonpath expression.
+
+        The ``jsons_and`` argument is similar to the ``jsons`` argument, but all
+        the values must match for a message to be returned.
+        """
+        query = cls.make_query(**kwargs)
         # Finally, tag on our pagination arguments
-        total = session.scalar(query.with_only_columns(func.count(Message.id)))
+        Message = cls
+
+        query_total = query.with_only_columns(func.count(Message.id))
+        total = None
         query = query.order_by(getattr(Message.timestamp, order)())
 
         if not rows_per_page:
             pages = 1
         else:
+            total = session.scalar(query_total)
             pages = int(math.ceil(total / float(rows_per_page)))
             query = query.offset(rows_per_page * (page - 1)).limit(rows_per_page)
 
         if defer:
-            return total, page, query
+            if total is None:
+                total = session.scalar(query_total)
+            return total, pages, query
         else:
             # Execute!
             messages = session.scalars(query).all()
+            if pages == 1:
+                total = len(messages)
             return total, pages, messages
 
+    @classmethod
+    def get_first(cls, *, order="asc", **kwargs):
+        """Get the first message matching the regular grep filters."""
+        query = cls.make_query(**kwargs)
+        query = query.order_by(getattr(Message.timestamp, order)())
+        return session.scalars(query).first()
+
 
 class NamedSingleton:
     id = Column(Integer, primary_key=True, autoincrement=True)
     name = Column(UnicodeText, index=True, unique=True)
 
     @classmethod
     def get_or_create(cls, name):
```

### Comparing `datanommer_models-1.2.0/datanommer/models/alembic/env.py` & `datanommer_models-1.3.0/datanommer/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.2.0/datanommer/models/alembic/versions/951c40020acc_unique.py` & `datanommer_models-1.3.0/datanommer/models/alembic/versions/951c40020acc_unique.py`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.2.0/datanommer/models/testing/__init__.py` & `datanommer_models-1.3.0/datanommer/models/testing/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,31 +17,39 @@
     return (
         f"postgresql+psycopg2://{postgresql_proc.user}:@"
         f"{postgresql_proc.host}:{postgresql_proc.port}"
         f"/{postgresql_proc.dbname}"
     )
 
 
-@pytest.fixture()
-def datanommer_db(postgresql_proc, datanommer_db_url):
+@pytest.fixture(scope="session")
+def datanommer_db_engine(postgresql_proc, datanommer_db_url):
     with DatabaseJanitor(
         user=postgresql_proc.user,
         host=postgresql_proc.host,
         port=postgresql_proc.port,
         dbname=postgresql_proc.dbname,
         # Don't use a template database
         # template_dbname=postgresql_proc.template_dbname,
         version=postgresql_proc.version,
     ):
-        engine = sa.create_engine(datanommer_db_url, future=True, poolclass=sa.pool.NullPool)
+        engine = sa.create_engine(datanommer_db_url, future=True)
         # Renew the global object, dm.init checks a custom attribute
         dm.session = scoped_session(dm.maker)
         dm.init(engine=engine, create=True)
         yield engine
-        dm.session.close()
+        engine.dispose()
+
+
+@pytest.fixture()
+def datanommer_db(datanommer_db_url, datanommer_db_engine):
+    for table in reversed(dm.DeclarativeBase.metadata.sorted_tables):
+        dm.session.execute(table.delete())
+    dm.session.commit()
+    yield datanommer_db_engine
 
 
 @pytest.fixture()
 def datanommer_models(datanommer_db):
     dm.User.clear_cache()
     dm.Package.clear_cache()
     yield dm.session
```

### Comparing `datanommer_models-1.2.0/pyproject.toml` & `datanommer_models-1.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datanommer.models"
-version = "1.2.0"
+version = "1.3.0"
 description = "SQLAlchemy models for datanommer"
 authors = [
   "Fedora Infrastructure <admin@fedoraproject.org>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.rst"
 repository = "https://github.com/fedora-infra/datanommer"
@@ -44,14 +44,15 @@
 fedora-messaging-git-hook-messages = {version = "*", optional = true}
 fedora-messaging-the-new-hotness-schema = {version = "*", optional = true}
 fedora-planet-messages = {version = "*", optional = true}
 fmn-messages = {version = "*", optional = true}
 kerneltest-messages = {version = "^1.0.0", optional = true}
 koji-fedoramessaging-messages = {version = "^1.2.2", optional = true}
 koschei-messages = {version = "*", optional = true}
+maubot-fedora-messages = {version = "*", optional = true}
 mediawiki-messages = {version = "*", optional = true}
 meetbot-messages = {version = "*", optional = true}
 mdapi-messages = {version = "*", optional = true}
 noggin-messages = {version = "*", optional = true}
 nuancier-messages = {version = "*", optional = true}
 pagure-messages = {version = "*", optional = true}
 tahrir-messages = {version = "*", optional = true}
@@ -82,14 +83,15 @@
   "fedora-messaging-git-hook-messages",
   "fedora-messaging-the-new-hotness-schema",
   "fedora-planet-messages",
   "fmn-messages",
   "kerneltest-messages",
   "koji-fedoramessaging-messages",
   "koschei-messages",
+  "maubot-fedora-messages",
   "mediawiki-messages",
   "meetbot-messages",
   "mdapi-messages",
   "noggin-messages",
   "nuancier-messages",
   "pagure-messages",
   "tahrir-messages",
```

### Comparing `datanommer_models-1.2.0/tests/test_jsonencodeddict.py` & `datanommer_models-1.3.0/tests/test_jsonencodeddict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from sqlalchemy import Column, create_engine, Integer, MetaData, select, Table, text
 
-from datanommer.models import JSONEncodedDict
+from datanommer.models import _JSONEncodedDict
 
 
 @pytest.fixture
 def connection():
     engine = create_engine("sqlite:///:memory:", future=True)
     with engine.connect() as connection:
         yield connection
@@ -14,15 +14,15 @@
 @pytest.fixture
 def table(connection):
     metadata = MetaData()
     table = Table(
         "test_table",
         metadata,
         Column("id", Integer, primary_key=True),
-        Column("data", JSONEncodedDict),
+        Column("data", _JSONEncodedDict),
     )
     metadata.create_all(connection)
     yield table
     metadata.drop_all(connection)
 
 
 def test_jsonencodeddict(connection, table):
```

### Comparing `datanommer_models-1.2.0/tests/test_model.py` & `datanommer_models-1.3.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,23 @@
             }
         }
     )
     msg.topic = f"org.fedoraproject.stg.{msg.topic}"
     return msg
 
 
+@pytest.fixture
+def add_200_messages(datanommer_models):
+    for x in range(0, 200):
+        example_message = generate_message()
+        example_message.id = f"{x}"
+        dm.add(example_message)
+    dm.session.flush()
+
+
 def test_init_uri_and_engine():
     uri = "sqlite:///db.db"
     engine = create_engine(uri, future=True)
 
     with pytest.raises(ValueError, match="uri and engine cannot both be specified"):
         dm.init(uri, engine=engine)
 
@@ -127,17 +136,17 @@
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = None
 
     dm.add(example_message)
 
     dbmsg = dm.session.scalar(select(dm.Message))
     timediff = datetime.datetime.now() - dbmsg.timestamp
-    # 10 seconds between adding the message and checking
+    # 60 seconds between adding the message and checking
     # the timestamp should be more than enough.
-    assert timediff < datetime.timedelta(seconds=10)
+    assert timediff < datetime.timedelta(seconds=60)
 
 
 def test_add_timestamp_with_Z(datanommer_models):
     example_message = generate_message()
     example_message._properties.headers["sent-at"] = "2021-07-27T04:22:42Z"
 
     dm.add(example_message)
@@ -415,61 +424,69 @@
     t, p, r = dm.Message.grep(contains=["doing"])
     assert t == 1
     assert p == 1
     assert len(r) == 1
     assert r[0].msg == example_message.body
 
 
-def test_grep_rows_per_page_none(datanommer_models):
-    for x in range(0, 200):
-        example_message = generate_message()
-        example_message.id = f"{x}"
-        dm.add(example_message)
-
-    dm.session.flush()
-
+def test_grep_rows_per_page(datanommer_models, add_200_messages):
     total, pages, messages = dm.Message.grep()
     assert total == 200
     assert pages == 2
     assert len(messages) == 100
 
-    total, pages, messages = dm.Message.grep(rows_per_page=None)
-    assert total == 200
-    assert pages == 1
-    assert len(messages) == 200
-
-
-def test_grep_rows_per_page_zero(datanommer_models):
-    for x in range(0, 200):
-        example_message = generate_message()
-        example_message.id = f"{x}"
-        dm.add(example_message)
-    dm.session.flush()
-
-    try:
-        total, pages, messages = dm.Message.grep(rows_per_page=0)
-    except ZeroDivisionError as e:
-        pytest.fail(e)
-    assert total == 200
-    assert pages == 1
-    assert len(messages) == 200
+    for rows_per_page in (None, 0):
+        try:
+            total, pages, messages = dm.Message.grep(rows_per_page=rows_per_page)
+        except ZeroDivisionError as e:
+            pytest.fail(e)
+        assert total == 200
+        assert pages == 1
+        assert len(messages) == 200
 
 
 def test_grep_defer(datanommer_models):
     example_message = generate_message()
     dm.add(example_message)
 
     dm.session.flush()
 
     total, pages, query = dm.Message.grep(defer=True)
     assert isinstance(query, Select)
 
     assert dm.session.scalars(query).all() == dm.Message.grep()[2]
 
 
+def test_grep_no_paging_and_defer(datanommer_models, add_200_messages):
+    total, pages, messages = dm.Message.grep(rows_per_page=0, defer=True)
+    assert total == 200
+    assert pages == 1
+
+
+def test_grep_no_total_if_single_page(datanommer_models, add_200_messages, mocker):
+    # Assert we don't query the total of messages if we're getting them all anyway
+    scalar_spy = mocker.spy(dm.session, "scalar")
+    total, pages, messages = dm.Message.grep(rows_per_page=0)
+    assert total == 200
+    scalar_spy.assert_not_called()
+
+
+def test_get_first(datanommer_models):
+    messages = []
+    for x in range(0, 200):
+        example_message = generate_message()
+        example_message.id = f"{x}"
+        dm.add(example_message)
+        messages.append(example_message)
+    dm.session.flush()
+    msg = dm.Message.get_first()
+    assert msg.msg_id == "0"
+    assert msg.msg == messages[0].body
+
+
 def test_add_duplicate(datanommer_models, caplog):
     example_message = generate_message()
     dm.add(example_message)
     dm.add(example_message)
     # if no exception was thrown, then we successfully ignored the
     # duplicate message
     assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
@@ -507,38 +524,46 @@
         pytest.fail(e)
     assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
     dbmsg = dm.session.scalar(select(dm.Message))
     assert len(dbmsg.packages) == 1
     assert dbmsg.packages[0].name == "pkg"
 
 
-def test_add_message_with_error_on_packages(datanommer_models, caplog):
+@pytest.mark.parametrize(
+    "property_name,name_in_msg", [("usernames", "users"), ("packages", "packages")]
+)
+def test_add_message_with_error_on_property(datanommer_models, caplog, property_name, name_in_msg):
     # Define a special message schema and register it
     class CustomMessage(fedora_message.Message):
         @property
         def packages(self):
             raise KeyError
 
         def _filter_headers(self):
             return {}
 
+    def _crash(self):
+        raise KeyError
+
+    setattr(CustomMessage, property_name, property(_crash))
+
     fedora_message._schema_name_to_class["CustomMessage"] = CustomMessage
     fedora_message._class_to_schema_name[CustomMessage] = "CustomMessage"
     example_message = CustomMessage(
         topic="org.fedoraproject.test.a.nice.message",
         body={"encouragement": "You're doing great!"},
         headers=None,
     )
     try:
         dm.add(example_message)
     except KeyError as e:
         pytest.fail(e)
     assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
     assert caplog.records[0].message == (
-        f"Could not get the list of packages from a message on "
+        f"Could not get the list of {name_in_msg} from a message on "
         f"org.fedoraproject.test.a.nice.message with id {example_message.id}"
     )
 
 
 def test_as_fedora_message_dict(datanommer_models):
     example_message = generate_message()
     dm.add(example_message)
```

### Comparing `datanommer_models-1.2.0/tox.ini` & `datanommer_models-1.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `datanommer_models-1.2.0/PKG-INFO` & `datanommer_models-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datanommer.models
-Version: 1.2.0
+Version: 1.3.0
 Summary: SQLAlchemy models for datanommer
 Home-page: https://github.com/fedora-infra/datanommer
 License: GPL-3.0-or-later
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -28,14 +28,15 @@
 Requires-Dist: fedora-messaging-the-new-hotness-schema ; extra == "schemas"
 Requires-Dist: fedora-planet-messages ; extra == "schemas"
 Requires-Dist: fedorainfra-ansible-messages ; extra == "schemas"
 Requires-Dist: fmn-messages ; extra == "schemas"
 Requires-Dist: kerneltest-messages (>=1.0.0,<2.0.0) ; extra == "schemas"
 Requires-Dist: koji-fedoramessaging-messages (>=1.2.2,<2.0.0) ; extra == "schemas"
 Requires-Dist: koschei-messages ; extra == "schemas"
+Requires-Dist: maubot-fedora-messages ; extra == "schemas"
 Requires-Dist: mdapi-messages ; extra == "schemas"
 Requires-Dist: mediawiki-messages ; extra == "schemas"
 Requires-Dist: meetbot-messages ; extra == "schemas"
 Requires-Dist: noggin-messages ; extra == "schemas"
 Requires-Dist: nuancier-messages ; extra == "schemas"
 Requires-Dist: pagure-messages ; extra == "schemas"
 Requires-Dist: psycopg2 (>=2.9.1,<3.0.0)
```

