# Comparing `tmp/edwh_auth_rbac-0.1.1.tar.gz` & `tmp/edwh_auth_rbac-0.2.0.tar.gz`

## Comparing `edwh_auth_rbac-0.1.1.tar` & `edwh_auth_rbac-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,28 @@
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/helpers.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/migrations.py
--rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/model.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/rbac.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/tests/test_rbac.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/.gitignore
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/README.md
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/.gitignore
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/class_index.html
+-rw-r--r--   0        0        0    24699 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/coverage_html_cb_da166b87.js
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/favicon_32_cb_58284776.png
+-rw-r--r--   0        0        0    36695 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/function_index.html
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/keybd_closed_cb_ce680311.png
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/status.json
+-rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/style_cb_8e611ae1.css
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6___init___py.html
+-rw-r--r--   0        0        0     7068 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_helpers_py.html
+-rw-r--r--   0        0        0    15181 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_migrations_py.html
+-rw-r--r--   0        0        0   123833 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_model_py.html
+-rw-r--r--   0        0        0    61606 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_438b44bce6437be6_rbac_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    60186 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/htmlcov/z_a44f0ac069e85531_test_rbac_py.html
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/helpers.py
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/migrations.py
+-rw-r--r--   0        0        0    13060 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/model.py
+-rw-r--r--   0        0        0     7658 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/rbac.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/tests/test_rbac.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/.gitignore
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/README.md
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 edwh_auth_rbac-0.2.0/PKG-INFO
```

### Comparing `edwh_auth_rbac-0.1.1/src/edwh_auth_rbac/model.py` & `edwh_auth_rbac-0.2.0/src/edwh_auth_rbac/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,298 +1,356 @@
 import copy
-import datetime
+import datetime as dt
 import hashlib
 import hmac
+import typing
 import uuid
+from typing import Optional
+from uuid import UUID
 
 import dateutil.parser
-from pydal import Field
-from pydal import SQLCustomType
-from pydal.objects import SQLALL, Query
+from pydal import DAL, Field, SQLCustomType
+from pydal.objects import SQLALL, Query, Table
 
 from .helpers import IS_IN_LIST
 
 
 class DEFAULT:
     pass
 
 
-DEFAULT_STARTS = datetime.datetime(2000, 1, 1)
-DEFAULT_ENDS = datetime.datetime(3000, 1, 1)
+IdentityKey: typing.TypeAlias = str | int | UUID
+ObjectTypes = typing.Literal["user", "group", "item"]
+When: typing.TypeAlias = str | dt.datetime | typing.Type[DEFAULT]
 
+DEFAULT_STARTS = dt.datetime(2000, 1, 1)
+DEFAULT_ENDS = dt.datetime(3000, 1, 1)
 
-def unstr_datetime(s):
-    """json helper... might values arrive as str """
-    return dateutil.parser.parse(s) if isinstance(s, str) else s
+T = typing.TypeVar("T")
+
+
+def unstr_datetime(s: When | T) -> dt.datetime | T:
+    """json helper... might values arrive as str"""
+    return dateutil.parser.parse(s) if isinstance(s, str) else typing.cast(T, s)
 
 
 class Password:
     """
     Encode a password using: Password.encode('secret')
     """
 
     @classmethod
-    def hmac_hash(cls, value, key, salt=None):
+    def hmac_hash(cls, value: str, key: str, salt: Optional[str] = None) -> str:
         digest_alg = hashlib.sha512
         d = hmac.new(str(key).encode(), str(value).encode(), digest_alg)
         if salt:
             d.update(str(salt).encode())
         return d.hexdigest()
 
     @classmethod
-    def validate(cls, password, candidate):
-        salt, hashed = candidate.split(':', 1)
-        return cls.hmac_hash(value=password, key='secret_start', salt=salt) == hashed
+    def validate(cls, password: str, candidate: str) -> bool:
+        salt, hashed = candidate.split(":", 1)
+        return cls.hmac_hash(value=password, key="secret_start", salt=salt) == hashed
 
     @classmethod
-    def encode(cls, password):
+    def encode(cls, password: str) -> str:
         salt = uuid.uuid4().hex
-        return salt + ':' + cls.hmac_hash(value=password, key='secret_start', salt=salt)
+        return salt + ":" + cls.hmac_hash(value=password, key="secret_start", salt=salt)
 
 
-def is_uuid(s):
+def is_uuid(s) -> bool:
     try:
-        uuid.UUID(s)
+        UUID(s)
         return True
     except Exception:
         return False
 
 
-def key_lookup_query(db, identity_key: str | int | uuid.UUID, object_type=None) -> Query:
-    if '@' in str(identity_key):
-        query = db.identity.email == identity_key.lower()
+def key_lookup_query(db: DAL, identity_key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> Query:
+    if "@" in str(identity_key):
+        query = db.identity.email == str(identity_key).lower()
     elif isinstance(identity_key, int):
         query = db.identity.id == identity_key
     elif is_uuid(identity_key):
-        query = db.identity.object_id == identity_key.lower()
+        query = db.identity.object_id == str(identity_key).lower()
     else:
         query = db.identity.firstname == identity_key
 
     if object_type:
         query &= db.identity.object_type == object_type
 
     return query
 
 
-def key_lookup(db, identity_key, object_type=None) -> str | None:
+def key_lookup(db: DAL, identity_key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> str:
     query = key_lookup_query(db, identity_key, object_type)
 
     rowset = db(query).select(db.identity.object_id)
 
-    if not rowset:
-        return None
-    elif len(rowset) > 1:
-        raise ValueError('Keep lookup for {} returned {} results.'.format(identity_key, len(rowset)))
+    if len(rowset) != 1:
+        raise ValueError("Keep lookup for {} returned {} results.".format(identity_key, len(rowset)))
 
     return rowset.first().object_id
 
 
-my_datetime = SQLCustomType(type='string',
-                            native='char(35)',
-                            encoder=(lambda x: x.isoformat(' ')),
-                            decoder=(lambda x: dateutil.parser.parse(x)))
-
-
-def define_auth_rbac_model(db, other_args):
-    db.define_table('identity',
-                    # std uuid from uuid libs are 36 chars long
-                    Field('object_id', 'string', length=36, unique=True, notnull=True, default=str(uuid.uuid4())),
-                    Field('object_type', 'string', requires=(IS_IN_LIST(other_args['allowed_types']))),
-                    Field('created', 'datetime', default=datetime.datetime.now),
-                    # email needn't be unique, groups can share email addresses, and with people too
-                    Field('email', 'string'),
-                    Field('firstname', 'string', comment='also used as short code for groups'),
-                    Field('fullname', 'string'),
-                    Field('encoded_password', 'string'),
-                    )
-
-    db.define_table('membership',
-                    # beide zijn eigenlijk: reference:identity.object_id
-                    Field('subject', 'string', length=36, notnull=True),
-                    Field('member_of', 'string', length=36, notnull=True),
-                    # Field('starts','datetime', default=DEFAULT_STARTS),
-                    # Field('ends','datetime', default=DEFAULT_ENDS),
-                    )
-
-    db.define_table('permission',
-                    Field('privilege', 'string', length=20),
-                    # reference:identity.object_id
-                    Field('identity_object_id', 'string', length=36),
-                    Field('target_object_id', 'string', length=36),
-                    # Field('scope'), lets bail scope for now. every one needs a rule for everything
-                    # just to make sure, no 'wildcards' and 'every dossier for org x' etc ...
-                    Field('starts', type=my_datetime, default=DEFAULT_STARTS),
-                    Field('ends', type=my_datetime, default=DEFAULT_ENDS),
-                    )
-
-    db.define_table('recursive_memberships',
-                    Field('root'),
-                    Field('object_id'),
-                    Field('object_type'),
-                    Field('level', 'integer'),
-                    Field('email'),
-                    Field('firstname'),
-                    Field('fullname'),
-                    migrate=False,
-                    primarykey=['root', 'object_id']  # composed, no primary key
-                    )
-    db.define_table('recursive_members',
-                    Field('root'),
-                    Field('object_id'),
-                    Field('object_type'),
-                    Field('level', 'integer'),
-                    Field('email'),
-                    Field('firstname'),
-                    Field('fullname'),
-                    migrate=False,
-                    primarykey=['root', 'object_id']  # composed, no primary key
-                    )
+my_datetime = SQLCustomType(
+    type="string", native="char(35)", encoder=(lambda x: x.isoformat(" ")), decoder=(lambda x: dateutil.parser.parse(x))
+)
+
+
+class RbacKwargs(typing.TypedDict, total=False):
+    allowed_types: list[str]
+    migrate: bool
+
+
+class Identity(typing.Protocol):
+    object_id: str
+    object_type: str
+    created: dt.datetime
+    email: str
+    firstname: str
+    lastname: Optional[str]
+    fullname: str
+    encoded_password: str
+
+    def update_record(self, **data) -> None: ...
+
+
+def define_auth_rbac_model(db: DAL, other_args: RbacKwargs):
+    migrate = other_args.get("migrate", False)
+
+    db.define_table(
+        "identity",
+        # std uuid from uuid libs are 36 chars long
+        Field("object_id", "string", length=36, unique=True, notnull=True, default=str(uuid.uuid4())),
+        Field("object_type", "string", requires=(IS_IN_LIST(other_args["allowed_types"]))),
+        Field("created", "datetime", default=dt.datetime.now),
+        # email needn't be unique, groups can share email addresses, and with people too
+        Field("email", "string"),
+        Field("firstname", "string", comment="also used as short code for groups"),
+        Field("lastname", "string"),
+        Field("fullname", "string"),
+        Field("encoded_password", "string"),
+        migrate=migrate,
+    )
+
+    db.define_table(
+        "membership",
+        # beide zijn eigenlijk: reference:identity.object_id
+        Field("subject", "string", length=36, notnull=True),
+        Field("member_of", "string", length=36, notnull=True),
+        # Field('starts','datetime', default=DEFAULT_STARTS),
+        # Field('ends','datetime', default=DEFAULT_ENDS),
+        migrate=migrate,
+    )
+
+    db.define_table(
+        "permission",
+        Field("privilege", "string", length=20),
+        # reference:identity.object_id
+        Field("identity_object_id", "string", length=36),
+        Field("target_object_id", "string", length=36),
+        # Field('scope'), lets bail scope for now. every one needs a rule for everything
+        # just to make sure, no 'wildcards' and 'every dossier for org x' etc ...
+        Field("starts", type=my_datetime, default=DEFAULT_STARTS),
+        Field("ends", type=my_datetime, default=DEFAULT_ENDS),
+        migrate=migrate,
+    )
+
+    db.define_table(
+        "recursive_memberships",
+        Field("root"),
+        Field("object_id"),
+        Field("object_type"),
+        Field("level", "integer"),
+        Field("email"),
+        Field("firstname"),
+        Field("fullname"),
+        migrate=False,  # view
+        primarykey=["root", "object_id"],  # composed, no primary key
+    )
+    db.define_table(
+        "recursive_members",
+        Field("root"),
+        Field("object_id"),
+        Field("object_type"),
+        Field("level", "integer"),
+        Field("email"),
+        Field("firstname"),
+        Field("fullname"),
+        migrate=False,  # view
+        primarykey=["root", "object_id"],  # composed, no primary key
+    )
 
 
-def add_identity(db, email, password, member_of, name=None, firstname=None, fullname=None, gid=None, object_type=None):
-    """paramaters name and firstname are equal. """
+def add_identity(
+    db: DAL,
+    email: str,
+    member_of: list[IdentityKey],
+    name: Optional[str] = None,
+    firstname: Optional[str] = None,
+    fullname: Optional[str] = None,
+    password: Optional[str] = None,
+    gid: Optional[IdentityKey] = None,
+    object_type: Optional[ObjectTypes] = None,
+) -> str:
+    """paramaters name and firstname are equal."""
     email = email.lower().strip()
     if object_type is None:
-        raise ValueError('object_type parameter expected')
-    object_id = gid if gid else str(uuid.uuid4())
+        raise ValueError("object_type parameter expected")
+    object_id = gid if gid else uuid.uuid4()
     db.identity.validate_and_insert(
         object_id=object_id,
         object_type=object_type,
         email=email,
         firstname=name or firstname or None,
         fullname=fullname,
-        encoded_password=Password.encode(password)
+        encoded_password=Password.encode(password) if password else None,
     )
     db.commit()
     for key in member_of:
-        group_id = key_lookup(db, key, 'group')
+        group_id = key_lookup(db, key, "group")
         if get_group(db, group_id):
             # check each group if it exists.
             add_membership(db, identity_key=object_id, group_key=group_id)
     db.commit()
-    return object_id
+    return str(object_id)
 
 
-def add_group(db, email, name, member_of):
-    return add_identity(db, email, None, member_of, name=name, object_type='group')
+def add_group(db: DAL, email: str, name: str, member_of: list[IdentityKey]):
+    return add_identity(db, email, member_of, name=name, object_type="group")
 
 
-def remove_identity(db, object_id):
+def remove_identity(db: DAL, object_id: IdentityKey):
     removed = db(db.identity.object_id == object_id).delete()
     # todo: remove permissions and group memberships
     db.commit()
     return removed > 0
 
 
-def get_identity(db, key, object_type=None):
+def get_identity(db: DAL, key: IdentityKey, object_type: Optional[ObjectTypes] = None) -> Identity:
     """
     :param db: dal db connection
     :param key: can be the email, id, or object_id
     :return: user record or None when not found
     """
     query = key_lookup_query(db, key, object_type)
     rows = db(query).select()
     return rows.first()
 
 
-def get_user(db, key):
+def get_user(db: DAL, key: IdentityKey):
     """
     :param db: dal db connection
     :param key: can be the email, id, or object_id
     :return: user record or None when not found
     """
-    return get_identity(db, key, object_type='user')
+    return get_identity(db, key, object_type="user")
 
 
-def get_group(db, key):
+def get_group(db: DAL, key: IdentityKey):
     """
 
     :param db: dal db connection
     :param key: can be the name of the group, the id, object_id or email_address
     :return: user record or None when not found
     """
-    return get_identity(db, key, object_type='group')
+    return get_identity(db, key, object_type="group")
 
 
-def authenticate_user(db, password=None, user=None, key=None):
+def authenticate_user(
+    db: DAL, password: Optional[str] = None, user: Optional[Identity] = None, key: Optional[IdentityKey] = None
+) -> bool:
     if not password:
         return False
-    if not user:
+
+    if not user and key:
         user = get_user(db, key)
-    return Password.validate(password, user.encoded_password)
 
+    if user:
+        return Password.validate(password, user.encoded_password)
 
-def add_membership(db, identity_key, group_key):
+    return False
+
+
+def add_membership(db: DAL, identity_key: IdentityKey, group_key: IdentityKey) -> None:
     identity_oid = key_lookup(db, identity_key)
     if identity_oid is None:
-        raise ValueError('invalid identity_oid key: ' + identity_key)
+        raise ValueError(f"invalid identity_oid key: {identity_key}")
     group = get_group(db, group_key)
     if not group:
-        raise ValueError('invalid group key: ' + group_key)
+        raise ValueError(f"invalid group key: {group_key}")
     query = db.membership.subject == identity_oid
     query &= db.membership.member_of == group.object_id
     if db(query).count() == 0:
         db.membership.validate_and_insert(
             subject=identity_oid,
             member_of=group.object_id,
         )
     db.commit()
 
 
-def remove_membership(db, identity_key, group_key):
+def remove_membership(db: DAL, identity_key: IdentityKey, group_key: IdentityKey) -> int:
     identity = get_identity(db, identity_key)
     group = get_group(db, group_key)
     query = db.membership.subject == identity.object_id
     query &= db.membership.member_of == group.object_id
     deleted = db(query).delete()
     db.commit()
     return deleted
 
 
-def get_memberships(db, object_id, bare=True):
+def get_memberships(db: DAL, object_id: IdentityKey, bare: bool = True):
     query = db.recursive_memberships.root == object_id
-    fields = [db.recursive_memberships.object_id, db.recursive_memberships.object_type]
-    if not bare:
-        fields = []
+    fields = [db.recursive_memberships.object_id, db.recursive_memberships.object_type] if bare else []
     return db(query).select(*fields)
 
 
-def get_members(db, object_id, bare=True):
+def get_members(db: DAL, object_id: IdentityKey, bare: bool = True):
     query = db.recursive_members.root == object_id
-    fields = [db.recursive_members.object_id, db.recursive_members.object_type]
-    if not bare:
-        fields = []
+    fields = [db.recursive_members.object_id, db.recursive_members.object_type] if bare else []
     return db(query).select(*fields)
 
 
-def add_permission(db, identity_key, target_oid, privilege, starts=DEFAULT_STARTS, ends=DEFAULT_ENDS):
+def add_permission(
+    db: DAL,
+    identity_key: IdentityKey,
+    target_oid: IdentityKey,
+    privilege: str,
+    starts: dt.datetime | str = DEFAULT_STARTS,
+    ends: dt.datetime | str = DEFAULT_ENDS,
+) -> None:
     identity_oid = key_lookup(db, identity_key)
     starts = unstr_datetime(starts)
     ends = unstr_datetime(ends)
     if has_permission(db, identity_oid, target_oid, privilege, when=starts):
         # permission already granted. just skip it
         print(
-            '{privilege} permission already granted to {user_or_group_key} on {target_oid} @ {starts} '.format(
-                **locals()))
+            "{privilege} permission already granted to {user_or_group_key} on {target_oid} @ {starts} ".format(
+                **locals()
+            )
+        )
         # print(db._lastsql)
         return
     db.permission.validate_and_insert(
         privilege=privilege,
         identity_object_id=identity_oid,
         target_object_id=target_oid,
         starts=starts,
         ends=ends,
     )
     db.commit()
 
 
-def remove_permission(db, identity_key, target_oid, privilege, when=DEFAULT):
+def remove_permission(
+    db: DAL, identity_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+) -> bool:
     identity_oid = key_lookup(db, identity_key)
     if when is DEFAULT:
-        when = datetime.datetime.now()
+        when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
     # base object is is the root to check for, user or group
     permission = db.permission
     query = permission.identity_object_id == identity_oid
     query &= permission.target_object_id == target_oid
     query &= permission.privilege == privilege
@@ -300,44 +358,46 @@
     query &= permission.ends >= when
     result = db(query).delete() > 0
     db.commit()
     # print(db._lastsql)
     return result
 
 
-def with_alias(db, source, alias):
+def with_alias(db: DAL, source: Table, alias: str) -> Table:
     other = copy.copy(source)
-    other['ALL'] = SQLALL(other)
-    other['_tablename'] = alias
+    other["ALL"] = SQLALL(other)
+    other["_tablename"] = alias
     for fieldname in other.fields:
         tmp = source[fieldname].clone()
         tmp.bind(other)
         other[fieldname] = tmp
-    if 'id' in source and 'id' not in other.fields:
-        other['id'] = other[source.id.name]
+    if "id" in source and "id" not in other.fields:
+        other["id"] = other[source.id.name]
 
     if source_id := getattr(source, "_id", None):
         other._id = other[source_id.name]
     db[alias] = other
     return other
 
 
-def has_permission(db, user_or_group_key, target_oid, privilege, when=DEFAULT):
+def has_permission(
+    db: DAL, user_or_group_key: IdentityKey, target_oid: IdentityKey, privilege: str, when: When | None = DEFAULT
+) -> bool:
     user_or_group_oid = key_lookup(db, user_or_group_key)
     # the permission system
     if when is DEFAULT:
-        when = datetime.datetime.now()
+        when = dt.datetime.now()
     else:
         when = unstr_datetime(when)
     # base object is is the root to check for, user or group
     root_oid = user_or_group_oid
     permission = db.permission
     # ugly hack to satisfy pydal aliasing keyed tables /views
-    left = with_alias(db, db.recursive_memberships, 'left')
-    right = with_alias(db, db.recursive_memberships, 'right')
+    left = with_alias(db, db.recursive_memberships, "left")
+    right = with_alias(db, db.recursive_memberships, "right")
     # left = db.recursive_memberships.with_alias('left')
     # right = db.recursive_memberships.with_alias('right')
 
     # end of ugly hack
     query = left.root == root_oid
     query &= right.root == target_oid
     query &= permission.identity_object_id == left.object_id
```

### Comparing `edwh_auth_rbac-0.1.1/tests/test_rbac.py` & `edwh_auth_rbac-0.2.0/tests/test_rbac.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 import tempfile
-
-from pydal import DAL
 import uuid
-import pytest
+
 import dotmap
+import pytest
+from pydal import DAL
 
+from src.edwh_auth_rbac.migrations import rbac_views
 from src.edwh_auth_rbac.model import define_auth_rbac_model
 from src.edwh_auth_rbac.rbac import AuthRbac
-from src.edwh_auth_rbac.migrations import rbac_migrations
 
-namespace = uuid.UUID('84f5c757-4be0-49c8-a3ba-4f4d79167839')
+namespace = uuid.UUID("84f5c757-4be0-49c8-a3ba-4f4d79167839")
 
 
 @pytest.fixture(scope="module")
 def tmpdir():
     with tempfile.TemporaryDirectory() as tmpdirname:
-        print('new tempdir')
+        print("new tempdir")
         yield tmpdirname
 
 
 @pytest.fixture(scope="module")
 def database(tmpdir):
     class Database:
         def __enter__(self):
-            self.db = DAL('sqlite://auth_rbac.sqlite', folder=tmpdir)
+            self.db = DAL("sqlite://auth_rbac.sqlite", folder=tmpdir)
+
+            settings = dict(allowed_types=["user", "group"], migrate=True)
 
-            define_auth_rbac_model(self.db, dict(allowed_types=['user', 'group']))
-            rbac_migrations(self.db)
+            define_auth_rbac_model(self.db, settings)
+            rbac_views(self.db)
             return self.db
 
         def __exit__(self, exc_type, exc_value, traceback):
             self.db.close()
 
     return Database()
 
@@ -39,100 +41,102 @@
 def rbac(database):
     with database as db:
         yield AuthRbac(db)
 
 
 @pytest.fixture(scope="module")
 def store(_=dotmap.DotMap()):
-    print('store', _)
+    print("store", _)
     return _
 
 
 @pytest.mark.incremental
 class TestSequentially:
     def test_drop_all_test_users(self, database):
         with database as db:
-            users = db(db.identity.email.contains('@test.nl')).select()
-            db(db.identity.email.contains('@test.nl')).delete()
+            users = db(db.identity.email.contains("@test.nl")).select()
+            db(db.identity.email.contains("@test.nl")).delete()
             for user in users:
                 db((db.membership.member_of == user.object_id) | (db.membership.subject == user.object_id)).delete()
-                db((db.permission.identity_object_id == user.object_id) | (
-                        db.permission.target_object_id == user.object_id)).delete()
+                db(
+                    (db.permission.identity_object_id == user.object_id)
+                    | (db.permission.target_object_id == user.object_id)
+                ).delete()
             db.commit()
-            assert db(db.identity.email.contains('@test.nl')).count() == 0, 'Howcome @test.nl still exist?'
+            assert db(db.identity.email.contains("@test.nl")).count() == 0, "Howcome @test.nl still exist?"
 
     def test_user_creation(self, rbac, store):
-        store.remco = rbac.add_user('remco@test.nl', 'remco', 'remco test', 'secret', [])['object_id']
-        store.pietje = rbac.add_user('pietje@test.nl', 'pietje', 'pietje test', 'secret', [])['object_id']
-        store.truus = rbac.add_user('truus@test.nl', 'truus', 'truus test', 'secret', [])['object_id']
+        store.remco = rbac.add_user("remco@test.nl", "remco", "remco test", "secret", [])["object_id"]
+        store.pietje = rbac.add_user("pietje@test.nl", "pietje", "pietje test", "secret", [])["object_id"]
+        store.truus = rbac.add_user("truus@test.nl", "truus", "truus test", "secret", [])["object_id"]
 
     def test_group_creation(self, rbac, store):
-        store.articles = rbac.add_group('articles@test.nl', 'articles', [])['object_id']
-        store.all = rbac.add_group('all@test.nl', 'all', [])['object_id']
-        store.users = rbac.add_group('users@test.nl', 'users', [])['object_id']
-        store.admins = rbac.add_group('admins@test.nl', 'admins', [])['object_id']
+        store.articles = rbac.add_group("articles@test.nl", "articles", [])["object_id"]
+        store.all = rbac.add_group("all@test.nl", "all", [])["object_id"]
+        store.users = rbac.add_group("users@test.nl", "users", [])["object_id"]
+        store.admins = rbac.add_group("admins@test.nl", "admins", [])["object_id"]
 
     def test_item_creation(self, rbac, store):
-        for name in 'abcde':
-            store[name] = rbac.add_user('article_' + name + '@test.nl', name, 'article', '', [])[
-                'object_id']
+        for name in "abcde":
+            store[name] = rbac.add_user("article_" + name + "@test.nl", name, "article", "", [])["object_id"]
 
     def test_stash_users_in_groups(self, rbac, store):
         rbac.add_membership(store.remco, store.admins)
         rbac.add_membership(store.pietje, store.users)
         rbac.add_membership(store.truus, store.users)
         rbac.add_membership(store.users, store.all)
         rbac.add_membership(store.admins, store.all)
 
     def test_stash_items_in_groups(self, rbac, store):
-        for name in 'abcde':
+        for name in "abcde":
             rbac.add_membership(store[name], store.articles)
 
     def test_add_some_permissions(self, rbac, store):
-        rbac.add_permission(store.admins, store.articles, 'read')
-        rbac.add_permission(store.admins, store.articles, 'write')
-        rbac.add_permission(store.users, store.articles, 'read')
+        rbac.add_permission(store.admins, store.articles, "read")
+        rbac.add_permission(store.admins, store.articles, "write")
+        rbac.add_permission(store.users, store.articles, "read")
 
     def test_first_level_memberships(self, rbac, store):
         assert rbac.has_membership(store.remco, store.admins) is True
         assert rbac.has_membership(store.pietje, store.users) is True
         assert rbac.has_membership(store.remco, store.users) is False
         assert rbac.has_membership(store.pietje, store.admins) is False
 
     def test_second_level_memberships(self, rbac, store):
         assert rbac.has_membership(store.remco, store.all) is True
         assert rbac.has_membership(store.pietje, store.all) is True
 
     def test_first_level_permissions(self, rbac, store):
-        assert rbac.has_permission(store.admins, store.articles, 'read') is True
-        assert rbac.has_permission(store.admins, store.articles, 'write') is True
-        assert rbac.has_permission(store.users, store.articles, 'read') is True
-        assert rbac.has_permission(store.users, store.articles, 'write') is False
+        assert rbac.has_permission(store.admins, store.articles, "read") is True
+        assert rbac.has_permission(store.admins, store.articles, "write") is True
+        assert rbac.has_permission(store.users, store.articles, "read") is True
+        assert rbac.has_permission(store.users, store.articles, "write") is False
 
     def test_second_to_first_level_permissions(self, rbac, store):
-        assert rbac.has_permission(store.remco, store.articles, 'read') is True
-        assert rbac.has_permission(store.remco, store.articles, 'write') is True
-        assert rbac.has_permission(store.pietje, store.articles, 'read') is True
-        assert rbac.has_permission(store.pietje, store.articles, 'write') is False
+        assert rbac.has_permission(store.remco, store.articles, "read") is True
+        assert rbac.has_permission(store.remco, store.articles, "write") is True
+        assert rbac.has_permission(store.pietje, store.articles, "read") is True
+        assert rbac.has_permission(store.pietje, store.articles, "write") is False
 
     def test_second_to_second_level_permissions(self, rbac, store):
-        assert rbac.has_permission(store.remco, store.a, 'read') is True
-        assert rbac.has_permission(store.remco, store.a, 'write') is True
-        assert rbac.has_permission(store.pietje, store.a, 'read') is True
-        assert rbac.has_permission(store.pietje, store.a, 'write') is False
+        assert rbac.has_permission(store.remco, store.a, "read") is True
+        assert rbac.has_permission(store.remco, store.a, "write") is True
+        assert rbac.has_permission(store.pietje, store.a, "read") is True
+        assert rbac.has_permission(store.pietje, store.a, "write") is False
 
     def test_deeper_group_nesting(self, rbac, store):
-        store.subadmins = rbac.add_group('sub_admins@test.nl', 'subadmins', [])['object_id']
-        store.subarticles = rbac.add_group('sub_articles@test.nl', 'subarticles', [])['object_id']
+        store.subadmins = rbac.add_group("sub_admins@test.nl", "subadmins", [])["object_id"]
+        store.subarticles = rbac.add_group("sub_articles@test.nl", "subarticles", [])["object_id"]
         rbac.add_membership(store.subarticles, store.articles)
         rbac.add_membership(store.subadmins, store.admins)
-        store.nested_admin = rbac.add_user('nested_admin@test.nl', 'nested_admin', 'nested_admin test', 'secret', [])[
-            'object_id']
+        store.nested_admin = rbac.add_user("nested_admin@test.nl", "nested_admin", "nested_admin test", "secret", [])[
+            "object_id"
+        ]
         rbac.add_membership(store.nested_admin, store.subadmins)
-        for name in 'stuvw':
-            store[name] = rbac.add_user('article_' + name + '@test.nl', name, 'subarticle', '', [])['object_id']
+        for name in "stuvw":
+            store[name] = rbac.add_user("article_" + name + "@test.nl", name, "subarticle", "", [])["object_id"]
             rbac.add_membership(store[name], store.subarticles)
-        assert rbac.has_permission(store.nested_admin, store.s, 'read') is True
+        assert rbac.has_permission(store.nested_admin, store.s, "read") is True
 
     def test_removing_a_nested_group(self, rbac, store):
         rbac.remove_membership(store.nested_admin, store.subadmins)
-        assert rbac.has_permission(store.nested_admin, store.s, 'read') is False
+        assert rbac.has_permission(store.nested_admin, store.s, "read") is False
```

### Comparing `edwh_auth_rbac-0.1.1/pyproject.toml` & `edwh_auth_rbac-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -50,17 +50,15 @@
 version_variable = "src/edwh_auth_rbac/__init__.py:__version__"
 change_log = "CHANGELOG.md"
 upload_to_repository = false
 upload_to_release = false
 build_command = "hatch build"
 
 [tool.su6]
-# every checker:
-directory = "."
-# 'all' and 'fix':
+directory = "src"
 include = []
 exclude = []
 # 'all':
 stop-after-first-failure = false
 # pytest:
 coverage = 100
 badge = true
```

### Comparing `edwh_auth_rbac-0.1.1/PKG-INFO` & `edwh_auth_rbac-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: edwh-auth-rbac
-Version: 0.1.1
+Version: 0.2.0
 Summary: Recursive Memberships and Permissions for the Education Warehouse Authentication System
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-auth-rbac#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-auth-rbac/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-auth-rbac
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 Keywords: edwh,omgeving,whitelabel
```

