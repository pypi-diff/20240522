# Comparing `tmp/halchat-0.0.2.tar.gz` & `tmp/halchat-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halchat-0.0.2.tar", last modified: Mon May 20 17:53:07 2024, max compression
+gzip compressed data, was "halchat-0.0.2.1.tar", last modified: Wed May 22 15:30:02 2024, max compression
```

## Comparing `halchat-0.0.2.tar` & `halchat-0.0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.148060 halchat-0.0.2/
--rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      480 2024-05-20 17:53:07.147060 halchat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.2/README.md
--rw-rw-rw-   0        0        0      423 2024-05-19 12:45:04.000000 halchat-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 17:53:07.148060 halchat-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.135555 halchat-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-20 17:53:07.146061 halchat-0.0.2/src/HalChat.egg-info/
--rw-rw-rw-   0        0        0      480 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 17:53:07.000000 halchat-0.0.2/src/HalChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8037 2024-05-19 13:07:56.000000 halchat-0.0.2/src/HalChatAPI.py
--rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.2/src/HalEncryption.py
--rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.2/src/HalHash.py
--rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:30:02.185061 halchat-0.0.2.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      482 2024-05-22 15:30:02.184059 halchat-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.2.1/README.md
+-rw-rw-rw-   0        0        0      425 2024-05-22 15:25:00.000000 halchat-0.0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:30:02.185061 halchat-0.0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 15:30:02.175552 halchat-0.0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:30:02.184059 halchat-0.0.2.1/src/HalChat.egg-info/
+-rw-rw-rw-   0        0        0      482 2024-05-22 15:30:02.000000 halchat-0.0.2.1/src/HalChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-22 15:30:02.000000 halchat-0.0.2.1/src/HalChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:30:02.000000 halchat-0.0.2.1/src/HalChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:30:02.000000 halchat-0.0.2.1/src/HalChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8066 2024-05-22 15:29:36.000000 halchat-0.0.2.1/src/HalChatAPI.py
+-rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.2.1/src/HalEncryption.py
+-rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.2.1/src/HalHash.py
+-rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.2.1/src/__init__.py
```

### Comparing `halchat-0.0.2/LICENSE` & `halchat-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `halchat-0.0.2/src/HalChatAPI.py` & `halchat-0.0.2.1/src/HalChatAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,21 +67,21 @@
                     self.chats[str(msg['fromChat'])][0]=msg['uid']
                     if str(msg['fromChat']) in self.chatsPasswords:
                         msg['message']=self.he.decodeByHash(bytes.fromhex(msg['message']),self.chatsPasswords[str(msg['fromChat'])]+msg['encryptId'],10).decode("utf-8")
                     self.run_event("onNewMessage",[msg,str(msg['fromChat']) in self.chatsPasswords])
                 for chat in data['newChats']:
                     if self.auto_join_chats:
                         self.joinChatByInviteId(chat['inviteId'])
-                    self.chats[str(chat['chatId'])]=chat['maxLastMessage']
+                    self.chats[str(chat['chatId'])]=[chat['maxLastMessage'],chat['maxLastAction']]
                     self.run_event("onNewChat",[chat['chatId'],chat['inviteId']])
                 for v in data['events']:
                     self.chats[str(v['fromChat'])][1]=v['uid']
                     if v['type']==2:
                         if str(v['fromChat']) in self.requested_passwords:
-                            passw=self.requested_passwords[v['fromChat']].decrypt(base64.b64decode(v['data'])).decode('utf-8')
+                            passw=self.requested_passwords[str(v['fromChat'])].decrypt(base64.b64decode(v['data'])).decode('utf-8')
                             self.addChatPassword(v['fromChat'],passw)
                             self.savePasswords()
                             v['data']=passw
                             del self.requested_passwords[v['fromChat']]
                         self.run_event('onReceivePassword',[v['fromChat'],v['data']])
                     elif v['type']==6:
                         self.run_event('onClickButton',[v['fromChat'],v['fromId'],v['fromMsg'],v['data']])
```

### Comparing `halchat-0.0.2/src/HalEncryption.py` & `halchat-0.0.2.1/src/HalEncryption.py`

 * *Files identical despite different names*

### Comparing `halchat-0.0.2/src/HalHash.py` & `halchat-0.0.2.1/src/HalHash.py`

 * *Files identical despite different names*

