# Comparing `tmp/jiraA-0.0.1-py3-none-any.whl.zip` & `tmp/jiraA-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 9344 bytes, number of entries: 16
+Zip file size: 9523 bytes, number of entries: 16
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 16:23 jiraX/__init__.py
 -rw-r--r--  2.0 unx      784 b- defN 24-May-15 15:53 jiraX/backlog.py
 -rw-r--r--  2.0 unx      308 b- defN 24-May-14 16:23 jiraX/base.py
 -rw-r--r--  2.0 unx     1321 b- defN 24-May-15 15:28 jiraX/board.py
 -rw-r--r--  2.0 unx      823 b- defN 24-May-15 15:28 jiraX/comment.py
 -rw-r--r--  2.0 unx     1499 b- defN 24-May-14 16:23 jiraX/factories.py
--rw-r--r--  2.0 unx     4461 b- defN 24-May-15 17:03 jiraX/issue.py
--rw-r--r--  2.0 unx     2137 b- defN 24-May-15 15:28 jiraX/project.py
+-rw-r--r--  2.0 unx     4461 b- defN 24-May-22 16:56 jiraX/issue.py
+-rw-r--r--  2.0 unx     2643 b- defN 24-May-22 16:53 jiraX/project.py
 -rw-r--r--  2.0 unx     1306 b- defN 24-May-15 15:28 jiraX/role.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-14 17:51 jiraX/sprint.py
+-rw-r--r--  2.0 unx     1184 b- defN 24-May-22 16:55 jiraX/sprint.py
 -rw-r--r--  2.0 unx      787 b- defN 24-May-15 15:28 jiraX/sprintbacklog.py
 -rw-r--r--  2.0 unx     2895 b- defN 24-May-15 16:21 jiraX/user.py
--rw-r--r--  2.0 unx     3296 b- defN 24-May-21 18:29 jiraA-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 18:29 jiraA-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-May-21 18:29 jiraA-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1153 b- defN 24-May-21 18:29 jiraA-0.0.1.dist-info/RECORD
-16 files, 22092 bytes uncompressed, 7492 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     3296 b- defN 24-May-22 16:58 jiraA-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 16:58 jiraA-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-May-22 16:58 jiraA-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1153 b- defN 24-May-22 16:58 jiraA-0.0.2.dist-info/RECORD
+16 files, 22558 bytes uncompressed, 7671 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: jiraX/sprintbacklog.py
 Comment: 
 
 Filename: jiraX/user.py
 Comment: 
 
-Filename: jiraA-0.0.1.dist-info/METADATA
+Filename: jiraA-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: jiraA-0.0.1.dist-info/WHEEL
+Filename: jiraA-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: jiraA-0.0.1.dist-info/top_level.txt
+Filename: jiraA-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jiraA-0.0.1.dist-info/RECORD
+Filename: jiraA-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jiraX/project.py

```diff
@@ -7,28 +7,51 @@
 	Class responsable for documentation projects in Jira
 	"""
 	ERROR = "OS error: {0}"
 	
 	def __init__(self, user, apikey, server):
 		Base.__init__(self, user, apikey, server)
 	
+	def get_all_function(self, today=False, **kwargs):
+		result = []
+		projects = []
+		
+		try:
+			
+			function = kwargs["function"]
+
+			logging.info("Start function: get_projects")
+			result = self.find_all()
+			for project in result:
+				value = project.__dict__
+				projects.append(value)
+				if function is not None:
+					function (data=value, topic=kwargs["topic"], extra_data=kwargs["extra_data"])
+				
+		except Exception as e: 
+			logging.error("OS error: {0}".format(e))
+			logging.error(e.__dict__) 
+
+		logging.info("Retrieve All Projects")
+		return projects	
+
+	
 	def find_all(self): 
 		"""
 		Responsible for retreving information about projects
 
 		Returns:
 		
 			List -- Lits of projects
 
 		"""
 		try:
 			logging.info("Start function: find_all")
 			return self.jira.projects()	
-			self.jira.__init__
-			logging.info("End function: find_all")
+	
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 	def find_by_key(self, project_key):
 		"""
 		Responsible for finding project with the given key
```

## jiraX/sprint.py

```diff
@@ -43,14 +43,13 @@
 		Returns:
 		
 			Sprint/None -- Sprint if found
 
 		"""
 		try:
 			logging.info("Start function: find_by_id")
-			return self.jira.sprint(sprint_id)
-			logging.info("End funcion: find_by_id")
+			return self.jira.sprint(sprint_id)			
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__)
```

## Comparing `jiraA-0.0.1.dist-info/METADATA` & `jiraA-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiraA
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lib created based on documentaion https://docs.atlassian.com/DAC/rest/jira/6.1.html
 Home-page: https://gitlab.com/integration_seon/libs/application/jira
 Author: Paulo Sérgio dos Santos Júnior
 Author-email: paulossjunior@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `jiraA-0.0.1.dist-info/RECORD` & `jiraA-0.0.2.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 jiraX/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 jiraX/backlog.py,sha256=UPSnztuP5_UqSjE5qnhKqwqN91ntFYKnKjPSJNpWfLQ,784
 jiraX/base.py,sha256=jt2W8EInTdgEkCHa91Fupp_vjCjUZrNrwChC-osb0tE,308
 jiraX/board.py,sha256=NlZbWIqpwl7grHv50VABSrDqoU47Yf7snyP0tpfflsM,1321
 jiraX/comment.py,sha256=jf3A-g9DgjGQyQqQIMICfMQSUSfUZK7DffEmiKmvETw,823
 jiraX/factories.py,sha256=Ug9FHIpctrJxv1FwEOHqtjJ7iHbCvnBYptucLygvOgE,1499
 jiraX/issue.py,sha256=kTobi0gwaVJ69HhUVO3NGo7HlDqHKV75Bwh0Vjuhpg4,4461
-jiraX/project.py,sha256=I2eP5zOp3pQ_4o-dmEk8Ri4a5SEwEi0rK4mArSYo6E8,2137
+jiraX/project.py,sha256=qphzVp5yynOG75bqfEIwsOfi-FBgUPq-zZ17v0N3Urc,2643
 jiraX/role.py,sha256=amFxvL3Ij4Rzwl5CuKwpAPHgw2EMgWmlstsQZUQwJs0,1306
-jiraX/sprint.py,sha256=Z4Sa2CTH8OWpSrLN4FjThSTse9vW6i7WVxkbcbKAwc8,1224
+jiraX/sprint.py,sha256=MB7SocPAcBTeSQSUQX1NdQRphJjZ-wtswmaxulTgraY,1184
 jiraX/sprintbacklog.py,sha256=UTtOxNDY_NVmlhCBkwa1LSFgx-hDMYI9StfD0jK2aQs,787
 jiraX/user.py,sha256=RTQsx7RVm0j4zyNyjaDRrNLM5DcwVpbJKeRxCUv9IoE,2895
-jiraA-0.0.1.dist-info/METADATA,sha256=QbMxDA7aDADzZDVRWRw2Fl7cMklcARpk5mykvZHmCqg,3296
-jiraA-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-jiraA-0.0.1.dist-info/top_level.txt,sha256=ALK1II_rDaF8gAa1lmDaKiZ7nr23rPPmgEtSXv03tyY,6
-jiraA-0.0.1.dist-info/RECORD,,
+jiraA-0.0.2.dist-info/METADATA,sha256=RwxpsFqrDke8HHskba3xz8lwfw85r2sc1nPxHHmiBKQ,3296
+jiraA-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jiraA-0.0.2.dist-info/top_level.txt,sha256=ALK1II_rDaF8gAa1lmDaKiZ7nr23rPPmgEtSXv03tyY,6
+jiraA-0.0.2.dist-info/RECORD,,
```

