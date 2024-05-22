# Comparing `tmp/alq-0.0.2-py3-none-any.whl.zip` & `tmp/alq-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6698 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx      292 b- defN 24-May-16 08:05 alq-0.0.2.data/scripts/alq
+Zip file size: 6769 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx      292 b- defN 24-May-22 07:06 alq-0.0.3.data/scripts/alq
 -rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 02:29 subfunctions/__init__.py
 -rw-r--r--  2.0 unx     2177 b- defN 24-May-13 08:50 subfunctions/configuration.py
--rw-r--r--  2.0 unx     3330 b- defN 24-May-16 08:00 subfunctions/fileSystem.py
--rw-r--r--  2.0 unx     9806 b- defN 24-May-16 07:34 subfunctions/owncloud.py
--rw-r--r--  2.0 unx      217 b- defN 24-May-16 08:05 alq-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 08:05 alq-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 24-May-16 08:05 alq-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      691 b- defN 24-May-16 08:05 alq-0.0.2.dist-info/RECORD
-9 files, 16618 bytes uncompressed, 5510 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx     3490 b- defN 24-May-22 07:01 subfunctions/fileSystem.py
+-rw-r--r--  2.0 unx     9877 b- defN 24-May-22 07:05 subfunctions/owncloud.py
+-rw-r--r--  2.0 unx      217 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      691 b- defN 24-May-22 07:06 alq-0.0.3.dist-info/RECORD
+9 files, 16849 bytes uncompressed, 5581 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: alq-0.0.2.data/scripts/alq
+Filename: alq-0.0.3.data/scripts/alq
 Comment: 
 
 Filename: subfunctions/__init__.py
 Comment: 
 
 Filename: subfunctions/configuration.py
 Comment: 
 
 Filename: subfunctions/fileSystem.py
 Comment: 
 
 Filename: subfunctions/owncloud.py
 Comment: 
 
-Filename: alq-0.0.2.dist-info/METADATA
+Filename: alq-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: alq-0.0.2.dist-info/WHEEL
+Filename: alq-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: alq-0.0.2.dist-info/top_level.txt
+Filename: alq-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: alq-0.0.2.dist-info/RECORD
+Filename: alq-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## subfunctions/fileSystem.py

```diff
@@ -71,18 +71,21 @@
         localTag = f"{mid}_{cwd}" 
         tag = None
         for syncTag in conf['syncTags']:
             if localTag in conf['syncTags'][syncTag]['pcdir']:
                 tag = syncTag 
                 break 
         if tag is None:
-            print("This is the first sync in this dir. Which of the following target do you want to link?")
-            for syncTag in conf['syncTags']:
-                print(f" {syncTag} ") 
-            tag = input("Please type the syncTag name. If you type a new one that is not in the list, a new point will be created for you.")
+            if len(conf['syncTags']) >0:
+                print("This is the first sync in this dir. Which of the following target do you want to link?")
+                for syncTag in conf['syncTags']:
+                    print(f" * {syncTag} ") 
+                tag = input("Please type the syncTag name. If you type a new one that is not in the list, a new point will be created for you.\n")
+            else:
+                tag = input("Please type a new name for recording this sync.\n")
         remotePath = self._ALQ_RemoteSync + "/" + tag 
         if tag not in conf['syncTags']:
             conf['syncTags'][tag] = { 'pcdir':[] } 
             self._mkdirsIfNotExist( remotePath ) 
         if localTag not in conf['syncTags'][tag]['pcdir']:
             conf['syncTags'][tag]['pcdir'].append(localTag) 
         self._setConfigDict(conf)
```

## subfunctions/owncloud.py

```diff
@@ -184,18 +184,16 @@
     #         temp_file_path = os.path.join(temp_dir, metaFileName)
     #         with open(temp_file_path, 'w') as temp_file:
     #             temp_file.write(sharedURL)
     #         oc = Client2.from_public_link(metaDir)
     #         oc.drop_file(temp_file_path)
 
     def sendshare(self,localPath:str):
-        '''
-        share a local file or directory to public, other can download it by:
-           getsharefrom <username> 
-        '''
+        """ <localPath>,  share a local file or directory to public, other can download it by: getsharefrom <username> 
+        """        
         username,password = self._getUserPass() 
         if not ( username is not None and password is not None  ):
             raise Exception('owncloud is not set')
         lp = os.path.abspath(localPath) 
         basename = os.path.basename(lp)
         poc = self._getPublicDirClient()
         if os.path.isdir( lp ):
@@ -217,14 +215,15 @@
             # single file 
             poc.drop_file(lp) 
             poc.move( f"{basename}" , f"share_{username}_data" )
         poc.put_file_contents(remote_path=f"share_{username}_meta.txt",data=json.dumps(meta))
         return "done!"
 
     def getsharefrom(self,username:str):
+        '''<username>, get a shared resource from the <username>'''
         poc = self._getPublicDirClient() 
         metaFile = f"share_{username}_meta.txt" 
         dataFile = f"share_{username}_data"
         meta = json.loads(poc.get_file_contents(metaFile).decode())
         if meta['isdir']:
             localPath = os.path.join( os.getcwd(),meta['filename'] ) 
             with tempfile.TemporaryDirectory() as temp_dir:
```

