# Comparing `tmp/pybotx-0.66.0.tar.gz` & `tmp/pybotx-0.66.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx-0.66.0.tar", max compression
+gzip compressed data, was "pybotx-0.66.1.tar", max compression
```

## Comparing `pybotx-0.66.0.tar` & `pybotx-0.66.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0     6078 2024-04-12 07:48:47.896246 pybotx-0.66.0/LICENSE
--rw-r--r--   0        0        0    24562 2024-04-12 07:48:47.896246 pybotx-0.66.0/README.md
--rw-r--r--   0        0        0     7504 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/__init__.py
--rw-r--r--   0        0        0      847 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/async_buffer.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/__init__.py
--rw-r--r--   0        0        0      560 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/__init__.py
--rw-r--r--   0        0        0     1048 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/bot_disabled.py
--rw-r--r--   0        0        0      275 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/command_accepted.py
--rw-r--r--   0        0        0     1185 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/api/responses/unverified_request.py
--rw-r--r--   0        0        0    63728 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/bot.py
--rw-r--r--   0        0        0     1558 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/bot_accounts_storage.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_manager.py
--rw-r--r--   0        0        0     2176 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_memory_repo.py
--rw-r--r--   0        0        0      983 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/callbacks/callback_repo_proto.py
--rw-r--r--   0        0        0      330 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/contextvars.py
--rw-r--r--   0        0        0     1324 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/exceptions.py
--rw-r--r--   0        0        0     2790 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/handler.py
--rw-r--r--   0        0        0    14811 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/handler_collector.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/middlewares/__init__.py
--rw-r--r--   0        0        0     1749 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/middlewares/exception_middleware.py
--rw-r--r--   0        0        0      293 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/bot/testing.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/__init__.py
--rw-r--r--   0        0        0     1617 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/authorized_botx_method.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/__init__.py
--rw-r--r--   0        0        0     1946 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/bot_catalog.py
--rw-r--r--   0        0        0     1235 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/bots_api/get_token.py
--rw-r--r--   0        0        0     6809 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/botx_method.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/__init__.py
--rw-r--r--   0        0        0     2201 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/add_admin.py
--rw-r--r--   0        0        0     1443 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/add_user.py
--rw-r--r--   0        0        0     2985 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/chat_info.py
--rw-r--r--   0        0        0     2177 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/create_chat.py
--rw-r--r--   0        0        0     1415 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/disable_stealth.py
--rw-r--r--   0        0        0     2004 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/list_chats.py
--rw-r--r--   0        0        0     1398 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/pin_message.py
--rw-r--r--   0        0        0     1430 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/remove_user.py
--rw-r--r--   0        0        0     1699 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/set_stealth.py
--rw-r--r--   0        0        0     1354 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/chats_api/unpin_message.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/__init__.py
--rw-r--r--   0        0        0     1355 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/delete_event.py
--rw-r--r--   0        0        0     3295 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/edit_event.py
--rw-r--r--   0        0        0     2324 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/message_status_event.py
--rw-r--r--   0        0        0     3770 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/reply_event.py
--rw-r--r--   0        0        0     1019 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/stop_typing_event.py
--rw-r--r--   0        0        0      955 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/events_api/typing_event.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/__init__.py
--rw-r--r--   0        0        0     1301 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/base.py
--rw-r--r--   0        0        0      889 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/callbacks.py
--rw-r--r--   0        0        0      424 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/chats.py
--rw-r--r--   0        0        0      429 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/common.py
--rw-r--r--   0        0        0      130 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/event.py
--rw-r--r--   0        0        0      289 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/files.py
--rw-r--r--   0        0        0      750 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/http.py
--rw-r--r--   0        0        0      134 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/message.py
--rw-r--r--   0        0        0      378 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/notifications.py
--rw-r--r--   0        0        0      293 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/exceptions/users.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/__init__.py
--rw-r--r--   0        0        0     2093 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/download_file.py
--rw-r--r--   0        0        0     2448 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/files_api/upload_file.py
--rw-r--r--   0        0        0      812 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/get_token.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/mertics_api/__init__.py
--rw-r--r--   0        0        0     1255 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/mertics_api/collect_bot_function.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/__init__.py
--rw-r--r--   0        0        0     5567 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/direct_notification.py
--rw-r--r--   0        0        0     2925 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/notifications_api/internal_bot_notification.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/openid_api/__init__.py
--rw-r--r--   0        0        0     1245 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/openid_api/refresh_access_token.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/__init__.py
--rw-r--r--   0        0        0     2319 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_custom_notification.py
--rw-r--r--   0        0        0     2259 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_event.py
--rw-r--r--   0        0        0     1995 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_manifest.py
--rw-r--r--   0        0        0     1836 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_notification.py
--rw-r--r--   0        0        0     2195 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/smartapps_list.py
--rw-r--r--   0        0        0     1652 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/smartapps_api/upload_file.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/__init__.py
--rw-r--r--   0        0        0     2883 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/add_sticker.py
--rw-r--r--   0        0        0     1689 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/create_sticker_pack.py
--rw-r--r--   0        0        0     1506 2024-04-12 07:48:47.896246 pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker.py
--rw-r--r--   0        0        0     1426 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker_pack.py
--rw-r--r--   0        0        0     1793 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/edit_sticker_pack.py
--rw-r--r--   0        0        0      311 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/exceptions.py
--rw-r--r--   0        0        0     1984 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker.py
--rw-r--r--   0        0        0     1397 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_pack.py
--rw-r--r--   0        0        0     2352 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_packs.py
--rw-r--r--   0        0        0     1321 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/stickers_api/sticker_pack.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/__init__.py
--rw-r--r--   0        0        0     1231 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_email.py
--rw-r--r--   0        0        0     1066 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_emails.py
--rw-r--r--   0        0        0     1257 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_huid.py
--rw-r--r--   0        0        0     1330 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_login.py
--rw-r--r--   0        0        0     1254 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/search_user_by_other_id.py
--rw-r--r--   0        0        0     3020 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/update_user_profile.py
--rw-r--r--   0        0        0     1737 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/user_from_csv.py
--rw-r--r--   0        0        0     2092 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/user_from_search.py
--rw-r--r--   0        0        0     1473 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/client/users_api/users_as_csv.py
--rw-r--r--   0        0        0      421 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/constants.py
--rw-r--r--   0        0        0      221 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/converters.py
--rw-r--r--   0        0        0      789 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/image_validators.py
--rw-r--r--   0        0        0     1341 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/logger.py
--rw-r--r--   0        0        0      648 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/missing.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/__init__.py
--rw-r--r--   0        0        0     2079 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/api_base.py
--rw-r--r--   0        0        0     7256 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/async_files.py
--rw-r--r--   0        0        0    13393 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/attachments.py
--rw-r--r--   0        0        0     2480 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/base_command.py
--rw-r--r--   0        0        0      644 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_account.py
--rw-r--r--   0        0        0      435 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_catalog.py
--rw-r--r--   0        0        0      199 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/bot_sender.py
--rw-r--r--   0        0        0     1635 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/chats.py
--rw-r--r--   0        0        0     1709 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/commands.py
--rw-r--r--   0        0        0     8899 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/enums.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/__init__.py
--rw-r--r--   0        0        0      670 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/edit_message.py
--rw-r--r--   0        0        0      742 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/forward.py
--rw-r--r--   0        0        0    10453 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/incoming_message.py
--rw-r--r--   0        0        0     7095 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/markup.py
--rw-r--r--   0        0        0     9106 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/mentions.py
--rw-r--r--   0        0        0      270 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/message_status.py
--rw-r--r--   0        0        0      882 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/outgoing_message.py
--rw-r--r--   0        0        0      696 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/reply.py
--rw-r--r--   0        0        0      825 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/message/reply_message.py
--rw-r--r--   0        0        0      538 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/method_callbacks.py
--rw-r--r--   0        0        0      547 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/smartapps.py
--rw-r--r--   0        0        0     2691 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/status.py
--rw-r--r--   0        0        0     1744 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/stickers.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/__init__.py
--rw-r--r--   0        0        0     1591 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/added_to_chat.py
--rw-r--r--   0        0        0     2964 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/chat_created.py
--rw-r--r--   0        0        0     1267 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/cts_login.py
--rw-r--r--   0        0        0     1277 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/cts_logout.py
--rw-r--r--   0        0        0     1746 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/deleted_from_chat.py
--rw-r--r--   0        0        0     2181 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/event_edit.py
--rw-r--r--   0        0        0     2144 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/internal_bot_notification.py
--rw-r--r--   0        0        0     1600 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/left_from_chat.py
--rw-r--r--   0        0        0     3744 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/system_events/smartapp_event.py
--rw-r--r--   0        0        0     1571 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/models/users.py
--rw-r--r--   0        0        0        0 2024-04-12 07:48:47.900246 pybotx-0.66.0/pybotx/py.typed
--rw-r--r--   0        0        0     1459 2024-04-12 07:48:47.900246 pybotx-0.66.0/pyproject.toml
--rw-r--r--   0        0        0    25658 1970-01-01 00:00:00.000000 pybotx-0.66.0/PKG-INFO
+-rw-r--r--   0        0        0     6078 2024-05-22 07:43:19.132807 pybotx-0.66.1/LICENSE
+-rw-r--r--   0        0        0    24562 2024-05-22 07:43:19.136807 pybotx-0.66.1/README.md
+-rw-r--r--   0        0        0     7504 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/async_buffer.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/__init__.py
+-rw-r--r--   0        0        0      560 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/responses/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/responses/bot_disabled.py
+-rw-r--r--   0        0        0      275 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/responses/command_accepted.py
+-rw-r--r--   0        0        0     1185 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/api/responses/unverified_request.py
+-rw-r--r--   0        0        0    63728 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/bot.py
+-rw-r--r--   0        0        0     1558 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/bot_accounts_storage.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/callbacks/callback_manager.py
+-rw-r--r--   0        0        0     2176 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/callbacks/callback_memory_repo.py
+-rw-r--r--   0        0        0      983 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/callbacks/callback_repo_proto.py
+-rw-r--r--   0        0        0      330 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/contextvars.py
+-rw-r--r--   0        0        0     1324 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/exceptions.py
+-rw-r--r--   0        0        0     2790 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/handler.py
+-rw-r--r--   0        0        0    14811 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/handler_collector.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/middlewares/__init__.py
+-rw-r--r--   0        0        0     1749 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/middlewares/exception_middleware.py
+-rw-r--r--   0        0        0      293 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/bot/testing.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/__init__.py
+-rw-r--r--   0        0        0     1617 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/authorized_botx_method.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/bots_api/__init__.py
+-rw-r--r--   0        0        0     1946 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/bots_api/bot_catalog.py
+-rw-r--r--   0        0        0     1235 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/bots_api/get_token.py
+-rw-r--r--   0        0        0     6809 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/botx_method.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/__init__.py
+-rw-r--r--   0        0        0     2201 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/add_admin.py
+-rw-r--r--   0        0        0     1443 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/add_user.py
+-rw-r--r--   0        0        0     2985 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/chat_info.py
+-rw-r--r--   0        0        0     2177 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/create_chat.py
+-rw-r--r--   0        0        0     1415 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/disable_stealth.py
+-rw-r--r--   0        0        0     2004 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/list_chats.py
+-rw-r--r--   0        0        0     1398 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/pin_message.py
+-rw-r--r--   0        0        0     1430 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/remove_user.py
+-rw-r--r--   0        0        0     1699 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/set_stealth.py
+-rw-r--r--   0        0        0     1354 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/chats_api/unpin_message.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/__init__.py
+-rw-r--r--   0        0        0     1355 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/delete_event.py
+-rw-r--r--   0        0        0     3295 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/edit_event.py
+-rw-r--r--   0        0        0     2324 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/message_status_event.py
+-rw-r--r--   0        0        0     3770 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/reply_event.py
+-rw-r--r--   0        0        0     1019 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/stop_typing_event.py
+-rw-r--r--   0        0        0      955 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/events_api/typing_event.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/base.py
+-rw-r--r--   0        0        0      889 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/callbacks.py
+-rw-r--r--   0        0        0      424 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/chats.py
+-rw-r--r--   0        0        0      429 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/common.py
+-rw-r--r--   0        0        0      130 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/event.py
+-rw-r--r--   0        0        0      289 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/files.py
+-rw-r--r--   0        0        0      750 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/http.py
+-rw-r--r--   0        0        0      134 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/message.py
+-rw-r--r--   0        0        0      378 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/notifications.py
+-rw-r--r--   0        0        0      293 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/exceptions/users.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/files_api/__init__.py
+-rw-r--r--   0        0        0     2093 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/files_api/download_file.py
+-rw-r--r--   0        0        0     2448 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/files_api/upload_file.py
+-rw-r--r--   0        0        0      812 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/get_token.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/mertics_api/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/mertics_api/collect_bot_function.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/notifications_api/__init__.py
+-rw-r--r--   0        0        0     5567 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/notifications_api/direct_notification.py
+-rw-r--r--   0        0        0     2925 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/notifications_api/internal_bot_notification.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/openid_api/__init__.py
+-rw-r--r--   0        0        0     1245 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/openid_api/refresh_access_token.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/__init__.py
+-rw-r--r--   0        0        0     2319 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_custom_notification.py
+-rw-r--r--   0        0        0     2259 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_event.py
+-rw-r--r--   0        0        0     1995 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_manifest.py
+-rw-r--r--   0        0        0     1836 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_notification.py
+-rw-r--r--   0        0        0     2195 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/smartapps_list.py
+-rw-r--r--   0        0        0     1652 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/smartapps_api/upload_file.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/__init__.py
+-rw-r--r--   0        0        0     2883 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/add_sticker.py
+-rw-r--r--   0        0        0     1689 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/create_sticker_pack.py
+-rw-r--r--   0        0        0     1506 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/delete_sticker.py
+-rw-r--r--   0        0        0     1426 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/delete_sticker_pack.py
+-rw-r--r--   0        0        0     1793 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/edit_sticker_pack.py
+-rw-r--r--   0        0        0      311 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/exceptions.py
+-rw-r--r--   0        0        0     1984 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/get_sticker.py
+-rw-r--r--   0        0        0     1397 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/get_sticker_pack.py
+-rw-r--r--   0        0        0     2352 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/get_sticker_packs.py
+-rw-r--r--   0        0        0     1321 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/stickers_api/sticker_pack.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/__init__.py
+-rw-r--r--   0        0        0     1231 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/search_user_by_email.py
+-rw-r--r--   0        0        0     1066 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/search_user_by_emails.py
+-rw-r--r--   0        0        0     1257 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/search_user_by_huid.py
+-rw-r--r--   0        0        0     1330 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/search_user_by_login.py
+-rw-r--r--   0        0        0     1254 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/search_user_by_other_id.py
+-rw-r--r--   0        0        0     3020 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/update_user_profile.py
+-rw-r--r--   0        0        0     1737 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/user_from_csv.py
+-rw-r--r--   0        0        0     2092 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/user_from_search.py
+-rw-r--r--   0        0        0     1473 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/client/users_api/users_as_csv.py
+-rw-r--r--   0        0        0      421 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/constants.py
+-rw-r--r--   0        0        0      221 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/converters.py
+-rw-r--r--   0        0        0      789 2024-05-22 07:43:19.136807 pybotx-0.66.1/pybotx/image_validators.py
+-rw-r--r--   0        0        0     1341 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/logger.py
+-rw-r--r--   0        0        0      648 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/missing.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/__init__.py
+-rw-r--r--   0        0        0     2079 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/api_base.py
+-rw-r--r--   0        0        0     7256 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/async_files.py
+-rw-r--r--   0        0        0    13393 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/attachments.py
+-rw-r--r--   0        0        0     2480 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/base_command.py
+-rw-r--r--   0        0        0      644 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/bot_account.py
+-rw-r--r--   0        0        0      435 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/bot_catalog.py
+-rw-r--r--   0        0        0      199 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/bot_sender.py
+-rw-r--r--   0        0        0     1635 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/chats.py
+-rw-r--r--   0        0        0     1709 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/commands.py
+-rw-r--r--   0        0        0     8899 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/enums.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/__init__.py
+-rw-r--r--   0        0        0      670 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/edit_message.py
+-rw-r--r--   0        0        0      742 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/forward.py
+-rw-r--r--   0        0        0    10453 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/incoming_message.py
+-rw-r--r--   0        0        0     7095 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/markup.py
+-rw-r--r--   0        0        0     9106 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/mentions.py
+-rw-r--r--   0        0        0      270 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/message_status.py
+-rw-r--r--   0        0        0      882 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/outgoing_message.py
+-rw-r--r--   0        0        0      696 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/reply.py
+-rw-r--r--   0        0        0      825 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/message/reply_message.py
+-rw-r--r--   0        0        0      538 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/method_callbacks.py
+-rw-r--r--   0        0        0      547 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/smartapps.py
+-rw-r--r--   0        0        0     2691 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/status.py
+-rw-r--r--   0        0        0     1744 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/stickers.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/__init__.py
+-rw-r--r--   0        0        0     1591 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/added_to_chat.py
+-rw-r--r--   0        0        0     2964 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/chat_created.py
+-rw-r--r--   0        0        0     1267 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/cts_login.py
+-rw-r--r--   0        0        0     1277 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/cts_logout.py
+-rw-r--r--   0        0        0     1746 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/deleted_from_chat.py
+-rw-r--r--   0        0        0     2592 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/event_edit.py
+-rw-r--r--   0        0        0     2144 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/internal_bot_notification.py
+-rw-r--r--   0        0        0     1600 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/left_from_chat.py
+-rw-r--r--   0        0        0     3744 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/system_events/smartapp_event.py
+-rw-r--r--   0        0        0     1571 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/models/users.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:43:19.140807 pybotx-0.66.1/pybotx/py.typed
+-rw-r--r--   0        0        0     1459 2024-05-22 07:43:19.140807 pybotx-0.66.1/pyproject.toml
+-rw-r--r--   0        0        0    25658 1970-01-01 00:00:00.000000 pybotx-0.66.1/PKG-INFO
```

### Comparing `pybotx-0.66.0/LICENSE` & `pybotx-0.66.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/README.md` & `pybotx-0.66.1/README.md`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/__init__.py` & `pybotx-0.66.1/pybotx/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/async_buffer.py` & `pybotx-0.66.1/pybotx/async_buffer.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/api/exceptions.py` & `pybotx-0.66.1/pybotx/bot/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/api/responses/bot_disabled.py` & `pybotx-0.66.1/pybotx/bot/api/responses/bot_disabled.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/api/responses/unverified_request.py` & `pybotx-0.66.1/pybotx/bot/api/responses/unverified_request.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/bot.py` & `pybotx-0.66.1/pybotx/bot/bot.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/bot_accounts_storage.py` & `pybotx-0.66.1/pybotx/bot/bot_accounts_storage.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/callbacks/callback_manager.py` & `pybotx-0.66.1/pybotx/bot/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/callbacks/callback_memory_repo.py` & `pybotx-0.66.1/pybotx/bot/callbacks/callback_memory_repo.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/callbacks/callback_repo_proto.py` & `pybotx-0.66.1/pybotx/bot/callbacks/callback_repo_proto.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/exceptions.py` & `pybotx-0.66.1/pybotx/bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/handler.py` & `pybotx-0.66.1/pybotx/bot/handler.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/handler_collector.py` & `pybotx-0.66.1/pybotx/bot/handler_collector.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/bot/middlewares/exception_middleware.py` & `pybotx-0.66.1/pybotx/bot/middlewares/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/authorized_botx_method.py` & `pybotx-0.66.1/pybotx/client/authorized_botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/bots_api/bot_catalog.py` & `pybotx-0.66.1/pybotx/client/bots_api/bot_catalog.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/bots_api/get_token.py` & `pybotx-0.66.1/pybotx/client/bots_api/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/botx_method.py` & `pybotx-0.66.1/pybotx/client/botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/add_admin.py` & `pybotx-0.66.1/pybotx/client/chats_api/add_admin.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/add_user.py` & `pybotx-0.66.1/pybotx/client/chats_api/add_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/chat_info.py` & `pybotx-0.66.1/pybotx/client/chats_api/chat_info.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/create_chat.py` & `pybotx-0.66.1/pybotx/client/chats_api/create_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/disable_stealth.py` & `pybotx-0.66.1/pybotx/client/chats_api/disable_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/list_chats.py` & `pybotx-0.66.1/pybotx/client/chats_api/list_chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/pin_message.py` & `pybotx-0.66.1/pybotx/client/chats_api/pin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/remove_user.py` & `pybotx-0.66.1/pybotx/client/chats_api/remove_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/set_stealth.py` & `pybotx-0.66.1/pybotx/client/chats_api/set_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/chats_api/unpin_message.py` & `pybotx-0.66.1/pybotx/client/chats_api/unpin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/delete_event.py` & `pybotx-0.66.1/pybotx/client/events_api/delete_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/edit_event.py` & `pybotx-0.66.1/pybotx/client/events_api/edit_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/message_status_event.py` & `pybotx-0.66.1/pybotx/client/events_api/message_status_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/reply_event.py` & `pybotx-0.66.1/pybotx/client/events_api/reply_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/stop_typing_event.py` & `pybotx-0.66.1/pybotx/client/events_api/stop_typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/events_api/typing_event.py` & `pybotx-0.66.1/pybotx/client/events_api/typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/exceptions/base.py` & `pybotx-0.66.1/pybotx/client/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/exceptions/callbacks.py` & `pybotx-0.66.1/pybotx/client/exceptions/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/exceptions/http.py` & `pybotx-0.66.1/pybotx/client/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/files_api/download_file.py` & `pybotx-0.66.1/pybotx/client/files_api/download_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/files_api/upload_file.py` & `pybotx-0.66.1/pybotx/client/files_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/get_token.py` & `pybotx-0.66.1/pybotx/client/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/mertics_api/collect_bot_function.py` & `pybotx-0.66.1/pybotx/client/mertics_api/collect_bot_function.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/notifications_api/direct_notification.py` & `pybotx-0.66.1/pybotx/client/notifications_api/direct_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/notifications_api/internal_bot_notification.py` & `pybotx-0.66.1/pybotx/client/notifications_api/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/openid_api/refresh_access_token.py` & `pybotx-0.66.1/pybotx/client/openid_api/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_custom_notification.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_custom_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_event.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_manifest.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_manifest.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/smartapp_notification.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/smartapp_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/smartapps_list.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/smartapps_list.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/smartapps_api/upload_file.py` & `pybotx-0.66.1/pybotx/client/smartapps_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/add_sticker.py` & `pybotx-0.66.1/pybotx/client/stickers_api/add_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/create_sticker_pack.py` & `pybotx-0.66.1/pybotx/client/stickers_api/create_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker.py` & `pybotx-0.66.1/pybotx/client/stickers_api/delete_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/delete_sticker_pack.py` & `pybotx-0.66.1/pybotx/client/stickers_api/delete_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/edit_sticker_pack.py` & `pybotx-0.66.1/pybotx/client/stickers_api/edit_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker.py` & `pybotx-0.66.1/pybotx/client/stickers_api/get_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_pack.py` & `pybotx-0.66.1/pybotx/client/stickers_api/get_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/get_sticker_packs.py` & `pybotx-0.66.1/pybotx/client/stickers_api/get_sticker_packs.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/stickers_api/sticker_pack.py` & `pybotx-0.66.1/pybotx/client/stickers_api/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/search_user_by_email.py` & `pybotx-0.66.1/pybotx/client/users_api/search_user_by_email.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/search_user_by_emails.py` & `pybotx-0.66.1/pybotx/client/users_api/search_user_by_emails.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/search_user_by_huid.py` & `pybotx-0.66.1/pybotx/client/users_api/search_user_by_huid.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/search_user_by_login.py` & `pybotx-0.66.1/pybotx/client/users_api/search_user_by_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/search_user_by_other_id.py` & `pybotx-0.66.1/pybotx/client/users_api/search_user_by_other_id.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/update_user_profile.py` & `pybotx-0.66.1/pybotx/client/users_api/update_user_profile.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/user_from_csv.py` & `pybotx-0.66.1/pybotx/client/users_api/user_from_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/user_from_search.py` & `pybotx-0.66.1/pybotx/client/users_api/user_from_search.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/client/users_api/users_as_csv.py` & `pybotx-0.66.1/pybotx/client/users_api/users_as_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/image_validators.py` & `pybotx-0.66.1/pybotx/image_validators.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/logger.py` & `pybotx-0.66.1/pybotx/logger.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/missing.py` & `pybotx-0.66.1/pybotx/missing.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/api_base.py` & `pybotx-0.66.1/pybotx/models/api_base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/async_files.py` & `pybotx-0.66.1/pybotx/models/async_files.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/attachments.py` & `pybotx-0.66.1/pybotx/models/attachments.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/base_command.py` & `pybotx-0.66.1/pybotx/models/base_command.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/bot_account.py` & `pybotx-0.66.1/pybotx/models/bot_account.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/chats.py` & `pybotx-0.66.1/pybotx/models/chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/commands.py` & `pybotx-0.66.1/pybotx/models/commands.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/enums.py` & `pybotx-0.66.1/pybotx/models/enums.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/edit_message.py` & `pybotx-0.66.1/pybotx/models/message/edit_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/forward.py` & `pybotx-0.66.1/pybotx/models/message/forward.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/incoming_message.py` & `pybotx-0.66.1/pybotx/models/message/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/markup.py` & `pybotx-0.66.1/pybotx/models/message/markup.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/mentions.py` & `pybotx-0.66.1/pybotx/models/message/mentions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/outgoing_message.py` & `pybotx-0.66.1/pybotx/models/message/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/reply.py` & `pybotx-0.66.1/pybotx/models/message/reply.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/message/reply_message.py` & `pybotx-0.66.1/pybotx/models/message/reply_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/method_callbacks.py` & `pybotx-0.66.1/pybotx/models/method_callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/smartapps.py` & `pybotx-0.66.1/pybotx/models/smartapps.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/status.py` & `pybotx-0.66.1/pybotx/models/status.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/stickers.py` & `pybotx-0.66.1/pybotx/models/stickers.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/added_to_chat.py` & `pybotx-0.66.1/pybotx/models/system_events/added_to_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/chat_created.py` & `pybotx-0.66.1/pybotx/models/system_events/chat_created.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/cts_login.py` & `pybotx-0.66.1/pybotx/models/system_events/cts_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/cts_logout.py` & `pybotx-0.66.1/pybotx/models/system_events/cts_logout.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/deleted_from_chat.py` & `pybotx-0.66.1/pybotx/models/system_events/deleted_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/event_edit.py` & `pybotx-0.66.1/pybotx/models/system_events/event_edit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from dataclasses import dataclass
 from typing import Any, Dict, List, Literal, Optional
+from uuid import UUID
 
 from pydantic import Field
 
 from pybotx.models.api_base import VerifiedPayloadBaseModel
 from pybotx.models.attachments import (
     BotAPIAttachment,
     IncomingAttachment,
     convert_api_attachment_to_domain,
 )
 from pybotx.models.base_command import (
-    BaseBotAPIContext,
     BotAPIBaseCommand,
     BotAPIBaseSystemEventPayload,
+    BotAPIUserContext,
     BotCommandBase,
 )
 from pybotx.models.bot_account import BotAccount
 from pybotx.models.enums import BotAPISystemEventTypes
 from pybotx.models.message.incoming_message import (
     BotAPIEntity,
     Entity,
@@ -26,35 +27,47 @@
 
 @dataclass
 class EventEdit(BotCommandBase):
     """Event `system:event_edit`.
 
     Attributes:
         body: Updated message body.
+        sync_id: Updated message sync id.
+        chat_id: Updated message chat id.
+        huid: Updated message user huid.
         attachments: Attachments from updated message.
         entities: Entities from updated message.
     """
 
     body: Optional[str]
+    sync_id: UUID
+    chat_id: UUID
+    huid: UUID
     attachments: List[IncomingAttachment]
     entities: List[Entity]
 
 
 class BotAPIEventEditData(VerifiedPayloadBaseModel):
     body: Optional[str]
 
 
 class BotAPIEventEditPayload(BotAPIBaseSystemEventPayload):
     body: Literal[BotAPISystemEventTypes.EVENT_EDIT]
     data: BotAPIEventEditData
 
 
+class BotAPIBotContext(BotAPIUserContext):
+    """Bot context."""
+
+    group_chat_id: UUID
+
+
 class BotAPIEventEdit(BotAPIBaseCommand):
     payload: BotAPIEventEditPayload = Field(..., alias="command")
-    sender: BaseBotAPIContext = Field(..., alias="from")
+    sender: BotAPIBotContext = Field(..., alias="from")
     attachments: List[BotAPIAttachment]
     entities: List[BotAPIEntity]
 
     def to_domain(self, raw_command: Dict[str, Any]) -> EventEdit:
         return EventEdit(
             bot=BotAccount(
                 id=self.bot_id,
@@ -69,8 +82,11 @@
                 )
                 for attachment in self.attachments
             ],
             entities=[
                 convert_bot_api_entity_to_domain(api_entity=entity)
                 for entity in self.entities
             ],
+            sync_id=self.sync_id,
+            chat_id=self.sender.group_chat_id,
+            huid=self.sender.user_huid,
         )
```

### Comparing `pybotx-0.66.0/pybotx/models/system_events/internal_bot_notification.py` & `pybotx-0.66.1/pybotx/models/system_events/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/left_from_chat.py` & `pybotx-0.66.1/pybotx/models/system_events/left_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/system_events/smartapp_event.py` & `pybotx-0.66.1/pybotx/models/system_events/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pybotx/models/users.py` & `pybotx-0.66.1/pybotx/models/users.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.66.0/pyproject.toml` & `pybotx-0.66.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybotx"
-version = "0.66.0"
+version = "0.66.1"
 description = "A python library for interacting with eXpress BotX API"
 authors = [
     "Sidnev Nikolay <nsidnev@ccsteam.ru>",
     "Maxim Gorbachev <mgorbachev@ccsteam.ru>",
     "Alexander Samoylenko <alexandr.samojlenko@ccsteam.ru>",
     "Arseniy Zhiltsov <arseniy.zhiltsov@ccsteam.ru>"
 ]
```

### Comparing `pybotx-0.66.0/PKG-INFO` & `pybotx-0.66.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotx
-Version: 0.66.0
+Version: 0.66.1
 Summary: A python library for interacting with eXpress BotX API
 Home-page: https://github.com/ExpressApp/pybotx
 Author: Sidnev Nikolay
 Author-email: nsidnev@ccsteam.ru
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

