# Comparing `tmp/nonebot_adapter_tailchat-0.1.0b8.tar.gz` & `tmp/nonebot_adapter_tailchat-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b8.tar", max compression
+gzip compressed data, was "nonebot_adapter_tailchat-0.1.0b9.tar", max compression
```

## Comparing `nonebot_adapter_tailchat-0.1.0b8.tar` & `nonebot_adapter_tailchat-0.1.0b9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11335 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/LICENSE
--rw-r--r--   0        0        0     1786 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/README.md
--rw-r--r--   0        0        0      260 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/__init__.py
--rw-r--r--   0        0        0     7279 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/adapter.py
--rw-r--r--   0        0        0    24793 2024-05-14 11:19:49.524181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/api.py
--rw-r--r--   0        0        0     8185 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bbcode.py
--rw-r--r--   0        0        0     4249 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bot.py
--rw-r--r--   0        0        0      675 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/config.py
--rw-r--r--   0        0        0      158 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/const.py
--rw-r--r--   0        0        0    14519 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/event.py
--rw-r--r--   0        0        0     1517 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/exception.py
--rw-r--r--   0        0        0    16040 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/message.py
--rw-r--r--   0        0        0     5976 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/model.py
--rw-r--r--   0        0        0      374 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/permission.py
--rw-r--r--   0        0        0      470 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/rule.py
--rw-r--r--   0        0        0     2103 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/util.py
--rw-r--r--   0        0        0     1423 2024-05-14 11:19:49.528181 nonebot_adapter_tailchat-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-05-15 13:46:58.125391 nonebot_adapter_tailchat-0.1.0b9/LICENSE
+-rw-r--r--   0        0        0     1786 2024-05-15 13:46:58.125391 nonebot_adapter_tailchat-0.1.0b9/README.md
+-rw-r--r--   0        0        0      260 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/__init__.py
+-rw-r--r--   0        0        0     7240 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/adapter.py
+-rw-r--r--   0        0        0    26323 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/api.py
+-rw-r--r--   0        0        0     8403 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/bbcode.py
+-rw-r--r--   0        0        0     4701 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/bot.py
+-rw-r--r--   0        0        0      675 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/config.py
+-rw-r--r--   0        0        0      158 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/const.py
+-rw-r--r--   0        0        0    14881 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/event.py
+-rw-r--r--   0        0        0     1517 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/exception.py
+-rw-r--r--   0        0        0    16374 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/message.py
+-rw-r--r--   0        0        0     6172 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/model.py
+-rw-r--r--   0        0        0      374 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/permission.py
+-rw-r--r--   0        0        0      470 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/rule.py
+-rw-r--r--   0        0        0     2103 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/util.py
+-rw-r--r--   0        0        0     1423 2024-05-15 13:46:58.129391 nonebot_adapter_tailchat-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 nonebot_adapter_tailchat-0.1.0b9/PKG-INFO
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/LICENSE` & `nonebot_adapter_tailchat-0.1.0b9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b8/README.md` & `nonebot_adapter_tailchat-0.1.0b9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/adapter.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,18 +96,17 @@
         bot = Bot(self, bot_info.appId, bot_info)
         bot.sio.on("*", partial(self._handle_event, bot))
         bot.sio.on("disconnect", _check)
         while True:
             try:
                 await wait_for(bot.login(bot.base_info.jwt), self.adapter_config.time_out)
                 await wait_for(self._connect_bot(bot), self.adapter_config.time_out)
-                await bot.update_info(bot.base_info.jwt)
                 self._bot_connect(bot)
                 connected = True
-                await gather(bot.sio.wait(), _wait())
+                await gather(bot.sio.wait(), _wait(), bot.keep_alive())
             except DisconnectException:
                 log.warning(f"Bot {escape_tag(str(bot))} socketio connection closed")
             except AsyncTimeoutError:
                 log.warning(f"Bot {escape_tag(str(bot))} connection timeout")
             except ConnectionException as e:
                 log.error(f"Error when chat.converse.findAndJoinRoom: {repr(e)}")
             except Exception as e:
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/api.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,21 @@
 from pydantic import TypeAdapter
 
 from .const import Optional, Undefined
 from .model import (
     Ack,
     AddFriendRequestRet,
     BaseGroupInfo,
+    BotInfoRet,
     ClientConfig,
     ConverseInfo,
     FileInfo,
     FindAndJoinRoomRet,
     GroupAndPanelIds,
+    GroupDataRet,
     GroupInfo,
     Health,
     InviteCodeInfo,
     LastMessages,
     MessageRet,
     Panel,
     TemporaryUserInfo,
@@ -41,18 +43,18 @@
         return await self.call_api("openapi.app.get", appId=appId)
 
     async def whoami(self) -> Whoami:
         """获取当前账户信息"""
         return TypeAdapter(Whoami).validate_python(await self.call_api("user.whoami"))
 
     async def getFile(self, *, objectName: str):
-        """获取文件url (但是参数不知道填啥)"""
+        """获取客户端的信息"""
         return await self.call_api("file.get", objectName=objectName)
 
-    async def ackInbox(self, *, inboxItemIds: list[str]):
+    async def ackInbox(self, *, inboxItemIds: list[str]) -> bool:
         """标记消息为已读"""
         return await self.call_api("chat.inbox.ack", inboxItemIds=inboxItemIds)
 
     async def allInbox(self) -> MessageRet:
         """获取用户收件箱中所有内容"""
         return TypeAdapter(MessageRet).validate_python(await self.call_api("chat.inbox.all"))
 
@@ -66,44 +68,49 @@
         password: str,
         email: Optional[str] = Undefined,
         avatar: Optional[str] = Undefined,
         emailOTP: Optional[str] = Undefined,
         nickname: Optional[str] = Undefined,
         username: Optional[str] = Undefined,
     ):
+        """用户注册"""
         return await self.call_api(
             "user.register",
             email=email,
             avatar=avatar,
             emailOTP=emailOTP,
             nickname=nickname,
             password=password,
             username=username,
         )
 
     async def saveFile(self):
+        """通过文件流存储到本地"""
         return await self.call_api("file.save")
 
     async def statFile(self, *, objectName: str):
+        """获取客户端的信息"""
         return await self.call_api("file.stat", objectName=objectName)
 
     async def upload(self, *, file: bytes) -> FileInfo:
         """上传文件"""
         return TypeAdapter(FileInfo).validate_python(
             await self.call_api("upload", file=file, use_api_=False, use_http_=True, use_sio_=False)
         )
 
-    async def authToken(self, *, appId: str, token: str, capability: Optional[list[str]] = Undefined):
+    async def authToken(self, *, appId: str, token: str, capability: Optional[list[str]] = Undefined) -> bool:
         """验证token"""
         return await self.call_api("openapi.app.authToken", appId=appId, token=token, capability=capability)
 
     async def createApp(self, *, appDesc: str, appIcon: str, appName: str):
+        """创建一个第三方应用"""
         return await self.call_api("openapi.app.create", appDesc=appDesc, appIcon=appIcon, appName=appName)
 
-    async def deleteApp(self, *, appId: str):
+    async def deleteApp(self, *, appId: str) -> bool:
+        """删除开放平台应用"""
         return await self.call_api("openapi.app.delete", appId=appId)
 
     async def loginUser(
         self, *, password: str, email: Optional[str] = Undefined, username: Optional[str] = Undefined
     ) -> TokenInfo:
         """标准登录API"""
         return TypeAdapter(TokenInfo).validate_python(
@@ -115,42 +122,46 @@
         return await self.call_api("group.quitGroup", groupId=groupId)
 
     async def updateAck(self, *, converseId: str, lastMessageId: str):
         """更新用户在会话中已读的最后一条消息"""
         return await self.call_api("chat.ack.update", converseId=converseId, lastMessageId=lastMessageId)
 
     async def addBotUser(self, *, appId: str, groupId: str):
+        """在群组中添加机器人用户"""
         return await self.call_api("openapi.integration.addBotUser", appId=appId, groupId=groupId)
 
     async def addRequest(self, *, to: str, message: Optional[str] = Undefined) -> AddFriendRequestRet:
         """发送好友申请(message好像没用, 请求处理界面看不到message).不存在的id也能发送成功.不符合格式的id会报错."""
         return TypeAdapter(AddFriendRequestRet).validate_python(
             await self.call_api("friend.request.add", to=to, message=message)
         )
 
-    async def allRelated(self):
-        return await self.call_api("friend.request.allRelated")
+    async def allRelated(self) -> list[AddFriendRequestRet]:
+        """所有与自己相关的好友请求, 包括自己发出的和别人发给自己的"""
+        return TypeAdapter(list[AddFriendRequestRet]).validate_python(await self.call_api("friend.request.allRelated"))
 
-    async def clearInbox(self):
+    async def clearInbox(self) -> bool:
         """清空所有的收件箱内容"""
         return await self.call_api("chat.inbox.clear")
 
-    async def setAppInfo(self, *, appId: str, fieldName: str, fieldValue: str):
+    async def setAppInfo(self, *, appId: str, fieldValue: str, fieldName: Literal["appName", "appDesc", "appIcon"]):
+        """修改应用信息"""
         return await self.call_api("openapi.app.setAppInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue)
 
     async def getMessage(self, *, messageId: str) -> MessageRet:
         """获取消息"""
         return TypeAdapter(MessageRet).validate_python(
             await self.call_api("chat.message.getMessage", messageId=messageId)
         )
 
     async def addConverse(self, *, converseId: str):
+        """加入或创建会话"""
         return await self.call_api("user.dmlist.addConverse", converseId=converseId)
 
-    async def addReaction(self, *, emoji: str, messageId: str):
+    async def addReaction(self, *, emoji: str, messageId: str) -> bool:
         """添加消息表情"""
         return await self.call_api("chat.message.addReaction", emoji=emoji, messageId=messageId)
 
     async def applyInvite(self, *, code: str):
         """通过邀请码加群"""
         return await self.call_api("group.invite.applyInvite", code=code)
 
@@ -186,36 +197,39 @@
                 content=content,
                 groupId=groupId,
                 converseId=converseId,
             )
         )
 
     async def verifyEmail(self, *, email: str):
+        """验证用户邮箱, 会往邮箱发送一个 OTP 作为唯一标识
+        需要在注册的时候带上"""
         return await self.call_api("user.verifyEmail", email=email)
 
     async def configClient(self) -> ClientConfig:
         """获取客户端配置"""
         return TypeAdapter(ClientConfig).validate_python(await self.call_api("config.client"))
 
     async def deleteInvite(self, *, groupId: str, inviteId: str):
         """删除邀请码"""
         return await self.call_api("group.invite.deleteInvite", groupId=groupId, inviteId=inviteId)
 
-    async def getGroupData(self, *, name: str, groupId: str):
+    async def getGroupData(self, *, name: str, groupId: str) -> GroupDataRet:
         return await self.call_api("group.extra.getGroupData", name=name, groupId=groupId)
 
-    async def getPanelData(self, *, name: str, groupId: str, panelId: str):
+    async def getPanelData(self, *, name: str, groupId: str, panelId: str) -> dict:
         """获取面板数据"""
         return await self.call_api("group.extra.getPanelData", name=name, groupId=groupId, panelId=panelId)
 
     async def isGroupOwner(self, *, groupId: str):
         """是否为创建者"""
         return await self.call_api("group.isGroupOwner", groupId=groupId)
 
     async def listRegistry(self):
+        """getPluginList"""
         return await self.call_api("plugin.registry.list")
 
     async def removeFriend(self, *, friendUserId: str):
         """移除单项好友关系"""
         return await self.call_api("friend.removeFriend", friendUserId=friendUserId)
 
     async def resolveToken(self, *, token: str) -> TokenInfo:
@@ -226,90 +240,97 @@
         """接受好友请求"""
         return await self.call_api("friend.request.accept", requestId=requestId)
 
     async def cancelRequest(self, *, requestId: str):
         """撤销申请好友请求. 填不存在的requestId会报错, 不符合格式的也会报错"""
         return await self.call_api("friend.request.cancel", requestId=requestId)
 
-    async def checkIsFriend(self, *, targetId: str):
+    async def checkIsFriend(self, *, targetId: str) -> bool:
         """检查对方是否为自己好友"""
         return await self.call_api("friend.checkIsFriend", targetId=targetId)
 
-    async def deleteMessage(self, *, messageId: str):
+    async def deleteMessage(self, *, messageId: str) -> bool:
         """删除消息"""
         return await self.call_api("chat.message.deleteMessage", messageId=messageId)
 
     async def gatewayHealth(self) -> Health:
         """获取网关健康状态"""
         return TypeAdapter(Health).validate_python(await self.call_api("gateway.health"))
 
-    async def getAllFriends(self):
+    async def getAllFriends(self) -> list[dict[str, str]]:
         """获取全部好友的ID
         [{'id': '***'}]"""
         return await self.call_api("friend.getAllFriends")
 
     async def getUserGroups(self) -> list[GroupInfo]:
         """获取用户的群组"""
         return TypeAdapter(list[GroupInfo]).validate_python(await self.call_api("group.getUserGroups"))
 
     async def recallMessage(self, *, messageId: str) -> MessageRet:
         """撤回消息, 大于15分钟的消息无法撤回, 会报错"""
         return TypeAdapter(MessageRet).validate_python(
             await self.call_api("chat.message.recallMessage", messageId=messageId)
         )
 
-    async def resetPassword(self, *, otp: str, email: str, password: str):
+    async def resetPassword(self, *, otp: str, email: str, password: str) -> bool:
+        """重置密码"""
         return await self.call_api("user.resetPassword", otp=otp, email=email, password=password)
 
-    async def saveGroupData(self, *, data: str, name: str, groupId: str):
+    async def saveGroupData(self, *, data: str, name: str, groupId: str) -> bool:
         return await self.call_api("group.extra.saveGroupData", data=data, name=name, groupId=groupId)
 
-    async def savePanelData(self, *, data: str, name: str, groupId: str, panelId: str):
+    async def savePanelData(self, *, data: str, name: str, groupId: str, panelId: str) -> bool:
         """保存面板数据"""
         return await self.call_api("group.extra.savePanelData", data=data, name=name, groupId=groupId, panelId=panelId)
 
     async def searchMessage(
         self, *, text: str, converseId: str, groupId: Optional[str] = Undefined
     ) -> list[MessageRet]:
         """搜索消息"""
         return TypeAdapter(list[MessageRet]).validate_python(
             await self.call_api("chat.message.searchMessage", text=text, groupId=groupId, converseId=converseId)
         )
 
     async def setAppBotInfo(self, *, appId: str, fieldName: str, fieldValue: Any):
+        """设置Bot的设置信息"""
         return await self.call_api("openapi.app.setAppBotInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue)
 
     async def forgetPassword(self, *, email: str):
+        """忘记密码
+        流程: 发送一个链接到远程，点开后可以直接重置密码"""
         return await self.call_api("user.forgetPassword", email=email)
 
     async def getAllConverse(self) -> list[str]:
         """获取所有会话"""
-        return TypeAdapter(list[str]).validate_python(await self.call_api("user.dmlist.getAllConverse"))
+        return await self.call_api("user.dmlist.getAllConverse")
 
-    async def getPermissions(self, *, groupId: str):
+    async def getPermissions(self, *, groupId: str) -> list[str]:
+        """获取群组成员权限(对外)"""
         return await self.call_api("group.getPermissions", groupId=groupId)
 
     async def modifyPassword(self, *, newPassword: str, oldPassword: str):
         """修改密码(好像没啥用)"""
         return await self.call_api("user.modifyPassword", newPassword=newPassword, oldPassword=oldPassword)
 
-    async def removeConverse(self, *, converseId: str):
-        """删除会话\n{"modifiedCount":1}"""
+    async def removeConverse(self, *, converseId: str) -> dict:
+        """删除会话
+        {"modifiedCount":1}"""
         return await self.call_api("user.dmlist.removeConverse", converseId=converseId)
 
-    async def removeReaction(self, *, emoji: str, messageId: str):
+    async def removeReaction(self, *, emoji: str, messageId: str) -> bool:
         """删除消息表情"""
         return await self.call_api("chat.message.removeReaction", emoji=emoji, messageId=messageId)
 
     async def checkTokenValid(self, *, token: str):
+        """检查授权是否可用"""
         return await self.call_api("user.checkTokenValid", token=token)
 
     async def checkUserOnline(self, *, userIds: list[str]) -> list[bool]:
         """检查用户是否在线"""
-        return TypeAdapter(list[bool]).validate_python(await self.call_api("gateway.checkUserOnline", userIds=userIds))
+        return await self.call_api("gateway.checkUserOnline", userIds=userIds)
 
     async def createGroupRole(self, *, groupId: str, roleName: str, permissions: list[str]) -> GroupInfo:
         """创建群用户组"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.createGroupRole", groupId=groupId, roleName=roleName, permissions=permissions)
         )
 
@@ -317,15 +338,15 @@
         """删除群用户组"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.deleteGroupRole", roleId=roleId, groupId=groupId)
         )
 
     async def editGroupInvite(
         self, *, code: str, groupId: str, expireAt: Optional[int] = Undefined, usageLimit: Optional[int] = Undefined
-    ):
+    ) -> bool:
         """编辑群组邀请码"""
         return await self.call_api(
             "group.invite.editGroupInvite", code=code, groupId=groupId, expireAt=expireAt, usageLimit=usageLimit
         )
 
     async def ensurePluginBot(self, *, botId: str, nickname: str, avatar: Optional[str] = Undefined):
         return await self.call_api("user.ensurePluginBot", botId=botId, avatar=avatar, nickname=nickname)
@@ -334,32 +355,34 @@
         """查找用户相关的所有会话并加入房间"""
         return TypeAdapter(FindAndJoinRoomRet).validate_python(await self.call_api("chat.converse.findAndJoinRoom"))
 
     async def getUserInfoList(self, *, userIds: list[str]) -> list[UserInfo]:
         """获取多个用户信息"""
         return TypeAdapter(list[UserInfo]).validate_python(await self.call_api("user.getUserInfoList", userIds=userIds))
 
-    async def getUserSettings(self):
+    async def getUserSettings(self) -> dict:
         """获取用户设置"""
         return await self.call_api("user.getUserSettings")
 
-    async def muteGroupMember(self, *, muteMs: int, groupId: str, memberId: str):
+    async def muteGroupMember(self, *, muteMs: int, groupId: str, memberId: str) -> bool:
         """禁言群成员"""
         return await self.call_api("group.muteGroupMember", muteMs=muteMs, groupId=groupId, memberId=memberId)
 
     async def setAppOAuthInfo(self, *, appId: str, fieldName: str, fieldValue: Any):
+        """设置OAuth的设置信息"""
         return await self.call_api(
             "openapi.app.setAppOAuthInfo", appId=appId, fieldName=fieldName, fieldValue=fieldValue
         )
 
-    async def setUserSettings(self, *, settings: dict):
+    async def setUserSettings(self, *, settings: dict) -> dict:
         """修改用户设置"""
         return await self.call_api("user.setUserSettings", settings=settings)
 
     async def updateUserExtra(self, *, fieldName: str, fieldValue: Any):
+        """修改用户额外数据"""
         return await self.call_api("user.updateUserExtra", fieldName=fieldName, fieldValue=fieldValue)
 
     async def updateUserField(self, *, fieldName: str, fieldValue: Any) -> UserInfo:
         """更改用户信息"""
         return TypeAdapter(UserInfo).validate_python(
             await self.call_api("user.updateUserField", fieldName=fieldName, fieldValue=fieldValue)
         )
@@ -376,15 +399,15 @@
         name: str,
         type_: int,
         groupId: str,
         meta: Optional[dict] = Undefined,
         parentId: Optional[str] = Undefined,
         provider: Optional[str] = Undefined,
         pluginPanelName: Optional[str] = Undefined,
-    ):
+    ) -> dict:
         """创建群组面板"""
         return await self.call_api(
             "group.createGroupPanel",
             name=name,
             meta=meta,
             type=type_,
             groupId=groupId,
@@ -395,29 +418,34 @@
 
     async def deleteGroupPanel(self, *, groupId: str, panelId: str) -> GroupInfo:
         """删除群组面板"""
         return TypeAdapter(GroupInfo).validate_python(
             await self.call_api("group.deleteGroupPanel", groupId=groupId, panelId=panelId)
         )
 
-    async def ensureOpenapiBot(self, *, botId: str, nickname: str, avatar: Optional[str] = Undefined):
-        return await self.call_api("user.ensureOpenapiBot", botId=botId, avatar=avatar, nickname=nickname)
+    async def ensureOpenapiBot(self, *, botId: str, nickname: str, avatar: Optional[str] = Undefined) -> BotInfoRet:
+        """确保第三方开放平台机器人存在(没有则自动创建)"""
+        return TypeAdapter(BotInfoRet).validate_python(
+            await self.call_api("user.ensureOpenapiBot", botId=botId, avatar=avatar, nickname=nickname)
+        )
 
     async def findConverseInfo(self, *, converseId: str) -> ConverseInfo:
         """获取会话信息"""
         return TypeAdapter(ConverseInfo).validate_python(
             await self.call_api("chat.converse.findConverseInfo", converseId=converseId)
         )
 
     async def findInviteByCode(self, *, code: str) -> Optional[InviteCodeInfo]:
+        """通过邀请码查找群组邀请信息"""
         return TypeAdapter(Optional[InviteCodeInfo]).validate_python(
             await self.call_api("group.invite.findInviteByCode", code=code)
         )
 
     async def findOpenapiBotId(self, *, email: str):
+        """根据用户邮箱获取开放平台机器人id"""
         return await self.call_api("user.findOpenapiBotId", email=email)
 
     async def modifyGroupPanel(
         self,
         *,
         name: str,
         type_: int,
@@ -425,28 +453,30 @@
         panelId: str,
         meta: Optional[dict] = Undefined,
         provider: Optional[str] = Undefined,
         permissionMap: Optional[dict] = Undefined,
         pluginPanelName: Optional[str] = Undefined,
         fallbackPermissions: Optional[list[str]] = Undefined,
     ):
+        """修改群组面板"""
         return await self.call_api(
             "group.modifyGroupPanel",
             meta=meta,
             name=name,
             type=type_,
             groupId=groupId,
             panelId=panelId,
             provider=provider,
             permissionMap=permissionMap,
             pluginPanelName=pluginPanelName,
             fallbackPermissions=fallbackPermissions,
         )
 
     async def setAppCapability(self, *, appId: str, capability: list[str]):
+        """设置应用开放的能力"""
         return await self.call_api("openapi.app.setAppCapability", appId=appId, capability=capability)
 
     async def updateGroupField(self, *, groupId: str, fieldName: str, fieldValue: Any):
         """更新群组字段"""
         return await self.call_api(
             "group.updateGroupField", groupId=groupId, fieldName=fieldName, fieldValue=fieldValue
         )
@@ -463,15 +493,15 @@
 
     async def getGroupBasicInfo(self, *, groupId: str) -> BaseGroupInfo:
         """获取群基本消息"""
         return TypeAdapter(BaseGroupInfo).validate_python(
             await self.call_api("group.getGroupBasicInfo", groupId=groupId)
         )
 
-    async def setFriendNickname(self, *, nickname: str, targetId: str):
+    async def setFriendNickname(self, *, nickname: str, targetId: str) -> bool:
         """设置好友昵称"""
         return await self.call_api("friend.setFriendNickname", nickname=nickname, targetId=targetId)
 
     async def updateGroupConfig(self, *, groupId: str, configName: str, configValue: Any):
         """更新群组配置"""
         return await self.call_api(
             "group.updateGroupConfig", groupId=groupId, configName=configName, configValue=configValue
@@ -482,14 +512,15 @@
         *,
         email: str,
         userId: str,
         password: str,
         emailOTP: Optional[str] = Undefined,
         username: Optional[str] = Undefined,
     ):
+        """认领临时用户"""
         return await self.call_api(
             "user.claimTemporaryUser",
             email=email,
             userId=userId,
             emailOTP=emailOTP,
             password=password,
             username=username,
@@ -545,16 +576,16 @@
         """移除群用户组成员"""
         return await self.call_api("group.removeGroupMemberRoles", roles=roles, groupId=groupId, memberIds=memberIds)
 
     async def appendDMConverseMembers(self, *, converseId: str, memberIds: list[str]):
         """在多人会话中添加成员"""
         return await self.call_api("chat.converse.appendDMConverseMembers", memberIds=memberIds, converseId=converseId)
 
-    async def getGroupLobbyConverseId(self, *, groupId: str):
-        """不知道啥作用, 但是返回的是converseId"""
+    async def getGroupLobbyConverseId(self, *, groupId: str) -> str:
+        """获取群组大厅的会话ID"""
         return await self.call_api("group.getGroupLobbyConverseId", groupId=groupId)
 
     async def searchUserWithUniqueName(self, *, uniqueName: str) -> Optional[UserInfo]:
         """根据唯一名搜索用户"""
         return TypeAdapter(Optional[UserInfo]).validate_python(
             await self.call_api("user.searchUserWithUniqueName", uniqueName=uniqueName)
         )
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bbcode.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/bbcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from .message import BBCODE, MessageSegment
 
 
 class Parser:
     def __init__(
         self,
         seg: type["MessageSegment"],
-        tags: dict[str, type["BBCODE"]],
+        tags: dict[str, Union[type["BBCODE"], dict[str, "BBCODE"]]],
         drop_unrecognized=False,
         max_tag_depth=None,
     ):
         self.seg = seg
         self.tag_opener = "["
         self.tag_closer = "]"
         self.tags = tags
@@ -157,15 +157,19 @@
                                         i.extend(tag_start)
                                 else:  # 是标签
                                     _tag_name = i[1]
                                     if _tag_name == tag_name:
                                         tokens.remove(i)
                                         break
                         else:
-                            seg = self.seg.build("", [self.tags[tag_name]], opts)
+                            seg = self.seg.build(
+                                "",
+                                [self.tags["card"][opts.get("type")] if tag_name == "card" else self.tags[tag_name]],
+                                opts,
+                            )
                             tags[tag_name].append(seg)
                             tokens.append((seg, tag_name, tag))
                     elif valid and self.drop_unrecognized and tag_name not in self.tags:
                         # If we found a valid (but unrecognized) tag and self.drop_unrecognized is True, just drop it.
                         pass
                     else:
                         tokens.append(self.seg.text(tag))
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/bot.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/bot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from asyncio import sleep
 from base64 import urlsafe_b64decode
 from functools import wraps
 from hashlib import md5
 from json import loads
 from time import time
 from typing import TYPE_CHECKING, Optional, Union
 
@@ -14,14 +15,15 @@
 from .message import Message, MessageSegment
 from .model import (
     BaseBotInfo,
     JwtPayload,
     MessageRet,
     TokenInfo,
 )
+from .util import log
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 def _with_update_info(func):
     @wraps(func)
@@ -101,26 +103,37 @@
     async def loginBot(self, *, appId: str, appSecret: str) -> BaseBotInfo:
         return TypeAdapter(BaseBotInfo).validate_python(
             await self.call_api(
                 "openapi.bot.login", token=self.md5(appId + appSecret), appId=appId, use_http_=True, use_sio_=False
             )
         )
 
+    @_with_update_info
     async def login(self, jwt: Optional[str] = None):
         if jwt:
             jwt_data = self.decode_jwt(jwt)[1]
-            if jwt_data.exp.timestamp() > time():
+            if (jwt_data.exp.timestamp() - time()) > 3600:
                 self.base_info.jwt = jwt
                 return
         if self.base_info.appId and self.base_info.appSecret:
             data = await self.loginBot(appId=self.base_info.appId, appSecret=self.base_info.appSecret)
             self.base_info.jwt = data.jwt
             return
         raise ValueError("必须提供jwt或appId和appSecret")
 
+    async def keep_alive(self):
+        try:
+            jwt_data = self.decode_jwt(self.base_info.jwt)[1]
+            if (jwt_data.exp.timestamp() - time()) < 3600:
+                await self.login()
+            log.debug(f"{self} | keep alive")
+            await sleep(60)
+        except Exception as e:
+            log.debug(f"{self} | keep alive failed: <r>{e}</r>")
+
     @_with_update_info
     async def updateNickname(self, nickname: str):
         """更新昵称，机器人重登后就失效了"""
         return await self.updateUserField(fieldName="nickname", fieldValue=nickname)
 
     @_with_update_info
     async def updateAvatar(self, avatar: str):
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/config.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/event.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,19 +83,19 @@
             log.debug(f"Event.build error: {e}")
         return event
 
 
 class NoticeEvent(Event, ABC):
     event_type: Literal["notice"] = "notice"
 
-    def get_message(self) -> Message:
-        raise ValueError("Event has no message!")
-
     def get_session_id(self) -> str:
-        raise ValueError("Event has no context!")
+        raise NotImplementedError
+
+    def get_message(self) -> Message:
+        raise NotImplementedError
 
 
 class RequestEvent(Event, ABC):
     event_type: Literal["request"] = "request"
 
     def get_session_id(self) -> str:
         raise ValueError("Event has no context!")
@@ -169,14 +169,25 @@
         raise ValueError(
             f"Event class {event_class} must have a default value or Literal[str] type annotation for `event_name`"
         ) from e  # event_name 必须 有默认值 或 Literal[str] 类型注解
     EVENT_CLASSES[event_name] = event_class
     return event_class
 
 
+def remove_event_class(event_class: type[E]) -> type[E]:
+    if event_class.model_fields["event_type"].default == PydanticUndefined:
+        return event_class
+    try:
+        event_name = getattr(event_class, "event_name", get_args(event_class.__annotations__["event_name"])[0])
+        EVENT_CLASSES.pop(event_name, None)
+        return event_class
+    except:
+        return event_class
+
+
 @register_event_class
 class ClientConfigUpdateEvent(NoticeEvent):
     event_name: Literal["notify:config.updateClientConfig"]
 
     serverName: str
     serverEntryImage: str
     announcement: Union[StaticAnnouncement, Literal[False]]
@@ -448,26 +459,25 @@
 @register_event_class
 class MessageUpdateEvent(DefaultMessageEvent):
     """消息更新事件(撤回消息)"""
 
     event_name: Literal["notify:chat.message.update"]
 
 
-class AtEvent(Event, ABC):
-    event_type: Literal["message"] = "message"
-
-    type: str
-
-    v: int = Field(alias="__v")
+class AtEvent(Event, ABC): ...
 
 
 @register_event_class
-class AtMessageEvent(AtEvent, MessageEvent):
+class AtMessageEvent(MessageEvent, AtEvent):
     event_name: Literal["notify:chat.inbox.append"]
 
+    type: str
+
+    v: int = Field(alias="__v")
+
     id: ObjectId = Field(alias="_id")
     userId: ObjectId
     payload: Union[Payload, Announcement]
     readed: bool
     createdAt: datetime
     updatedAt: datetime
 
@@ -497,16 +507,17 @@
             f"AtMessage {self.payload.messageId} from {self.payload.messageAuthor}"
             + (f"@[群:{self.get_group_id()}]" if self.payload.groupId else "")
             + f" {self.payload.messageSnippet.show()}"
         )
 
 
 @register_event_class
-class AtMessageUpdateEvent(AtEvent, NoticeEvent):
-    """At 消息更新事件"""
+class AtMessageUpdateEvent(NoticeEvent, AtEvent):
+    """At 消息更新事件
+    (目前只有@Bot消息删除会触发)"""
 
     event_name: Literal["notify:chat.inbox.updated"]
 
     @property
     def _is_tome(self) -> bool:
         return True
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/exception.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/message.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 from abc import ABC
 from collections import UserDict, defaultdict, deque
 from collections.abc import Iterable
 from dataclasses import dataclass
 from functools import wraps
 from inspect import isclass
-from typing import Optional, SupportsIndex, TypedDict, TypeVar, Union
+from typing import Final, Optional, SupportsIndex, TypedDict, TypeVar, Union
 
 from nonebot.adapters import (
     Message as BaseMessage,
 )
 from nonebot.adapters import (
     MessageSegment as BaseMessageSegment,
 )
 from typing_extensions import Self, overload
 
 from .bbcode import Parser
 
 BBCODE = TypeVar("BBCODE", bound="BBCode")
-BBCODES: dict[str, type[BBCODE]] = {}
+BBCODES: dict[str, Union[type[BBCODE], dict[str, BBCODE]]] = {}
 RELATION: dict[int, list[BBCODE]] = defaultdict(list)
 
 
 def _register_bbcode(code: Union[int, type[BBCODE]]):
+    def _(bb: type[BBCODE]) -> type[BBCODE]:
+        if bb.tags != {"card"}:
+            for tag in bb.tags:
+                BBCODES[tag] = bb
+            return bb
+        if (card := BBCODES.get("card")) is None:
+            BBCODES["card"] = defaultdict(lambda: Card)  # type: ignore
+        if bb.__name__ != "Card":
+            card[bb.type] = bb
+
     if isinstance(code, int):
 
-        def _(bbcode: type[BBCODE]) -> type[BBCODE]:
+        def __(bbcode: type[BBCODE]) -> type[BBCODE]:
             bbcode.relation = code
-            for tag in bbcode.tags:
-                BBCODES[tag] = bbcode
+            _(bbcode)
             RELATION[code].append(bbcode)
             return bbcode
 
-        return _
-    for tag in code.tags:
-        BBCODES[tag] = code
+        return __
+    _(code)
     _code = min(min(RELATION.keys() or [0]), 0) - 1
     code.relation = _code
     RELATION[_code].append(code)
     return code
 
 
 class Box(TypedDict):
@@ -71,15 +79,17 @@
     @property
     def head(self) -> str:
         return (
             "["
             + (
                 (f"{self.tag}={self.main}" if self.main else self.tag)
                 + " "
-                + " ".join(f"{k}={v}" for k, v in self.items() if v and k in self.keys_ and k not in self.tags)
+                + " ".join(
+                    f"{k}={v}" for k in sorted(self.keys_, reverse=True) if (v := self[k]) and k not in self.tags
+                )
             ).rstrip(" ")
             + "]"
         )
 
     @property
     def tail(self) -> str:
         return f"[/{self.tag}]"
@@ -106,40 +116,39 @@
     def __str__(self):
         return self.head + self.text + self.tail
 
     def __repr__(self):
         return f"{self.tag}({self.data})" if len(self.data) else f"{self.tag}"
 
     def __missing__(self, key) -> None:
-        return None
+        return getattr(self, key, None)
 
 
 @_register_bbcode
 class Markdown(BBCode):
     tags = {"md", "markdown"}
 
 
 @_register_bbcode
 class Card(BBCode):
-    tags = {"card"}
+    tags: Final[set[str]] = {"card"}
     keys_ = {"type", "data"}
 
-    @property
-    def type(self) -> str:
-        return self["type"]
+    type: str
 
     @property
     def card_data(self) -> str:
         return self["data"]
 
 
 @_register_bbcode
-class File(BBCode):
-    tags = {"file"}
-    keys_ = {"url"}
+class File(Card):
+    keys_ = {"type", "url"}
+
+    type: str = "file"
 
     @property
     def url(self) -> str:
         return self["url"]
 
 
 @_register_bbcode
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/model.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import UserDict
 from datetime import datetime as raw_datetime
 from typing import Annotated, Literal, Optional
 
 from pydantic import BaseModel, BeforeValidator, ByteSize, ConfigDict, Field, RootModel
 
 from .config import BotInfo
 from .message import Message, MessageSegment
@@ -316,7 +317,18 @@
 
 
 class FindAndJoinRoomRet(RawModel):
     dmConverseIds: list[ObjectId]
     groupIds: list[ObjectId]
     textPanelIds: list[ObjectId]
     subscribeFeaturePanelIds: list[ObjectId]
+
+
+class BotInfoRet(RawModel):
+    id: ObjectId = Field(alias="_id")
+    email: str
+    nickname: str
+    avatar: str
+
+
+class GroupDataRet(UserDict):
+    data: any
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/nonebot_adapter_tailchat/util.py` & `nonebot_adapter_tailchat-0.1.0b9/nonebot_adapter_tailchat/util.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_tailchat-0.1.0b8/pyproject.toml` & `nonebot_adapter_tailchat-0.1.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-tailchat"
-version = "0.1.0b8"
+version = "0.1.0b9"
 description = "NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2"
 authors = ["eya46 <61458340+eya46@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "nonebot_adapter_tailchat" }]
 keywords = ["bot", "tailchat", "nonebot2"]
 repository = "https://github.com/eya46/nonebot-adapter-tailchat"
```

### Comparing `nonebot_adapter_tailchat-0.1.0b8/PKG-INFO` & `nonebot_adapter_tailchat-0.1.0b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-tailchat
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: NoneBot2 Tailchat 适配器 / Tailchat adapter for nonebot2
 Home-page: https://github.com/eya46/nonebot-adapter-tailchat
 License: Apache-2.0
 Keywords: bot,tailchat,nonebot2
 Author: eya46
 Author-email: 61458340+eya46@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b8 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-tailchat Version: 0.1.0b9 Summary:
 NoneBot2 Tailchat ééå¨ / Tailchat adapter for nonebot2 Home-page: https://
 github.com/eya46/nonebot-adapter-tailchat License: Apache-2.0 Keywords:
 bot,tailchat,nonebot2 Author: eya46 Author-email:
 61458340+eya46@users.noreply.github.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
```

