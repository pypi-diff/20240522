# Comparing `tmp/tenb2jira-2.0.4.tar.gz` & `tmp/tenb2jira-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tenb2jira-2.0.4.tar", last modified: Tue May 21 15:41:22 2024, max compression
+gzip compressed data, was "tenb2jira-2.0.5.tar", last modified: Wed May 22 17:32:55 2024, max compression
```

## Comparing `tenb2jira-2.0.4.tar` & `tenb2jira-2.0.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.643429 tenb2jira-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-21 15:41:22.643429 tenb2jira-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 15:41:22.643429 tenb2jira-2.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.635429 tenb2jira-2.0.4/tenb2jira/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.639429 tenb2jira-2.0.4/tenb2jira/jira/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.639429 tenb2jira-2.0.4/tenb2jira/jira/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/issuetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/api/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/jira.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/jira/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18919 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.639429 tenb2jira-2.0.4/tenb2jira/tenable/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/tenable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/tenable/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/tenable/tenable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tenb2jira/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.639429 tenb2jira-2.0.4/tenb2jira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 15:41:22.000000 tenb2jira-2.0.4/tenb2jira.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:41:22.639429 tenb2jira-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-21 15:41:15.000000 tenb2jira-2.0.4/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.755729 tenb2jira-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-22 17:32:55.755729 tenb2jira-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9934 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:32:55.755729 tenb2jira-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.747729 tenb2jira-2.0.5/tenb2jira/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.751729 tenb2jira-2.0.5/tenb2jira/jira/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.751729 tenb2jira-2.0.5/tenb2jira/jira/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/issuetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6990 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/jira.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/jira/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20298 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.751729 tenb2jira-2.0.5/tenb2jira/tenable/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/tenable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/tenable/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/tenable/tenable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tenb2jira/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.751729 tenb2jira-2.0.5/tenb2jira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 17:32:55.000000 tenb2jira-2.0.5/tenb2jira.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:32:55.751729 tenb2jira-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-22 17:32:51.000000 tenb2jira-2.0.5/tests/test_processor.py
```

### Comparing `tenb2jira-2.0.4/PKG-INFO` & `tenb2jira-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.4
+Version: 2.0.5
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.4/README.md` & `tenb2jira-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/pyproject.toml` & `tenb2jira-2.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/cli.py` & `tenb2jira-2.0.5/tenb2jira/cli.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/fields.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/fields.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/issues.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/issues.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/issuetypes.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/issuetypes.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/iterator.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/iterator.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/projects.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/projects.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/screens.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/screens.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/api/session.py` & `tenb2jira-2.0.5/tenb2jira/jira/api/session.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/field.py` & `tenb2jira-2.0.5/tenb2jira/jira/field.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/jira.py` & `tenb2jira-2.0.5/tenb2jira/jira/jira.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/jira/task.py` & `tenb2jira-2.0.5/tenb2jira/jira/task.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/models.py` & `tenb2jira-2.0.5/tenb2jira/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class SubTaskMap(Base):
     __tablename__ = 'subtask'
     finding_id: Mapped[UUID] = mapped_column(primary_key=True,
                                              sqlite_on_conflict_unique='IGNORE'
                                              )
     asset_id: Mapped[UUID]
-    jira_key: Mapped[str]
+    jira_id: Mapped[str]
     plugin_id: Mapped[int] = mapped_column(ForeignKey('task.plugin_id'))
     is_open: Mapped[bool]
     updated: Mapped[datetime]
     task: Mapped["TaskMap"] = relationship(back_populates="subtasks")
 
     def __init__(self,
                  finding_id: str,
```

### Comparing `tenb2jira-2.0.4/tenb2jira/processor.py` & `tenb2jira-2.0.5/tenb2jira/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,16 +151,16 @@
         associated action.
         """
         task = self.jira.task.generate(finding)
 
         # If the finding related to this task is not in an open state, then
         # there is no reason to continue.  Return back a NoneType value.
         if not task.is_open:
-            log.info(f'Finding related to Task {task.fields[self.plugin_id]} '
-                     'is closed, skipping'
+            log.info(f'Finding related to Plugin {task.fields[self.plugin_id]}'
+                     ' is closed, skipping'
                      )
             return None
 
         sql = s.query(TaskMap)\
                .filter_by(plugin_id=task.fields[self.plugin_id])\
                .one_or_none()
 
@@ -217,15 +217,15 @@
             sql = TaskMap(plugin_id=task.fields[self.plugin_id],
                           jira_id=resp.key,
                           updated=datetime.now()
                           )
             s.add(sql)
             s.commit()
             log.info(f'Created Task "{resp.key}" and added to SQL Cache.')
-            return resp.id
+            return resp.key
 
         # In the event that multiple tasks are returned from the search,
         # something went seriously wrong.  We will log to the console, then
         # raise an exception to terminate further processing at this point.
         if len(page.issues) > 1:
             msg = ('Multiple Jira Tasks match Plugin '
                    f'"{task.fields[self.plugin_id]}".  Jira IDs are '
@@ -241,15 +241,15 @@
                        ) -> (int | None):
         """
         Performs subtask generation && checks both the local cache and Jira to
         determine if the subtask is a new issue or an existing and performs the
         associated action.
         """
         task = self.jira.subtask.generate(finding)
-        task.fields['parent'] = {'id': str(task_id)}
+        task.fields['parent'] = {'key': str(task_id)}
         sql = s.query(SubTaskMap)\
                .filter_by(finding_id=UUID(task.fields[self.finding_id]))\
                .one_or_none()
 
         # If we had a match from the SQL cache we will then update the task in
         # Jira and return the jira issue id back to the caller.
         if sql:
@@ -289,15 +289,15 @@
         match len(page.issues):
             # If only 1 match was found (and we should generally only ever
             # have) a single match if one exists), then we will update the sql
             # cache with the mapping and update the task.  Lastly, we will
             # return the Jira issue id back to the caller.
             case 1:
                 sql = SubTaskMap(plugin_id=task.fields[self.plugin_id],
-                                 asset_id=task.fields[self.asset_id],
+                                 asset_id=task.fields[self.asset_id][0],
                                  finding_id=task.fields[self.finding_id],
                                  jira_id=page.issues[0].key,
                                  is_open=task.is_open,
                                  updated=datetime.now(),
                                  )
                 s.add(sql)
                 s.commit()
@@ -328,24 +328,25 @@
                                      updated=datetime.now(),
                                      )
                     s.add(sql)
                     s.commit()
                     log.info(f'Created Subtask "{resp.key}" and '
                              'added to SQL Cache.'
                              )
-                    return resp.id
+                    return resp.key
 
             # In the event that multiple tasks are returned from the
             # search, something went seriously wrong.  We will log to the
             # console, then raise an exception to terminate further
             # processing at this point.
             case _:
                 msg = ('Multiple Jira SubTasks match Finding '
                        f'"{task.fields[self.finding_id]}".  Jira IDs are '
                        f'"{", ".join(i.key for i in page.issues)}".'
+                       '  SKIPPING.'
                        )
                 log.error(msg)
                 raise Exception(msg)
 
     def close_dead_assets(self, dead_assets: iter):
         """
         Closes all subtasks associated with dead hosts.
@@ -392,14 +393,15 @@
     def finding_job(self, finding: dict):
         """
         A simple worker method for updating a task & subtask
         """
         with Session(self.engine) as session:
             task_id = self.upsert_task(s=session, finding=finding)
             self.upsert_subtask(s=session, task_id=task_id, finding=finding)
+            session.commit()
 
     def sync(self):
         """
         Tenable to Jira Synchronization method.
         """
         self.start_time = datetime.now()
         ts = int(arrow.get(self.start_time).timestamp())
@@ -407,19 +409,48 @@
         # Get the findings and the asset cleanup generators.
         findings = self.tenable.get_generator()
         asset_cleanup = self.tenable.get_asset_cleanup()
 
         # build the db cache
         self.build_cache()
 
-        # Using as many threads as we need (up to the max configured)
-        # go ahead and process the findings.
-        with ThreadPoolExecutor(max_workers=self.max_workers) as e:
+        # If only a single thread was set, then we wont even run through a
+        # threaded execution worker.
+        if self.max_workers <= 1:
             for finding in findings:
-                e.submit(self.finding_job, finding)
+                self.finding_job(finding)
+
+        # Using as many threads as we need (up to the max configured)
+        # go ahead and process the findings.  We will store the job results
+        # and confirm that no exceptions had occurred.  if any did, then we'll
+        # raise those exceptions and refuse to continue with closing any issues
+        # to ensure that we don't put the project into a weird state.
+        else:
+            jobs = []
+            exc_count = 0
+
+            # launch the threat executor and store each future job for later
+            # analysis.
+            with ThreadPoolExecutor(max_workers=self.max_workers) as e:
+                for finding in findings:
+                    jobs.append(e.submit(self.finding_job, finding))
+
+            # Check each job to see if any exceptions were raised.  If so, then
+            # log those exceptions and increment the exception counter.
+            for job in jobs:
+                if job.exception():
+                    log.exception(job.exception())
+                    exc_count += 1
+
+            # If we have a non-zero value from the exception counter, then
+            # log the total number of exceptions encountered and terminate.
+            if exc_count > 0:
+                log.error(f'Refusing to continue ({exc_count} errors) '
+                          '& terminating sync.')
+                return
 
         # cleanup the dead hosts and clear out the empty tasks.
         self.close_dead_assets(asset_cleanup)
         self.close_empty_tasks()
 
         # update the last_run timestamp with the time that we started the sync.
         self.config['tenable']['last_run'] = ts
```

### Comparing `tenb2jira-2.0.4/tenb2jira/tenable/generators.py` & `tenb2jira-2.0.5/tenb2jira/tenable/generators.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/tenable/tenable.py` & `tenb2jira-2.0.5/tenb2jira/tenable/tenable.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira/validator.py` & `tenb2jira-2.0.5/tenb2jira/validator.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tenb2jira.egg-info/PKG-INFO` & `tenb2jira-2.0.5/tenb2jira.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tenb2jira
-Version: 2.0.4
+Version: 2.0.5
 Summary: Tenable Vulnerability Management to Jira Cloud issue manager
 Author-email: "Tenable, Inc." <smcgrath@tenable.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/tenable/integration-jira-cloud
 Project-URL: Repository, https://github.com/tenable/integration-jira-cloud
 Project-URL: Issues, https://github.com/tenable/integration-jira-cloud/issues
 Project-URL: Changelog, https://github.com/tenable/integration-jira-cloud/blob/master/CHANGELOG.md
```

### Comparing `tenb2jira-2.0.4/tenb2jira.egg-info/SOURCES.txt` & `tenb2jira-2.0.5/tenb2jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tests/test_models.py` & `tenb2jira-2.0.5/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `tenb2jira-2.0.4/tests/test_processor.py` & `tenb2jira-2.0.5/tests/test_processor.py`

 * *Files identical despite different names*

