# Comparing `tmp/abilian_sbe-1.1.8.tar.gz` & `tmp/abilian_sbe-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abilian_sbe-1.1.8.tar", max compression
+gzip compressed data, was "abilian_sbe-1.1.9.tar", max compression
```

## Comparing `abilian_sbe-1.1.8.tar` & `abilian_sbe-1.1.9.tar`

### file list

```diff
@@ -1,1553 +1,1553 @@
--rw-r--r--   0        0        0     7652 2023-11-02 14:44:52.025373 abilian_sbe-1.1.8/LICENCE.txt
--rw-r--r--   0        0        0     4223 2024-02-07 15:10:35.344658 abilian_sbe-1.1.8/README.md
--rw-r--r--   0        0        0     8485 2024-04-26 16:03:35.086169 abilian_sbe-1.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-16 12:51:19.000000 abilian_sbe-1.1.8/src/abilian/__init__.py
--rw-r--r--   0        0        0    16539 2024-04-25 09:37:10.377469 abilian_sbe-1.1.8/src/abilian/app.py
--rw-r--r--   0        0        0      126 2022-01-10 11:24:05.307322 abilian_sbe-1.1.8/src/abilian/cli/__init__.py
--rw-r--r--   0        0        0     6556 2024-02-07 15:10:35.354478 abilian_sbe-1.1.8/src/abilian/cli/base.py
--rw-r--r--   0        0        0      612 2024-03-25 13:17:52.042182 abilian_sbe-1.1.8/src/abilian/cli/config.py
--rw-r--r--   0        0        0     6127 2024-02-07 15:10:35.354767 abilian_sbe-1.1.8/src/abilian/cli/indexing.py
--rw-r--r--   0        0        0     2099 2024-03-27 10:19:57.119194 abilian_sbe-1.1.8/src/abilian/config.py
--rw-r--r--   0        0        0        0 2024-03-25 06:54:43.962129 abilian_sbe-1.1.8/src/abilian/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:54:43.923145 abilian_sbe-1.1.8/src/abilian/core/dramatiq/__init__.py
--rw-r--r--   0        0        0      280 2024-03-25 06:54:43.927420 abilian_sbe-1.1.8/src/abilian/core/dramatiq/cli.py
--rw-r--r--   0        0        0     1809 2024-03-25 06:56:05.424351 abilian_sbe-1.1.8/src/abilian/core/dramatiq/scheduler.py
--rw-r--r--   0        0        0     3345 2024-03-25 13:17:52.042319 abilian_sbe-1.1.8/src/abilian/core/dramatiq/setup.py
--rw-r--r--   0        0        0      347 2024-03-25 13:17:52.042426 abilian_sbe-1.1.8/src/abilian/core/dramatiq/singleton.py
--rw-r--r--   0        0        0    18367 2024-04-26 15:46:20.164523 abilian_sbe-1.1.8/src/abilian/core/entities.py
--rw-r--r--   0        0        0     4170 2024-03-25 13:17:52.042733 abilian_sbe-1.1.8/src/abilian/core/extensions/__init__.py
--rw-r--r--   0        0        0     2536 2024-03-25 13:17:52.042999 abilian_sbe-1.1.8/src/abilian/core/extensions/csrf.py
--rw-r--r--   0        0        0     2807 2024-03-25 06:56:05.428498 abilian_sbe-1.1.8/src/abilian/core/extensions/jinjaext.py
--rw-r--r--   0        0        0      566 2024-03-25 06:56:05.429357 abilian_sbe-1.1.8/src/abilian/core/extensions/login.py
--rw-r--r--   0        0        0      682 2024-03-25 06:56:05.429526 abilian_sbe-1.1.8/src/abilian/core/extensions/redis.py
--rw-r--r--   0        0        0     2071 2024-03-25 13:17:52.043117 abilian_sbe-1.1.8/src/abilian/core/extensions/upstream_info.py
--rw-r--r--   0        0        0     1425 2024-03-25 13:17:52.043410 abilian_sbe-1.1.8/src/abilian/core/logger_patch.py
--rw-r--r--   0        0        0     1518 2024-03-25 13:17:52.043568 abilian_sbe-1.1.8/src/abilian/core/logging.py
--rw-r--r--   0        0        0      363 2024-03-25 13:17:52.043699 abilian_sbe-1.1.8/src/abilian/core/models/__init__.py
--rw-r--r--   0        0        0     3001 2024-03-25 13:17:52.043965 abilian_sbe-1.1.8/src/abilian/core/models/attachment.py
--rw-r--r--   0        0        0     2212 2024-04-26 15:32:02.656547 abilian_sbe-1.1.8/src/abilian/core/models/base.py
--rw-r--r--   0        0        0     1674 2024-03-25 13:17:52.044035 abilian_sbe-1.1.8/src/abilian/core/models/base_mixin.py
--rw-r--r--   0        0        0     3886 2024-03-25 13:17:52.044155 abilian_sbe-1.1.8/src/abilian/core/models/blob.py
--rw-r--r--   0        0        0     2622 2024-03-25 13:17:52.044406 abilian_sbe-1.1.8/src/abilian/core/models/comment.py
--rw-r--r--   0        0        0     1941 2024-03-25 06:56:05.432557 abilian_sbe-1.1.8/src/abilian/core/models/owned.py
--rw-r--r--   0        0        0    10370 2024-04-26 15:34:05.280067 abilian_sbe-1.1.8/src/abilian/core/models/subjects.py
--rw-r--r--   0        0        0     2872 2024-03-25 13:17:52.045001 abilian_sbe-1.1.8/src/abilian/core/models/tag.py
--rw-r--r--   0        0        0     1050 2024-03-25 06:54:42.810857 abilian_sbe-1.1.8/src/abilian/core/signals.py
--rw-r--r--   0        0        0     2634 2024-03-25 06:56:05.433575 abilian_sbe-1.1.8/src/abilian/core/singleton.py
--rw-r--r--   0        0        0    12834 2024-03-25 13:17:52.045335 abilian_sbe-1.1.8/src/abilian/core/sqlalchemy.py
--rw-r--r--   0        0        0     6620 2024-03-25 13:17:52.045822 abilian_sbe-1.1.8/src/abilian/core/util.py
--rw-r--r--   0        0        0    12627 2024-03-25 13:17:52.046301 abilian_sbe-1.1.8/src/abilian/i18n.py
--rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/__init__.py
--rw-r--r--   0        0        0     1558 2024-03-27 10:19:57.119395 abilian_sbe-1.1.8/src/abilian/sbe/app.py
--rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/__init__.py
--rw-r--r--   0        0        0      245 2024-02-07 15:10:35.360668 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/__init__.py
--rw-r--r--   0        0        0     1424 2023-11-15 13:48:35.641820 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/actions.py
--rw-r--r--   0        0        0     2155 2024-03-25 13:17:52.046578 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/forms.py
--rw-r--r--   0        0        0     1241 2023-12-08 09:38:36.961819 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/models.py
--rw-r--r--   0        0        0      665 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/_base.html
--rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/archives.html
--rw-r--r--   0        0        0      936 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/event.html
--rw-r--r--   0        0        0      693 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/index.html
--rw-r--r--   0        0        0     3089 2024-03-25 13:17:52.046855 abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/views.py
--rw-r--r--   0        0        0      293 2024-02-07 15:10:35.361199 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/__init__.py
--rw-r--r--   0        0        0     2608 2024-02-01 15:04:46.166107 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/actions.py
--rw-r--r--   0        0        0     2526 2024-03-25 13:17:52.047212 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/blueprint.py
--rw-r--r--   0        0        0     1728 2023-11-02 14:44:40.640316 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/common.py
--rw-r--r--   0        0        0      891 2024-03-23 14:15:18.391077 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/events.py
--rw-r--r--   0        0        0     4386 2024-03-25 13:17:52.047690 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/forms.py
--rw-r--r--   0        0        0    17078 2024-04-25 11:34:05.550253 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/models.py
--rw-r--r--   0        0        0      343 2022-01-10 11:24:05.321254 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/presenters.py
--rw-r--r--   0        0        0     2551 2024-02-07 15:10:35.362310 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/search.py
--rw-r--r--   0        0        0     2580 2024-03-25 13:17:52.048210 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/security.py
--rw-r--r--   0        0        0      484 2022-01-10 11:24:05.321878 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/signals.py
--rw-r--r--   0        0        0     1257 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/_base.html
--rw-r--r--   0        0        0     1211 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/_forumbase.html
--rw-r--r--   0        0        0     2510 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/edit.html
--rw-r--r--   0        0        0     2252 2023-01-06 15:21:07.908153 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/home.html
--rw-r--r--   0        0        0     2086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/macros.html
--rw-r--r--   0        0        0     5480 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members.html
--rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members_macros.html
--rw-r--r--   0        0        0     3693 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members_std_macros.html
--rw-r--r--   0        0        0     7470 2023-01-06 15:38:25.307247 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_add_emails.html
--rw-r--r--   0        0        0     3970 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_check_members.html
--rw-r--r--   0        0        0     8574 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_new_accounts.html
--rw-r--r--   0        0        0     4705 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_users_std_macros.html
--rw-r--r--   0        0        0      136 2024-02-01 15:05:42.035137 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/__init__.py
--rw-r--r--   0        0        0     5106 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/data/community.png
--rw-r--r--   0        0        0    15826 2024-03-25 13:17:52.048550 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/views.py
--rw-r--r--   0        0        0     9917 2024-03-25 08:00:55.932036 abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/wizard.py
--rw-r--r--   0        0        0      558 2024-03-25 13:17:52.048729 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/__init__.py
--rw-r--r--   0        0        0     9829 2024-03-23 14:15:18.486736 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/actions.py
--rw-r--r--   0        0        0      789 2023-12-22 14:52:32.481243 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cli.py
--rw-r--r--   0        0        0      132 2024-02-07 15:10:35.363648 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/__init__.py
--rw-r--r--   0        0        0    11897 2024-03-23 14:15:18.496755 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/atompub.py
--rw-r--r--   0        0        0     3766 2024-04-26 14:16:17.827236 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/parser.py
--rw-r--r--   0        0        0     1549 2022-01-10 11:24:05.325636 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/renderer.py
--rw-r--r--   0        0        0     1684 2022-03-29 05:40:32.396040 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/lock.py
--rw-r--r--   0        0        0    24675 2024-04-26 14:28:57.903880 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/models.py
--rw-r--r--   0        0        0     5299 2024-03-23 14:15:18.491465 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/repository.py
--rw-r--r--   0        0        0     1860 2024-03-23 14:15:18.490357 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/search.py
--rw-r--r--   0        0        0     1629 2024-03-23 14:15:18.476992 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/signals.py
--rw-r--r--   0        0        0     6505 2024-03-25 13:17:52.049224 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/tasks.py
--rw-r--r--   0        0        0      123 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/allowableactions.xml
--rw-r--r--   0        0        0     1140 2024-03-23 14:17:59.600802 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/children.xml
--rw-r--r--   0        0        0     8119 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/document.xml
--rw-r--r--   0        0        0      927 2024-03-23 14:17:52.327057 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/feed.xml
--rw-r--r--   0        0        0     4312 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/folder.xml
--rw-r--r--   0        0        0     4309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/macros.xml
--rw-r--r--   0        0        0    13863 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/service.xml
--rw-r--r--   0        0        0    23100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-document.xml
--rw-r--r--   0        0        0    13734 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-folder.xml
--rw-r--r--   0        0        0    11986 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-policy.xml
--rw-r--r--   0        0        0    13066 2024-03-23 14:18:13.142503 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-relationship.xml
--rw-r--r--   0        0        0     9553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/types.xml
--rw-r--r--   0        0        0    17052 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros.html
--rw-r--r--   0        0        0     2586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros_audit.html
--rw-r--r--   0        0        0    16442 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros_gallery_view.html
--rw-r--r--   0        0        0      237 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document.html
--rw-r--r--   0        0        0     1007 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_delete.html
--rw-r--r--   0        0        0     2218 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_edit.html
--rw-r--r--   0        0        0     1549 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_send_by_email.html
--rw-r--r--   0        0        0     1452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_upload_new_version.html
--rw-r--r--   0        0        0      452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder.html
--rw-r--r--   0        0        0     3571 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_change_owner.html
--rw-r--r--   0        0        0     1121 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_delete.html
--rw-r--r--   0        0        0     2146 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_edit.html
--rw-r--r--   0        0        0     1148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_move.html
--rw-r--r--   0        0        0     1963 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_new.html
--rw-r--r--   0        0        0     3761 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_upload.html
--rw-r--r--   0        0        0     3784 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_roles.html
--rw-r--r--   0        0        0     1909 2022-03-29 05:55:53.926477 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/descendants.html
--rw-r--r--   0        0        0    11321 2022-03-29 05:55:53.922772 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/document.html
--rw-r--r--   0        0        0     2571 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/document_viewers.html
--rw-r--r--   0        0        0      698 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/folder.html
--rw-r--r--   0        0        0      731 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/folder_gallery_view.html
--rw-r--r--   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/mail_file_sent.fr.txt
--rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/mail_file_sent.txt
--rw-r--r--   0        0        0     8948 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/permissions.html
--rw-r--r--   0        0        0    21512 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/view_pdf.html
--rw-r--r--   0        0        0      167 2024-03-25 13:17:52.049428 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/__init__.py
--rw-r--r--   0        0        0    11642 2024-03-25 13:17:52.049656 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/documents.py
--rw-r--r--   0        0        0    34367 2024-03-25 13:17:52.049979 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/folders.py
--rw-r--r--   0        0        0     6644 2024-02-07 15:10:35.366814 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/util.py
--rw-r--r--   0        0        0     1003 2024-03-25 13:17:52.050169 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/views.py
--rw-r--r--   0        0        0      114 2024-02-07 15:10:35.367048 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/__init__.py
--rw-r--r--   0        0        0     1780 2024-02-07 15:10:35.367282 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/constants.py
--rw-r--r--   0        0        0     9113 2024-03-25 13:17:52.050324 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/views.py
--rw-r--r--   0        0        0     2241 2024-02-07 15:10:35.367683 abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/xml.py
--rw-r--r--   0        0        0      882 2024-03-25 13:17:52.050682 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/__init__.py
--rw-r--r--   0        0        0     3343 2024-03-25 13:17:52.050857 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/actions.py
--rw-r--r--   0        0        0     1630 2024-02-07 15:10:35.367924 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/cli.py
--rw-r--r--   0        0        0     2311 2024-02-07 15:10:35.368176 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/forms.py
--rw-r--r--   0        0        0     6833 2024-02-07 15:10:35.368307 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/models.py
--rw-r--r--   0        0        0    17463 2024-03-23 14:15:18.428404 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/tasks.py
--rw-r--r--   0        0        0       37 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/_base.html
--rw-r--r--   0        0        0     2769 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/_macros.html
--rw-r--r--   0        0        0     1540 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/archives.html
--rw-r--r--   0        0        0     1373 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/attachments.html
--rw-r--r--   0        0        0     3389 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/index.html
--rw-r--r--   0        0        0     1129 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.fr.html
--rw-r--r--   0        0        0     1127 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.html
--rw-r--r--   0        0        0    10422 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread.html
--rw-r--r--   0        0        0     2547 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread_attachments.html
--rw-r--r--   0        0        0     4817 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread_create.html
--rw-r--r--   0        0        0    17860 2024-03-25 13:17:52.051168 abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/views.py
--rw-r--r--   0        0        0      328 2024-02-07 15:10:35.369016 abilian_sbe-1.1.8/src/abilian/sbe/apps/main/__init__.py
--rw-r--r--   0        0        0      387 2022-01-10 11:24:05.334109 abilian_sbe-1.1.8/src/abilian/sbe/apps/main/main.py
--rw-r--r--   0        0        0      762 2024-02-07 15:10:35.369378 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/__init__.py
--rw-r--r--   0        0        0        0 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/tasks/__init__.py
--rw-r--r--   0        0        0     8943 2024-03-23 14:15:18.526749 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/tasks/social.py
--rw-r--r--   0        0        0     1988 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/_base.html
--rw-r--r--   0        0        0    11699 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/_style.css
--rw-r--r--   0        0        0      388 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/confirm-unsubscribe.fr.html
--rw-r--r--   0        0        0      309 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/confirm-unsubscribe.html
--rw-r--r--   0        0        0     4278 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.fr.html
--rw-r--r--   0        0        0     4204 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.html
--rw-r--r--   0        0        0      356 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/invalid-token.fr.html
--rw-r--r--   0        0        0      314 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/invalid-token.html
--rw-r--r--   0        0        0      164 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/unsubscribed.fr.html
--rw-r--r--   0        0        0      140 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/unsubscribed.html
--rw-r--r--   0        0        0      198 2022-01-10 11:24:05.334999 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/views/__init__.py
--rw-r--r--   0        0        0     1952 2024-03-23 14:15:18.530523 abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/views/social.py
--rw-r--r--   0        0        0      420 2024-03-23 14:15:18.363614 abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/__init__.py
--rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/panels/__init__.py
--rw-r--r--   0        0        0     2429 2024-02-07 15:10:35.369798 abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/panels/sbe_notifications.py
--rw-r--r--   0        0        0      701 2022-04-12 15:38:51.537046 abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/templates/preferences/sbe_notifications.html
--rw-r--r--   0        0        0      455 2024-02-07 15:10:35.369912 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/__init__.py
--rw-r--r--   0        0        0     1119 2024-02-07 15:10:35.370157 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/forms.py
--rw-r--r--   0        0        0     2645 2024-02-07 15:10:35.370262 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/models.py
--rw-r--r--   0        0        0     7998 2024-03-23 14:15:18.451083 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/restapi.py
--rw-r--r--   0        0        0     1290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/_sidebar.html
--rw-r--r--   0        0        0     1654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/base.html
--rw-r--r--   0        0        0     4308 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/group.html
--rw-r--r--   0        0        0     1663 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/groups-new.html
--rw-r--r--   0        0        0     2769 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/groups.html
--rw-r--r--   0        0        0      353 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/home.html
--rw-r--r--   0        0        0     1250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/invite.html
--rw-r--r--   0        0        0     4100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/macros.html
--rw-r--r--   0        0        0      208 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/mail/invite.txt
--rw-r--r--   0        0        0     1835 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/user.html
--rw-r--r--   0        0        0     3166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/users.html
--rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/widget_user_photo.html
--rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/__init__.py
--rw-r--r--   0        0        0     5810 2024-03-23 14:15:18.461633 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/groups.py
--rw-r--r--   0        0        0     1823 2024-03-23 14:15:18.455097 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/invites.py
--rw-r--r--   0        0        0     1445 2024-03-23 14:15:18.472104 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/sidebars.py
--rw-r--r--   0        0        0     1356 2022-01-10 11:24:05.337926 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/social.py
--rw-r--r--   0        0        0     9083 2024-03-23 14:15:18.459486 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/users.py
--rw-r--r--   0        0        0      590 2024-03-25 13:17:52.051315 abilian_sbe-1.1.8/src/abilian/sbe/apps/social/widgets.py
--rw-r--r--   0        0        0      187 2022-01-10 11:24:05.338437 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/__init__.py
--rw-r--r--   0        0        0     6373 2024-02-07 15:10:35.371158 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/presenters.py
--rw-r--r--   0        0        0      522 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/templates/wall/_base.html
--rw-r--r--   0        0        0      759 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/templates/wall/files.html
--rw-r--r--   0        0        0      309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/templates/wall/index.html
--rw-r--r--   0        0        0     2993 2024-03-25 13:17:52.051430 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/util.py
--rw-r--r--   0        0        0     4560 2024-03-25 13:17:52.051689 abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/views.py
--rw-r--r--   0        0        0      444 2024-03-25 13:17:52.051928 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/__init__.py
--rw-r--r--   0        0        0     2781 2022-01-10 11:24:05.339289 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/actions.py
--rw-r--r--   0        0        0      266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/data/default_page.txt
--rw-r--r--   0        0        0     1532 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/data/help.txt
--rw-r--r--   0        0        0     1959 2024-03-23 14:15:18.418706 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/forms.py
--rw-r--r--   0        0        0     2057 2024-03-23 14:15:18.417707 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/markup.py
--rw-r--r--   0        0        0     4976 2023-12-08 09:38:30.278323 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/models.py
--rw-r--r--   0        0        0     4322 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/_base.html
--rw-r--r--   0        0        0      392 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/all_pages.html
--rw-r--r--   0        0        0     1144 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/changes.html
--rw-r--r--   0        0        0      357 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/compare.html
--rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/edit_conflict_error.html
--rw-r--r--   0        0        0      190 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/help.html
--rw-r--r--   0        0        0      372 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/macros.html
--rw-r--r--   0        0        0     1717 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/page.html
--rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/page_readers.html
--rw-r--r--   0        0        0      212 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/source.html
--rw-r--r--   0        0        0      333 2022-01-10 11:24:05.340492 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/util.py
--rw-r--r--   0        0        0    16918 2024-03-25 13:17:52.052210 abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/views.py
--rw-r--r--   0        0        0     3267 2024-02-07 15:10:35.372295 abilian_sbe-1.1.8/src/abilian/sbe/boot.py
--rw-r--r--   0        0        0     1897 2024-03-25 13:17:52.052361 abilian_sbe-1.1.8/src/abilian/sbe/extension.py
--rw-r--r--   0        0        0       32 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/csv/csv_example.csv
--rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/7z.png
--rw-r--r--   0        0        0       60 2023-12-08 18:07:26.554324 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/README.txt
--rw-r--r--   0        0        0      634 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ai.png
--rw-r--r--   0        0        0      604 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/aiff.png
--rw-r--r--   0        0        0      480 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/asc.png
--rw-r--r--   0        0        0      514 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/audio.png
--rw-r--r--   0        0        0      458 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/bin.png
--rw-r--r--   0        0        0      576 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/bz2.png
--rw-r--r--   0        0        0      584 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/c.png
--rw-r--r--   0        0        0      577 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cfc.png
--rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cfm.png
--rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/chm.png
--rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/class.png
--rw-r--r--   0        0        0      557 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/conf.png
--rw-r--r--   0        0        0      629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cpp.png
--rw-r--r--   0        0        0      618 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cs.png
--rw-r--r--   0        0        0      654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/css.png
--rw-r--r--   0        0        0      366 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/csv.png
--rw-r--r--   0        0        0      564 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/deb.png
--rw-r--r--   0        0        0      661 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/divx.png
--rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/doc.png
--rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/docx.png
--rw-r--r--   0        0        0      475 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/dot.png
--rw-r--r--   0        0        0      302 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/eml.png
--rw-r--r--   0        0        0      474 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/enc.png
--rw-r--r--   0        0        0      358 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/file.png
--rw-r--r--   0        0        0      358 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/folder.png
--rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/gif.png
--rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/gz.png
--rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/hlp.png
--rw-r--r--   0        0        0      611 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/htm.png
--rw-r--r--   0        0        0      611 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/html.png
--rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/image.png
--rw-r--r--   0        0        0      581 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/iso.png
--rw-r--r--   0        0        0      599 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jar.png
--rw-r--r--   0        0        0      604 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/java.png
--rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jpeg.png
--rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jpg.png
--rw-r--r--   0        0        0      622 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/js.png
--rw-r--r--   0        0        0      390 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/lua.png
--rw-r--r--   0        0        0      567 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/m.png
--rw-r--r--   0        0        0      323 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mm.png
--rw-r--r--   0        0        0      665 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mov.png
--rw-r--r--   0        0        0      629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mp3.png
--rw-r--r--   0        0        0      660 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mpg.png
--rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odc.png
--rw-r--r--   0        0        0      621 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odf.png
--rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odg.png
--rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odi.png
--rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odp.png
--rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ods.png
--rw-r--r--   0        0        0      479 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odt.png
--rw-r--r--   0        0        0      613 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ogg.png
--rw-r--r--   0        0        0      522 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pdf.png
--rw-r--r--   0        0        0      481 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pgp.png
--rw-r--r--   0        0        0      633 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/php.png
--rw-r--r--   0        0        0      605 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pl.png
--rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/png.png
--rw-r--r--   0        0        0      602 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ppt.png
--rw-r--r--   0        0        0      602 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pptx.png
--rw-r--r--   0        0        0      446 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ps.png
--rw-r--r--   0        0        0      614 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/py.png
--rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ram.png
--rw-r--r--   0        0        0      499 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rar.png
--rw-r--r--   0        0        0      623 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rb.png
--rw-r--r--   0        0        0      605 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rm.png
--rw-r--r--   0        0        0      445 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rpm.png
--rw-r--r--   0        0        0      384 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rtf.png
--rw-r--r--   0        0        0      498 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sig.png
--rw-r--r--   0        0        0      583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sql.png
--rw-r--r--   0        0        0      632 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/swf.png
--rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxc.png
--rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxd.png
--rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxi.png
--rw-r--r--   0        0        0      479 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxw.png
--rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tar.png
--rw-r--r--   0        0        0      643 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tex.png
--rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tgz.png
--rw-r--r--   0        0        0      398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/txt.png
--rw-r--r--   0        0        0      552 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/vcf.png
--rw-r--r--   0        0        0      540 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/video.png
--rw-r--r--   0        0        0      574 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/vsd.png
--rw-r--r--   0        0        0      615 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wav.png
--rw-r--r--   0        0        0      636 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wma.png
--rw-r--r--   0        0        0      670 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wmv.png
--rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xls.png
--rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xlsx.png
--rw-r--r--   0        0        0      367 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xml.png
--rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xpi.png
--rw-r--r--   0        0        0      653 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xvid.png
--rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/zip.png
--rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/account-12.png
--rwxr-xr-x   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/account-16.png
--rw-r--r--   0        0        0      349 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/actionfiliere-12.png
--rw-r--r--   0        0        0      412 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/checkbox-checked-12.png
--rwxr-xr-x   0        0        0      281 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/checkbox-checked-16.png
--rw-r--r--   0        0        0      327 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/checkbox-unchecked-12.png
--rwxr-xr-x   0        0        0      204 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/checkbox-unchecked-16.png
--rwxr-xr-x   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/cog-16.png
--rw-r--r--   0        0        0      332 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/contact-12.png
--rwxr-xr-x   0        0        0      208 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/contact-16.png
--rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/document-12.png
--rwxr-xr-x   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/document-16.png
--rwxr-xr-x   0        0        0      207 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/download-16.png
--rw-r--r--   0        0        0      362 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/image-12.png
--rwxr-xr-x   0        0        0      234 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/image-16.png
--rw-r--r--   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/lead-12.png
--rwxr-xr-x   0        0        0      214 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/lead-16.png
--rw-r--r--   0        0        0      343 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/opportunity-12.png
--rwxr-xr-x   0        0        0      233 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/opportunity-16.png
--rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/partenaire-12.png
--rw-r--r--   0        0        0      320 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/programmefiliere-12.png
--rw-r--r--   0        0        0      333 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/projet-12.png
--rwxr-xr-x   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/round-minus-16.png
--rwxr-xr-x   0        0        0      316 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/round-minus-24.png
--rwxr-xr-x   0        0        0      250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/round-plus-16.png
--rwxr-xr-x   0        0        0      367 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/round-plus-24.png
--rwxr-xr-x   0        0        0      401 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/visite-12.png
--rwxr-xr-x   0        0        0      237 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/icons/wrench-16.png
--rw-r--r--   0        0        0     1171 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/arrows.png
--rw-r--r--   0        0        0     1361 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_disabled.png
--rw-r--r--   0        0        0     1379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_enabled.png
--rw-r--r--   0        0        0     1375 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_enabled_hover.png
--rw-r--r--   0        0        0     4123 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/backgrd.png
--rw-r--r--   0        0        0    46666 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/eagle.jpg
--rw-r--r--   0        0        0     2170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/error.png
--rw-r--r--   0        0        0     1579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/favicon.png
--rw-r--r--   0        0        0     1363 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_disabled.png
--rw-r--r--   0        0        0     1380 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_enabled.png
--rw-r--r--   0        0        0     1379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_enabled_hover.png
--rw-r--r--   0        0        0    50718 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/frog.jpg
--rw-r--r--   0        0        0     8777 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/glyphicons-halflings-white.png
--rw-r--r--   0        0        0    13826 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/glyphicons-halflings.png
--rw-r--r--   0        0        0      191 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/greendot.png
--rw-r--r--   0        0        0    14264 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/group-icon.png
--rw-r--r--   0        0        0   325765 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/login-background.jpg
--rwxr-xr-x   0        0        0      209 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/next.png
--rw-r--r--   0        0        0     7609 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/noise_bg.png
--rwxr-xr-x   0        0        0      203 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/prev.png
--rw-r--r--   0        0        0      679 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/preview_missing.png
--rw-r--r--   0        0        0    12517 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_man.png
--rw-r--r--   0        0        0    10266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_unknown.png
--rw-r--r--   0        0        0    12333 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_woman.png
--rw-r--r--   0        0        0     1118 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_asc.png
--rw-r--r--   0        0        0     1050 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_asc_disabled.png
--rw-r--r--   0        0        0     1136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_both.png
--rw-r--r--   0        0        0     1127 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_desc.png
--rw-r--r--   0        0        0     1045 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_desc_disabled.png
--rw-r--r--   0        0        0      314 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/state.png
--rw-r--r--   0        0        0    11584 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/user-icon.png
--rw-r--r--   0        0        0     2294 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/images/valid.png
--rw-r--r--   0        0        0      240 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/arrows.png
--rw-r--r--   0        0        0     7710 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/avatar140.jpg
--rw-r--r--   0        0        0     4340 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/avatar45.png
--rw-r--r--   0        0        0      345 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/back_disabled.png
--rw-r--r--   0        0        0      459 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/back_enabled.png
--rw-r--r--   0        0        0      457 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/back_enabled_hover.png
--rw-r--r--   0        0        0     2487 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/backgrd.png
--rw-r--r--   0        0        0     1182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/error.png
--rw-r--r--   0        0        0     1069 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/favicon.png
--rw-r--r--   0        0        0      350 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/forward_disabled.png
--rw-r--r--   0        0        0      468 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/forward_enabled.png
--rw-r--r--   0        0        0      467 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/forward_enabled_hover.png
--rw-r--r--   0        0        0     8768 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/glyphicons-halflings-white.png
--rw-r--r--   0        0        0    11896 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/glyphicons-halflings.png
--rw-r--r--   0        0        0      136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/greendot.png
--rw-r--r--   0        0        0    12299 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/group-icon.png
--rw-r--r--   0        0        0     1056 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/group64.png
--rw-r--r--   0        0        0  1304297 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/login-background.jpg
--rw-r--r--   0        0        0     5071 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/me-25x25.jpg
--rwxr-xr-x   0        0        0      142 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/next.png
--rwxr-xr-x   0        0        0      141 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/prev.png
--rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/sort_asc.png
--rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/sort_asc_disabled.png
--rw-r--r--   0        0        0      209 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/sort_both.png
--rw-r--r--   0        0        0      172 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/sort_desc.png
--rw-r--r--   0        0        0      159 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/sort_desc_disabled.png
--rw-r--r--   0        0        0      107 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/state.png
--rw-r--r--   0        0        0     9815 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/user-icon.png
--rw-r--r--   0        0        0     1323 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/img/valid.png
--rw-r--r--   0        0        0     1599 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/document_viewer.js
--rw-r--r--   0        0        0     6462 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder.js
--rw-r--r--   0        0        0     1165 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_edit.js
--rw-r--r--   0        0        0     4638 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_gallery.js
--rw-r--r--   0        0        0     3040 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_upload.js
--rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/js/sbe-datatable.js
--rw-r--r--   0        0        0      221 2023-12-08 18:07:26.555085 abilian_sbe-1.1.8/src/abilian/sbe/static/less/README.txt
--rw-r--r--   0        0        0      377 2022-04-04 14:22:56.768469 abilian_sbe-1.1.8/src/abilian/sbe/static/less/abilian-sbe.less
--rw-r--r--   0        0        0      165 2022-04-04 14:15:12.852861 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/base.less
--rw-r--r--   0        0        0     1357 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/bootstrap-tagsinput.less
--rw-r--r--   0        0        0     1002 2022-04-04 14:16:11.444824 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/communities.less
--rw-r--r--   0        0        0     5985 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/documents.less
--rw-r--r--   0        0        0      273 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/excel.less
--rw-r--r--   0        0        0    11908 2022-04-04 14:20:50.191106 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/forum.less
--rw-r--r--   0        0        0     1676 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/misc.less
--rw-r--r--   0        0        0      279 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/social.less
--rw-r--r--   0        0        0      241 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/wiki.less
--rw-r--r--   0        0        0     2811 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/wizard_steps.less
--rw-r--r--   0        0        0     1328 2022-04-04 14:15:00.639617 abilian_sbe-1.1.8/src/abilian/sbe/static/less/overrides.less
--rw-r--r--   0        0        0      224 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/less/print.less
--rw-r--r--   0        0        0    14684 2023-12-08 18:07:26.555690 abilian_sbe-1.1.8/src/abilian/sbe/static/moment/moment.min.js
--rw-r--r--   0        0        0       86 2023-12-08 18:07:26.556277 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/README.txt
--rw-r--r--   0        0        0     2404 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-H.bcmap
--rw-r--r--   0        0        0      173 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-V.bcmap
--rw-r--r--   0        0        0     2379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-H.bcmap
--rw-r--r--   0        0        0     2398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-H.bcmap
--rw-r--r--   0        0        0      173 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-V.bcmap
--rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-V.bcmap
--rw-r--r--   0        0        0     2651 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-H.bcmap
--rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-V.bcmap
--rw-r--r--   0        0        0      905 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/83pv-RKSJ-H.bcmap
--rw-r--r--   0        0        0      721 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-H.bcmap
--rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-V.bcmap
--rw-r--r--   0        0        0      715 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-H.bcmap
--rw-r--r--   0        0        0      291 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-V.bcmap
--rw-r--r--   0        0        0      982 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-H.bcmap
--rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-V.bcmap
--rw-r--r--   0        0        0     2419 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-H.bcmap
--rw-r--r--   0        0        0     2413 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-H.bcmap
--rw-r--r--   0        0        0      287 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-V.bcmap
--rw-r--r--   0        0        0      282 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-V.bcmap
--rw-r--r--   0        0        0      317 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-0.bcmap
--rw-r--r--   0        0        0      371 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-1.bcmap
--rw-r--r--   0        0        0      376 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-2.bcmap
--rw-r--r--   0        0        0      401 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-3.bcmap
--rw-r--r--   0        0        0      405 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-4.bcmap
--rw-r--r--   0        0        0      406 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-5.bcmap
--rw-r--r--   0        0        0      406 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-6.bcmap
--rw-r--r--   0        0        0    41193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
--rw-r--r--   0        0        0      217 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-0.bcmap
--rw-r--r--   0        0        0      250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-1.bcmap
--rw-r--r--   0        0        0      465 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-2.bcmap
--rw-r--r--   0        0        0      470 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-3.bcmap
--rw-r--r--   0        0        0      601 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-4.bcmap
--rw-r--r--   0        0        0      625 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-5.bcmap
--rw-r--r--   0        0        0    33974 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
--rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-0.bcmap
--rw-r--r--   0        0        0      226 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-1.bcmap
--rw-r--r--   0        0        0      233 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-2.bcmap
--rw-r--r--   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-3.bcmap
--rw-r--r--   0        0        0      337 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-4.bcmap
--rw-r--r--   0        0        0      430 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-5.bcmap
--rw-r--r--   0        0        0      485 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-6.bcmap
--rw-r--r--   0        0        0    40951 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
--rw-r--r--   0        0        0      241 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-0.bcmap
--rw-r--r--   0        0        0      386 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-1.bcmap
--rw-r--r--   0        0        0      391 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-2.bcmap
--rw-r--r--   0        0        0    23293 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
--rw-r--r--   0        0        0     1086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5-H.bcmap
--rw-r--r--   0        0        0      142 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5-V.bcmap
--rw-r--r--   0        0        0     1099 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5pc-H.bcmap
--rw-r--r--   0        0        0      144 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5pc-V.bcmap
--rw-r--r--   0        0        0     1780 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-H.bcmap
--rw-r--r--   0        0        0     1920 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-V.bcmap
--rw-r--r--   0        0        0      706 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS1-H.bcmap
--rw-r--r--   0        0        0      143 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS1-V.bcmap
--rw-r--r--   0        0        0      504 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS2-H.bcmap
--rw-r--r--   0        0        0       93 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS2-V.bcmap
--rw-r--r--   0        0        0     4426 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-H.bcmap
--rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-V.bcmap
--rw-r--r--   0        0        0     1125 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-H.bcmap
--rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-V.bcmap
--rw-r--r--   0        0        0      101 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETenms-B5-H.bcmap
--rw-r--r--   0        0        0      172 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETenms-B5-V.bcmap
--rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/EUC-H.bcmap
--rw-r--r--   0        0        0      170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/EUC-V.bcmap
--rw-r--r--   0        0        0     2536 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-H.bcmap
--rw-r--r--   0        0        0     2542 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-H.bcmap
--rw-r--r--   0        0        0      218 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-V.bcmap
--rw-r--r--   0        0        0      215 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-V.bcmap
--rw-r--r--   0        0        0      549 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-H.bcmap
--rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-V.bcmap
--rw-r--r--   0        0        0      528 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-H.bcmap
--rw-r--r--   0        0        0      175 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-V.bcmap
--rw-r--r--   0        0        0    14692 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-H.bcmap
--rw-r--r--   0        0        0      180 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-V.bcmap
--rw-r--r--   0        0        0    19662 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-H.bcmap
--rw-r--r--   0        0        0      219 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-V.bcmap
--rw-r--r--   0        0        0    14686 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-H.bcmap
--rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-V.bcmap
--rw-r--r--   0        0        0     7290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-H.bcmap
--rw-r--r--   0        0        0      180 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-V.bcmap
--rw-r--r--   0        0        0     7269 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-H.bcmap
--rw-r--r--   0        0        0      176 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-V.bcmap
--rw-r--r--   0        0        0     7298 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-H.bcmap
--rw-r--r--   0        0        0      182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-V.bcmap
--rw-r--r--   0        0        0      557 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-H.bcmap
--rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-V.bcmap
--rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/H.bcmap
--rw-r--r--   0        0        0     2654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-H.bcmap
--rw-r--r--   0        0        0      148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-V.bcmap
--rw-r--r--   0        0        0     2414 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-H.bcmap
--rw-r--r--   0        0        0      148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-V.bcmap
--rw-r--r--   0        0        0     2292 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-H.bcmap
--rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-V.bcmap
--rw-r--r--   0        0        0     1772 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-H.bcmap
--rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-V.bcmap
--rw-r--r--   0        0        0     2171 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-H.bcmap
--rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-V.bcmap
--rw-r--r--   0        0        0     4437 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-H.bcmap
--rw-r--r--   0        0        0      159 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-V.bcmap
--rw-r--r--   0        0        0      132 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Hankaku.bcmap
--rw-r--r--   0        0        0      124 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Hiragana.bcmap
--rw-r--r--   0        0        0     1848 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-H.bcmap
--rw-r--r--   0        0        0      164 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-V.bcmap
--rw-r--r--   0        0        0     1831 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-H.bcmap
--rw-r--r--   0        0        0    16791 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-H.bcmap
--rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-V.bcmap
--rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-V.bcmap
--rw-r--r--   0        0        0     2787 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-H.bcmap
--rw-r--r--   0        0        0     2789 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
--rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
--rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-V.bcmap
--rw-r--r--   0        0        0     2024 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-H.bcmap
--rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-V.bcmap
--rw-r--r--   0        0        0      100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Katakana.bcmap
--rw-r--r--   0        0        0     2080 2023-12-08 18:07:26.557356 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/LICENSE
--rw-r--r--   0        0        0     2765 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/NWP-H.bcmap
--rw-r--r--   0        0        0      252 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/NWP-V.bcmap
--rw-r--r--   0        0        0      534 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-H.bcmap
--rw-r--r--   0        0        0      170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-V.bcmap
--rw-r--r--   0        0        0       96 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Roman.bcmap
--rw-r--r--   0        0        0    48280 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
--rw-r--r--   0        0        0      156 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
--rw-r--r--   0        0        0    50419 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
--rw-r--r--   0        0        0      156 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
--rw-r--r--   0        0        0    52679 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
--rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
--rw-r--r--   0        0        0    53629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
--rw-r--r--   0        0        0      157 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
--rw-r--r--   0        0        0    43366 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-H.bcmap
--rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-V.bcmap
--rw-r--r--   0        0        0    44086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-H.bcmap
--rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-V.bcmap
--rw-r--r--   0        0        0    45738 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-H.bcmap
--rw-r--r--   0        0        0      182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-V.bcmap
--rw-r--r--   0        0        0    46837 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-H.bcmap
--rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-V.bcmap
--rw-r--r--   0        0        0    25439 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
--rw-r--r--   0        0        0      119 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
--rw-r--r--   0        0        0      680 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
--rw-r--r--   0        0        0      664 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
--rw-r--r--   0        0        0    39443 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
--rw-r--r--   0        0        0      643 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
--rw-r--r--   0        0        0    40539 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
--rw-r--r--   0        0        0      677 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
--rw-r--r--   0        0        0    41695 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
--rw-r--r--   0        0        0      678 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
--rw-r--r--   0        0        0    39534 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
--rw-r--r--   0        0        0      647 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
--rw-r--r--   0        0        0    40630 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
--rw-r--r--   0        0        0      681 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
--rw-r--r--   0        0        0    41779 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
--rw-r--r--   0        0        0      682 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
--rw-r--r--   0        0        0      705 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
--rw-r--r--   0        0        0      689 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
--rw-r--r--   0        0        0      726 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
--rw-r--r--   0        0        0    40517 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
--rw-r--r--   0        0        0      684 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
--rw-r--r--   0        0        0    40608 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
--rw-r--r--   0        0        0      688 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
--rw-r--r--   0        0        0    25783 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-H.bcmap
--rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-V.bcmap
--rw-r--r--   0        0        0    26327 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-H.bcmap
--rw-r--r--   0        0        0      164 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-V.bcmap
--rw-r--r--   0        0        0    26451 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-H.bcmap
--rw-r--r--   0        0        0      168 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-V.bcmap
--rw-r--r--   0        0        0    27790 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-H.bcmap
--rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-V.bcmap
--rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/V.bcmap
--rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/WP-Symbol.bcmap
--rw-r--r--   0        0        0    17788 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/compatibility.js
--rw-r--r--   0        0        0    19583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/debugger.js
--rw-r--r--   0        0        0      415 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-check.svg
--rw-r--r--   0        0        0      883 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-comment.svg
--rw-r--r--   0        0        0     2168 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-help.svg
--rw-r--r--   0        0        0      408 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-insert.svg
--rw-r--r--   0        0        0     1452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-key.svg
--rw-r--r--   0        0        0      426 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-newparagraph.svg
--rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-noicon.svg
--rw-r--r--   0        0        0     1041 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-note.svg
--rw-r--r--   0        0        0     1143 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-paragraph.svg
--rw-r--r--   0        0        0      199 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-next-rtl.png
--rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-next-rtl@2x.png
--rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-next.png
--rw-r--r--   0        0        0      296 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-next@2x.png
--rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-previous-rtl.png
--rw-r--r--   0        0        0      296 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-previous-rtl@2x.png
--rw-r--r--   0        0        0      199 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-previous.png
--rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/findbarButton-previous@2x.png
--rw-r--r--   0        0        0      326 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/grab.cur
--rw-r--r--   0        0        0      326 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/grabbing.cur
--rw-r--r--   0        0        0     2545 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-icon.gif
--rw-r--r--   0        0        0     7402 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-small.png
--rw-r--r--   0        0        0    16131 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-small@2x.png
--rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties.png
--rw-r--r--   0        0        0      933 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties@2x.png
--rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-firstPage.png
--rw-r--r--   0        0        0      266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-firstPage@2x.png
--rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool.png
--rw-r--r--   0        0        0      583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool@2x.png
--rw-r--r--   0        0        0      175 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-lastPage.png
--rw-r--r--   0        0        0      276 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-lastPage@2x.png
--rw-r--r--   0        0        0      360 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw.png
--rw-r--r--   0        0        0      731 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw@2x.png
--rw-r--r--   0        0        0      359 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw.png
--rw-r--r--   0        0        0      714 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw@2x.png
--rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/shadow.png
--rw-r--r--   0        0        0     2418 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/texture.png
--rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-bookmark.png
--rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-bookmark@2x.png
--rw-r--r--   0        0        0      259 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-download.png
--rw-r--r--   0        0        0      425 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-download@2x.png
--rw-r--r--   0        0        0      108 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-menuArrows.png
--rw-r--r--   0        0        0      152 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-menuArrows@2x.png
--rw-r--r--   0        0        0      295 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile.png
--rw-r--r--   0        0        0      550 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile@2x.png
--rw-r--r--   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown-rtl.png
--rw-r--r--   0        0        0      398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown-rtl@2x.png
--rw-r--r--   0        0        0      238 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown.png
--rw-r--r--   0        0        0      396 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown@2x.png
--rw-r--r--   0        0        0      245 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp-rtl.png
--rw-r--r--   0        0        0      405 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp-rtl@2x.png
--rw-r--r--   0        0        0      246 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp.png
--rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp@2x.png
--rw-r--r--   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode.png
--rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode@2x.png
--rw-r--r--   0        0        0      257 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-print.png
--rw-r--r--   0        0        0      464 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-print@2x.png
--rw-r--r--   0        0        0      309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-search.png
--rw-r--r--   0        0        0      653 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-search@2x.png
--rw-r--r--   0        0        0      246 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle-rtl.png
--rw-r--r--   0        0        0      456 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
--rw-r--r--   0        0        0      243 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle.png
--rw-r--r--   0        0        0      458 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle@2x.png
--rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle-rtl.png
--rw-r--r--   0        0        0      344 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle-rtl@2x.png
--rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle.png
--rw-r--r--   0        0        0      331 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle@2x.png
--rw-r--r--   0        0        0      384 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments.png
--rw-r--r--   0        0        0      871 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments@2x.png
--rw-r--r--   0        0        0      177 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline-rtl.png
--rw-r--r--   0        0        0      394 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline-rtl@2x.png
--rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline.png
--rw-r--r--   0        0        0      331 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline@2x.png
--rw-r--r--   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewThumbnail.png
--rw-r--r--   0        0        0      220 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewThumbnail@2x.png
--rw-r--r--   0        0        0      136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomIn.png
--rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomIn@2x.png
--rw-r--r--   0        0        0       88 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomOut.png
--rw-r--r--   0        0        0      109 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomOut@2x.png
--rw-r--r--   0        0        0    29253 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/l10n.js
--rw-r--r--   0        0        0     6355 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/locale/en-US/viewer.properties
--rw-r--r--   0        0        0     6988 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/locale/fr/viewer.properties
--rw-r--r--   0        0        0      128 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/locale/locale.properties
--rw-r--r--   0        0        0   262071 2023-12-08 18:07:26.559387 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/pdf.js
--rw-r--r--   0        0        0  1258826 2023-12-08 18:07:26.565065 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/pdf.worker.js
--rw-r--r--   0        0        0    46023 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/viewer.css
--rw-r--r--   0        0        0   255262 2023-12-08 18:07:26.566971 abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/viewer.js
--rw-r--r--   0        0        0    22075 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/vendor/bootstrap-tagsinput.js
--rw-r--r--   0        0        0    38161 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/static/vendor/jquery.fileapi.js
--rw-r--r--   0        0        0      131 2021-09-16 12:23:46.000000 abilian_sbe-1.1.8/src/abilian/sbe/templates/help.html
--rw-r--r--   0        0        0    60321 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    62372 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/translations/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    50456 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/translations/messages.pot
--rw-r--r--   0        0        0    59863 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/translations/tr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    58090 2021-09-16 12:23:47.000000 abilian_sbe-1.1.8/src/abilian/sbe/translations/zh/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0     1189 2024-02-07 15:10:35.372662 abilian_sbe-1.1.8/src/abilian/services/__init__.py
--rw-r--r--   0        0        0      155 2022-01-10 11:24:05.342770 abilian_sbe-1.1.8/src/abilian/services/activity/__init__.py
--rw-r--r--   0        0        0     2248 2024-03-25 13:17:52.052476 abilian_sbe-1.1.8/src/abilian/services/activity/models.py
--rw-r--r--   0        0        0     2025 2024-03-23 14:15:18.818784 abilian_sbe-1.1.8/src/abilian/services/activity/service.py
--rw-r--r--   0        0        0       65 2024-02-01 15:05:42.048849 abilian_sbe-1.1.8/src/abilian/services/antivirus/__init__.py
--rw-r--r--   0        0        0     3871 2024-03-25 13:17:52.052593 abilian_sbe-1.1.8/src/abilian/services/antivirus/service.py
--rw-r--r--   0        0        0      109 2023-01-06 16:41:12.890699 abilian_sbe-1.1.8/src/abilian/services/audit/__init__.py
--rw-r--r--   0        0        0     7330 2024-03-25 13:17:52.052871 abilian_sbe-1.1.8/src/abilian/services/audit/models.py
--rw-r--r--   0        0        0    13713 2024-04-26 15:34:45.867876 abilian_sbe-1.1.8/src/abilian/services/audit/service.py
--rw-r--r--   0        0        0       77 2024-02-07 15:10:35.373938 abilian_sbe-1.1.8/src/abilian/services/auth/__init__.py
--rw-r--r--   0        0        0     3158 2024-04-26 15:35:17.584615 abilian_sbe-1.1.8/src/abilian/services/auth/models.py
--rw-r--r--   0        0        0     8511 2024-03-23 14:15:18.811603 abilian_sbe-1.1.8/src/abilian/services/auth/service.py
--rw-r--r--   0        0        0      453 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/email/password_reset_instructions.fr.txt
--rw-r--r--   0        0        0      366 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/email/password_reset_instructions.txt
--rw-r--r--   0        0        0      640 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/forgotten_password.html
--rw-r--r--   0        0        0     1088 2021-09-21 08:49:20.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/login.html
--rw-r--r--   0        0        0      912 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/password_reset.fr.html
--rw-r--r--   0        0        0      893 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/password_reset.html
--rw-r--r--   0        0        0    12248 2024-03-25 13:17:52.053741 abilian_sbe-1.1.8/src/abilian/services/auth/views.py
--rw-r--r--   0        0        0     3158 2024-02-07 15:10:35.374760 abilian_sbe-1.1.8/src/abilian/services/base.py
--rw-r--r--   0        0        0      144 2024-02-07 15:10:35.374889 abilian_sbe-1.1.8/src/abilian/services/blob_store/__init__.py
--rw-r--r--   0        0        0    15894 2024-03-25 13:17:52.054147 abilian_sbe-1.1.8/src/abilian/services/blob_store/service.py
--rw-r--r--   0        0        0     1097 2024-02-07 15:10:35.375234 abilian_sbe-1.1.8/src/abilian/services/conversion/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-27 16:00:06.095921 abilian_sbe-1.1.8/src/abilian/services/conversion/cache.py
--rw-r--r--   0        0        0    35636 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/mugshot.jpg
--rw-r--r--   0        0        0    52951 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/onepage.pdf
--rw-r--r--   0        0        0    39540 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/picture.jpg
--rw-r--r--   0        0        0   675299 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/rammstein.pdf
--rw-r--r--   0        0        0      136 2024-02-07 15:10:35.375476 abilian_sbe-1.1.8/src/abilian/services/conversion/exceptions.py
--rw-r--r--   0        0        0     1183 2024-02-07 15:10:35.375690 abilian_sbe-1.1.8/src/abilian/services/conversion/handler_lock.py
--rw-r--r--   0        0        0    18221 2024-02-07 15:10:35.375994 abilian_sbe-1.1.8/src/abilian/services/conversion/handlers.py
--rw-r--r--   0        0        0     7169 2024-03-25 13:17:52.054335 abilian_sbe-1.1.8/src/abilian/services/conversion/service.py
--rw-r--r--   0        0        0     1032 2024-02-07 15:10:35.376858 abilian_sbe-1.1.8/src/abilian/services/conversion/util.py
--rw-r--r--   0        0        0     3156 2024-02-07 15:10:35.376986 abilian_sbe-1.1.8/src/abilian/services/image/__init__.py
--rw-r--r--   0        0        0      149 2024-02-07 15:10:35.377117 abilian_sbe-1.1.8/src/abilian/services/indexing/__init__.py
--rw-r--r--   0        0        0     7037 2024-03-25 13:17:52.054588 abilian_sbe-1.1.8/src/abilian/services/indexing/adapter.py
--rw-r--r--   0        0        0     2698 2024-02-07 15:10:35.377379 abilian_sbe-1.1.8/src/abilian/services/indexing/debug_toolbar.py
--rw-r--r--   0        0        0     3172 2024-03-23 14:15:17.899575 abilian_sbe-1.1.8/src/abilian/services/indexing/schema.py
--rw-r--r--   0        0        0    20879 2024-03-25 16:34:02.573063 abilian_sbe-1.1.8/src/abilian/services/indexing/service.py
--rw-r--r--   0        0        0       96 2022-01-10 11:24:05.349623 abilian_sbe-1.1.8/src/abilian/services/preferences/__init__.py
--rw-r--r--   0        0        0      911 2024-04-26 15:35:32.880378 abilian_sbe-1.1.8/src/abilian/services/preferences/models.py
--rw-r--r--   0        0        0      557 2023-12-08 09:38:30.281087 abilian_sbe-1.1.8/src/abilian/services/preferences/panel.py
--rw-r--r--   0        0        0     6325 2024-02-07 15:10:35.378602 abilian_sbe-1.1.8/src/abilian/services/preferences/service.py
--rw-r--r--   0        0        0      872 2024-02-07 15:10:35.378849 abilian_sbe-1.1.8/src/abilian/services/security/__init__.py
--rw-r--r--   0        0        0     2579 2024-03-23 14:15:18.808146 abilian_sbe-1.1.8/src/abilian/services/security/debug_toolbar.py
--rw-r--r--   0        0        0    12170 2024-04-22 06:37:41.714744 abilian_sbe-1.1.8/src/abilian/services/security/models.py
--rw-r--r--   0        0        0    30163 2024-03-23 14:15:18.804362 abilian_sbe-1.1.8/src/abilian/services/security/service.py
--rw-r--r--   0        0        0      182 2024-02-07 15:10:35.379428 abilian_sbe-1.1.8/src/abilian/services/settings/__init__.py
--rw-r--r--   0        0        0     3401 2024-03-25 13:17:52.055390 abilian_sbe-1.1.8/src/abilian/services/settings/models.py
--rw-r--r--   0        0        0     3958 2024-03-23 14:15:18.793633 abilian_sbe-1.1.8/src/abilian/services/settings/service.py
--rw-r--r--   0        0        0       96 2022-01-10 11:24:05.352465 abilian_sbe-1.1.8/src/abilian/services/viewtracker/__init__.py
--rw-r--r--   0        0        0     1620 2022-01-10 11:24:05.352622 abilian_sbe-1.1.8/src/abilian/services/viewtracker/models.py
--rw-r--r--   0        0        0     2022 2022-01-10 11:24:05.352797 abilian_sbe-1.1.8/src/abilian/services/viewtracker/service.py
--rw-r--r--   0        0        0      185 2024-02-07 15:10:35.380063 abilian_sbe-1.1.8/src/abilian/services/vocabularies/__init__.py
--rw-r--r--   0        0        0     7075 2024-02-07 15:10:35.380319 abilian_sbe-1.1.8/src/abilian/services/vocabularies/admin.py
--rw-r--r--   0        0        0     1061 2024-03-25 13:17:52.055514 abilian_sbe-1.1.8/src/abilian/services/vocabularies/forms.py
--rw-r--r--   0        0        0     4962 2024-04-26 15:36:07.554631 abilian_sbe-1.1.8/src/abilian/services/vocabularies/models.py
--rw-r--r--   0        0        0     1623 2024-03-25 13:17:52.055812 abilian_sbe-1.1.8/src/abilian/services/vocabularies/service.py
--rw-r--r--   0        0        0     2203 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/vocabularies/templates/admin/macros/vocabularies.html
--rw-r--r--   0        0        0      743 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/services/vocabularies/templates/admin/vocabularies.html
--rw-r--r--   0        0        0    24611 2023-12-08 18:07:26.568967 abilian_sbe-1.1.8/src/abilian/translations/de_DE/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    26454 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    26922 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24612 2023-12-08 18:07:26.569726 abilian_sbe-1.1.8/src/abilian/translations/es_ES/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    32978 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/translations/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24610 2023-12-08 18:07:26.570308 abilian_sbe-1.1.8/src/abilian/translations/fr_FR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24556 2023-12-08 18:07:26.570781 abilian_sbe-1.1.8/src/abilian/translations/id_ID/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24656 2023-12-08 18:07:26.571595 abilian_sbe-1.1.8/src/abilian/translations/it_IT/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24657 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/translations/messages.pot
--rw-r--r--   0        0        0    30696 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/translations/nl/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24610 2023-12-08 18:07:26.572264 abilian_sbe-1.1.8/src/abilian/translations/nl_NL/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24626 2023-12-08 18:07:26.573015 abilian_sbe-1.1.8/src/abilian/translations/pt_BR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24656 2023-12-08 18:07:26.573244 abilian_sbe-1.1.8/src/abilian/translations/pt_PT/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24612 2023-12-08 18:07:26.573938 abilian_sbe-1.1.8/src/abilian/translations/tr_TR/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24607 2023-12-08 18:07:26.574531 abilian_sbe-1.1.8/src/abilian/translations/zh_CN/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0    24607 2023-12-08 18:07:26.575133 abilian_sbe-1.1.8/src/abilian/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0      217 2023-12-08 09:38:30.283288 abilian_sbe-1.1.8/src/abilian/web/__init__.py
--rw-r--r--   0        0        0     2085 2024-03-25 13:17:52.056056 abilian_sbe-1.1.8/src/abilian/web/access_blueprint.py
--rw-r--r--   0        0        0    19133 2024-03-25 13:17:52.056460 abilian_sbe-1.1.8/src/abilian/web/action.py
--rw-r--r--   0        0        0      138 2024-02-07 15:10:35.381341 abilian_sbe-1.1.8/src/abilian/web/admin/__init__.py
--rw-r--r--   0        0        0     6430 2024-03-25 13:17:52.056755 abilian_sbe-1.1.8/src/abilian/web/admin/extension.py
--rw-r--r--   0        0        0     1354 2024-02-07 15:10:35.381576 abilian_sbe-1.1.8/src/abilian/web/admin/panel.py
--rw-r--r--   0        0        0       55 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/panels/__init__.py
--rw-r--r--   0        0        0    13276 2024-03-25 13:17:52.057294 abilian_sbe-1.1.8/src/abilian/web/admin/panels/audit.py
--rw-r--r--   0        0        0     6479 2024-02-07 15:10:35.382146 abilian_sbe-1.1.8/src/abilian/web/admin/panels/dashboard.py
--rw-r--r--   0        0        0        0 2024-03-25 13:17:52.057346 abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/__init__.py
--rw-r--r--   0        0        0  2190838 2024-03-25 13:17:52.068043 abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/ip_country.mmdb
--rw-r--r--   0        0        0      676 2024-03-25 13:17:52.068455 abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/ip_country_code.py
--rwxr-xr-x   0        0        0     2105 2024-03-25 13:17:52.068739 abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/update_ip_country.py
--rw-r--r--   0        0        0     2067 2024-03-23 14:15:18.699919 abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/__init__.py
--rw-r--r--   0        0        0      726 2024-03-25 13:17:52.068861 abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/forms.py
--rw-r--r--   0        0        0     6249 2024-03-23 14:15:18.701819 abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/views.py
--rw-r--r--   0        0        0      633 2022-01-10 11:24:05.356234 abilian_sbe-1.1.8/src/abilian/web/admin/panels/impersonate.py
--rw-r--r--   0        0        0      987 2024-03-25 13:17:52.069560 abilian_sbe-1.1.8/src/abilian/web/admin/panels/login_sessions.py
--rw-r--r--   0        0        0     4106 2024-02-07 15:10:35.382607 abilian_sbe-1.1.8/src/abilian/web/admin/panels/settings.py
--rw-r--r--   0        0        0     1079 2024-03-25 13:17:52.070475 abilian_sbe-1.1.8/src/abilian/web/admin/panels/sysinfo.py
--rw-r--r--   0        0        0     2036 2024-03-23 14:15:18.704352 abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/__init__.py
--rw-r--r--   0        0        0     2817 2024-03-25 13:17:52.070598 abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/forms.py
--rw-r--r--   0        0        0     7029 2024-03-25 13:17:52.071238 abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/views.py
--rw-r--r--   0        0        0      566 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/_base.html
--rw-r--r--   0        0        0     1084 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/_macros.html
--rw-r--r--   0        0        0     5133 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/audit.html
--rw-r--r--   0        0        0     5542 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/dashboard.html
--rw-r--r--   0        0        0     3907 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/group_view.html
--rw-r--r--   0        0        0     1032 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/groups.html
--rw-r--r--   0        0        0     1073 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/login_sessions.html
--rw-r--r--   0        0        0      641 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/settings.html
--rw-r--r--   0        0        0      684 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/settings_session_lifetime.html
--rw-r--r--   0        0        0     1224 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/sysinfo.html
--rw-r--r--   0        0        0     1129 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/users.html
--rw-r--r--   0        0        0     3835 2024-03-25 13:17:52.071356 abilian_sbe-1.1.8/src/abilian/web/assets/__init__.py
--rw-r--r--   0        0        0    13476 2024-03-25 13:17:52.072069 abilian_sbe-1.1.8/src/abilian/web/assets/filters.py
--rw-r--r--   0        0        0     6336 2024-02-07 15:10:35.384025 abilian_sbe-1.1.8/src/abilian/web/assets/mixin.py
--rw-r--r--   0        0        0      230 2024-02-07 15:10:35.384143 abilian_sbe-1.1.8/src/abilian/web/attachments/__init__.py
--rw-r--r--   0        0        0     4373 2024-03-23 14:15:18.738293 abilian_sbe-1.1.8/src/abilian/web/attachments/extension.py
--rw-r--r--   0        0        0      701 2024-03-25 13:17:52.072175 abilian_sbe-1.1.8/src/abilian/web/attachments/forms.py
--rw-r--r--   0        0        0     4405 2024-03-25 13:17:52.072629 abilian_sbe-1.1.8/src/abilian/web/attachments/views.py
--rw-r--r--   0        0        0      170 2024-02-07 15:10:35.384555 abilian_sbe-1.1.8/src/abilian/web/comments/__init__.py
--rw-r--r--   0        0        0     1325 2024-03-23 14:15:18.557703 abilian_sbe-1.1.8/src/abilian/web/comments/extension.py
--rw-r--r--   0        0        0      684 2024-03-25 13:17:52.072741 abilian_sbe-1.1.8/src/abilian/web/comments/forms.py
--rw-r--r--   0        0        0     4027 2024-03-25 13:17:52.073071 abilian_sbe-1.1.8/src/abilian/web/comments/views.py
--rw-r--r--   0        0        0       43 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/coreviews/__init__.py
--rw-r--r--   0        0        0     2587 2024-02-07 15:10:35.384859 abilian_sbe-1.1.8/src/abilian/web/coreviews/users.py
--rw-r--r--   0        0        0    28073 2024-03-25 13:17:52.073415 abilian_sbe-1.1.8/src/abilian/web/crm_frontend.py
--rw-r--r--   0        0        0     2311 2024-03-25 13:17:52.073705 abilian_sbe-1.1.8/src/abilian/web/csrf.py
--rw-r--r--   0        0        0     5092 2024-03-25 13:17:52.073816 abilian_sbe-1.1.8/src/abilian/web/errors.py
--rw-r--r--   0        0        0     7697 2024-03-23 14:15:18.554813 abilian_sbe-1.1.8/src/abilian/web/filters.py
--rw-r--r--   0        0        0      231 2024-02-01 15:05:42.069192 abilian_sbe-1.1.8/src/abilian/web/forms/__init__.py
--rw-r--r--   0        0        0    26783 2024-03-25 13:17:52.074089 abilian_sbe-1.1.8/src/abilian/web/forms/fields.py
--rw-r--r--   0        0        0      602 2024-02-07 15:10:35.385499 abilian_sbe-1.1.8/src/abilian/web/forms/filters.py
--rw-r--r--   0        0        0     8273 2024-03-25 13:17:52.074393 abilian_sbe-1.1.8/src/abilian/web/forms/form.py
--rw-r--r--   0        0        0     5096 2024-03-25 13:17:52.074500 abilian_sbe-1.1.8/src/abilian/web/forms/permissions.py
--rw-r--r--   0        0        0     1014 2024-02-07 15:10:35.385952 abilian_sbe-1.1.8/src/abilian/web/forms/util.py
--rw-r--r--   0        0        0     7497 2024-02-07 15:10:35.386072 abilian_sbe-1.1.8/src/abilian/web/forms/validators.py
--rw-r--r--   0        0        0    52082 2024-03-25 13:17:52.074942 abilian_sbe-1.1.8/src/abilian/web/forms/widgets.py
--rw-r--r--   0        0        0      803 2024-03-25 13:17:52.075459 abilian_sbe-1.1.8/src/abilian/web/frontend.py
--rw-r--r--   0        0        0      397 2024-02-07 15:10:35.387073 abilian_sbe-1.1.8/src/abilian/web/http.py
--rw-r--r--   0        0        0     3514 2024-03-25 13:17:52.075564 abilian_sbe-1.1.8/src/abilian/web/jinja.py
--rw-r--r--   0        0        0     4670 2024-03-23 14:15:18.550644 abilian_sbe-1.1.8/src/abilian/web/nav.py
--rw-r--r--   0        0        0       43 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/preferences/__init__.py
--rw-r--r--   0        0        0     4703 2024-03-25 13:17:52.075688 abilian_sbe-1.1.8/src/abilian/web/preferences/user.py
--rw-r--r--   0        0        0    26581 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootbox/bootbox.js
--rw-r--r--   0        0        0    20127 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2023-12-08 18:07:26.582271 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    45404 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23424 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0    67546 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0    35951 2023-12-08 18:07:26.583029 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0      484 2023-12-08 18:07:26.583201 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/js/npm.js
--rw-r--r--   0        0        0     8099 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/.csscomb.json
--rw-r--r--   0        0        0      456 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/.csslintrc
--rw-r--r--   0        0        0     1518 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/alerts.less
--rw-r--r--   0        0        0     1201 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/badges.less
--rw-r--r--   0        0        0     1121 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/bootstrap.less
--rw-r--r--   0        0        0      594 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/breadcrumbs.less
--rw-r--r--   0        0        0     5659 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/button-groups.less
--rw-r--r--   0        0        0     3565 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/buttons.less
--rw-r--r--   0        0        0     5405 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/carousel.less
--rw-r--r--   0        0        0      764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/close.less
--rw-r--r--   0        0        0     1401 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/code.less
--rw-r--r--   0        0        0      666 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/component-animations.less
--rw-r--r--   0        0        0     4764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/dropdowns.less
--rw-r--r--   0        0        0    14935 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/forms.less
--rw-r--r--   0        0        0    19803 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/glyphicons.less
--rw-r--r--   0        0        0     1387 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/grid.less
--rw-r--r--   0        0        0     4215 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/input-groups.less
--rw-r--r--   0        0        0      984 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/jumbotron.less
--rw-r--r--   0        0        0     1079 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/labels.less
--rw-r--r--   0        0        0     3022 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/list-group.less
--rw-r--r--   0        0        0      780 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/media.less
--rw-r--r--   0        0        0      257 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/alerts.less
--rw-r--r--   0        0        0      139 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/background-variant.less
--rw-r--r--   0        0        0      468 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/border-radius.less
--rw-r--r--   0        0        0     1080 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/buttons.less
--rw-r--r--   0        0        0      120 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/center-block.less
--rw-r--r--   0        0        0      605 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/clearfix.less
--rw-r--r--   0        0        0     2641 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/forms.less
--rw-r--r--   0        0        0     4388 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/gradients.less
--rw-r--r--   0        0        0     2784 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/grid-framework.less
--rw-r--r--   0        0        0     3094 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/grid.less
--rw-r--r--   0        0        0      579 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/hide-text.less
--rw-r--r--   0        0        0     1062 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/image.less
--rw-r--r--   0        0        0      161 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/labels.less
--rw-r--r--   0        0        0      533 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/list-group.less
--rw-r--r--   0        0        0      232 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/nav-divider.less
--rw-r--r--   0        0        0      364 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/nav-vertical-align.less
--rw-r--r--   0        0        0      148 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/opacity.less
--rw-r--r--   0        0        0      438 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/pagination.less
--rw-r--r--   0        0        0      537 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/panels.less
--rw-r--r--   0        0        0      191 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/progress-bar.less
--rw-r--r--   0        0        0      248 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/reset-filter.less
--rw-r--r--   0        0        0      196 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/resize.less
--rw-r--r--   0        0        0      343 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/responsive-visibility.less
--rw-r--r--   0        0        0      127 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/size.less
--rw-r--r--   0        0        0      159 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/tab-focus.less
--rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/table-row.less
--rw-r--r--   0        0        0      116 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/text-emphasis.less
--rw-r--r--   0        0        0      162 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/text-overflow.less
--rw-r--r--   0        0        0     6650 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/vendor-prefixes.less
--rw-r--r--   0        0        0     1102 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins.less
--rw-r--r--   0        0        0     3565 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/modals.less
--rw-r--r--   0        0        0    14667 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/navbar.less
--rw-r--r--   0        0        0     4930 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/navs.less
--rw-r--r--   0        0        0     7650 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/normalize.less
--rw-r--r--   0        0        0      861 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/pager.less
--rw-r--r--   0        0        0     2001 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/pagination.less
--rw-r--r--   0        0        0     6151 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/panels.less
--rw-r--r--   0        0        0     3509 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/popovers.less
--rw-r--r--   0        0        0     2133 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/print.less
--rw-r--r--   0        0        0     1925 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/progress-bars.less
--rw-r--r--   0        0        0      546 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/responsive-embed.less
--rw-r--r--   0        0        0     4262 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/responsive-utilities.less
--rw-r--r--   0        0        0     3122 2023-12-08 18:07:26.583819 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/scaffolding.less
--rw-r--r--   0        0        0     4612 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/tables.less
--rw-r--r--   0        0        0     7812 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/theme.less
--rw-r--r--   0        0        0      753 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/thumbnails.less
--rw-r--r--   0        0        0     2937 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/tooltip.less
--rw-r--r--   0        0        0     5951 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/type.less
--rw-r--r--   0        0        0      747 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/utilities.less
--rw-r--r--   0        0        0    27053 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/variables.less
--rw-r--r--   0        0        0      527 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/wells.less
--rw-r--r--   0        0        0    32929 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/css/datepicker.css
--rw-r--r--   0        0        0    41744 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/bootstrap-datepicker.js
--rw-r--r--   0        0        0      949 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ar.js
--rw-r--r--   0        0        0      836 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.bg.js
--rw-r--r--   0        0        0      639 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ca.js
--rw-r--r--   0        0        0      711 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cs.js
--rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cy.js
--rw-r--r--   0        0        0      673 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.da.js
--rw-r--r--   0        0        0      697 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.de.js
--rw-r--r--   0        0        0      896 2023-12-08 18:07:26.575764 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.el.js
--rw-r--r--   0        0        0      647 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.es.js
--rw-r--r--   0        0        0      673 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.et.js
--rw-r--r--   0        0        0      726 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fi.js
--rw-r--r--   0        0        0      699 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fr.js
--rw-r--r--   0        0        0      563 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.gl.js
--rw-r--r--   0        0        0      767 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.he.js
--rw-r--r--   0        0        0      597 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hr.js
--rw-r--r--   0        0        0      715 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hu.js
--rw-r--r--   0        0        0      652 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.id.js
--rw-r--r--   0        0        0      709 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.is.js
--rw-r--r--   0        0        0      694 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.it.js
--rw-r--r--   0        0        0      665 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ja.js
--rw-r--r--   0        0        0     1209 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ka.js
--rw-r--r--   0        0        0      637 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.kr.js
--rw-r--r--   0        0        0      764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lt.js
--rw-r--r--   0        0        0      732 2023-12-08 18:07:26.576553 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lv.js
--rw-r--r--   0        0        0      888 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.mk.js
--rw-r--r--   0        0        0      621 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ms.js
--rw-r--r--   0        0        0      663 2023-12-08 18:07:26.577049 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nb.js
--rw-r--r--   0        0        0      754 2023-12-08 18:07:26.577726 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl-BE.js
--rw-r--r--   0        0        0      643 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl.js
--rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.no.js
--rw-r--r--   0        0        0      775 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pl.js
--rw-r--r--   0        0        0      662 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt-BR.js
--rw-r--r--   0        0        0      717 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt.js
--rw-r--r--   0        0        0      676 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ro.js
--rw-r--r--   0        0        0      647 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs-latin.js
--rw-r--r--   0        0        0      835 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs.js
--rw-r--r--   0        0        0      883 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ru.js
--rw-r--r--   0        0        0      693 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sk.js
--rw-r--r--   0        0        0      644 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sl.js
--rw-r--r--   0        0        0      659 2023-12-08 18:07:26.578317 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sq.js
--rw-r--r--   0        0        0      690 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sv.js
--rw-r--r--   0        0        0      773 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sw.js
--rw-r--r--   0        0        0     1008 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.th.js
--rw-r--r--   0        0        0      671 2023-12-08 18:07:26.578942 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.tr.js
--rw-r--r--   0        0        0      870 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ua.js
--rw-r--r--   0        0        0      889 2023-12-08 18:07:26.579365 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.uk.js
--rw-r--r--   0        0        0      796 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-CN.js
--rw-r--r--   0        0        0      891 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-TW.js
--rw-r--r--   0        0        0     5285 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/less/datepicker.less
--rw-r--r--   0        0        0    10173 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/LICENSE
--rw-r--r--   0        0        0    25530 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/bootstrap-switch.js
--rw-r--r--   0        0        0     4668 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/less/bootstrap3/bootstrap-switch.less
--rw-r--r--   0        0        0     2990 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.css
--rw-r--r--   0        0        0     2595 2023-12-08 18:07:26.579923 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.min.css
--rw-r--r--   0        0        0    28462 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.js
--rw-r--r--   0        0        0    16007 2023-12-08 18:07:26.580842 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.min.js
--rw-r--r--   0        0        0     3445 2023-12-08 18:07:26.581375 abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/less/timepicker.less
--rw-r--r--   0        0        0   314777 2024-03-27 08:36:58.813662 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/CHANGES.md
--rw-r--r--   0        0        0    78399 2024-03-27 08:36:58.814352 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/LICENSE.md
--rw-r--r--   0        0        0     1383 2024-03-27 08:36:58.814546 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/README.md
--rw-r--r--   0        0        0      568 2024-03-27 08:36:58.814630 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/SECURITY.md
--rw-r--r--   0        0        0     3180 2024-03-27 08:36:58.814794 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/adapters/jquery.js
--rw-r--r--   0        0        0      246 2024-03-27 08:36:58.814878 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/bender-runner.config.json
--rw-r--r--   0        0        0     3138 2024-03-27 08:36:58.815054 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/build-config.js
--rw-r--r--   0        0        0   680302 2024-03-27 08:36:58.818578 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/ckeditor.js
--rw-r--r--   0        0        0     1345 2024-03-27 08:36:58.818829 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/config.js
--rw-r--r--   0        0        0     3092 2024-03-27 08:36:58.818979 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/contents.css
--rw-r--r--   0        0        0    12599 2024-03-27 08:36:58.819304 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/af.js
--rw-r--r--   0        0        0    15803 2024-03-27 08:36:58.819573 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ar.js
--rw-r--r--   0        0        0    13612 2024-03-27 08:36:58.819747 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/az.js
--rw-r--r--   0        0        0    18969 2024-03-27 08:36:58.819974 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bg.js
--rw-r--r--   0        0        0    16521 2024-03-27 08:36:58.820237 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bn.js
--rw-r--r--   0        0        0    12681 2024-03-27 08:36:58.820529 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bs.js
--rw-r--r--   0        0        0    13924 2024-03-27 08:36:58.820809 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ca.js
--rw-r--r--   0        0        0    13874 2024-03-27 08:36:58.821190 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/cs.js
--rw-r--r--   0        0        0    12979 2024-03-27 08:36:58.821446 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/cy.js
--rw-r--r--   0        0        0    13251 2024-03-27 08:36:58.821751 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/da.js
--rw-r--r--   0        0        0    13952 2024-03-27 08:36:58.821967 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/de-ch.js
--rw-r--r--   0        0        0    13945 2024-03-27 08:36:58.822246 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/de.js
--rw-r--r--   0        0        0    20454 2024-03-27 08:36:58.822491 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/el.js
--rw-r--r--   0        0        0    12617 2024-03-27 08:36:58.822779 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-au.js
--rw-r--r--   0        0        0    12617 2024-03-27 08:36:58.823094 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-ca.js
--rw-r--r--   0        0        0    12637 2024-03-27 08:36:58.823345 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-gb.js
--rw-r--r--   0        0        0    12635 2024-03-27 08:36:58.823691 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en.js
--rw-r--r--   0        0        0    13319 2024-03-27 08:36:58.823989 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/eo.js
--rw-r--r--   0        0        0    14075 2024-03-27 08:36:58.824178 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/es-mx.js
--rw-r--r--   0        0        0    14031 2024-03-27 08:36:58.824543 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/es.js
--rw-r--r--   0        0        0    13022 2024-03-27 08:36:58.824939 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/et.js
--rw-r--r--   0        0        0    13738 2024-03-27 08:36:58.825146 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/eu.js
--rw-r--r--   0        0        0    17129 2024-03-27 08:36:58.825521 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fa.js
--rw-r--r--   0        0        0    13363 2024-03-27 08:36:58.825793 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fi.js
--rw-r--r--   0        0        0    13296 2024-03-27 08:36:58.826040 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fo.js
--rw-r--r--   0        0        0    13769 2024-03-27 08:36:58.826334 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fr-ca.js
--rw-r--r--   0        0        0    14495 2024-03-27 08:36:58.826596 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fr.js
--rw-r--r--   0        0        0    14005 2024-03-27 08:36:58.826888 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/gl.js
--rw-r--r--   0        0        0    20558 2024-03-27 08:36:58.827125 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/gu.js
--rw-r--r--   0        0        0    15395 2024-03-27 08:36:58.827441 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/he.js
--rw-r--r--   0        0        0    16668 2024-03-27 08:36:58.827658 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hi.js
--rw-r--r--   0        0        0    12953 2024-03-27 08:36:58.827968 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hr.js
--rw-r--r--   0        0        0    14158 2024-03-27 08:36:58.828462 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hu.js
--rw-r--r--   0        0        0    12953 2024-03-27 08:36:58.828755 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/id.js
--rw-r--r--   0        0        0    13066 2024-03-27 08:36:58.829035 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/is.js
--rw-r--r--   0        0        0    14079 2024-03-27 08:36:58.829481 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/it.js
--rw-r--r--   0        0        0    15353 2024-03-27 08:36:58.829815 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ja.js
--rw-r--r--   0        0        0    21596 2024-03-27 08:36:58.830068 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ka.js
--rw-r--r--   0        0        0    23848 2024-03-27 08:36:58.830371 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/km.js
--rw-r--r--   0        0        0    13604 2024-03-27 08:36:58.830803 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ko.js
--rw-r--r--   0        0        0    18533 2024-03-27 08:36:58.831033 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ku.js
--rw-r--r--   0        0        0    13787 2024-03-27 08:36:58.831370 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/lt.js
--rw-r--r--   0        0        0    14013 2024-03-27 08:36:58.831702 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/lv.js
--rw-r--r--   0        0        0    14072 2024-03-27 08:36:58.832006 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/mk.js
--rw-r--r--   0        0        0    16013 2024-03-27 08:36:58.832312 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/mn.js
--rw-r--r--   0        0        0    12801 2024-03-27 08:36:58.832637 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ms.js
--rw-r--r--   0        0        0    12872 2024-03-27 08:36:58.832903 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/nb.js
--rw-r--r--   0        0        0    13274 2024-03-27 08:36:58.833202 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/nl.js
--rw-r--r--   0        0        0    12917 2024-03-27 08:36:58.833429 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/no.js
--rw-r--r--   0        0        0    14222 2024-03-27 08:36:58.833591 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/oc.js
--rw-r--r--   0        0        0    14008 2024-03-27 08:36:58.833856 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pl.js
--rw-r--r--   0        0        0    14028 2024-03-27 08:36:58.834089 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pt-br.js
--rw-r--r--   0        0        0    13937 2024-03-27 08:36:58.834355 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pt.js
--rw-r--r--   0        0        0    14562 2024-03-27 08:36:58.834607 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ro.js
--rw-r--r--   0        0        0    19388 2024-03-27 08:36:58.834803 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ru.js
--rw-r--r--   0        0        0    17745 2024-03-27 08:36:58.835027 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/si.js
--rw-r--r--   0        0        0    13968 2024-03-27 08:36:58.835337 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sk.js
--rw-r--r--   0        0        0    13157 2024-03-27 08:36:58.835684 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sl.js
--rw-r--r--   0        0        0    14209 2024-03-27 08:36:58.835922 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sq.js
--rw-r--r--   0        0        0    13226 2024-03-27 08:36:58.836159 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sr-latn.js
--rw-r--r--   0        0        0    18199 2024-03-27 08:36:58.836301 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sr.js
--rw-r--r--   0        0        0    13032 2024-03-27 08:36:58.836577 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sv.js
--rw-r--r--   0        0        0    19588 2024-03-27 08:36:58.836793 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/th.js
--rw-r--r--   0        0        0    13898 2024-03-27 08:36:58.837107 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/tr.js
--rw-r--r--   0        0        0    16206 2024-03-27 08:36:58.837385 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/tt.js
--rw-r--r--   0        0        0    18512 2024-03-27 08:36:58.837589 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ug.js
--rw-r--r--   0        0        0    19509 2024-03-27 08:36:58.837809 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/uk.js
--rw-r--r--   0        0        0    15078 2024-03-27 08:36:58.838109 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/vi.js
--rw-r--r--   0        0        0    12353 2024-03-27 08:36:58.838366 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/zh-cn.js
--rw-r--r--   0        0        0    12277 2024-03-27 08:36:58.838590 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/zh.js
--rw-r--r--   0        0        0     2953 2024-03-27 08:36:58.838756 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
--rw-r--r--   0        0        0      887 2024-03-27 08:36:58.838893 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4156 2024-03-27 08:36:58.839044 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
--rw-r--r--   0        0        0     4351 2024-03-27 08:36:58.839190 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
--rw-r--r--   0        0        0     4332 2024-03-27 08:36:58.839311 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
--rw-r--r--   0        0        0     4565 2024-03-27 08:36:58.839476 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
--rw-r--r--   0        0        0     4788 2024-03-27 08:36:58.839631 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4938 2024-03-27 08:36:58.839774 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4389 2024-03-27 08:36:58.839942 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
--rw-r--r--   0        0        0     4247 2024-03-27 08:36:58.840067 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
--rw-r--r--   0        0        0     4712 2024-03-27 08:36:58.840153 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4656 2024-03-27 08:36:58.840300 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
--rw-r--r--   0        0        0     7631 2024-03-27 08:36:58.840456 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
--rw-r--r--   0        0        0     4203 2024-03-27 08:36:58.840543 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4203 2024-03-27 08:36:58.840668 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4200 2024-03-27 08:36:58.840803 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
--rw-r--r--   0        0        0     4797 2024-03-27 08:36:58.840935 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4893 2024-03-27 08:36:58.841006 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4799 2024-03-27 08:36:58.841129 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
--rw-r--r--   0        0        0     4418 2024-03-27 08:36:58.841280 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
--rw-r--r--   0        0        0     4505 2024-03-27 08:36:58.841371 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
--rw-r--r--   0        0        0     6152 2024-03-27 08:36:58.841545 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4760 2024-03-27 08:36:58.841673 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
--rw-r--r--   0        0        0     4202 2024-03-27 08:36:58.841812 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
--rw-r--r--   0        0        0     4922 2024-03-27 08:36:58.841955 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     5309 2024-03-27 08:36:58.842085 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
--rw-r--r--   0        0        0     4814 2024-03-27 08:36:58.842251 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
--rw-r--r--   0        0        0     4410 2024-03-27 08:36:58.842392 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
--rw-r--r--   0        0        0     4955 2024-03-27 08:36:58.842533 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
--rw-r--r--   0        0        0     4214 2024-03-27 08:36:58.842681 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
--rw-r--r--   0        0        0     4281 2024-03-27 08:36:58.842819 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4766 2024-03-27 08:36:58.842973 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4039 2024-03-27 08:36:58.843092 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
--rw-r--r--   0        0        0     5237 2024-03-27 08:36:58.843201 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
--rw-r--r--   0        0        0     5200 2024-03-27 08:36:58.843327 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
--rw-r--r--   0        0        0     5218 2024-03-27 08:36:58.843452 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
--rw-r--r--   0        0        0     5599 2024-03-27 08:36:58.843592 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
--rw-r--r--   0        0        0     6033 2024-03-27 08:36:58.843732 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4209 2024-03-27 08:36:58.843857 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
--rw-r--r--   0        0        0     4832 2024-03-27 08:36:58.843990 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
--rw-r--r--   0        0        0     4591 2024-03-27 08:36:58.844115 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
--rw-r--r--   0        0        0     4207 2024-03-27 08:36:58.844220 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
--rw-r--r--   0        0        0     4457 2024-03-27 08:36:58.844334 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4532 2024-03-27 08:36:58.844484 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
--rw-r--r--   0        0        0     4443 2024-03-27 08:36:58.844609 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
--rw-r--r--   0        0        0     5098 2024-03-27 08:36:58.844711 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
--rw-r--r--   0        0        0     5160 2024-03-27 08:36:58.844838 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
--rw-r--r--   0        0        0     4927 2024-03-27 08:36:58.844966 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4568 2024-03-27 08:36:58.845105 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4559 2024-03-27 08:36:58.845213 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
--rw-r--r--   0        0        0     6646 2024-03-27 08:36:58.845338 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
--rw-r--r--   0        0        0     6145 2024-03-27 08:36:58.845453 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
--rw-r--r--   0        0        0     4769 2024-03-27 08:36:58.845564 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4548 2024-03-27 08:36:58.845694 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
--rw-r--r--   0        0        0     4933 2024-03-27 08:36:58.845809 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4896 2024-03-27 08:36:58.845922 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7514 2024-03-27 08:36:58.846042 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
--rw-r--r--   0        0        0     4369 2024-03-27 08:36:58.846156 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4578 2024-03-27 08:36:58.846278 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
--rw-r--r--   0        0        0     4579 2024-03-27 08:36:58.846392 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
--rw-r--r--   0        0        0     4518 2024-03-27 08:36:58.846513 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
--rw-r--r--   0        0        0     6936 2024-03-27 08:36:58.846671 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6926 2024-03-27 08:36:58.846788 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
--rw-r--r--   0        0        0     5400 2024-03-27 08:36:58.846908 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4148 2024-03-27 08:36:58.847025 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4357 2024-03-27 08:36:58.847138 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
--rw-r--r--   0        0        0     1934 2024-03-27 08:36:58.847247 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/about.js
--rw-r--r--   0        0        0    12236 2024-03-27 08:36:58.847437 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
--rw-r--r--   0        0        0     5650 2024-03-27 08:36:58.847545 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/logo_ckeditor.png
--rw-r--r--   0        0        0     3809 2024-03-27 08:36:58.847712 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/clipboard/dialogs/paste.js
--rw-r--r--   0        0        0      166 2024-03-27 08:36:58.847839 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/dialog/dialogDefinition.js
--rw-r--r--   0        0        0      231 2024-03-27 08:36:58.847949 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/dialog/styles/dialog.css
--rw-r--r--   0        0        0     5692 2024-03-27 08:36:58.848093 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/icons.png
--rw-r--r--   0        0        0    18632 2024-03-27 08:36:58.848248 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/icons_hidpi.png
--rw-r--r--   0        0        0    21529 2024-03-27 08:36:58.848475 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/image/dialogs/image.js
--rw-r--r--   0        0        0     1610 2024-03-27 08:36:58.848611 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/image/images/noimage.png
--rw-r--r--   0        0        0     2207 2024-03-27 08:36:58.848725 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/dialogs/anchor.js
--rw-r--r--   0        0        0    13234 2024-03-27 08:36:58.848992 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/dialogs/link.js
--rw-r--r--   0        0        0      752 2024-03-27 08:36:58.849097 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/images/anchor.png
--rw-r--r--   0        0        0     1109 2024-03-27 08:36:58.849197 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/images/hidpi/anchor.png
--rw-r--r--   0        0        0      176 2024-03-27 08:36:58.849305 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
--rw-r--r--   0        0        0      199 2024-03-27 08:36:58.849400 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/magicline/images/hidpi/icon.png
--rw-r--r--   0        0        0      138 2024-03-27 08:36:58.849492 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/magicline/images/icon-rtl.png
--rw-r--r--   0        0        0      133 2024-03-27 08:36:58.849599 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/magicline/images/icon.png
--rw-r--r--   0        0        0     2209 2024-03-27 08:36:58.849753 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromgdocs/filter/default.js
--rw-r--r--   0        0        0     3510 2024-03-27 08:36:58.849898 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromlibreoffice/filter/default.js
--rw-r--r--   0        0        0    19902 2024-03-27 08:36:58.850050 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromword/filter/default.js
--rw-r--r--   0        0        0    10380 2024-03-27 08:36:58.850275 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/common.js
--rw-r--r--   0        0        0     3932 2024-03-27 08:36:58.850347 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/image.js
--rw-r--r--   0        0        0      221 2024-03-27 08:36:58.850419 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/CHANGELOG.md
--rw-r--r--   0        0        0     1476 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/LICENSE.md
--rw-r--r--   0        0        0     4565 2024-03-27 08:36:58.850534 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/README.md
--rw-r--r--   0        0        0      396 2024-03-27 08:36:58.850602 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/dialog.css
--rw-r--r--   0        0        0    16136 2024-03-27 08:36:58.850817 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/options.js
--rw-r--r--   0        0        0     1302 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/toolbar.css
--rw-r--r--   0        0        0      356 2024-03-27 08:36:58.850962 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
--rw-r--r--   0        0        0      738 2024-03-27 08:36:58.851090 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
--rw-r--r--   0        0        0     4547 2024-03-27 08:36:58.851232 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/af.js
--rw-r--r--   0        0        0     4796 2024-03-27 08:36:58.851351 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ar.js
--rw-r--r--   0        0        0     3407 2024-03-27 08:36:58.851426 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/az.js
--rw-r--r--   0        0        0     4820 2024-03-27 08:36:58.851565 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/bg.js
--rw-r--r--   0        0        0     5028 2024-03-27 08:36:58.851691 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ca.js
--rw-r--r--   0        0        0     4985 2024-03-27 08:36:58.851844 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cs.js
--rw-r--r--   0        0        0     4909 2024-03-27 08:36:58.851959 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cy.js
--rw-r--r--   0        0        0     3380 2024-03-27 08:36:58.852068 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/da.js
--rw-r--r--   0        0        0     4807 2024-03-27 08:36:58.852143 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
--rw-r--r--   0        0        0     4798 2024-03-27 08:36:58.852257 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de.js
--rw-r--r--   0        0        0     7746 2024-03-27 08:36:58.852368 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/el.js
--rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852436 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
--rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852512 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
--rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852687 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
--rw-r--r--   0        0        0     4561 2024-03-27 08:36:58.852820 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en.js
--rw-r--r--   0        0        0     4082 2024-03-27 08:36:58.852936 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eo.js
--rw-r--r--   0        0        0     4790 2024-03-27 08:36:58.853011 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
--rw-r--r--   0        0        0     4961 2024-03-27 08:36:58.853127 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es.js
--rw-r--r--   0        0        0     3831 2024-03-27 08:36:58.853241 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/et.js
--rw-r--r--   0        0        0     4563 2024-03-27 08:36:58.853317 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eu.js
--rw-r--r--   0        0        0     5786 2024-03-27 08:36:58.853427 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fa.js
--rw-r--r--   0        0        0     4599 2024-03-27 08:36:58.853530 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fi.js
--rw-r--r--   0        0        0     3234 2024-03-27 08:36:58.853634 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
--rw-r--r--   0        0        0     3870 2024-03-27 08:36:58.853766 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr.js
--rw-r--r--   0        0        0     5018 2024-03-27 08:36:58.853893 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/gl.js
--rw-r--r--   0        0        0     5000 2024-03-27 08:36:58.854010 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/he.js
--rw-r--r--   0        0        0     4405 2024-03-27 08:36:58.854128 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hr.js
--rw-r--r--   0        0        0     4149 2024-03-27 08:36:58.854243 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hu.js
--rw-r--r--   0        0        0     4568 2024-03-27 08:36:58.854346 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/id.js
--rw-r--r--   0        0        0     5034 2024-03-27 08:36:58.854453 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/it.js
--rw-r--r--   0        0        0     3998 2024-03-27 08:36:58.854558 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ja.js
--rw-r--r--   0        0        0     4765 2024-03-27 08:36:58.854651 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/km.js
--rw-r--r--   0        0        0     4934 2024-03-27 08:36:58.854754 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ko.js
--rw-r--r--   0        0        0     7578 2024-03-27 08:36:58.854858 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ku.js
--rw-r--r--   0        0        0     4606 2024-03-27 08:36:58.854964 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lt.js
--rw-r--r--   0        0        0     5036 2024-03-27 08:36:58.855071 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lv.js
--rw-r--r--   0        0        0     3446 2024-03-27 08:36:58.855172 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nb.js
--rw-r--r--   0        0        0     4740 2024-03-27 08:36:58.855281 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nl.js
--rw-r--r--   0        0        0     3446 2024-03-27 08:36:58.855381 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/no.js
--rw-r--r--   0        0        0     3844 2024-03-27 08:36:58.855449 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/oc.js
--rw-r--r--   0        0        0     4343 2024-03-27 08:36:58.855588 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pl.js
--rw-r--r--   0        0        0     3844 2024-03-27 08:36:58.855694 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
--rw-r--r--   0        0        0     4809 2024-03-27 08:36:58.855803 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt.js
--rw-r--r--   0        0        0     4692 2024-03-27 08:36:58.855872 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ro.js
--rw-r--r--   0        0        0     7561 2024-03-27 08:36:58.855996 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ru.js
--rw-r--r--   0        0        0     4902 2024-03-27 08:36:58.856110 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/si.js
--rw-r--r--   0        0        0     4778 2024-03-27 08:36:58.856242 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sk.js
--rw-r--r--   0        0        0     4363 2024-03-27 08:36:58.856360 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sl.js
--rw-r--r--   0        0        0     5005 2024-03-27 08:36:58.856472 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sq.js
--rw-r--r--   0        0        0     4728 2024-03-27 08:36:58.856546 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
--rw-r--r--   0        0        0     7530 2024-03-27 08:36:58.856619 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr.js
--rw-r--r--   0        0        0     3498 2024-03-27 08:36:58.856725 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sv.js
--rw-r--r--   0        0        0     4690 2024-03-27 08:36:58.856826 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/th.js
--rw-r--r--   0        0        0     4493 2024-03-27 08:36:58.856936 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tr.js
--rw-r--r--   0        0        0     6743 2024-03-27 08:36:58.857049 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tt.js
--rw-r--r--   0        0        0     5017 2024-03-27 08:36:58.857170 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ug.js
--rw-r--r--   0        0        0     6384 2024-03-27 08:36:58.857274 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/uk.js
--rw-r--r--   0        0        0     6099 2024-03-27 08:36:58.857376 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/vi.js
--rw-r--r--   0        0        0     4395 2024-03-27 08:36:58.857478 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
--rw-r--r--   0        0        0     4175 2024-03-27 08:36:58.857593 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh.js
--rw-r--r--   0        0        0     5005 2024-03-27 08:36:58.857726 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/specialchar.js
--rw-r--r--   0        0        0     9043 2024-03-27 08:36:58.857909 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/table/dialogs/table.js
--rw-r--r--   0        0        0     1109 2024-03-27 08:36:58.858052 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/tableselection/styles/tableselection.css
--rw-r--r--   0        0        0     7354 2024-03-27 08:36:58.858181 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/tabletools/dialogs/tableCell.js
--rw-r--r--   0        0        0      220 2024-03-27 08:36:58.858318 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/widget/images/handle.png
--rw-r--r--   0        0        0    67340 2024-03-27 08:36:58.858668 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/css/samples.css
--rw-r--r--   0        0        0      383 2024-03-27 08:36:58.858798 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/github-top.png
--rw-r--r--   0        0        0    13086 2024-03-27 08:36:58.859050 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/header-bg.png
--rw-r--r--   0        0        0      123 2024-03-27 08:36:58.859145 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/header-separator.png
--rw-r--r--   0        0        0     5634 2024-03-27 08:36:58.859237 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/logo.png
--rw-r--r--   0        0        0    10887 2024-03-27 08:36:58.859344 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/logo.svg
--rw-r--r--   0        0        0    12029 2024-03-27 08:36:58.859505 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/navigation-tip.png
--rw-r--r--   0        0        0     7234 2024-03-27 08:36:58.859645 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/index.html
--rw-r--r--   0        0        0     1594 2024-03-27 08:36:58.859750 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/js/sample.js
--rw-r--r--   0        0        0     6426 2024-03-27 08:36:58.859870 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/js/sf.js
--rw-r--r--   0        0        0     2911 2024-03-27 08:36:58.859981 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/ajax.html
--rw-r--r--   0        0        0     7545 2024-03-27 08:36:58.860098 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/api.html
--rw-r--r--   0        0        0     2523 2024-03-27 08:36:58.860207 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/appendto.html
--rw-r--r--   0        0        0     4283 2024-03-27 08:36:58.860312 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/inlineall/logo.png
--rw-r--r--   0        0        0     2161 2024-03-27 08:36:58.860417 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css
--rw-r--r--   0        0        0     1627 2024-03-27 08:36:58.860526 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/posteddata.php
--rw-r--r--   0        0        0    14449 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/sample.jpg
--rw-r--r--   0        0        0     1461 2024-03-27 08:36:58.860633 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/uilanguages/languages.js
--rw-r--r--   0        0        0    47840 2024-03-27 08:36:58.860818 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/datafiltering.html
--rw-r--r--   0        0        0      895 2024-03-27 08:36:58.860941 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/dialog/assets/my_dialog.js
--rw-r--r--   0        0        0     7590 2024-03-27 08:36:58.861067 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/dialog/dialog.html
--rw-r--r--   0        0        0     4893 2024-03-27 08:36:58.861179 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/divreplace.html
--rw-r--r--   0        0        0     4598 2024-03-27 08:36:58.861295 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/enterkey/enterkey.html
--rw-r--r--   0        0        0     7565 2024-03-27 08:36:58.861448 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/htmlwriter/outputhtml.html
--rw-r--r--   0        0        0     6054 2024-03-27 08:36:58.861567 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/index.html
--rw-r--r--   0        0        0    10399 2024-03-27 08:36:58.861721 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlineall.html
--rw-r--r--   0        0        0     6395 2024-03-27 08:36:58.861841 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlinebycode.html
--rw-r--r--   0        0        0     5125 2024-03-27 08:36:58.861956 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlinetextarea.html
--rw-r--r--   0        0        0     7754 2024-03-27 08:36:58.862073 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/jquery.html
--rw-r--r--   0        0        0     8585 2024-03-27 08:36:58.862229 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/magicline/magicline.html
--rw-r--r--   0        0        0     3132 2024-03-27 08:36:58.862377 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/readonly.html
--rw-r--r--   0        0        0     7234 2024-03-27 08:36:58.862493 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/replacebyclass.html
--rw-r--r--   0        0        0     7119 2024-03-27 08:36:58.862614 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/replacebycode.html
--rw-r--r--   0        0        0     5112 2024-03-27 08:36:58.862729 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample.css
--rw-r--r--   0        0        0     1693 2024-03-27 08:36:58.862825 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample.js
--rw-r--r--   0        0        0      807 2024-03-27 08:36:58.862920 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample_posteddata.php
--rw-r--r--   0        0        0     2609 2024-03-27 08:36:58.863020 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/tabindex.html
--rw-r--r--   0        0        0     9122 2024-03-27 08:36:58.863173 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/toolbar/toolbar.html
--rw-r--r--   0        0        0     2810 2024-03-27 08:36:58.863286 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/uicolor.html
--rw-r--r--   0        0        0     4741 2024-03-27 08:36:58.863424 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/uilanguages.html
--rw-r--r--   0        0        0     8311 2024-03-27 08:36:58.863572 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/wysiwygarea/fullpage.html
--rw-r--r--   0        0        0     7233 2024-03-27 08:36:58.863692 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/xhtmlstyle.html
--rw-r--r--   0        0        0     1758 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/css/fontello.css
--rw-r--r--   0        0        0      188 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/LICENSE.txt
--rw-r--r--   0        0        0      557 2023-12-08 18:07:26.684149 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/config.json
--rw-r--r--   0        0        0     4988 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.eot
--rw-r--r--   0        0        0     1701 2023-12-08 18:07:26.684402 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.svg
--rw-r--r--   0        0        0     4820 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.ttf
--rw-r--r--   0        0        0     2904 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.woff
--rw-r--r--   0        0        0    15808 2024-03-27 08:36:58.863921 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/index.html
--rw-r--r--   0        0        0     6523 2024-03-27 08:36:58.864052 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
--rw-r--r--   0        0        0     3838 2024-03-27 08:36:58.864165 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js
--rw-r--r--   0        0        0    16651 2024-03-27 08:36:58.864280 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js
--rw-r--r--   0        0        0     6850 2024-03-27 08:36:58.864475 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js
--rw-r--r--   0        0        0     1094 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/LICENSE
--rw-r--r--   0        0        0     8096 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.css
--rw-r--r--   0        0        0   148874 2024-03-27 08:36:58.865555 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.js
--rw-r--r--   0        0        0    12285 2024-03-27 08:36:58.865736 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/javascript.js
--rw-r--r--   0        0        0      851 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/neo.css
--rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.css
--rw-r--r--   0        0        0     8080 2024-03-27 08:36:58.865871 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.js
--rw-r--r--   0        0        0    13630 2024-03-27 08:36:58.866111 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog.css
--rw-r--r--   0        0        0    14653 2024-03-27 08:36:58.866266 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie.css
--rw-r--r--   0        0        0    15202 2024-03-27 08:36:58.866416 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie8.css
--rw-r--r--   0        0        0    14682 2024-03-27 08:36:58.866559 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_iequirks.css
--rw-r--r--   0        0        0    35902 2024-03-27 08:36:58.866699 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor.css
--rw-r--r--   0        0        0    35983 2024-03-27 08:36:58.866811 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_gecko.css
--rw-r--r--   0        0        0    36901 2024-03-27 08:36:58.866896 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie.css
--rw-r--r--   0        0        0    37707 2024-03-27 08:36:58.866991 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie8.css
--rw-r--r--   0        0        0    37550 2024-03-27 08:36:58.867085 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_iequirks.css
--rw-r--r--   0        0        0     5692 2024-03-27 08:36:58.867195 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons.png
--rw-r--r--   0        0        0    18632 2024-03-27 08:36:58.867294 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons_hidpi.png
--rw-r--r--   0        0        0      191 2024-03-27 08:36:58.867401 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/arrow.png
--rw-r--r--   0        0        0      615 2024-03-27 08:36:58.867463 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/close.png
--rw-r--r--   0        0        0     1238 2024-03-27 08:36:58.867578 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/close.png
--rw-r--r--   0        0        0     1071 2024-03-27 08:36:58.867645 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
--rw-r--r--   0        0        0     1062 2024-03-27 08:36:58.867710 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock.png
--rw-r--r--   0        0        0     1623 2024-03-27 08:36:58.867777 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
--rw-r--r--   0        0        0      511 2024-03-27 08:36:58.867843 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/lock-open.png
--rw-r--r--   0        0        0      506 2024-03-27 08:36:58.867906 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/lock.png
--rw-r--r--   0        0        0      757 2024-03-27 08:36:58.867968 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/refresh.png
--rw-r--r--   0        0        0     2984 2024-03-27 08:36:58.868188 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/spinner.gif
--rw-r--r--   0        0        0     2238 2024-03-27 08:36:58.868273 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/readme.md
--rw-r--r--   0        0        0     5577 2024-03-27 08:36:58.868402 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/styles.js
--rw-r--r--   0        0        0     6297 2024-03-27 08:36:58.868516 abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/vendor/promise.js
--rw-r--r--   0        0        0     4554 2023-12-08 18:07:26.696227 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/css/jquery.dataTables.css
--rw-r--r--   0        0        0     4477 2023-12-08 18:07:26.696469 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/css/jquery.dataTables_themeroller.css
--rw-r--r--   0        0        0    27490 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/Sorting icons.psd
--rw-r--r--   0        0        0      345 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/back_disabled.png
--rw-r--r--   0        0        0      459 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/back_enabled.png
--rw-r--r--   0        0        0      457 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/back_enabled_hover.png
--rw-r--r--   0        0        0      894 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/favicon.ico
--rw-r--r--   0        0        0      350 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/forward_disabled.png
--rw-r--r--   0        0        0      468 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/forward_enabled.png
--rw-r--r--   0        0        0      467 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/forward_enabled_hover.png
--rw-r--r--   0        0        0      174 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/sort_asc.png
--rw-r--r--   0        0        0      174 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/sort_asc_disabled.png
--rw-r--r--   0        0        0      209 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/sort_both.png
--rw-r--r--   0        0        0      172 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/sort_desc.png
--rw-r--r--   0        0        0      159 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/sort_desc_disabled.png
--rw-r--r--   0        0        0   377686 2023-12-08 18:07:26.698522 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/js/jquery.dataTables.js
--rw-r--r--   0        0        0    70857 2023-12-08 18:07:26.699408 abilian_sbe-1.1.8/src/abilian/web/resources/datatables/js/jquery.dataTables.min.js
--rw-r--r--   0        0        0     1635 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.camera.swf
--rw-r--r--   0        0        0     2136 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.image.swf
--rw-r--r--   0        0        0    32484 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.swf
--rw-r--r--   0        0        0    84949 2023-12-08 18:07:26.700061 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.html5.js
--rw-r--r--   0        0        0    34040 2023-12-08 18:07:26.700460 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.html5.min.js
--rw-r--r--   0        0        0   104385 2023-12-08 18:07:26.701379 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.js
--rw-r--r--   0        0        0    43718 2023-12-08 18:07:26.702196 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.min.js
--rw-r--r--   0        0        0     1382 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/LICENSE
--rw-r--r--   0        0        0    11508 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/FileAPI.exif.js
--rw-r--r--   0        0        0    14866 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/FileAPI.id3.js
--rwxr-xr-x   0        0        0    74053 2023-12-08 18:07:26.702774 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/caman.full.min.js
--rwxr-xr-x   0        0        0    46149 2023-12-08 18:07:26.703173 abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/caman.min.js
--rw-r--r--   0        0        0    32318 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/css/font-awesome.css
--rw-r--r--   0        0        0    26711 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/css/font-awesome.min.css
--rw-r--r--   0        0        0   106260 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/FontAwesome.otf
--rw-r--r--   0        0        0    68875 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.eot
--rw-r--r--   0        0        0   355981 2024-03-23 14:18:13.144763 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.svg
--rw-r--r--   0        0        0   138204 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.ttf
--rw-r--r--   0        0        0    81284 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff
--rw-r--r--   0        0        0    64464 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff2
--rw-r--r--   0        0        0      713 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/animated.less
--rw-r--r--   0        0        0      585 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/bordered-pulled.less
--rw-r--r--   0        0        0      452 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/core.less
--rw-r--r--   0        0        0      119 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/fixed-width.less
--rw-r--r--   0        0        0      465 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/font-awesome.less
--rw-r--r--   0        0        0    42489 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/icons.less
--rw-r--r--   0        0        0      370 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/larger.less
--rw-r--r--   0        0        0      377 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/list.less
--rw-r--r--   0        0        0      926 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/mixins.less
--rw-r--r--   0        0        0      770 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/path.less
--rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/rotated-flipped.less
--rw-r--r--   0        0        0      476 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/stacked.less
--rw-r--r--   0        0        0    19203 2023-12-08 18:07:26.705406 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/variables.less
--rw-r--r--   0        0        0      715 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_animated.scss
--rw-r--r--   0        0        0      592 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_bordered-pulled.scss
--rw-r--r--   0        0        0      459 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_core.scss
--rw-r--r--   0        0        0      120 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_fixed-width.scss
--rw-r--r--   0        0        0    43163 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_icons.scss
--rw-r--r--   0        0        0      375 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_larger.scss
--rw-r--r--   0        0        0      378 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_list.scss
--rw-r--r--   0        0        0      946 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_mixins.scss
--rw-r--r--   0        0        0      783 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_path.scss
--rw-r--r--   0        0        0      672 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_rotated-flipped.scss
--rw-r--r--   0        0        0      482 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_stacked.scss
--rw-r--r--   0        0        0    19284 2023-12-08 18:07:26.705733 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_variables.scss
--rw-r--r--   0        0        0      405 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/font-awesome.scss
--rw-r--r--   0        0        0     2299 2023-12-08 18:07:26.705997 abilian_sbe-1.1.8/src/abilian/web/resources/highlightjs/default.min.css
--rw-r--r--   0        0        0    34929 2023-12-08 18:07:26.706390 abilian_sbe-1.1.8/src/abilian/web/resources/highlightjs/highlight.min.js
--rw-r--r--   0        0        0    73763 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/img/abilian.png
--rw-r--r--   0        0        0     2242 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/img/avatar-default.png
--rw-r--r--   0        0        0     2413 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/img/logo-abilian-32x32.png
--rw-r--r--   0        0        0     2367 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/img/logo-abilian.png
--rw-r--r--   0        0        0   284394 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/jquery/js/jquery-1.11.3.js
--rw-r--r--   0        0        0    16621 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/jquery/js/jquery-migrate-1.2.1.js
--rw-r--r--   0        0        0     1883 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/abilian-namespace.js
--rw-r--r--   0        0        0     5096 2024-03-27 08:36:58.869020 abilian_sbe-1.1.8/src/abilian/web/resources/js/abilian.js
--rw-r--r--   0        0        0    26660 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/datatables-advanced-search.js
--rw-r--r--   0        0        0     4444 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/datatables-setup.js
--rw-r--r--   0        0        0     1187 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/base.js
--rw-r--r--   0        0        0     2420 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/delete.js
--rw-r--r--   0        0        0     3226 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/dynamic-row.js
--rw-r--r--   0        0        0     6988 2024-04-22 09:33:28.131121 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/file.js
--rw-r--r--   0        0        0     3012 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/image.js
--rw-r--r--   0        0        0     1910 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/richtext.js
--rw-r--r--   0        0        0     3046 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/select2.js
--rw-r--r--   0        0        0      783 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/tags.js
--rw-r--r--   0        0        0     1002 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/abilian.less
--rw-r--r--   0        0        0     1289 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/activities.less
--rw-r--r--   0        0        0      612 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/admin.less
--rw-r--r--   0        0        0       95 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/attachments.less
--rw-r--r--   0        0        0      575 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/comments.less
--rw-r--r--   0        0        0      157 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/compat.less
--rw-r--r--   0        0        0      987 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/datatables.less
--rw-r--r--   0        0        0     3050 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/form.less
--rw-r--r--   0        0        0      155 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/layout.less
--rw-r--r--   0        0        0      105 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/models.less
--rw-r--r--   0        0        0     1054 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/navbar.less
--rw-r--r--   0        0        0      624 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/print.less
--rw-r--r--   0        0        0      225 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/search.less
--rw-r--r--   0        0        0       74 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/user.less
--rw-r--r--   0        0        0      165 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/less/variables.less
--rw-r--r--   0        0        0      112 2023-12-08 18:07:26.706906 abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/cdn.txt
--rw-r--r--   0        0        0   151701 2023-12-08 18:07:26.708021 abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/d3.min.js
--rw-r--r--   0        0        0    12985 2023-12-08 18:07:26.708286 abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/nv.d3.css
--rw-r--r--   0        0        0   587960 2023-12-08 18:07:26.710483 abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/nv.d3.js
--rw-r--r--   0        0        0     4047 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/requirejs/domReady.js
--rw-r--r--   0        0        0    86482 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/requirejs/require.js
--rw-r--r--   0        0        0     4858 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/CONTRIBUTING.md
--rw-r--r--   0        0        0      939 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/LICENSE
--rw-r--r--   0        0        0     4727 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/README.md
--rw-r--r--   0        0        0      206 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/bower.json
--rw-r--r--   0        0        0     1732 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/component.json
--rw-r--r--   0        0        0      637 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/composer.json
--rw-r--r--   0        0        0      678 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/package.json
--rwxr-xr-x   0        0        0     1490 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/release.sh
--rw-r--r--   0        0        0    16890 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2-bootstrap.css
--rw-r--r--   0        0        0     1849 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2-spinner.gif
--rw-r--r--   0        0        0    19457 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.css
--rw-r--r--   0        0        0     1030 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.jquery.json
--rw-r--r--   0        0        0   148536 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.js
--rw-r--r--   0        0        0    66596 2023-12-08 18:07:26.711090 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.min.js
--rw-r--r--   0        0        0      529 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.png
--rw-r--r--   0        0        0     1389 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ar.js
--rw-r--r--   0        0        0     1003 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_az.js
--rw-r--r--   0        0        0     1081 2023-12-08 18:07:26.711330 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_bg.js
--rw-r--r--   0        0        0      952 2023-12-08 18:07:26.711571 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ca.js
--rw-r--r--   0        0        0     1988 2023-12-08 18:07:26.711836 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_cs.js
--rw-r--r--   0        0        0      853 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_da.js
--rw-r--r--   0        0        0     1014 2023-12-08 18:07:26.712200 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_de.js
--rw-r--r--   0        0        0     1128 2023-12-08 18:07:26.712422 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_el.js
--rw-r--r--   0        0        0     1102 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_en.js.template
--rw-r--r--   0        0        0     1177 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_es.js
--rw-r--r--   0        0        0      886 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_et.js
--rw-r--r--   0        0        0     1313 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_eu.js
--rw-r--r--   0        0        0     1207 2023-12-08 18:07:26.712658 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fa.js
--rw-r--r--   0        0        0      940 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fi.js
--rw-r--r--   0        0        0     1077 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fr.js
--rw-r--r--   0        0        0     1339 2023-12-08 18:07:26.712886 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_gl.js
--rw-r--r--   0        0        0      885 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_he.js
--rw-r--r--   0        0        0     1002 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_hr.js
--rw-r--r--   0        0        0      802 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_hu.js
--rw-r--r--   0        0        0      891 2023-12-08 18:07:26.713117 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_id.js
--rw-r--r--   0        0        0      855 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_is.js
--rw-r--r--   0        0        0      866 2023-12-08 18:07:26.713388 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_it.js
--rw-r--r--   0        0        0      812 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ja.js
--rw-r--r--   0        0        0     1078 2023-12-08 18:07:26.713638 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ka.js
--rw-r--r--   0        0        0      871 2023-12-08 18:07:26.713909 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ko.js
--rw-r--r--   0        0        0     1144 2023-12-08 18:07:26.714151 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_lt.js
--rw-r--r--   0        0        0      999 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_lv.js
--rw-r--r--   0        0        0     1064 2023-12-08 18:07:26.714300 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_mk.js
--rw-r--r--   0        0        0      836 2023-12-08 18:07:26.714533 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ms.js
--rw-r--r--   0        0        0     1145 2023-12-08 18:07:26.714857 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_nb.js
--rw-r--r--   0        0        0      846 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_nl.js
--rw-r--r--   0        0        0     2015 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pl.js
--rw-r--r--   0        0        0      969 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pt-BR.js
--rw-r--r--   0        0        0      891 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pt-PT.js
--rw-r--r--   0        0        0      902 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ro.js
--rw-r--r--   0        0        0     1058 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_rs.js
--rw-r--r--   0        0        0     1171 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ru.js
--rw-r--r--   0        0        0     1948 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_sk.js
--rw-r--r--   0        0        0      847 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_sv.js
--rw-r--r--   0        0        0     1063 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_th.js
--rw-r--r--   0        0        0      831 2023-12-08 18:07:26.715096 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_tr.js
--rw-r--r--   0        0        0      904 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ug-CN.js
--rw-r--r--   0        0        0     1415 2023-12-08 18:07:26.715322 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_uk.js
--rw-r--r--   0        0        0      959 2023-12-08 18:07:26.715543 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_vi.js
--rw-r--r--   0        0        0      762 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_zh-CN.js
--rw-r--r--   0        0        0      774 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_zh-TW.js
--rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2x2.png
--rw-r--r--   0        0        0    15246 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/hogan-2.0.0.js
--rw-r--r--   0        0        0    49022 2023-12-08 18:07:26.715929 abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js
--rw-r--r--   0        0        0     1394 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.css
--rw-r--r--   0        0        0      736 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.less
--rw-r--r--   0        0        0    21804 2023-12-08 18:07:26.716267 abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.min.js
--rw-r--r--   0        0        0      646 2024-04-22 07:49:45.045295 abilian_sbe-1.1.8/src/abilian/web/search/__init__.py
--rw-r--r--   0        0        0     7183 2024-04-22 07:49:45.045624 abilian_sbe-1.1.8/src/abilian/web/search/criterion.py
--rw-r--r--   0        0        0      318 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/search/templates/search/_base.html
--rw-r--r--   0        0        0     4163 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/search/templates/search/search.html
--rw-r--r--   0        0        0     5804 2024-02-07 15:10:35.387923 abilian_sbe-1.1.8/src/abilian/web/search/views.py
--rw-r--r--   0        0        0      277 2024-04-22 07:49:45.046196 abilian_sbe-1.1.8/src/abilian/web/tags/__init__.py
--rw-r--r--   0        0        0     9266 2024-03-23 14:15:18.718464 abilian_sbe-1.1.8/src/abilian/web/tags/admin.py
--rw-r--r--   0        0        0     2463 2024-04-22 07:49:45.046500 abilian_sbe-1.1.8/src/abilian/web/tags/criterion.py
--rw-r--r--   0        0        0     4193 2024-03-23 14:15:18.719515 abilian_sbe-1.1.8/src/abilian/web/tags/extension.py
--rw-r--r--   0        0        0     2692 2024-03-25 13:17:52.075808 abilian_sbe-1.1.8/src/abilian/web/tags/forms.py
--rw-r--r--   0        0        0      758 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/tags/templates/admin/tags.html
--rw-r--r--   0        0        0     2322 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/tags/templates/admin/tags_ns.html
--rw-r--r--   0        0        0     3470 2024-03-25 13:17:52.075979 abilian_sbe-1.1.8/src/abilian/web/tags/views.py
--rw-r--r--   0        0        0     4537 2024-03-25 13:17:52.076246 abilian_sbe-1.1.8/src/abilian/web/templates/abilian_base.html
--rw-r--r--   0        0        0     2634 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/abilian_init.js
--rw-r--r--   0        0        0       35 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/base.html
--rw-r--r--   0        0        0      160 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/breadcrumbs.html
--rw-r--r--   0        0        0      826 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/actions_panel.html
--rw-r--r--   0        0        0     1292 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/indexing_panel.html
--rw-r--r--   0        0        0     1179 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/security_info_panel.html
--rw-r--r--   0        0        0     1196 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/signals_panel.html
--rw-r--r--   0        0        0      457 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/default/avatar.svg
--rw-r--r--   0        0        0     3846 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/default/list_view.html
--rw-r--r--   0        0        0      397 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/default/object_edit.html
--rw-r--r--   0        0        0      715 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/default/object_view.html
--rw-r--r--   0        0        0     2768 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/default/single_view.html
--rw-r--r--   0        0        0      242 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/error403.html
--rw-r--r--   0        0        0      222 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/error404.html
--rw-r--r--   0        0        0      261 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/error500.html
--rw-r--r--   0        0        0      459 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/flash-messages.html
--rw-r--r--   0        0        0      157 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/index.html
--rw-r--r--   0        0        0      902 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/activity.html
--rw-r--r--   0        0        0      697 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/attachment.html
--rw-r--r--   0        0        0     2887 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/attachment_default.html
--rw-r--r--   0        0        0     2394 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/audit.html
--rw-r--r--   0        0        0     2028 2022-04-04 15:58:58.324607 abilian_sbe-1.1.8/src/abilian/web/templates/macros/box.html
--rw-r--r--   0        0        0      295 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/buttons.html
--rw-r--r--   0        0        0     2628 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/comment.html
--rw-r--r--   0        0        0     4520 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/form.html
--rw-r--r--   0        0        0      536 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/recent.html
--rw-r--r--   0        0        0      492 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/table.html
--rw-r--r--   0        0        0     1399 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/tag.html
--rw-r--r--   0        0        0      544 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/macros/user.html
--rw-r--r--   0        0        0     2206 2022-04-12 15:39:37.791321 abilian_sbe-1.1.8/src/abilian/web/templates/navbar.html
--rw-r--r--   0        0        0      587 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/preferences/_base.html
--rw-r--r--   0        0        0     1094 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/preferences/user.html
--rw-r--r--   0        0        0      335 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/fieldlist.html
--rw-r--r--   0        0        0       90 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/fieldlist_view.html
--rw-r--r--   0        0        0     1152 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/file_input.html
--rw-r--r--   0        0        0      542 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/frontend_action_delete_confim.html
--rw-r--r--   0        0        0      450 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/horizontal_table.html
--rw-r--r--   0        0        0     1740 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/image_input.html
--rw-r--r--   0        0        0      505 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/model_fieldlist.html
--rw-r--r--   0        0        0      281 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/model_widget_edit.html
--rw-r--r--   0        0        0      226 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/model_widget_view.html
--rw-r--r--   0        0        0     2652 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_ajax_table.html
--rw-r--r--   0        0        0     2515 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_for_edit.html
--rw-r--r--   0        0        0     1194 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_single.html
--rw-r--r--   0        0        0     1727 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_table.html
--rw-r--r--   0        0        0      340 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/richtext.html
--rw-r--r--   0        0        0      219 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/select2ajax.html
--rw-r--r--   0        0        0      887 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/tabular_fieldlist_widget.html
--rw-r--r--   0        0        0      357 2021-09-16 12:23:36.000000 abilian_sbe-1.1.8/src/abilian/web/templates/widgets/timepicker.html
--rw-r--r--   0        0        0        0 2021-09-16 12:23:35.000000 abilian_sbe-1.1.8/src/abilian/web/tools/__init__.py
--rw-r--r--   0        0        0     3656 2024-02-07 15:10:35.389493 abilian_sbe-1.1.8/src/abilian/web/tools/debug_toolbar.py
--rw-r--r--   0        0        0      196 2024-03-23 14:15:18.709905 abilian_sbe-1.1.8/src/abilian/web/uploads/__init__.py
--rw-r--r--   0        0        0     6607 2024-03-25 13:17:52.076414 abilian_sbe-1.1.8/src/abilian/web/uploads/extension.py
--rw-r--r--   0        0        0     3122 2024-04-22 09:26:28.623044 abilian_sbe-1.1.8/src/abilian/web/uploads/views.py
--rw-r--r--   0        0        0     1483 2024-03-25 13:17:52.076803 abilian_sbe-1.1.8/src/abilian/web/util.py
--rw-r--r--   0        0        0      535 2024-02-07 15:10:35.390562 abilian_sbe-1.1.8/src/abilian/web/views/__init__.py
--rw-r--r--   0        0        0     3502 2024-03-25 13:17:52.077071 abilian_sbe-1.1.8/src/abilian/web/views/base.py
--rw-r--r--   0        0        0     4434 2024-03-23 14:15:18.741263 abilian_sbe-1.1.8/src/abilian/web/views/files.py
--rw-r--r--   0        0        0     7141 2024-03-25 13:17:52.077244 abilian_sbe-1.1.8/src/abilian/web/views/images.py
--rw-r--r--   0        0        0    20078 2024-03-23 14:15:18.743288 abilian_sbe-1.1.8/src/abilian/web/views/object.py
--rw-r--r--   0        0        0     4820 2023-12-08 09:38:30.290727 abilian_sbe-1.1.8/src/abilian/web/views/registry.py
--rw-r--r--   0        0        0        0 2021-09-16 12:00:44.000000 abilian_sbe-1.1.8/src/extranet/__init__.py
--rw-r--r--   0        0        0     4698 2024-03-27 08:36:58.869181 abilian_sbe-1.1.8/src/extranet/app.py
--rw-r--r--   0        0        0      939 2023-11-02 14:44:40.650969 abilian_sbe-1.1.8/src/extranet/config.py
--rw-r--r--   0        0        0      164 2024-03-25 13:17:52.077774 abilian_sbe-1.1.8/src/extranet/wsgi.py
--rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 abilian_sbe-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-11-02 14:44:52.025373 abilian_sbe-1.1.9/LICENCE.txt
+-rw-r--r--   0        0        0     4223 2024-02-07 15:10:35.344658 abilian_sbe-1.1.9/README.md
+-rw-r--r--   0        0        0     8485 2024-04-29 20:27:01.390128 abilian_sbe-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-16 12:51:19.000000 abilian_sbe-1.1.9/src/abilian/__init__.py
+-rw-r--r--   0        0        0    16539 2024-04-25 09:37:10.377469 abilian_sbe-1.1.9/src/abilian/app.py
+-rw-r--r--   0        0        0      126 2022-01-10 11:24:05.307322 abilian_sbe-1.1.9/src/abilian/cli/__init__.py
+-rw-r--r--   0        0        0     6556 2024-02-07 15:10:35.354478 abilian_sbe-1.1.9/src/abilian/cli/base.py
+-rw-r--r--   0        0        0      612 2024-03-25 13:17:52.042182 abilian_sbe-1.1.9/src/abilian/cli/config.py
+-rw-r--r--   0        0        0     6127 2024-02-07 15:10:35.354767 abilian_sbe-1.1.9/src/abilian/cli/indexing.py
+-rw-r--r--   0        0        0     2099 2024-03-27 10:19:57.119194 abilian_sbe-1.1.9/src/abilian/config.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:54:43.962129 abilian_sbe-1.1.9/src/abilian/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:54:43.923145 abilian_sbe-1.1.9/src/abilian/core/dramatiq/__init__.py
+-rw-r--r--   0        0        0      280 2024-03-25 06:54:43.927420 abilian_sbe-1.1.9/src/abilian/core/dramatiq/cli.py
+-rw-r--r--   0        0        0     1809 2024-03-25 06:56:05.424351 abilian_sbe-1.1.9/src/abilian/core/dramatiq/scheduler.py
+-rw-r--r--   0        0        0     3345 2024-03-25 13:17:52.042319 abilian_sbe-1.1.9/src/abilian/core/dramatiq/setup.py
+-rw-r--r--   0        0        0      347 2024-03-25 13:17:52.042426 abilian_sbe-1.1.9/src/abilian/core/dramatiq/singleton.py
+-rw-r--r--   0        0        0    18367 2024-04-26 15:46:20.164523 abilian_sbe-1.1.9/src/abilian/core/entities.py
+-rw-r--r--   0        0        0     4170 2024-03-25 13:17:52.042733 abilian_sbe-1.1.9/src/abilian/core/extensions/__init__.py
+-rw-r--r--   0        0        0     2536 2024-03-25 13:17:52.042999 abilian_sbe-1.1.9/src/abilian/core/extensions/csrf.py
+-rw-r--r--   0        0        0     2807 2024-03-25 06:56:05.428498 abilian_sbe-1.1.9/src/abilian/core/extensions/jinjaext.py
+-rw-r--r--   0        0        0      566 2024-03-25 06:56:05.429357 abilian_sbe-1.1.9/src/abilian/core/extensions/login.py
+-rw-r--r--   0        0        0      682 2024-03-25 06:56:05.429526 abilian_sbe-1.1.9/src/abilian/core/extensions/redis.py
+-rw-r--r--   0        0        0     2071 2024-03-25 13:17:52.043117 abilian_sbe-1.1.9/src/abilian/core/extensions/upstream_info.py
+-rw-r--r--   0        0        0     1425 2024-03-25 13:17:52.043410 abilian_sbe-1.1.9/src/abilian/core/logger_patch.py
+-rw-r--r--   0        0        0     1518 2024-03-25 13:17:52.043568 abilian_sbe-1.1.9/src/abilian/core/logging.py
+-rw-r--r--   0        0        0      363 2024-03-25 13:17:52.043699 abilian_sbe-1.1.9/src/abilian/core/models/__init__.py
+-rw-r--r--   0        0        0     3001 2024-03-25 13:17:52.043965 abilian_sbe-1.1.9/src/abilian/core/models/attachment.py
+-rw-r--r--   0        0        0     2212 2024-04-26 15:32:02.656547 abilian_sbe-1.1.9/src/abilian/core/models/base.py
+-rw-r--r--   0        0        0     1674 2024-03-25 13:17:52.044035 abilian_sbe-1.1.9/src/abilian/core/models/base_mixin.py
+-rw-r--r--   0        0        0     3886 2024-03-25 13:17:52.044155 abilian_sbe-1.1.9/src/abilian/core/models/blob.py
+-rw-r--r--   0        0        0     2622 2024-03-25 13:17:52.044406 abilian_sbe-1.1.9/src/abilian/core/models/comment.py
+-rw-r--r--   0        0        0     1941 2024-03-25 06:56:05.432557 abilian_sbe-1.1.9/src/abilian/core/models/owned.py
+-rw-r--r--   0        0        0    10370 2024-04-26 15:34:05.280067 abilian_sbe-1.1.9/src/abilian/core/models/subjects.py
+-rw-r--r--   0        0        0     2872 2024-03-25 13:17:52.045001 abilian_sbe-1.1.9/src/abilian/core/models/tag.py
+-rw-r--r--   0        0        0     1050 2024-03-25 06:54:42.810857 abilian_sbe-1.1.9/src/abilian/core/signals.py
+-rw-r--r--   0        0        0     2634 2024-03-25 06:56:05.433575 abilian_sbe-1.1.9/src/abilian/core/singleton.py
+-rw-r--r--   0        0        0    12834 2024-03-25 13:17:52.045335 abilian_sbe-1.1.9/src/abilian/core/sqlalchemy.py
+-rw-r--r--   0        0        0     6620 2024-03-25 13:17:52.045822 abilian_sbe-1.1.9/src/abilian/core/util.py
+-rw-r--r--   0        0        0    12627 2024-03-25 13:17:52.046301 abilian_sbe-1.1.9/src/abilian/i18n.py
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/__init__.py
+-rw-r--r--   0        0        0     1558 2024-03-27 10:19:57.119395 abilian_sbe-1.1.9/src/abilian/sbe/app.py
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/__init__.py
+-rw-r--r--   0        0        0      245 2024-02-07 15:10:35.360668 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/__init__.py
+-rw-r--r--   0        0        0     1424 2023-11-15 13:48:35.641820 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/actions.py
+-rw-r--r--   0        0        0     2155 2024-03-25 13:17:52.046578 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/forms.py
+-rw-r--r--   0        0        0     1241 2023-12-08 09:38:36.961819 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/models.py
+-rw-r--r--   0        0        0      665 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/_base.html
+-rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/archives.html
+-rw-r--r--   0        0        0      936 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/event.html
+-rw-r--r--   0        0        0      693 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/index.html
+-rw-r--r--   0        0        0     3089 2024-03-25 13:17:52.046855 abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/views.py
+-rw-r--r--   0        0        0      293 2024-02-07 15:10:35.361199 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/__init__.py
+-rw-r--r--   0        0        0     2608 2024-02-01 15:04:46.166107 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/actions.py
+-rw-r--r--   0        0        0     2526 2024-03-25 13:17:52.047212 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/blueprint.py
+-rw-r--r--   0        0        0     1728 2023-11-02 14:44:40.640316 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/common.py
+-rw-r--r--   0        0        0      891 2024-03-23 14:15:18.391077 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/events.py
+-rw-r--r--   0        0        0     4386 2024-03-25 13:17:52.047690 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/forms.py
+-rw-r--r--   0        0        0    17078 2024-04-25 11:34:05.550253 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/models.py
+-rw-r--r--   0        0        0      343 2022-01-10 11:24:05.321254 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/presenters.py
+-rw-r--r--   0        0        0     2551 2024-02-07 15:10:35.362310 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/search.py
+-rw-r--r--   0        0        0     2580 2024-03-25 13:17:52.048210 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/security.py
+-rw-r--r--   0        0        0      484 2022-01-10 11:24:05.321878 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/signals.py
+-rw-r--r--   0        0        0     1257 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/_base.html
+-rw-r--r--   0        0        0     1211 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/_forumbase.html
+-rw-r--r--   0        0        0     2510 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/edit.html
+-rw-r--r--   0        0        0     2252 2023-01-06 15:21:07.908153 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/home.html
+-rw-r--r--   0        0        0     2086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/macros.html
+-rw-r--r--   0        0        0     5480 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members.html
+-rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members_macros.html
+-rw-r--r--   0        0        0     3693 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members_std_macros.html
+-rw-r--r--   0        0        0     7470 2023-01-06 15:38:25.307247 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_add_emails.html
+-rw-r--r--   0        0        0     3970 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_check_members.html
+-rw-r--r--   0        0        0     8574 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_new_accounts.html
+-rw-r--r--   0        0        0     4705 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_users_std_macros.html
+-rw-r--r--   0        0        0      136 2024-02-01 15:05:42.035137 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/__init__.py
+-rw-r--r--   0        0        0     5106 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/data/community.png
+-rw-r--r--   0        0        0    15826 2024-03-25 13:17:52.048550 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/views.py
+-rw-r--r--   0        0        0     9917 2024-03-25 08:00:55.932036 abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/wizard.py
+-rw-r--r--   0        0        0      558 2024-03-25 13:17:52.048729 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/__init__.py
+-rw-r--r--   0        0        0     9829 2024-03-23 14:15:18.486736 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/actions.py
+-rw-r--r--   0        0        0      789 2023-12-22 14:52:32.481243 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cli.py
+-rw-r--r--   0        0        0      132 2024-02-07 15:10:35.363648 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/__init__.py
+-rw-r--r--   0        0        0    11897 2024-03-23 14:15:18.496755 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/atompub.py
+-rw-r--r--   0        0        0     3766 2024-04-26 14:16:17.827236 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/parser.py
+-rw-r--r--   0        0        0     1549 2022-01-10 11:24:05.325636 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/renderer.py
+-rw-r--r--   0        0        0     1684 2022-03-29 05:40:32.396040 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/lock.py
+-rw-r--r--   0        0        0    24675 2024-04-26 14:28:57.903880 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/models.py
+-rw-r--r--   0        0        0     5299 2024-03-23 14:15:18.491465 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/repository.py
+-rw-r--r--   0        0        0     1860 2024-03-23 14:15:18.490357 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/search.py
+-rw-r--r--   0        0        0     1629 2024-03-23 14:15:18.476992 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/signals.py
+-rw-r--r--   0        0        0     6505 2024-03-25 13:17:52.049224 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/tasks.py
+-rw-r--r--   0        0        0      123 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/allowableactions.xml
+-rw-r--r--   0        0        0     1140 2024-03-23 14:17:59.600802 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/children.xml
+-rw-r--r--   0        0        0     8119 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/document.xml
+-rw-r--r--   0        0        0      927 2024-03-23 14:17:52.327057 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/feed.xml
+-rw-r--r--   0        0        0     4312 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/folder.xml
+-rw-r--r--   0        0        0     4309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/macros.xml
+-rw-r--r--   0        0        0    13863 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/service.xml
+-rw-r--r--   0        0        0    23100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-document.xml
+-rw-r--r--   0        0        0    13734 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-folder.xml
+-rw-r--r--   0        0        0    11986 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-policy.xml
+-rw-r--r--   0        0        0    13066 2024-03-23 14:18:13.142503 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-relationship.xml
+-rw-r--r--   0        0        0     9553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/types.xml
+-rw-r--r--   0        0        0    17052 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros.html
+-rw-r--r--   0        0        0     2586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros_audit.html
+-rw-r--r--   0        0        0    16442 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros_gallery_view.html
+-rw-r--r--   0        0        0      237 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document.html
+-rw-r--r--   0        0        0     1007 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_delete.html
+-rw-r--r--   0        0        0     2218 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_edit.html
+-rw-r--r--   0        0        0     1549 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_send_by_email.html
+-rw-r--r--   0        0        0     1452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_upload_new_version.html
+-rw-r--r--   0        0        0      452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder.html
+-rw-r--r--   0        0        0     3571 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_change_owner.html
+-rw-r--r--   0        0        0     1121 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_delete.html
+-rw-r--r--   0        0        0     2146 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_edit.html
+-rw-r--r--   0        0        0     1148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_move.html
+-rw-r--r--   0        0        0     1963 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_new.html
+-rw-r--r--   0        0        0     3761 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_upload.html
+-rw-r--r--   0        0        0     3784 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_roles.html
+-rw-r--r--   0        0        0     1909 2022-03-29 05:55:53.926477 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/descendants.html
+-rw-r--r--   0        0        0    11321 2022-03-29 05:55:53.922772 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/document.html
+-rw-r--r--   0        0        0     2571 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/document_viewers.html
+-rw-r--r--   0        0        0      698 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/folder.html
+-rw-r--r--   0        0        0      731 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/folder_gallery_view.html
+-rw-r--r--   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/mail_file_sent.fr.txt
+-rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/mail_file_sent.txt
+-rw-r--r--   0        0        0     8948 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/permissions.html
+-rw-r--r--   0        0        0    21512 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/view_pdf.html
+-rw-r--r--   0        0        0      167 2024-03-25 13:17:52.049428 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/__init__.py
+-rw-r--r--   0        0        0    11642 2024-03-25 13:17:52.049656 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/documents.py
+-rw-r--r--   0        0        0    34367 2024-03-25 13:17:52.049979 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/folders.py
+-rw-r--r--   0        0        0     6644 2024-02-07 15:10:35.366814 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/util.py
+-rw-r--r--   0        0        0     1003 2024-03-25 13:17:52.050169 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/views.py
+-rw-r--r--   0        0        0      114 2024-02-07 15:10:35.367048 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/__init__.py
+-rw-r--r--   0        0        0     1780 2024-02-07 15:10:35.367282 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/constants.py
+-rw-r--r--   0        0        0     9113 2024-03-25 13:17:52.050324 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/views.py
+-rw-r--r--   0        0        0     2241 2024-02-07 15:10:35.367683 abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/xml.py
+-rw-r--r--   0        0        0      882 2024-03-25 13:17:52.050682 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/__init__.py
+-rw-r--r--   0        0        0     3343 2024-03-25 13:17:52.050857 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/actions.py
+-rw-r--r--   0        0        0     1630 2024-02-07 15:10:35.367924 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/cli.py
+-rw-r--r--   0        0        0     2311 2024-02-07 15:10:35.368176 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/forms.py
+-rw-r--r--   0        0        0     6833 2024-02-07 15:10:35.368307 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/models.py
+-rw-r--r--   0        0        0    17463 2024-03-23 14:15:18.428404 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/tasks.py
+-rw-r--r--   0        0        0       37 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/_base.html
+-rw-r--r--   0        0        0     2769 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/_macros.html
+-rw-r--r--   0        0        0     1540 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/archives.html
+-rw-r--r--   0        0        0     1373 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/attachments.html
+-rw-r--r--   0        0        0     3389 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/index.html
+-rw-r--r--   0        0        0     1129 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.fr.html
+-rw-r--r--   0        0        0     1127 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.html
+-rw-r--r--   0        0        0    10422 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread.html
+-rw-r--r--   0        0        0     2547 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread_attachments.html
+-rw-r--r--   0        0        0     4817 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread_create.html
+-rw-r--r--   0        0        0    17860 2024-03-25 13:17:52.051168 abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/views.py
+-rw-r--r--   0        0        0      328 2024-02-07 15:10:35.369016 abilian_sbe-1.1.9/src/abilian/sbe/apps/main/__init__.py
+-rw-r--r--   0        0        0      387 2022-01-10 11:24:05.334109 abilian_sbe-1.1.9/src/abilian/sbe/apps/main/main.py
+-rw-r--r--   0        0        0      762 2024-02-07 15:10:35.369378 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/tasks/__init__.py
+-rw-r--r--   0        0        0     8943 2024-03-23 14:15:18.526749 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/tasks/social.py
+-rw-r--r--   0        0        0     1988 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/_base.html
+-rw-r--r--   0        0        0    11699 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/_style.css
+-rw-r--r--   0        0        0      388 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/confirm-unsubscribe.fr.html
+-rw-r--r--   0        0        0      309 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/confirm-unsubscribe.html
+-rw-r--r--   0        0        0     4278 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.fr.html
+-rw-r--r--   0        0        0     4204 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.html
+-rw-r--r--   0        0        0      356 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/invalid-token.fr.html
+-rw-r--r--   0        0        0      314 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/invalid-token.html
+-rw-r--r--   0        0        0      164 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/unsubscribed.fr.html
+-rw-r--r--   0        0        0      140 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/unsubscribed.html
+-rw-r--r--   0        0        0      198 2022-01-10 11:24:05.334999 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/views/__init__.py
+-rw-r--r--   0        0        0     1952 2024-03-23 14:15:18.530523 abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/views/social.py
+-rw-r--r--   0        0        0      420 2024-03-23 14:15:18.363614 abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/panels/__init__.py
+-rw-r--r--   0        0        0     2429 2024-02-07 15:10:35.369798 abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/panels/sbe_notifications.py
+-rw-r--r--   0        0        0      701 2022-04-12 15:38:51.537046 abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/templates/preferences/sbe_notifications.html
+-rw-r--r--   0        0        0      455 2024-02-07 15:10:35.369912 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/__init__.py
+-rw-r--r--   0        0        0     1119 2024-02-07 15:10:35.370157 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/forms.py
+-rw-r--r--   0        0        0     2645 2024-02-07 15:10:35.370262 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/models.py
+-rw-r--r--   0        0        0     7998 2024-03-23 14:15:18.451083 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/restapi.py
+-rw-r--r--   0        0        0     1290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/_sidebar.html
+-rw-r--r--   0        0        0     1654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/base.html
+-rw-r--r--   0        0        0     4308 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/group.html
+-rw-r--r--   0        0        0     1663 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/groups-new.html
+-rw-r--r--   0        0        0     2769 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/groups.html
+-rw-r--r--   0        0        0      353 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/home.html
+-rw-r--r--   0        0        0     1250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/invite.html
+-rw-r--r--   0        0        0     4100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/macros.html
+-rw-r--r--   0        0        0      208 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/mail/invite.txt
+-rw-r--r--   0        0        0     1835 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/user.html
+-rw-r--r--   0        0        0     3166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/users.html
+-rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/widget_user_photo.html
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/__init__.py
+-rw-r--r--   0        0        0     5810 2024-03-23 14:15:18.461633 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/groups.py
+-rw-r--r--   0        0        0     1823 2024-03-23 14:15:18.455097 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/invites.py
+-rw-r--r--   0        0        0     1445 2024-03-23 14:15:18.472104 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/sidebars.py
+-rw-r--r--   0        0        0     1356 2022-01-10 11:24:05.337926 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/social.py
+-rw-r--r--   0        0        0     9083 2024-03-23 14:15:18.459486 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/users.py
+-rw-r--r--   0        0        0      590 2024-03-25 13:17:52.051315 abilian_sbe-1.1.9/src/abilian/sbe/apps/social/widgets.py
+-rw-r--r--   0        0        0      187 2022-01-10 11:24:05.338437 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/__init__.py
+-rw-r--r--   0        0        0     6373 2024-02-07 15:10:35.371158 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/presenters.py
+-rw-r--r--   0        0        0      522 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/templates/wall/_base.html
+-rw-r--r--   0        0        0      759 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/templates/wall/files.html
+-rw-r--r--   0        0        0      309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/templates/wall/index.html
+-rw-r--r--   0        0        0     2993 2024-03-25 13:17:52.051430 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/util.py
+-rw-r--r--   0        0        0     4560 2024-03-25 13:17:52.051689 abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/views.py
+-rw-r--r--   0        0        0      444 2024-03-25 13:17:52.051928 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/__init__.py
+-rw-r--r--   0        0        0     2781 2022-01-10 11:24:05.339289 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/actions.py
+-rw-r--r--   0        0        0      266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/data/default_page.txt
+-rw-r--r--   0        0        0     1532 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/data/help.txt
+-rw-r--r--   0        0        0     1959 2024-03-23 14:15:18.418706 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/forms.py
+-rw-r--r--   0        0        0     2057 2024-03-23 14:15:18.417707 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/markup.py
+-rw-r--r--   0        0        0     4976 2023-12-08 09:38:30.278323 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/models.py
+-rw-r--r--   0        0        0     4322 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/_base.html
+-rw-r--r--   0        0        0      392 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/all_pages.html
+-rw-r--r--   0        0        0     1144 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/changes.html
+-rw-r--r--   0        0        0      357 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/compare.html
+-rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/edit_conflict_error.html
+-rw-r--r--   0        0        0      190 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/help.html
+-rw-r--r--   0        0        0      372 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/macros.html
+-rw-r--r--   0        0        0     1717 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/page.html
+-rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/page_readers.html
+-rw-r--r--   0        0        0      212 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/source.html
+-rw-r--r--   0        0        0      333 2022-01-10 11:24:05.340492 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/util.py
+-rw-r--r--   0        0        0    16918 2024-03-25 13:17:52.052210 abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/views.py
+-rw-r--r--   0        0        0     3267 2024-02-07 15:10:35.372295 abilian_sbe-1.1.9/src/abilian/sbe/boot.py
+-rw-r--r--   0        0        0     1897 2024-03-25 13:17:52.052361 abilian_sbe-1.1.9/src/abilian/sbe/extension.py
+-rw-r--r--   0        0        0       32 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/csv/csv_example.csv
+-rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/7z.png
+-rw-r--r--   0        0        0       60 2023-12-08 18:07:26.554324 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/README.txt
+-rw-r--r--   0        0        0      634 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ai.png
+-rw-r--r--   0        0        0      604 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/aiff.png
+-rw-r--r--   0        0        0      480 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/asc.png
+-rw-r--r--   0        0        0      514 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/audio.png
+-rw-r--r--   0        0        0      458 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/bin.png
+-rw-r--r--   0        0        0      576 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/bz2.png
+-rw-r--r--   0        0        0      584 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/c.png
+-rw-r--r--   0        0        0      577 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cfc.png
+-rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cfm.png
+-rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/chm.png
+-rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/class.png
+-rw-r--r--   0        0        0      557 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/conf.png
+-rw-r--r--   0        0        0      629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cpp.png
+-rw-r--r--   0        0        0      618 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cs.png
+-rw-r--r--   0        0        0      654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/css.png
+-rw-r--r--   0        0        0      366 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/csv.png
+-rw-r--r--   0        0        0      564 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/deb.png
+-rw-r--r--   0        0        0      661 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/divx.png
+-rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/doc.png
+-rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/docx.png
+-rw-r--r--   0        0        0      475 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/dot.png
+-rw-r--r--   0        0        0      302 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/eml.png
+-rw-r--r--   0        0        0      474 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/enc.png
+-rw-r--r--   0        0        0      358 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/file.png
+-rw-r--r--   0        0        0      358 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/folder.png
+-rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/gif.png
+-rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/gz.png
+-rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/hlp.png
+-rw-r--r--   0        0        0      611 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/htm.png
+-rw-r--r--   0        0        0      611 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/html.png
+-rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/image.png
+-rw-r--r--   0        0        0      581 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/iso.png
+-rw-r--r--   0        0        0      599 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jar.png
+-rw-r--r--   0        0        0      604 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/java.png
+-rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jpeg.png
+-rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jpg.png
+-rw-r--r--   0        0        0      622 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/js.png
+-rw-r--r--   0        0        0      390 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/lua.png
+-rw-r--r--   0        0        0      567 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/m.png
+-rw-r--r--   0        0        0      323 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mm.png
+-rw-r--r--   0        0        0      665 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mov.png
+-rw-r--r--   0        0        0      629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mp3.png
+-rw-r--r--   0        0        0      660 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mpg.png
+-rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odc.png
+-rw-r--r--   0        0        0      621 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odf.png
+-rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odg.png
+-rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odi.png
+-rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odp.png
+-rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ods.png
+-rw-r--r--   0        0        0      479 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odt.png
+-rw-r--r--   0        0        0      613 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ogg.png
+-rw-r--r--   0        0        0      522 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pdf.png
+-rw-r--r--   0        0        0      481 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pgp.png
+-rw-r--r--   0        0        0      633 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/php.png
+-rw-r--r--   0        0        0      605 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pl.png
+-rw-r--r--   0        0        0      675 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/png.png
+-rw-r--r--   0        0        0      602 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ppt.png
+-rw-r--r--   0        0        0      602 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pptx.png
+-rw-r--r--   0        0        0      446 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ps.png
+-rw-r--r--   0        0        0      614 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/py.png
+-rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ram.png
+-rw-r--r--   0        0        0      499 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rar.png
+-rw-r--r--   0        0        0      623 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rb.png
+-rw-r--r--   0        0        0      605 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rm.png
+-rw-r--r--   0        0        0      445 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rpm.png
+-rw-r--r--   0        0        0      384 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rtf.png
+-rw-r--r--   0        0        0      498 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sig.png
+-rw-r--r--   0        0        0      583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sql.png
+-rw-r--r--   0        0        0      632 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/swf.png
+-rw-r--r--   0        0        0      579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxc.png
+-rw-r--r--   0        0        0      620 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxd.png
+-rw-r--r--   0        0        0      593 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxi.png
+-rw-r--r--   0        0        0      479 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxw.png
+-rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tar.png
+-rw-r--r--   0        0        0      643 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tex.png
+-rw-r--r--   0        0        0      570 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tgz.png
+-rw-r--r--   0        0        0      398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/txt.png
+-rw-r--r--   0        0        0      552 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/vcf.png
+-rw-r--r--   0        0        0      540 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/video.png
+-rw-r--r--   0        0        0      574 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/vsd.png
+-rw-r--r--   0        0        0      615 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wav.png
+-rw-r--r--   0        0        0      636 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wma.png
+-rw-r--r--   0        0        0      670 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wmv.png
+-rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xls.png
+-rw-r--r--   0        0        0      580 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xlsx.png
+-rw-r--r--   0        0        0      367 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xml.png
+-rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xpi.png
+-rw-r--r--   0        0        0      653 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xvid.png
+-rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/zip.png
+-rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/account-12.png
+-rwxr-xr-x   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/account-16.png
+-rw-r--r--   0        0        0      349 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/actionfiliere-12.png
+-rw-r--r--   0        0        0      412 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/checkbox-checked-12.png
+-rwxr-xr-x   0        0        0      281 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/checkbox-checked-16.png
+-rw-r--r--   0        0        0      327 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/checkbox-unchecked-12.png
+-rwxr-xr-x   0        0        0      204 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/checkbox-unchecked-16.png
+-rwxr-xr-x   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/cog-16.png
+-rw-r--r--   0        0        0      332 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/contact-12.png
+-rwxr-xr-x   0        0        0      208 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/contact-16.png
+-rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/document-12.png
+-rwxr-xr-x   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/document-16.png
+-rwxr-xr-x   0        0        0      207 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/download-16.png
+-rw-r--r--   0        0        0      362 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/image-12.png
+-rwxr-xr-x   0        0        0      234 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/image-16.png
+-rw-r--r--   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/lead-12.png
+-rwxr-xr-x   0        0        0      214 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/lead-16.png
+-rw-r--r--   0        0        0      343 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/opportunity-12.png
+-rwxr-xr-x   0        0        0      233 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/opportunity-16.png
+-rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/partenaire-12.png
+-rw-r--r--   0        0        0      320 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/programmefiliere-12.png
+-rw-r--r--   0        0        0      333 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/projet-12.png
+-rwxr-xr-x   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/round-minus-16.png
+-rwxr-xr-x   0        0        0      316 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/round-minus-24.png
+-rwxr-xr-x   0        0        0      250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/round-plus-16.png
+-rwxr-xr-x   0        0        0      367 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/round-plus-24.png
+-rwxr-xr-x   0        0        0      401 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/visite-12.png
+-rwxr-xr-x   0        0        0      237 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/icons/wrench-16.png
+-rw-r--r--   0        0        0     1171 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/arrows.png
+-rw-r--r--   0        0        0     1361 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_disabled.png
+-rw-r--r--   0        0        0     1379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_enabled.png
+-rw-r--r--   0        0        0     1375 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_enabled_hover.png
+-rw-r--r--   0        0        0     4123 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/backgrd.png
+-rw-r--r--   0        0        0    46666 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/eagle.jpg
+-rw-r--r--   0        0        0     2170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/error.png
+-rw-r--r--   0        0        0     1579 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/favicon.png
+-rw-r--r--   0        0        0     1363 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_disabled.png
+-rw-r--r--   0        0        0     1380 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_enabled.png
+-rw-r--r--   0        0        0     1379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_enabled_hover.png
+-rw-r--r--   0        0        0    50718 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/frog.jpg
+-rw-r--r--   0        0        0     8777 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/glyphicons-halflings-white.png
+-rw-r--r--   0        0        0    13826 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/glyphicons-halflings.png
+-rw-r--r--   0        0        0      191 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/greendot.png
+-rw-r--r--   0        0        0    14264 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/group-icon.png
+-rw-r--r--   0        0        0   325765 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/login-background.jpg
+-rwxr-xr-x   0        0        0      209 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/next.png
+-rw-r--r--   0        0        0     7609 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/noise_bg.png
+-rwxr-xr-x   0        0        0      203 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/prev.png
+-rw-r--r--   0        0        0      679 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/preview_missing.png
+-rw-r--r--   0        0        0    12517 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_man.png
+-rw-r--r--   0        0        0    10266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_unknown.png
+-rw-r--r--   0        0        0    12333 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_woman.png
+-rw-r--r--   0        0        0     1118 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_asc.png
+-rw-r--r--   0        0        0     1050 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_asc_disabled.png
+-rw-r--r--   0        0        0     1136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_both.png
+-rw-r--r--   0        0        0     1127 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_desc.png
+-rw-r--r--   0        0        0     1045 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_desc_disabled.png
+-rw-r--r--   0        0        0      314 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/state.png
+-rw-r--r--   0        0        0    11584 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/user-icon.png
+-rw-r--r--   0        0        0     2294 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/images/valid.png
+-rw-r--r--   0        0        0      240 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/arrows.png
+-rw-r--r--   0        0        0     7710 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/avatar140.jpg
+-rw-r--r--   0        0        0     4340 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/avatar45.png
+-rw-r--r--   0        0        0      345 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/back_disabled.png
+-rw-r--r--   0        0        0      459 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/back_enabled.png
+-rw-r--r--   0        0        0      457 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/back_enabled_hover.png
+-rw-r--r--   0        0        0     2487 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/backgrd.png
+-rw-r--r--   0        0        0     1182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/error.png
+-rw-r--r--   0        0        0     1069 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/favicon.png
+-rw-r--r--   0        0        0      350 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/forward_disabled.png
+-rw-r--r--   0        0        0      468 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/forward_enabled.png
+-rw-r--r--   0        0        0      467 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/forward_enabled_hover.png
+-rw-r--r--   0        0        0     8768 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/glyphicons-halflings-white.png
+-rw-r--r--   0        0        0    11896 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/glyphicons-halflings.png
+-rw-r--r--   0        0        0      136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/greendot.png
+-rw-r--r--   0        0        0    12299 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/group-icon.png
+-rw-r--r--   0        0        0     1056 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/group64.png
+-rw-r--r--   0        0        0  1304297 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/login-background.jpg
+-rw-r--r--   0        0        0     5071 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/me-25x25.jpg
+-rwxr-xr-x   0        0        0      142 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/next.png
+-rwxr-xr-x   0        0        0      141 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/prev.png
+-rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/sort_asc.png
+-rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/sort_asc_disabled.png
+-rw-r--r--   0        0        0      209 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/sort_both.png
+-rw-r--r--   0        0        0      172 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/sort_desc.png
+-rw-r--r--   0        0        0      159 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/sort_desc_disabled.png
+-rw-r--r--   0        0        0      107 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/state.png
+-rw-r--r--   0        0        0     9815 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/user-icon.png
+-rw-r--r--   0        0        0     1323 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/img/valid.png
+-rw-r--r--   0        0        0     1599 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/document_viewer.js
+-rw-r--r--   0        0        0     6462 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder.js
+-rw-r--r--   0        0        0     1165 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_edit.js
+-rw-r--r--   0        0        0     4638 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_gallery.js
+-rw-r--r--   0        0        0     3040 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_upload.js
+-rw-r--r--   0        0        0      562 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/js/sbe-datatable.js
+-rw-r--r--   0        0        0      221 2023-12-08 18:07:26.555085 abilian_sbe-1.1.9/src/abilian/sbe/static/less/README.txt
+-rw-r--r--   0        0        0      377 2022-04-04 14:22:56.768469 abilian_sbe-1.1.9/src/abilian/sbe/static/less/abilian-sbe.less
+-rw-r--r--   0        0        0      165 2022-04-04 14:15:12.852861 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/base.less
+-rw-r--r--   0        0        0     1357 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/bootstrap-tagsinput.less
+-rw-r--r--   0        0        0     1002 2022-04-04 14:16:11.444824 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/communities.less
+-rw-r--r--   0        0        0     5985 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/documents.less
+-rw-r--r--   0        0        0      273 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/excel.less
+-rw-r--r--   0        0        0    11908 2022-04-04 14:20:50.191106 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/forum.less
+-rw-r--r--   0        0        0     1676 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/misc.less
+-rw-r--r--   0        0        0      279 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/social.less
+-rw-r--r--   0        0        0      241 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/wiki.less
+-rw-r--r--   0        0        0     2811 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/wizard_steps.less
+-rw-r--r--   0        0        0     1328 2022-04-04 14:15:00.639617 abilian_sbe-1.1.9/src/abilian/sbe/static/less/overrides.less
+-rw-r--r--   0        0        0      224 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/less/print.less
+-rw-r--r--   0        0        0    14684 2023-12-08 18:07:26.555690 abilian_sbe-1.1.9/src/abilian/sbe/static/moment/moment.min.js
+-rw-r--r--   0        0        0       86 2023-12-08 18:07:26.556277 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/README.txt
+-rw-r--r--   0        0        0     2404 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-H.bcmap
+-rw-r--r--   0        0        0      173 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-V.bcmap
+-rw-r--r--   0        0        0     2379 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-H.bcmap
+-rw-r--r--   0        0        0     2398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      173 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-V.bcmap
+-rw-r--r--   0        0        0     2651 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      905 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/83pv-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      721 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      715 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      291 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      982 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-V.bcmap
+-rw-r--r--   0        0        0     2419 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-H.bcmap
+-rw-r--r--   0        0        0     2413 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      287 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      282 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-V.bcmap
+-rw-r--r--   0        0        0      317 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-0.bcmap
+-rw-r--r--   0        0        0      371 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-1.bcmap
+-rw-r--r--   0        0        0      376 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-2.bcmap
+-rw-r--r--   0        0        0      401 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-3.bcmap
+-rw-r--r--   0        0        0      405 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-4.bcmap
+-rw-r--r--   0        0        0      406 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-5.bcmap
+-rw-r--r--   0        0        0      406 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-6.bcmap
+-rw-r--r--   0        0        0    41193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap
+-rw-r--r--   0        0        0      217 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-0.bcmap
+-rw-r--r--   0        0        0      250 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-1.bcmap
+-rw-r--r--   0        0        0      465 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-2.bcmap
+-rw-r--r--   0        0        0      470 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-3.bcmap
+-rw-r--r--   0        0        0      601 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-4.bcmap
+-rw-r--r--   0        0        0      625 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-5.bcmap
+-rw-r--r--   0        0        0    33974 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap
+-rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-0.bcmap
+-rw-r--r--   0        0        0      226 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-1.bcmap
+-rw-r--r--   0        0        0      233 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-2.bcmap
+-rw-r--r--   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-3.bcmap
+-rw-r--r--   0        0        0      337 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-4.bcmap
+-rw-r--r--   0        0        0      430 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-5.bcmap
+-rw-r--r--   0        0        0      485 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-6.bcmap
+-rw-r--r--   0        0        0    40951 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap
+-rw-r--r--   0        0        0      241 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-0.bcmap
+-rw-r--r--   0        0        0      386 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-1.bcmap
+-rw-r--r--   0        0        0      391 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-2.bcmap
+-rw-r--r--   0        0        0    23293 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap
+-rw-r--r--   0        0        0     1086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5-H.bcmap
+-rw-r--r--   0        0        0      142 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5-V.bcmap
+-rw-r--r--   0        0        0     1099 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5pc-H.bcmap
+-rw-r--r--   0        0        0      144 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5pc-V.bcmap
+-rw-r--r--   0        0        0     1780 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-H.bcmap
+-rw-r--r--   0        0        0     1920 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-V.bcmap
+-rw-r--r--   0        0        0      706 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS1-H.bcmap
+-rw-r--r--   0        0        0      143 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS1-V.bcmap
+-rw-r--r--   0        0        0      504 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS2-H.bcmap
+-rw-r--r--   0        0        0       93 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS2-V.bcmap
+-rw-r--r--   0        0        0     4426 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-H.bcmap
+-rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-V.bcmap
+-rw-r--r--   0        0        0     1125 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-H.bcmap
+-rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-V.bcmap
+-rw-r--r--   0        0        0      101 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETenms-B5-H.bcmap
+-rw-r--r--   0        0        0      172 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETenms-B5-V.bcmap
+-rw-r--r--   0        0        0      578 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/EUC-H.bcmap
+-rw-r--r--   0        0        0      170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/EUC-V.bcmap
+-rw-r--r--   0        0        0     2536 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-H.bcmap
+-rw-r--r--   0        0        0     2542 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-H.bcmap
+-rw-r--r--   0        0        0      218 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-V.bcmap
+-rw-r--r--   0        0        0      215 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-V.bcmap
+-rw-r--r--   0        0        0      549 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-H.bcmap
+-rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-V.bcmap
+-rw-r--r--   0        0        0      528 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-H.bcmap
+-rw-r--r--   0        0        0      175 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-V.bcmap
+-rw-r--r--   0        0        0    14692 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-H.bcmap
+-rw-r--r--   0        0        0      180 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-V.bcmap
+-rw-r--r--   0        0        0    19662 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-H.bcmap
+-rw-r--r--   0        0        0      219 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-V.bcmap
+-rw-r--r--   0        0        0    14686 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-H.bcmap
+-rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-V.bcmap
+-rw-r--r--   0        0        0     7290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-H.bcmap
+-rw-r--r--   0        0        0      180 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-V.bcmap
+-rw-r--r--   0        0        0     7269 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-H.bcmap
+-rw-r--r--   0        0        0      176 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-V.bcmap
+-rw-r--r--   0        0        0     7298 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-V.bcmap
+-rw-r--r--   0        0        0      557 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-V.bcmap
+-rw-r--r--   0        0        0      553 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/H.bcmap
+-rw-r--r--   0        0        0     2654 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-H.bcmap
+-rw-r--r--   0        0        0      148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-V.bcmap
+-rw-r--r--   0        0        0     2414 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-H.bcmap
+-rw-r--r--   0        0        0      148 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-V.bcmap
+-rw-r--r--   0        0        0     2292 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-V.bcmap
+-rw-r--r--   0        0        0     1772 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-V.bcmap
+-rw-r--r--   0        0        0     2171 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-H.bcmap
+-rw-r--r--   0        0        0      149 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-V.bcmap
+-rw-r--r--   0        0        0     4437 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-H.bcmap
+-rw-r--r--   0        0        0      159 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-V.bcmap
+-rw-r--r--   0        0        0      132 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Hankaku.bcmap
+-rw-r--r--   0        0        0      124 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Hiragana.bcmap
+-rw-r--r--   0        0        0     1848 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-H.bcmap
+-rw-r--r--   0        0        0      164 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-V.bcmap
+-rw-r--r--   0        0        0     1831 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-H.bcmap
+-rw-r--r--   0        0        0    16791 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-H.bcmap
+-rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-V.bcmap
+-rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-V.bcmap
+-rw-r--r--   0        0        0     2787 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-H.bcmap
+-rw-r--r--   0        0        0     2789 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap
+-rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-V.bcmap
+-rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-V.bcmap
+-rw-r--r--   0        0        0     2024 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-H.bcmap
+-rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-V.bcmap
+-rw-r--r--   0        0        0      100 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Katakana.bcmap
+-rw-r--r--   0        0        0     2080 2023-12-08 18:07:26.557356 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/LICENSE
+-rw-r--r--   0        0        0     2765 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/NWP-H.bcmap
+-rw-r--r--   0        0        0      252 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/NWP-V.bcmap
+-rw-r--r--   0        0        0      534 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-H.bcmap
+-rw-r--r--   0        0        0      170 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-V.bcmap
+-rw-r--r--   0        0        0       96 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Roman.bcmap
+-rw-r--r--   0        0        0    48280 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      156 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    50419 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      156 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    52679 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    53629 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      157 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-V.bcmap
+-rw-r--r--   0        0        0    43366 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-H.bcmap
+-rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-V.bcmap
+-rw-r--r--   0        0        0    44086 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-H.bcmap
+-rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-V.bcmap
+-rw-r--r--   0        0        0    45738 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-H.bcmap
+-rw-r--r--   0        0        0      182 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-V.bcmap
+-rw-r--r--   0        0        0    46837 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-H.bcmap
+-rw-r--r--   0        0        0      181 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-V.bcmap
+-rw-r--r--   0        0        0    25439 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      119 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-H.bcmap
+-rw-r--r--   0        0        0      680 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap
+-rw-r--r--   0        0        0      664 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    39443 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      643 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    40539 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      677 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    41695 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      678 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-V.bcmap
+-rw-r--r--   0        0        0    39534 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap
+-rw-r--r--   0        0        0      647 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap
+-rw-r--r--   0        0        0    40630 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap
+-rw-r--r--   0        0        0      681 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap
+-rw-r--r--   0        0        0    41779 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap
+-rw-r--r--   0        0        0      682 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap
+-rw-r--r--   0        0        0      705 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap
+-rw-r--r--   0        0        0      689 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap
+-rw-r--r--   0        0        0      726 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap
+-rw-r--r--   0        0        0    40517 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap
+-rw-r--r--   0        0        0      684 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap
+-rw-r--r--   0        0        0    40608 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap
+-rw-r--r--   0        0        0      688 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap
+-rw-r--r--   0        0        0    25783 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-H.bcmap
+-rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-V.bcmap
+-rw-r--r--   0        0        0    26327 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-H.bcmap
+-rw-r--r--   0        0        0      164 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-V.bcmap
+-rw-r--r--   0        0        0    26451 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-H.bcmap
+-rw-r--r--   0        0        0      168 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-V.bcmap
+-rw-r--r--   0        0        0    27790 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-H.bcmap
+-rw-r--r--   0        0        0      169 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-V.bcmap
+-rw-r--r--   0        0        0      166 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/V.bcmap
+-rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/WP-Symbol.bcmap
+-rw-r--r--   0        0        0    17788 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/compatibility.js
+-rw-r--r--   0        0        0    19583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/debugger.js
+-rw-r--r--   0        0        0      415 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-check.svg
+-rw-r--r--   0        0        0      883 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-comment.svg
+-rw-r--r--   0        0        0     2168 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-help.svg
+-rw-r--r--   0        0        0      408 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-insert.svg
+-rw-r--r--   0        0        0     1452 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-key.svg
+-rw-r--r--   0        0        0      426 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-newparagraph.svg
+-rw-r--r--   0        0        0      158 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-noicon.svg
+-rw-r--r--   0        0        0     1041 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-note.svg
+-rw-r--r--   0        0        0     1143 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-paragraph.svg
+-rw-r--r--   0        0        0      199 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-next-rtl.png
+-rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-next-rtl@2x.png
+-rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-next.png
+-rw-r--r--   0        0        0      296 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-next@2x.png
+-rw-r--r--   0        0        0      193 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-previous-rtl.png
+-rw-r--r--   0        0        0      296 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-previous-rtl@2x.png
+-rw-r--r--   0        0        0      199 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-previous.png
+-rw-r--r--   0        0        0      304 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/findbarButton-previous@2x.png
+-rw-r--r--   0        0        0      326 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/grab.cur
+-rw-r--r--   0        0        0      326 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/grabbing.cur
+-rw-r--r--   0        0        0     2545 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-icon.gif
+-rw-r--r--   0        0        0     7402 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-small.png
+-rw-r--r--   0        0        0    16131 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-small@2x.png
+-rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties.png
+-rw-r--r--   0        0        0      933 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties@2x.png
+-rw-r--r--   0        0        0      179 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-firstPage.png
+-rw-r--r--   0        0        0      266 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-firstPage@2x.png
+-rw-r--r--   0        0        0      301 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool.png
+-rw-r--r--   0        0        0      583 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool@2x.png
+-rw-r--r--   0        0        0      175 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-lastPage.png
+-rw-r--r--   0        0        0      276 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-lastPage@2x.png
+-rw-r--r--   0        0        0      360 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw.png
+-rw-r--r--   0        0        0      731 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw@2x.png
+-rw-r--r--   0        0        0      359 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw.png
+-rw-r--r--   0        0        0      714 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw@2x.png
+-rw-r--r--   0        0        0      290 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/shadow.png
+-rw-r--r--   0        0        0     2418 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/texture.png
+-rw-r--r--   0        0        0      174 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-bookmark.png
+-rw-r--r--   0        0        0      260 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-bookmark@2x.png
+-rw-r--r--   0        0        0      259 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-download.png
+-rw-r--r--   0        0        0      425 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-download@2x.png
+-rw-r--r--   0        0        0      108 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-menuArrows.png
+-rw-r--r--   0        0        0      152 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-menuArrows@2x.png
+-rw-r--r--   0        0        0      295 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile.png
+-rw-r--r--   0        0        0      550 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile@2x.png
+-rw-r--r--   0        0        0      242 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown-rtl.png
+-rw-r--r--   0        0        0      398 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown-rtl@2x.png
+-rw-r--r--   0        0        0      238 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown.png
+-rw-r--r--   0        0        0      396 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageDown@2x.png
+-rw-r--r--   0        0        0      245 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp-rtl.png
+-rw-r--r--   0        0        0      405 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp-rtl@2x.png
+-rw-r--r--   0        0        0      246 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp.png
+-rw-r--r--   0        0        0      403 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-pageUp@2x.png
+-rw-r--r--   0        0        0      321 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode.png
+-rw-r--r--   0        0        0      586 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode@2x.png
+-rw-r--r--   0        0        0      257 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-print.png
+-rw-r--r--   0        0        0      464 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-print@2x.png
+-rw-r--r--   0        0        0      309 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-search.png
+-rw-r--r--   0        0        0      653 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-search@2x.png
+-rw-r--r--   0        0        0      246 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle-rtl.png
+-rw-r--r--   0        0        0      456 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle-rtl@2x.png
+-rw-r--r--   0        0        0      243 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle.png
+-rw-r--r--   0        0        0      458 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-secondaryToolbarToggle@2x.png
+-rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle-rtl.png
+-rw-r--r--   0        0        0      344 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle-rtl@2x.png
+-rw-r--r--   0        0        0      225 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle.png
+-rw-r--r--   0        0        0      331 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-sidebarToggle@2x.png
+-rw-r--r--   0        0        0      384 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments.png
+-rw-r--r--   0        0        0      871 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments@2x.png
+-rw-r--r--   0        0        0      177 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline-rtl.png
+-rw-r--r--   0        0        0      394 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline-rtl@2x.png
+-rw-r--r--   0        0        0      178 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline.png
+-rw-r--r--   0        0        0      331 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewOutline@2x.png
+-rw-r--r--   0        0        0      185 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewThumbnail.png
+-rw-r--r--   0        0        0      220 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewThumbnail@2x.png
+-rw-r--r--   0        0        0      136 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomIn.png
+-rw-r--r--   0        0        0      160 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomIn@2x.png
+-rw-r--r--   0        0        0       88 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomOut.png
+-rw-r--r--   0        0        0      109 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-zoomOut@2x.png
+-rw-r--r--   0        0        0    29253 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/l10n.js
+-rw-r--r--   0        0        0     6355 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/locale/en-US/viewer.properties
+-rw-r--r--   0        0        0     6988 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/locale/fr/viewer.properties
+-rw-r--r--   0        0        0      128 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/locale/locale.properties
+-rw-r--r--   0        0        0   262071 2023-12-08 18:07:26.559387 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/pdf.js
+-rw-r--r--   0        0        0  1258826 2023-12-08 18:07:26.565065 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/pdf.worker.js
+-rw-r--r--   0        0        0    46023 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/viewer.css
+-rw-r--r--   0        0        0   255262 2023-12-08 18:07:26.566971 abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/viewer.js
+-rw-r--r--   0        0        0    22075 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/vendor/bootstrap-tagsinput.js
+-rw-r--r--   0        0        0    38161 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/static/vendor/jquery.fileapi.js
+-rw-r--r--   0        0        0      131 2021-09-16 12:23:46.000000 abilian_sbe-1.1.9/src/abilian/sbe/templates/help.html
+-rw-r--r--   0        0        0    60321 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    62372 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    50456 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/translations/messages.pot
+-rw-r--r--   0        0        0    59863 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/translations/tr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    58090 2021-09-16 12:23:47.000000 abilian_sbe-1.1.9/src/abilian/sbe/translations/zh/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0     1189 2024-02-07 15:10:35.372662 abilian_sbe-1.1.9/src/abilian/services/__init__.py
+-rw-r--r--   0        0        0      155 2022-01-10 11:24:05.342770 abilian_sbe-1.1.9/src/abilian/services/activity/__init__.py
+-rw-r--r--   0        0        0     2248 2024-03-25 13:17:52.052476 abilian_sbe-1.1.9/src/abilian/services/activity/models.py
+-rw-r--r--   0        0        0     2025 2024-03-23 14:15:18.818784 abilian_sbe-1.1.9/src/abilian/services/activity/service.py
+-rw-r--r--   0        0        0       65 2024-02-01 15:05:42.048849 abilian_sbe-1.1.9/src/abilian/services/antivirus/__init__.py
+-rw-r--r--   0        0        0     3871 2024-03-25 13:17:52.052593 abilian_sbe-1.1.9/src/abilian/services/antivirus/service.py
+-rw-r--r--   0        0        0      109 2023-01-06 16:41:12.890699 abilian_sbe-1.1.9/src/abilian/services/audit/__init__.py
+-rw-r--r--   0        0        0     7330 2024-03-25 13:17:52.052871 abilian_sbe-1.1.9/src/abilian/services/audit/models.py
+-rw-r--r--   0        0        0    13713 2024-04-26 15:34:45.867876 abilian_sbe-1.1.9/src/abilian/services/audit/service.py
+-rw-r--r--   0        0        0       77 2024-02-07 15:10:35.373938 abilian_sbe-1.1.9/src/abilian/services/auth/__init__.py
+-rw-r--r--   0        0        0     3158 2024-04-26 15:35:17.584615 abilian_sbe-1.1.9/src/abilian/services/auth/models.py
+-rw-r--r--   0        0        0     8511 2024-03-23 14:15:18.811603 abilian_sbe-1.1.9/src/abilian/services/auth/service.py
+-rw-r--r--   0        0        0      453 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/email/password_reset_instructions.fr.txt
+-rw-r--r--   0        0        0      366 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/email/password_reset_instructions.txt
+-rw-r--r--   0        0        0      640 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/forgotten_password.html
+-rw-r--r--   0        0        0     1088 2021-09-21 08:49:20.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/login.html
+-rw-r--r--   0        0        0      912 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/password_reset.fr.html
+-rw-r--r--   0        0        0      893 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/password_reset.html
+-rw-r--r--   0        0        0    12248 2024-03-25 13:17:52.053741 abilian_sbe-1.1.9/src/abilian/services/auth/views.py
+-rw-r--r--   0        0        0     3158 2024-02-07 15:10:35.374760 abilian_sbe-1.1.9/src/abilian/services/base.py
+-rw-r--r--   0        0        0      144 2024-02-07 15:10:35.374889 abilian_sbe-1.1.9/src/abilian/services/blob_store/__init__.py
+-rw-r--r--   0        0        0    15894 2024-03-25 13:17:52.054147 abilian_sbe-1.1.9/src/abilian/services/blob_store/service.py
+-rw-r--r--   0        0        0     1097 2024-02-07 15:10:35.375234 abilian_sbe-1.1.9/src/abilian/services/conversion/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-27 16:00:06.095921 abilian_sbe-1.1.9/src/abilian/services/conversion/cache.py
+-rw-r--r--   0        0        0    35636 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/mugshot.jpg
+-rw-r--r--   0        0        0    52951 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/onepage.pdf
+-rw-r--r--   0        0        0    39540 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/picture.jpg
+-rw-r--r--   0        0        0   675299 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/rammstein.pdf
+-rw-r--r--   0        0        0      136 2024-02-07 15:10:35.375476 abilian_sbe-1.1.9/src/abilian/services/conversion/exceptions.py
+-rw-r--r--   0        0        0     1183 2024-02-07 15:10:35.375690 abilian_sbe-1.1.9/src/abilian/services/conversion/handler_lock.py
+-rw-r--r--   0        0        0    18184 2024-04-29 20:13:20.570800 abilian_sbe-1.1.9/src/abilian/services/conversion/handlers.py
+-rw-r--r--   0        0        0     7169 2024-03-25 13:17:52.054335 abilian_sbe-1.1.9/src/abilian/services/conversion/service.py
+-rw-r--r--   0        0        0     1032 2024-02-07 15:10:35.376858 abilian_sbe-1.1.9/src/abilian/services/conversion/util.py
+-rw-r--r--   0        0        0     3156 2024-02-07 15:10:35.376986 abilian_sbe-1.1.9/src/abilian/services/image/__init__.py
+-rw-r--r--   0        0        0      149 2024-02-07 15:10:35.377117 abilian_sbe-1.1.9/src/abilian/services/indexing/__init__.py
+-rw-r--r--   0        0        0     7037 2024-03-25 13:17:52.054588 abilian_sbe-1.1.9/src/abilian/services/indexing/adapter.py
+-rw-r--r--   0        0        0     2698 2024-02-07 15:10:35.377379 abilian_sbe-1.1.9/src/abilian/services/indexing/debug_toolbar.py
+-rw-r--r--   0        0        0     3172 2024-03-23 14:15:17.899575 abilian_sbe-1.1.9/src/abilian/services/indexing/schema.py
+-rw-r--r--   0        0        0    20879 2024-03-25 16:34:02.573063 abilian_sbe-1.1.9/src/abilian/services/indexing/service.py
+-rw-r--r--   0        0        0       96 2022-01-10 11:24:05.349623 abilian_sbe-1.1.9/src/abilian/services/preferences/__init__.py
+-rw-r--r--   0        0        0      911 2024-04-26 15:35:32.880378 abilian_sbe-1.1.9/src/abilian/services/preferences/models.py
+-rw-r--r--   0        0        0      557 2023-12-08 09:38:30.281087 abilian_sbe-1.1.9/src/abilian/services/preferences/panel.py
+-rw-r--r--   0        0        0     6325 2024-02-07 15:10:35.378602 abilian_sbe-1.1.9/src/abilian/services/preferences/service.py
+-rw-r--r--   0        0        0      872 2024-02-07 15:10:35.378849 abilian_sbe-1.1.9/src/abilian/services/security/__init__.py
+-rw-r--r--   0        0        0     2579 2024-03-23 14:15:18.808146 abilian_sbe-1.1.9/src/abilian/services/security/debug_toolbar.py
+-rw-r--r--   0        0        0    12170 2024-04-22 06:37:41.714744 abilian_sbe-1.1.9/src/abilian/services/security/models.py
+-rw-r--r--   0        0        0    30163 2024-03-23 14:15:18.804362 abilian_sbe-1.1.9/src/abilian/services/security/service.py
+-rw-r--r--   0        0        0      182 2024-02-07 15:10:35.379428 abilian_sbe-1.1.9/src/abilian/services/settings/__init__.py
+-rw-r--r--   0        0        0     3401 2024-03-25 13:17:52.055390 abilian_sbe-1.1.9/src/abilian/services/settings/models.py
+-rw-r--r--   0        0        0     3958 2024-03-23 14:15:18.793633 abilian_sbe-1.1.9/src/abilian/services/settings/service.py
+-rw-r--r--   0        0        0       96 2022-01-10 11:24:05.352465 abilian_sbe-1.1.9/src/abilian/services/viewtracker/__init__.py
+-rw-r--r--   0        0        0     1620 2022-01-10 11:24:05.352622 abilian_sbe-1.1.9/src/abilian/services/viewtracker/models.py
+-rw-r--r--   0        0        0     2022 2022-01-10 11:24:05.352797 abilian_sbe-1.1.9/src/abilian/services/viewtracker/service.py
+-rw-r--r--   0        0        0      185 2024-02-07 15:10:35.380063 abilian_sbe-1.1.9/src/abilian/services/vocabularies/__init__.py
+-rw-r--r--   0        0        0     7075 2024-02-07 15:10:35.380319 abilian_sbe-1.1.9/src/abilian/services/vocabularies/admin.py
+-rw-r--r--   0        0        0     1061 2024-03-25 13:17:52.055514 abilian_sbe-1.1.9/src/abilian/services/vocabularies/forms.py
+-rw-r--r--   0        0        0     4962 2024-04-26 15:36:07.554631 abilian_sbe-1.1.9/src/abilian/services/vocabularies/models.py
+-rw-r--r--   0        0        0     1623 2024-03-25 13:17:52.055812 abilian_sbe-1.1.9/src/abilian/services/vocabularies/service.py
+-rw-r--r--   0        0        0     2203 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/vocabularies/templates/admin/macros/vocabularies.html
+-rw-r--r--   0        0        0      743 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/services/vocabularies/templates/admin/vocabularies.html
+-rw-r--r--   0        0        0    24611 2023-12-08 18:07:26.568967 abilian_sbe-1.1.9/src/abilian/translations/de_DE/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    26454 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    26922 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24612 2023-12-08 18:07:26.569726 abilian_sbe-1.1.9/src/abilian/translations/es_ES/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    32978 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24610 2023-12-08 18:07:26.570308 abilian_sbe-1.1.9/src/abilian/translations/fr_FR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24556 2023-12-08 18:07:26.570781 abilian_sbe-1.1.9/src/abilian/translations/id_ID/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24656 2023-12-08 18:07:26.571595 abilian_sbe-1.1.9/src/abilian/translations/it_IT/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24657 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/translations/messages.pot
+-rw-r--r--   0        0        0    30696 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/translations/nl/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24610 2023-12-08 18:07:26.572264 abilian_sbe-1.1.9/src/abilian/translations/nl_NL/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24626 2023-12-08 18:07:26.573015 abilian_sbe-1.1.9/src/abilian/translations/pt_BR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24656 2023-12-08 18:07:26.573244 abilian_sbe-1.1.9/src/abilian/translations/pt_PT/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24612 2023-12-08 18:07:26.573938 abilian_sbe-1.1.9/src/abilian/translations/tr_TR/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24607 2023-12-08 18:07:26.574531 abilian_sbe-1.1.9/src/abilian/translations/zh_CN/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    24607 2023-12-08 18:07:26.575133 abilian_sbe-1.1.9/src/abilian/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0      217 2023-12-08 09:38:30.283288 abilian_sbe-1.1.9/src/abilian/web/__init__.py
+-rw-r--r--   0        0        0     2085 2024-03-25 13:17:52.056056 abilian_sbe-1.1.9/src/abilian/web/access_blueprint.py
+-rw-r--r--   0        0        0    19133 2024-03-25 13:17:52.056460 abilian_sbe-1.1.9/src/abilian/web/action.py
+-rw-r--r--   0        0        0      138 2024-02-07 15:10:35.381341 abilian_sbe-1.1.9/src/abilian/web/admin/__init__.py
+-rw-r--r--   0        0        0     6430 2024-03-25 13:17:52.056755 abilian_sbe-1.1.9/src/abilian/web/admin/extension.py
+-rw-r--r--   0        0        0     1354 2024-02-07 15:10:35.381576 abilian_sbe-1.1.9/src/abilian/web/admin/panel.py
+-rw-r--r--   0        0        0       55 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/panels/__init__.py
+-rw-r--r--   0        0        0    13276 2024-03-25 13:17:52.057294 abilian_sbe-1.1.9/src/abilian/web/admin/panels/audit.py
+-rw-r--r--   0        0        0     6479 2024-02-07 15:10:35.382146 abilian_sbe-1.1.9/src/abilian/web/admin/panels/dashboard.py
+-rw-r--r--   0        0        0        0 2024-03-25 13:17:52.057346 abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/__init__.py
+-rw-r--r--   0        0        0  2190838 2024-03-25 13:17:52.068043 abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/ip_country.mmdb
+-rw-r--r--   0        0        0      676 2024-03-25 13:17:52.068455 abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/ip_country_code.py
+-rwxr-xr-x   0        0        0     2105 2024-03-25 13:17:52.068739 abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/update_ip_country.py
+-rw-r--r--   0        0        0     2067 2024-03-23 14:15:18.699919 abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/__init__.py
+-rw-r--r--   0        0        0      726 2024-03-25 13:17:52.068861 abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/forms.py
+-rw-r--r--   0        0        0     6249 2024-03-23 14:15:18.701819 abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/views.py
+-rw-r--r--   0        0        0      633 2022-01-10 11:24:05.356234 abilian_sbe-1.1.9/src/abilian/web/admin/panels/impersonate.py
+-rw-r--r--   0        0        0      987 2024-03-25 13:17:52.069560 abilian_sbe-1.1.9/src/abilian/web/admin/panels/login_sessions.py
+-rw-r--r--   0        0        0     4106 2024-02-07 15:10:35.382607 abilian_sbe-1.1.9/src/abilian/web/admin/panels/settings.py
+-rw-r--r--   0        0        0     1079 2024-03-25 13:17:52.070475 abilian_sbe-1.1.9/src/abilian/web/admin/panels/sysinfo.py
+-rw-r--r--   0        0        0     2036 2024-03-23 14:15:18.704352 abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/__init__.py
+-rw-r--r--   0        0        0     2817 2024-03-25 13:17:52.070598 abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/forms.py
+-rw-r--r--   0        0        0     7029 2024-03-25 13:17:52.071238 abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/views.py
+-rw-r--r--   0        0        0      566 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/_base.html
+-rw-r--r--   0        0        0     1084 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/_macros.html
+-rw-r--r--   0        0        0     5133 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/audit.html
+-rw-r--r--   0        0        0     5542 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/dashboard.html
+-rw-r--r--   0        0        0     3907 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/group_view.html
+-rw-r--r--   0        0        0     1032 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/groups.html
+-rw-r--r--   0        0        0     1073 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/login_sessions.html
+-rw-r--r--   0        0        0      641 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/settings.html
+-rw-r--r--   0        0        0      684 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/settings_session_lifetime.html
+-rw-r--r--   0        0        0     1224 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/sysinfo.html
+-rw-r--r--   0        0        0     1129 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/users.html
+-rw-r--r--   0        0        0     3835 2024-03-25 13:17:52.071356 abilian_sbe-1.1.9/src/abilian/web/assets/__init__.py
+-rw-r--r--   0        0        0    13476 2024-03-25 13:17:52.072069 abilian_sbe-1.1.9/src/abilian/web/assets/filters.py
+-rw-r--r--   0        0        0     6336 2024-02-07 15:10:35.384025 abilian_sbe-1.1.9/src/abilian/web/assets/mixin.py
+-rw-r--r--   0        0        0      230 2024-02-07 15:10:35.384143 abilian_sbe-1.1.9/src/abilian/web/attachments/__init__.py
+-rw-r--r--   0        0        0     4373 2024-03-23 14:15:18.738293 abilian_sbe-1.1.9/src/abilian/web/attachments/extension.py
+-rw-r--r--   0        0        0      701 2024-03-25 13:17:52.072175 abilian_sbe-1.1.9/src/abilian/web/attachments/forms.py
+-rw-r--r--   0        0        0     4405 2024-03-25 13:17:52.072629 abilian_sbe-1.1.9/src/abilian/web/attachments/views.py
+-rw-r--r--   0        0        0      170 2024-02-07 15:10:35.384555 abilian_sbe-1.1.9/src/abilian/web/comments/__init__.py
+-rw-r--r--   0        0        0     1325 2024-03-23 14:15:18.557703 abilian_sbe-1.1.9/src/abilian/web/comments/extension.py
+-rw-r--r--   0        0        0      684 2024-03-25 13:17:52.072741 abilian_sbe-1.1.9/src/abilian/web/comments/forms.py
+-rw-r--r--   0        0        0     4027 2024-03-25 13:17:52.073071 abilian_sbe-1.1.9/src/abilian/web/comments/views.py
+-rw-r--r--   0        0        0       43 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/coreviews/__init__.py
+-rw-r--r--   0        0        0     2587 2024-02-07 15:10:35.384859 abilian_sbe-1.1.9/src/abilian/web/coreviews/users.py
+-rw-r--r--   0        0        0    28073 2024-03-25 13:17:52.073415 abilian_sbe-1.1.9/src/abilian/web/crm_frontend.py
+-rw-r--r--   0        0        0     2311 2024-03-25 13:17:52.073705 abilian_sbe-1.1.9/src/abilian/web/csrf.py
+-rw-r--r--   0        0        0     5092 2024-03-25 13:17:52.073816 abilian_sbe-1.1.9/src/abilian/web/errors.py
+-rw-r--r--   0        0        0     7697 2024-03-23 14:15:18.554813 abilian_sbe-1.1.9/src/abilian/web/filters.py
+-rw-r--r--   0        0        0      231 2024-02-01 15:05:42.069192 abilian_sbe-1.1.9/src/abilian/web/forms/__init__.py
+-rw-r--r--   0        0        0    26783 2024-03-25 13:17:52.074089 abilian_sbe-1.1.9/src/abilian/web/forms/fields.py
+-rw-r--r--   0        0        0      602 2024-02-07 15:10:35.385499 abilian_sbe-1.1.9/src/abilian/web/forms/filters.py
+-rw-r--r--   0        0        0     8273 2024-03-25 13:17:52.074393 abilian_sbe-1.1.9/src/abilian/web/forms/form.py
+-rw-r--r--   0        0        0     5096 2024-03-25 13:17:52.074500 abilian_sbe-1.1.9/src/abilian/web/forms/permissions.py
+-rw-r--r--   0        0        0     1014 2024-02-07 15:10:35.385952 abilian_sbe-1.1.9/src/abilian/web/forms/util.py
+-rw-r--r--   0        0        0     7497 2024-02-07 15:10:35.386072 abilian_sbe-1.1.9/src/abilian/web/forms/validators.py
+-rw-r--r--   0        0        0    52082 2024-03-25 13:17:52.074942 abilian_sbe-1.1.9/src/abilian/web/forms/widgets.py
+-rw-r--r--   0        0        0      803 2024-03-25 13:17:52.075459 abilian_sbe-1.1.9/src/abilian/web/frontend.py
+-rw-r--r--   0        0        0      397 2024-02-07 15:10:35.387073 abilian_sbe-1.1.9/src/abilian/web/http.py
+-rw-r--r--   0        0        0     3514 2024-03-25 13:17:52.075564 abilian_sbe-1.1.9/src/abilian/web/jinja.py
+-rw-r--r--   0        0        0     4670 2024-03-23 14:15:18.550644 abilian_sbe-1.1.9/src/abilian/web/nav.py
+-rw-r--r--   0        0        0       43 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/preferences/__init__.py
+-rw-r--r--   0        0        0     4703 2024-03-25 13:17:52.075688 abilian_sbe-1.1.9/src/abilian/web/preferences/user.py
+-rw-r--r--   0        0        0    26581 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootbox/bootbox.js
+-rw-r--r--   0        0        0    20127 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2023-12-08 18:07:26.582271 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0    67546 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0    35951 2023-12-08 18:07:26.583029 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0      484 2023-12-08 18:07:26.583201 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/js/npm.js
+-rw-r--r--   0        0        0     8099 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/.csscomb.json
+-rw-r--r--   0        0        0      456 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/.csslintrc
+-rw-r--r--   0        0        0     1518 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/alerts.less
+-rw-r--r--   0        0        0     1201 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/badges.less
+-rw-r--r--   0        0        0     1121 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/bootstrap.less
+-rw-r--r--   0        0        0      594 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/breadcrumbs.less
+-rw-r--r--   0        0        0     5659 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/button-groups.less
+-rw-r--r--   0        0        0     3565 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/buttons.less
+-rw-r--r--   0        0        0     5405 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/carousel.less
+-rw-r--r--   0        0        0      764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/close.less
+-rw-r--r--   0        0        0     1401 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/code.less
+-rw-r--r--   0        0        0      666 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/component-animations.less
+-rw-r--r--   0        0        0     4764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/dropdowns.less
+-rw-r--r--   0        0        0    14935 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/forms.less
+-rw-r--r--   0        0        0    19803 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/glyphicons.less
+-rw-r--r--   0        0        0     1387 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/grid.less
+-rw-r--r--   0        0        0     4215 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/input-groups.less
+-rw-r--r--   0        0        0      984 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/jumbotron.less
+-rw-r--r--   0        0        0     1079 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/labels.less
+-rw-r--r--   0        0        0     3022 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/list-group.less
+-rw-r--r--   0        0        0      780 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/media.less
+-rw-r--r--   0        0        0      257 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/alerts.less
+-rw-r--r--   0        0        0      139 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/background-variant.less
+-rw-r--r--   0        0        0      468 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/border-radius.less
+-rw-r--r--   0        0        0     1080 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/buttons.less
+-rw-r--r--   0        0        0      120 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/center-block.less
+-rw-r--r--   0        0        0      605 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/clearfix.less
+-rw-r--r--   0        0        0     2641 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/forms.less
+-rw-r--r--   0        0        0     4388 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/gradients.less
+-rw-r--r--   0        0        0     2784 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/grid-framework.less
+-rw-r--r--   0        0        0     3094 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/grid.less
+-rw-r--r--   0        0        0      579 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/hide-text.less
+-rw-r--r--   0        0        0     1062 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/image.less
+-rw-r--r--   0        0        0      161 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/labels.less
+-rw-r--r--   0        0        0      533 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/list-group.less
+-rw-r--r--   0        0        0      232 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/nav-divider.less
+-rw-r--r--   0        0        0      364 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/nav-vertical-align.less
+-rw-r--r--   0        0        0      148 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/opacity.less
+-rw-r--r--   0        0        0      438 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/pagination.less
+-rw-r--r--   0        0        0      537 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/panels.less
+-rw-r--r--   0        0        0      191 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/progress-bar.less
+-rw-r--r--   0        0        0      248 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/reset-filter.less
+-rw-r--r--   0        0        0      196 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/resize.less
+-rw-r--r--   0        0        0      343 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/responsive-visibility.less
+-rw-r--r--   0        0        0      127 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/size.less
+-rw-r--r--   0        0        0      159 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/tab-focus.less
+-rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/table-row.less
+-rw-r--r--   0        0        0      116 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/text-emphasis.less
+-rw-r--r--   0        0        0      162 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/text-overflow.less
+-rw-r--r--   0        0        0     6650 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/vendor-prefixes.less
+-rw-r--r--   0        0        0     1102 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins.less
+-rw-r--r--   0        0        0     3565 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/modals.less
+-rw-r--r--   0        0        0    14667 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/navbar.less
+-rw-r--r--   0        0        0     4930 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/navs.less
+-rw-r--r--   0        0        0     7650 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/normalize.less
+-rw-r--r--   0        0        0      861 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/pager.less
+-rw-r--r--   0        0        0     2001 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/pagination.less
+-rw-r--r--   0        0        0     6151 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/panels.less
+-rw-r--r--   0        0        0     3509 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/popovers.less
+-rw-r--r--   0        0        0     2133 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/print.less
+-rw-r--r--   0        0        0     1925 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/progress-bars.less
+-rw-r--r--   0        0        0      546 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/responsive-embed.less
+-rw-r--r--   0        0        0     4262 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/responsive-utilities.less
+-rw-r--r--   0        0        0     3122 2023-12-08 18:07:26.583819 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/scaffolding.less
+-rw-r--r--   0        0        0     4612 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/tables.less
+-rw-r--r--   0        0        0     7812 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/theme.less
+-rw-r--r--   0        0        0      753 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/thumbnails.less
+-rw-r--r--   0        0        0     2937 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/tooltip.less
+-rw-r--r--   0        0        0     5951 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/type.less
+-rw-r--r--   0        0        0      747 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/utilities.less
+-rw-r--r--   0        0        0    27053 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/variables.less
+-rw-r--r--   0        0        0      527 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/wells.less
+-rw-r--r--   0        0        0    32929 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/css/datepicker.css
+-rw-r--r--   0        0        0    41744 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/bootstrap-datepicker.js
+-rw-r--r--   0        0        0      949 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ar.js
+-rw-r--r--   0        0        0      836 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.bg.js
+-rw-r--r--   0        0        0      639 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ca.js
+-rw-r--r--   0        0        0      711 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cs.js
+-rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cy.js
+-rw-r--r--   0        0        0      673 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.da.js
+-rw-r--r--   0        0        0      697 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.de.js
+-rw-r--r--   0        0        0      896 2023-12-08 18:07:26.575764 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.el.js
+-rw-r--r--   0        0        0      647 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.es.js
+-rw-r--r--   0        0        0      673 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.et.js
+-rw-r--r--   0        0        0      726 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fi.js
+-rw-r--r--   0        0        0      699 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fr.js
+-rw-r--r--   0        0        0      563 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.gl.js
+-rw-r--r--   0        0        0      767 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.he.js
+-rw-r--r--   0        0        0      597 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hr.js
+-rw-r--r--   0        0        0      715 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hu.js
+-rw-r--r--   0        0        0      652 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.id.js
+-rw-r--r--   0        0        0      709 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.is.js
+-rw-r--r--   0        0        0      694 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.it.js
+-rw-r--r--   0        0        0      665 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ja.js
+-rw-r--r--   0        0        0     1209 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ka.js
+-rw-r--r--   0        0        0      637 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.kr.js
+-rw-r--r--   0        0        0      764 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lt.js
+-rw-r--r--   0        0        0      732 2023-12-08 18:07:26.576553 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lv.js
+-rw-r--r--   0        0        0      888 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.mk.js
+-rw-r--r--   0        0        0      621 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ms.js
+-rw-r--r--   0        0        0      663 2023-12-08 18:07:26.577049 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nb.js
+-rw-r--r--   0        0        0      754 2023-12-08 18:07:26.577726 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl-BE.js
+-rw-r--r--   0        0        0      643 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl.js
+-rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.no.js
+-rw-r--r--   0        0        0      775 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pl.js
+-rw-r--r--   0        0        0      662 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt-BR.js
+-rw-r--r--   0        0        0      717 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt.js
+-rw-r--r--   0        0        0      676 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ro.js
+-rw-r--r--   0        0        0      647 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs-latin.js
+-rw-r--r--   0        0        0      835 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs.js
+-rw-r--r--   0        0        0      883 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ru.js
+-rw-r--r--   0        0        0      693 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sk.js
+-rw-r--r--   0        0        0      644 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sl.js
+-rw-r--r--   0        0        0      659 2023-12-08 18:07:26.578317 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sq.js
+-rw-r--r--   0        0        0      690 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sv.js
+-rw-r--r--   0        0        0      773 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sw.js
+-rw-r--r--   0        0        0     1008 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.th.js
+-rw-r--r--   0        0        0      671 2023-12-08 18:07:26.578942 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.tr.js
+-rw-r--r--   0        0        0      870 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ua.js
+-rw-r--r--   0        0        0      889 2023-12-08 18:07:26.579365 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.uk.js
+-rw-r--r--   0        0        0      796 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-CN.js
+-rw-r--r--   0        0        0      891 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-TW.js
+-rw-r--r--   0        0        0     5285 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/less/datepicker.less
+-rw-r--r--   0        0        0    10173 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/LICENSE
+-rw-r--r--   0        0        0    25530 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/bootstrap-switch.js
+-rw-r--r--   0        0        0     4668 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/less/bootstrap3/bootstrap-switch.less
+-rw-r--r--   0        0        0     2990 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.css
+-rw-r--r--   0        0        0     2595 2023-12-08 18:07:26.579923 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.min.css
+-rw-r--r--   0        0        0    28462 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.js
+-rw-r--r--   0        0        0    16007 2023-12-08 18:07:26.580842 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.min.js
+-rw-r--r--   0        0        0     3445 2023-12-08 18:07:26.581375 abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/less/timepicker.less
+-rw-r--r--   0        0        0   314777 2024-03-27 08:36:58.813662 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/CHANGES.md
+-rw-r--r--   0        0        0    78399 2024-03-27 08:36:58.814352 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/LICENSE.md
+-rw-r--r--   0        0        0     1383 2024-03-27 08:36:58.814546 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/README.md
+-rw-r--r--   0        0        0      568 2024-03-27 08:36:58.814630 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/SECURITY.md
+-rw-r--r--   0        0        0     3180 2024-03-27 08:36:58.814794 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/adapters/jquery.js
+-rw-r--r--   0        0        0      246 2024-03-27 08:36:58.814878 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/bender-runner.config.json
+-rw-r--r--   0        0        0     3138 2024-03-27 08:36:58.815054 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/build-config.js
+-rw-r--r--   0        0        0   680302 2024-03-27 08:36:58.818578 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/ckeditor.js
+-rw-r--r--   0        0        0     1345 2024-03-27 08:36:58.818829 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/config.js
+-rw-r--r--   0        0        0     3092 2024-03-27 08:36:58.818979 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/contents.css
+-rw-r--r--   0        0        0    12599 2024-03-27 08:36:58.819304 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/af.js
+-rw-r--r--   0        0        0    15803 2024-03-27 08:36:58.819573 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ar.js
+-rw-r--r--   0        0        0    13612 2024-03-27 08:36:58.819747 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/az.js
+-rw-r--r--   0        0        0    18969 2024-03-27 08:36:58.819974 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bg.js
+-rw-r--r--   0        0        0    16521 2024-03-27 08:36:58.820237 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bn.js
+-rw-r--r--   0        0        0    12681 2024-03-27 08:36:58.820529 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bs.js
+-rw-r--r--   0        0        0    13924 2024-03-27 08:36:58.820809 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ca.js
+-rw-r--r--   0        0        0    13874 2024-03-27 08:36:58.821190 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/cs.js
+-rw-r--r--   0        0        0    12979 2024-03-27 08:36:58.821446 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/cy.js
+-rw-r--r--   0        0        0    13251 2024-03-27 08:36:58.821751 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/da.js
+-rw-r--r--   0        0        0    13952 2024-03-27 08:36:58.821967 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/de-ch.js
+-rw-r--r--   0        0        0    13945 2024-03-27 08:36:58.822246 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/de.js
+-rw-r--r--   0        0        0    20454 2024-03-27 08:36:58.822491 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/el.js
+-rw-r--r--   0        0        0    12617 2024-03-27 08:36:58.822779 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-au.js
+-rw-r--r--   0        0        0    12617 2024-03-27 08:36:58.823094 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-ca.js
+-rw-r--r--   0        0        0    12637 2024-03-27 08:36:58.823345 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-gb.js
+-rw-r--r--   0        0        0    12635 2024-03-27 08:36:58.823691 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en.js
+-rw-r--r--   0        0        0    13319 2024-03-27 08:36:58.823989 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/eo.js
+-rw-r--r--   0        0        0    14075 2024-03-27 08:36:58.824178 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/es-mx.js
+-rw-r--r--   0        0        0    14031 2024-03-27 08:36:58.824543 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/es.js
+-rw-r--r--   0        0        0    13022 2024-03-27 08:36:58.824939 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/et.js
+-rw-r--r--   0        0        0    13738 2024-03-27 08:36:58.825146 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/eu.js
+-rw-r--r--   0        0        0    17129 2024-03-27 08:36:58.825521 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fa.js
+-rw-r--r--   0        0        0    13363 2024-03-27 08:36:58.825793 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fi.js
+-rw-r--r--   0        0        0    13296 2024-03-27 08:36:58.826040 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fo.js
+-rw-r--r--   0        0        0    13769 2024-03-27 08:36:58.826334 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fr-ca.js
+-rw-r--r--   0        0        0    14495 2024-03-27 08:36:58.826596 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fr.js
+-rw-r--r--   0        0        0    14005 2024-03-27 08:36:58.826888 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/gl.js
+-rw-r--r--   0        0        0    20558 2024-03-27 08:36:58.827125 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/gu.js
+-rw-r--r--   0        0        0    15395 2024-03-27 08:36:58.827441 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/he.js
+-rw-r--r--   0        0        0    16668 2024-03-27 08:36:58.827658 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hi.js
+-rw-r--r--   0        0        0    12953 2024-03-27 08:36:58.827968 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hr.js
+-rw-r--r--   0        0        0    14158 2024-03-27 08:36:58.828462 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hu.js
+-rw-r--r--   0        0        0    12953 2024-03-27 08:36:58.828755 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/id.js
+-rw-r--r--   0        0        0    13066 2024-03-27 08:36:58.829035 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/is.js
+-rw-r--r--   0        0        0    14079 2024-03-27 08:36:58.829481 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/it.js
+-rw-r--r--   0        0        0    15353 2024-03-27 08:36:58.829815 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ja.js
+-rw-r--r--   0        0        0    21596 2024-03-27 08:36:58.830068 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ka.js
+-rw-r--r--   0        0        0    23848 2024-03-27 08:36:58.830371 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/km.js
+-rw-r--r--   0        0        0    13604 2024-03-27 08:36:58.830803 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ko.js
+-rw-r--r--   0        0        0    18533 2024-03-27 08:36:58.831033 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ku.js
+-rw-r--r--   0        0        0    13787 2024-03-27 08:36:58.831370 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/lt.js
+-rw-r--r--   0        0        0    14013 2024-03-27 08:36:58.831702 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/lv.js
+-rw-r--r--   0        0        0    14072 2024-03-27 08:36:58.832006 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/mk.js
+-rw-r--r--   0        0        0    16013 2024-03-27 08:36:58.832312 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/mn.js
+-rw-r--r--   0        0        0    12801 2024-03-27 08:36:58.832637 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ms.js
+-rw-r--r--   0        0        0    12872 2024-03-27 08:36:58.832903 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/nb.js
+-rw-r--r--   0        0        0    13274 2024-03-27 08:36:58.833202 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/nl.js
+-rw-r--r--   0        0        0    12917 2024-03-27 08:36:58.833429 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/no.js
+-rw-r--r--   0        0        0    14222 2024-03-27 08:36:58.833591 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/oc.js
+-rw-r--r--   0        0        0    14008 2024-03-27 08:36:58.833856 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pl.js
+-rw-r--r--   0        0        0    14028 2024-03-27 08:36:58.834089 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pt-br.js
+-rw-r--r--   0        0        0    13937 2024-03-27 08:36:58.834355 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pt.js
+-rw-r--r--   0        0        0    14562 2024-03-27 08:36:58.834607 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ro.js
+-rw-r--r--   0        0        0    19388 2024-03-27 08:36:58.834803 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ru.js
+-rw-r--r--   0        0        0    17745 2024-03-27 08:36:58.835027 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/si.js
+-rw-r--r--   0        0        0    13968 2024-03-27 08:36:58.835337 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sk.js
+-rw-r--r--   0        0        0    13157 2024-03-27 08:36:58.835684 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sl.js
+-rw-r--r--   0        0        0    14209 2024-03-27 08:36:58.835922 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sq.js
+-rw-r--r--   0        0        0    13226 2024-03-27 08:36:58.836159 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sr-latn.js
+-rw-r--r--   0        0        0    18199 2024-03-27 08:36:58.836301 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sr.js
+-rw-r--r--   0        0        0    13032 2024-03-27 08:36:58.836577 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sv.js
+-rw-r--r--   0        0        0    19588 2024-03-27 08:36:58.836793 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/th.js
+-rw-r--r--   0        0        0    13898 2024-03-27 08:36:58.837107 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/tr.js
+-rw-r--r--   0        0        0    16206 2024-03-27 08:36:58.837385 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/tt.js
+-rw-r--r--   0        0        0    18512 2024-03-27 08:36:58.837589 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ug.js
+-rw-r--r--   0        0        0    19509 2024-03-27 08:36:58.837809 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/uk.js
+-rw-r--r--   0        0        0    15078 2024-03-27 08:36:58.838109 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/vi.js
+-rw-r--r--   0        0        0    12353 2024-03-27 08:36:58.838366 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/zh-cn.js
+-rw-r--r--   0        0        0    12277 2024-03-27 08:36:58.838590 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/zh.js
+-rw-r--r--   0        0        0     2953 2024-03-27 08:36:58.838756 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js
+-rw-r--r--   0        0        0      887 2024-03-27 08:36:58.838893 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4156 2024-03-27 08:36:58.839044 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4351 2024-03-27 08:36:58.839190 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     4332 2024-03-27 08:36:58.839311 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4565 2024-03-27 08:36:58.839476 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     4788 2024-03-27 08:36:58.839631 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4938 2024-03-27 08:36:58.839774 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4389 2024-03-27 08:36:58.839942 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     4247 2024-03-27 08:36:58.840067 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4712 2024-03-27 08:36:58.840153 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4656 2024-03-27 08:36:58.840300 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7631 2024-03-27 08:36:58.840456 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4203 2024-03-27 08:36:58.840543 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4203 2024-03-27 08:36:58.840668 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4200 2024-03-27 08:36:58.840803 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4797 2024-03-27 08:36:58.840935 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4893 2024-03-27 08:36:58.841006 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4799 2024-03-27 08:36:58.841129 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es.js
+-rw-r--r--   0        0        0     4418 2024-03-27 08:36:58.841280 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4505 2024-03-27 08:36:58.841371 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     6152 2024-03-27 08:36:58.841545 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4760 2024-03-27 08:36:58.841673 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     4202 2024-03-27 08:36:58.841812 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js
+-rw-r--r--   0        0        0     4922 2024-03-27 08:36:58.841955 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     5309 2024-03-27 08:36:58.842085 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     4814 2024-03-27 08:36:58.842251 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     4410 2024-03-27 08:36:58.842392 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js
+-rw-r--r--   0        0        0     4955 2024-03-27 08:36:58.842533 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4214 2024-03-27 08:36:58.842681 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js
+-rw-r--r--   0        0        0     4281 2024-03-27 08:36:58.842819 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4766 2024-03-27 08:36:58.842973 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4039 2024-03-27 08:36:58.843092 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5237 2024-03-27 08:36:58.843201 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/it.js
+-rw-r--r--   0        0        0     5200 2024-03-27 08:36:58.843327 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     5218 2024-03-27 08:36:58.843452 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/km.js
+-rw-r--r--   0        0        0     5599 2024-03-27 08:36:58.843592 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     6033 2024-03-27 08:36:58.843732 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4209 2024-03-27 08:36:58.843857 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     4832 2024-03-27 08:36:58.843990 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     4591 2024-03-27 08:36:58.844115 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js
+-rw-r--r--   0        0        0     4207 2024-03-27 08:36:58.844220 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js
+-rw-r--r--   0        0        0     4457 2024-03-27 08:36:58.844334 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4532 2024-03-27 08:36:58.844484 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     4443 2024-03-27 08:36:58.844609 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/no.js
+-rw-r--r--   0        0        0     5098 2024-03-27 08:36:58.844711 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     5160 2024-03-27 08:36:58.844838 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     4927 2024-03-27 08:36:58.844966 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4568 2024-03-27 08:36:58.845105 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4559 2024-03-27 08:36:58.845213 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     6646 2024-03-27 08:36:58.845338 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     6145 2024-03-27 08:36:58.845453 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4769 2024-03-27 08:36:58.845564 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4548 2024-03-27 08:36:58.845694 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     4933 2024-03-27 08:36:58.845809 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4896 2024-03-27 08:36:58.845922 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7514 2024-03-27 08:36:58.846042 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     4369 2024-03-27 08:36:58.846156 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4578 2024-03-27 08:36:58.846278 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4579 2024-03-27 08:36:58.846392 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     4518 2024-03-27 08:36:58.846513 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     6936 2024-03-27 08:36:58.846671 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6926 2024-03-27 08:36:58.846788 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     5400 2024-03-27 08:36:58.846908 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4148 2024-03-27 08:36:58.847025 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4357 2024-03-27 08:36:58.847138 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     1934 2024-03-27 08:36:58.847247 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/about.js
+-rw-r--r--   0        0        0    12236 2024-03-27 08:36:58.847437 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png
+-rw-r--r--   0        0        0     5650 2024-03-27 08:36:58.847545 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/logo_ckeditor.png
+-rw-r--r--   0        0        0     3809 2024-03-27 08:36:58.847712 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/clipboard/dialogs/paste.js
+-rw-r--r--   0        0        0      166 2024-03-27 08:36:58.847839 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/dialog/dialogDefinition.js
+-rw-r--r--   0        0        0      231 2024-03-27 08:36:58.847949 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/dialog/styles/dialog.css
+-rw-r--r--   0        0        0     5692 2024-03-27 08:36:58.848093 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/icons.png
+-rw-r--r--   0        0        0    18632 2024-03-27 08:36:58.848248 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/icons_hidpi.png
+-rw-r--r--   0        0        0    21529 2024-03-27 08:36:58.848475 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/image/dialogs/image.js
+-rw-r--r--   0        0        0     1610 2024-03-27 08:36:58.848611 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/image/images/noimage.png
+-rw-r--r--   0        0        0     2207 2024-03-27 08:36:58.848725 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/dialogs/anchor.js
+-rw-r--r--   0        0        0    13234 2024-03-27 08:36:58.848992 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/dialogs/link.js
+-rw-r--r--   0        0        0      752 2024-03-27 08:36:58.849097 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/images/anchor.png
+-rw-r--r--   0        0        0     1109 2024-03-27 08:36:58.849197 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/images/hidpi/anchor.png
+-rw-r--r--   0        0        0      176 2024-03-27 08:36:58.849305 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/magicline/images/hidpi/icon-rtl.png
+-rw-r--r--   0        0        0      199 2024-03-27 08:36:58.849400 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/magicline/images/hidpi/icon.png
+-rw-r--r--   0        0        0      138 2024-03-27 08:36:58.849492 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/magicline/images/icon-rtl.png
+-rw-r--r--   0        0        0      133 2024-03-27 08:36:58.849599 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/magicline/images/icon.png
+-rw-r--r--   0        0        0     2209 2024-03-27 08:36:58.849753 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromgdocs/filter/default.js
+-rw-r--r--   0        0        0     3510 2024-03-27 08:36:58.849898 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromlibreoffice/filter/default.js
+-rw-r--r--   0        0        0    19902 2024-03-27 08:36:58.850050 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromword/filter/default.js
+-rw-r--r--   0        0        0    10380 2024-03-27 08:36:58.850275 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/common.js
+-rw-r--r--   0        0        0     3932 2024-03-27 08:36:58.850347 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/image.js
+-rw-r--r--   0        0        0      221 2024-03-27 08:36:58.850419 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/CHANGELOG.md
+-rw-r--r--   0        0        0     1476 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/LICENSE.md
+-rw-r--r--   0        0        0     4565 2024-03-27 08:36:58.850534 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/README.md
+-rw-r--r--   0        0        0      396 2024-03-27 08:36:58.850602 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/dialog.css
+-rw-r--r--   0        0        0    16136 2024-03-27 08:36:58.850817 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/options.js
+-rw-r--r--   0        0        0     1302 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/toolbar.css
+-rw-r--r--   0        0        0      356 2024-03-27 08:36:58.850962 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/skins/moono-lisa/scayt.css
+-rw-r--r--   0        0        0      738 2024-03-27 08:36:58.851090 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt
+-rw-r--r--   0        0        0     4547 2024-03-27 08:36:58.851232 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/af.js
+-rw-r--r--   0        0        0     4796 2024-03-27 08:36:58.851351 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ar.js
+-rw-r--r--   0        0        0     3407 2024-03-27 08:36:58.851426 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/az.js
+-rw-r--r--   0        0        0     4820 2024-03-27 08:36:58.851565 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/bg.js
+-rw-r--r--   0        0        0     5028 2024-03-27 08:36:58.851691 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ca.js
+-rw-r--r--   0        0        0     4985 2024-03-27 08:36:58.851844 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cs.js
+-rw-r--r--   0        0        0     4909 2024-03-27 08:36:58.851959 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cy.js
+-rw-r--r--   0        0        0     3380 2024-03-27 08:36:58.852068 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/da.js
+-rw-r--r--   0        0        0     4807 2024-03-27 08:36:58.852143 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js
+-rw-r--r--   0        0        0     4798 2024-03-27 08:36:58.852257 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de.js
+-rw-r--r--   0        0        0     7746 2024-03-27 08:36:58.852368 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/el.js
+-rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852436 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-au.js
+-rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852512 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js
+-rw-r--r--   0        0        0     4564 2024-03-27 08:36:58.852687 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js
+-rw-r--r--   0        0        0     4561 2024-03-27 08:36:58.852820 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en.js
+-rw-r--r--   0        0        0     4082 2024-03-27 08:36:58.852936 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eo.js
+-rw-r--r--   0        0        0     4790 2024-03-27 08:36:58.853011 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js
+-rw-r--r--   0        0        0     4961 2024-03-27 08:36:58.853127 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es.js
+-rw-r--r--   0        0        0     3831 2024-03-27 08:36:58.853241 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/et.js
+-rw-r--r--   0        0        0     4563 2024-03-27 08:36:58.853317 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eu.js
+-rw-r--r--   0        0        0     5786 2024-03-27 08:36:58.853427 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fa.js
+-rw-r--r--   0        0        0     4599 2024-03-27 08:36:58.853530 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fi.js
+-rw-r--r--   0        0        0     3234 2024-03-27 08:36:58.853634 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js
+-rw-r--r--   0        0        0     3870 2024-03-27 08:36:58.853766 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr.js
+-rw-r--r--   0        0        0     5018 2024-03-27 08:36:58.853893 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/gl.js
+-rw-r--r--   0        0        0     5000 2024-03-27 08:36:58.854010 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/he.js
+-rw-r--r--   0        0        0     4405 2024-03-27 08:36:58.854128 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hr.js
+-rw-r--r--   0        0        0     4149 2024-03-27 08:36:58.854243 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hu.js
+-rw-r--r--   0        0        0     4568 2024-03-27 08:36:58.854346 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/id.js
+-rw-r--r--   0        0        0     5034 2024-03-27 08:36:58.854453 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/it.js
+-rw-r--r--   0        0        0     3998 2024-03-27 08:36:58.854558 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ja.js
+-rw-r--r--   0        0        0     4765 2024-03-27 08:36:58.854651 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/km.js
+-rw-r--r--   0        0        0     4934 2024-03-27 08:36:58.854754 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ko.js
+-rw-r--r--   0        0        0     7578 2024-03-27 08:36:58.854858 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ku.js
+-rw-r--r--   0        0        0     4606 2024-03-27 08:36:58.854964 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lt.js
+-rw-r--r--   0        0        0     5036 2024-03-27 08:36:58.855071 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lv.js
+-rw-r--r--   0        0        0     3446 2024-03-27 08:36:58.855172 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nb.js
+-rw-r--r--   0        0        0     4740 2024-03-27 08:36:58.855281 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nl.js
+-rw-r--r--   0        0        0     3446 2024-03-27 08:36:58.855381 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/no.js
+-rw-r--r--   0        0        0     3844 2024-03-27 08:36:58.855449 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/oc.js
+-rw-r--r--   0        0        0     4343 2024-03-27 08:36:58.855588 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pl.js
+-rw-r--r--   0        0        0     3844 2024-03-27 08:36:58.855694 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js
+-rw-r--r--   0        0        0     4809 2024-03-27 08:36:58.855803 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt.js
+-rw-r--r--   0        0        0     4692 2024-03-27 08:36:58.855872 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ro.js
+-rw-r--r--   0        0        0     7561 2024-03-27 08:36:58.855996 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ru.js
+-rw-r--r--   0        0        0     4902 2024-03-27 08:36:58.856110 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/si.js
+-rw-r--r--   0        0        0     4778 2024-03-27 08:36:58.856242 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sk.js
+-rw-r--r--   0        0        0     4363 2024-03-27 08:36:58.856360 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sl.js
+-rw-r--r--   0        0        0     5005 2024-03-27 08:36:58.856472 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sq.js
+-rw-r--r--   0        0        0     4728 2024-03-27 08:36:58.856546 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js
+-rw-r--r--   0        0        0     7530 2024-03-27 08:36:58.856619 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr.js
+-rw-r--r--   0        0        0     3498 2024-03-27 08:36:58.856725 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sv.js
+-rw-r--r--   0        0        0     4690 2024-03-27 08:36:58.856826 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/th.js
+-rw-r--r--   0        0        0     4493 2024-03-27 08:36:58.856936 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tr.js
+-rw-r--r--   0        0        0     6743 2024-03-27 08:36:58.857049 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tt.js
+-rw-r--r--   0        0        0     5017 2024-03-27 08:36:58.857170 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ug.js
+-rw-r--r--   0        0        0     6384 2024-03-27 08:36:58.857274 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/uk.js
+-rw-r--r--   0        0        0     6099 2024-03-27 08:36:58.857376 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/vi.js
+-rw-r--r--   0        0        0     4395 2024-03-27 08:36:58.857478 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js
+-rw-r--r--   0        0        0     4175 2024-03-27 08:36:58.857593 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh.js
+-rw-r--r--   0        0        0     5005 2024-03-27 08:36:58.857726 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/specialchar.js
+-rw-r--r--   0        0        0     9043 2024-03-27 08:36:58.857909 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/table/dialogs/table.js
+-rw-r--r--   0        0        0     1109 2024-03-27 08:36:58.858052 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/tableselection/styles/tableselection.css
+-rw-r--r--   0        0        0     7354 2024-03-27 08:36:58.858181 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/tabletools/dialogs/tableCell.js
+-rw-r--r--   0        0        0      220 2024-03-27 08:36:58.858318 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/widget/images/handle.png
+-rw-r--r--   0        0        0    67340 2024-03-27 08:36:58.858668 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/css/samples.css
+-rw-r--r--   0        0        0      383 2024-03-27 08:36:58.858798 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/github-top.png
+-rw-r--r--   0        0        0    13086 2024-03-27 08:36:58.859050 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/header-bg.png
+-rw-r--r--   0        0        0      123 2024-03-27 08:36:58.859145 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/header-separator.png
+-rw-r--r--   0        0        0     5634 2024-03-27 08:36:58.859237 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/logo.png
+-rw-r--r--   0        0        0    10887 2024-03-27 08:36:58.859344 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/logo.svg
+-rw-r--r--   0        0        0    12029 2024-03-27 08:36:58.859505 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/navigation-tip.png
+-rw-r--r--   0        0        0     7234 2024-03-27 08:36:58.859645 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/index.html
+-rw-r--r--   0        0        0     1594 2024-03-27 08:36:58.859750 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/js/sample.js
+-rw-r--r--   0        0        0     6426 2024-03-27 08:36:58.859870 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/js/sf.js
+-rw-r--r--   0        0        0     2911 2024-03-27 08:36:58.859981 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/ajax.html
+-rw-r--r--   0        0        0     7545 2024-03-27 08:36:58.860098 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/api.html
+-rw-r--r--   0        0        0     2523 2024-03-27 08:36:58.860207 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/appendto.html
+-rw-r--r--   0        0        0     4283 2024-03-27 08:36:58.860312 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/inlineall/logo.png
+-rw-r--r--   0        0        0     2161 2024-03-27 08:36:58.860417 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css
+-rw-r--r--   0        0        0     1627 2024-03-27 08:36:58.860526 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/posteddata.php
+-rw-r--r--   0        0        0    14449 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/sample.jpg
+-rw-r--r--   0        0        0     1461 2024-03-27 08:36:58.860633 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/uilanguages/languages.js
+-rw-r--r--   0        0        0    47840 2024-03-27 08:36:58.860818 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/datafiltering.html
+-rw-r--r--   0        0        0      895 2024-03-27 08:36:58.860941 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/dialog/assets/my_dialog.js
+-rw-r--r--   0        0        0     7590 2024-03-27 08:36:58.861067 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/dialog/dialog.html
+-rw-r--r--   0        0        0     4893 2024-03-27 08:36:58.861179 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/divreplace.html
+-rw-r--r--   0        0        0     4598 2024-03-27 08:36:58.861295 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/enterkey/enterkey.html
+-rw-r--r--   0        0        0     7565 2024-03-27 08:36:58.861448 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/htmlwriter/outputhtml.html
+-rw-r--r--   0        0        0     6054 2024-03-27 08:36:58.861567 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/index.html
+-rw-r--r--   0        0        0    10399 2024-03-27 08:36:58.861721 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlineall.html
+-rw-r--r--   0        0        0     6395 2024-03-27 08:36:58.861841 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlinebycode.html
+-rw-r--r--   0        0        0     5125 2024-03-27 08:36:58.861956 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlinetextarea.html
+-rw-r--r--   0        0        0     7754 2024-03-27 08:36:58.862073 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/jquery.html
+-rw-r--r--   0        0        0     8585 2024-03-27 08:36:58.862229 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/magicline/magicline.html
+-rw-r--r--   0        0        0     3132 2024-03-27 08:36:58.862377 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/readonly.html
+-rw-r--r--   0        0        0     7234 2024-03-27 08:36:58.862493 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/replacebyclass.html
+-rw-r--r--   0        0        0     7119 2024-03-27 08:36:58.862614 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/replacebycode.html
+-rw-r--r--   0        0        0     5112 2024-03-27 08:36:58.862729 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample.css
+-rw-r--r--   0        0        0     1693 2024-03-27 08:36:58.862825 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample.js
+-rw-r--r--   0        0        0      807 2024-03-27 08:36:58.862920 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample_posteddata.php
+-rw-r--r--   0        0        0     2609 2024-03-27 08:36:58.863020 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/tabindex.html
+-rw-r--r--   0        0        0     9122 2024-03-27 08:36:58.863173 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/toolbar/toolbar.html
+-rw-r--r--   0        0        0     2810 2024-03-27 08:36:58.863286 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/uicolor.html
+-rw-r--r--   0        0        0     4741 2024-03-27 08:36:58.863424 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/uilanguages.html
+-rw-r--r--   0        0        0     8311 2024-03-27 08:36:58.863572 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/wysiwygarea/fullpage.html
+-rw-r--r--   0        0        0     7233 2024-03-27 08:36:58.863692 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/xhtmlstyle.html
+-rw-r--r--   0        0        0     1758 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/css/fontello.css
+-rw-r--r--   0        0        0      188 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/LICENSE.txt
+-rw-r--r--   0        0        0      557 2023-12-08 18:07:26.684149 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/config.json
+-rw-r--r--   0        0        0     4988 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.eot
+-rw-r--r--   0        0        0     1701 2023-12-08 18:07:26.684402 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.svg
+-rw-r--r--   0        0        0     4820 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.ttf
+-rw-r--r--   0        0        0     2904 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.woff
+-rw-r--r--   0        0        0    15808 2024-03-27 08:36:58.863921 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/index.html
+-rw-r--r--   0        0        0     6523 2024-03-27 08:36:58.864052 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js
+-rw-r--r--   0        0        0     3838 2024-03-27 08:36:58.864165 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js
+-rw-r--r--   0        0        0    16651 2024-03-27 08:36:58.864280 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js
+-rw-r--r--   0        0        0     6850 2024-03-27 08:36:58.864475 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js
+-rw-r--r--   0        0        0     1094 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/LICENSE
+-rw-r--r--   0        0        0     8096 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.css
+-rw-r--r--   0        0        0   148874 2024-03-27 08:36:58.865555 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.js
+-rw-r--r--   0        0        0    12285 2024-03-27 08:36:58.865736 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/javascript.js
+-rw-r--r--   0        0        0      851 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/neo.css
+-rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.css
+-rw-r--r--   0        0        0     8080 2024-03-27 08:36:58.865871 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.js
+-rw-r--r--   0        0        0    13630 2024-03-27 08:36:58.866111 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog.css
+-rw-r--r--   0        0        0    14653 2024-03-27 08:36:58.866266 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie.css
+-rw-r--r--   0        0        0    15202 2024-03-27 08:36:58.866416 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie8.css
+-rw-r--r--   0        0        0    14682 2024-03-27 08:36:58.866559 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_iequirks.css
+-rw-r--r--   0        0        0    35902 2024-03-27 08:36:58.866699 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor.css
+-rw-r--r--   0        0        0    35983 2024-03-27 08:36:58.866811 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_gecko.css
+-rw-r--r--   0        0        0    36901 2024-03-27 08:36:58.866896 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie.css
+-rw-r--r--   0        0        0    37707 2024-03-27 08:36:58.866991 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie8.css
+-rw-r--r--   0        0        0    37550 2024-03-27 08:36:58.867085 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_iequirks.css
+-rw-r--r--   0        0        0     5692 2024-03-27 08:36:58.867195 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons.png
+-rw-r--r--   0        0        0    18632 2024-03-27 08:36:58.867294 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons_hidpi.png
+-rw-r--r--   0        0        0      191 2024-03-27 08:36:58.867401 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/arrow.png
+-rw-r--r--   0        0        0      615 2024-03-27 08:36:58.867463 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/close.png
+-rw-r--r--   0        0        0     1238 2024-03-27 08:36:58.867578 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/close.png
+-rw-r--r--   0        0        0     1071 2024-03-27 08:36:58.867645 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png
+-rw-r--r--   0        0        0     1062 2024-03-27 08:36:58.867710 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock.png
+-rw-r--r--   0        0        0     1623 2024-03-27 08:36:58.867777 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/refresh.png
+-rw-r--r--   0        0        0      511 2024-03-27 08:36:58.867843 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/lock-open.png
+-rw-r--r--   0        0        0      506 2024-03-27 08:36:58.867906 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/lock.png
+-rw-r--r--   0        0        0      757 2024-03-27 08:36:58.867968 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/refresh.png
+-rw-r--r--   0        0        0     2984 2024-03-27 08:36:58.868188 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/spinner.gif
+-rw-r--r--   0        0        0     2238 2024-03-27 08:36:58.868273 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/readme.md
+-rw-r--r--   0        0        0     5577 2024-03-27 08:36:58.868402 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/styles.js
+-rw-r--r--   0        0        0     6297 2024-03-27 08:36:58.868516 abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/vendor/promise.js
+-rw-r--r--   0        0        0     4554 2023-12-08 18:07:26.696227 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/css/jquery.dataTables.css
+-rw-r--r--   0        0        0     4477 2023-12-08 18:07:26.696469 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/css/jquery.dataTables_themeroller.css
+-rw-r--r--   0        0        0    27490 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/Sorting icons.psd
+-rw-r--r--   0        0        0      345 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/back_disabled.png
+-rw-r--r--   0        0        0      459 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/back_enabled.png
+-rw-r--r--   0        0        0      457 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/back_enabled_hover.png
+-rw-r--r--   0        0        0      894 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/favicon.ico
+-rw-r--r--   0        0        0      350 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/forward_disabled.png
+-rw-r--r--   0        0        0      468 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/forward_enabled.png
+-rw-r--r--   0        0        0      467 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/forward_enabled_hover.png
+-rw-r--r--   0        0        0      174 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/sort_asc.png
+-rw-r--r--   0        0        0      174 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/sort_asc_disabled.png
+-rw-r--r--   0        0        0      209 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/sort_both.png
+-rw-r--r--   0        0        0      172 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/sort_desc.png
+-rw-r--r--   0        0        0      159 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/sort_desc_disabled.png
+-rw-r--r--   0        0        0   377686 2023-12-08 18:07:26.698522 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/js/jquery.dataTables.js
+-rw-r--r--   0        0        0    70857 2023-12-08 18:07:26.699408 abilian_sbe-1.1.9/src/abilian/web/resources/datatables/js/jquery.dataTables.min.js
+-rw-r--r--   0        0        0     1635 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.camera.swf
+-rw-r--r--   0        0        0     2136 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.image.swf
+-rw-r--r--   0        0        0    32484 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.swf
+-rw-r--r--   0        0        0    84949 2023-12-08 18:07:26.700061 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.html5.js
+-rw-r--r--   0        0        0    34040 2023-12-08 18:07:26.700460 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.html5.min.js
+-rw-r--r--   0        0        0   104385 2023-12-08 18:07:26.701379 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.js
+-rw-r--r--   0        0        0    43718 2023-12-08 18:07:26.702196 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.min.js
+-rw-r--r--   0        0        0     1382 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/LICENSE
+-rw-r--r--   0        0        0    11508 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/FileAPI.exif.js
+-rw-r--r--   0        0        0    14866 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/FileAPI.id3.js
+-rwxr-xr-x   0        0        0    74053 2023-12-08 18:07:26.702774 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/caman.full.min.js
+-rwxr-xr-x   0        0        0    46149 2023-12-08 18:07:26.703173 abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/caman.min.js
+-rw-r--r--   0        0        0    32318 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/css/font-awesome.css
+-rw-r--r--   0        0        0    26711 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/css/font-awesome.min.css
+-rw-r--r--   0        0        0   106260 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/FontAwesome.otf
+-rw-r--r--   0        0        0    68875 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.eot
+-rw-r--r--   0        0        0   355981 2024-03-23 14:18:13.144763 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.svg
+-rw-r--r--   0        0        0   138204 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0        0        0    81284 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff
+-rw-r--r--   0        0        0    64464 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0        0        0      713 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/animated.less
+-rw-r--r--   0        0        0      585 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/bordered-pulled.less
+-rw-r--r--   0        0        0      452 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/core.less
+-rw-r--r--   0        0        0      119 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/fixed-width.less
+-rw-r--r--   0        0        0      465 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/font-awesome.less
+-rw-r--r--   0        0        0    42489 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/icons.less
+-rw-r--r--   0        0        0      370 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/larger.less
+-rw-r--r--   0        0        0      377 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/list.less
+-rw-r--r--   0        0        0      926 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/mixins.less
+-rw-r--r--   0        0        0      770 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/path.less
+-rw-r--r--   0        0        0      622 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/rotated-flipped.less
+-rw-r--r--   0        0        0      476 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/stacked.less
+-rw-r--r--   0        0        0    19203 2023-12-08 18:07:26.705406 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/variables.less
+-rw-r--r--   0        0        0      715 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_animated.scss
+-rw-r--r--   0        0        0      592 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_bordered-pulled.scss
+-rw-r--r--   0        0        0      459 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_core.scss
+-rw-r--r--   0        0        0      120 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_fixed-width.scss
+-rw-r--r--   0        0        0    43163 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_icons.scss
+-rw-r--r--   0        0        0      375 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_larger.scss
+-rw-r--r--   0        0        0      378 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_list.scss
+-rw-r--r--   0        0        0      946 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_mixins.scss
+-rw-r--r--   0        0        0      783 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_path.scss
+-rw-r--r--   0        0        0      672 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_rotated-flipped.scss
+-rw-r--r--   0        0        0      482 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_stacked.scss
+-rw-r--r--   0        0        0    19284 2023-12-08 18:07:26.705733 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_variables.scss
+-rw-r--r--   0        0        0      405 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/font-awesome.scss
+-rw-r--r--   0        0        0     2299 2023-12-08 18:07:26.705997 abilian_sbe-1.1.9/src/abilian/web/resources/highlightjs/default.min.css
+-rw-r--r--   0        0        0    34929 2023-12-08 18:07:26.706390 abilian_sbe-1.1.9/src/abilian/web/resources/highlightjs/highlight.min.js
+-rw-r--r--   0        0        0    73763 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/img/abilian.png
+-rw-r--r--   0        0        0     2242 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/img/avatar-default.png
+-rw-r--r--   0        0        0     2413 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/img/logo-abilian-32x32.png
+-rw-r--r--   0        0        0     2367 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/img/logo-abilian.png
+-rw-r--r--   0        0        0   284394 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/jquery/js/jquery-1.11.3.js
+-rw-r--r--   0        0        0    16621 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/jquery/js/jquery-migrate-1.2.1.js
+-rw-r--r--   0        0        0     1883 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/abilian-namespace.js
+-rw-r--r--   0        0        0     5096 2024-03-27 08:36:58.869020 abilian_sbe-1.1.9/src/abilian/web/resources/js/abilian.js
+-rw-r--r--   0        0        0    26660 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/datatables-advanced-search.js
+-rw-r--r--   0        0        0     4444 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/datatables-setup.js
+-rw-r--r--   0        0        0     1187 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/base.js
+-rw-r--r--   0        0        0     2420 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/delete.js
+-rw-r--r--   0        0        0     3226 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/dynamic-row.js
+-rw-r--r--   0        0        0     6988 2024-04-22 09:33:28.131121 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/file.js
+-rw-r--r--   0        0        0     3012 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/image.js
+-rw-r--r--   0        0        0     1910 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/richtext.js
+-rw-r--r--   0        0        0     3046 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/select2.js
+-rw-r--r--   0        0        0      783 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/tags.js
+-rw-r--r--   0        0        0     1002 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/abilian.less
+-rw-r--r--   0        0        0     1289 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/activities.less
+-rw-r--r--   0        0        0      612 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/admin.less
+-rw-r--r--   0        0        0       95 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/attachments.less
+-rw-r--r--   0        0        0      575 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/comments.less
+-rw-r--r--   0        0        0      157 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/compat.less
+-rw-r--r--   0        0        0      987 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/datatables.less
+-rw-r--r--   0        0        0     3050 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/form.less
+-rw-r--r--   0        0        0      155 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/layout.less
+-rw-r--r--   0        0        0      105 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/models.less
+-rw-r--r--   0        0        0     1054 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/navbar.less
+-rw-r--r--   0        0        0      624 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/print.less
+-rw-r--r--   0        0        0      225 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/search.less
+-rw-r--r--   0        0        0       74 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/user.less
+-rw-r--r--   0        0        0      165 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/less/variables.less
+-rw-r--r--   0        0        0      112 2023-12-08 18:07:26.706906 abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/cdn.txt
+-rw-r--r--   0        0        0   151701 2023-12-08 18:07:26.708021 abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/d3.min.js
+-rw-r--r--   0        0        0    12985 2023-12-08 18:07:26.708286 abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/nv.d3.css
+-rw-r--r--   0        0        0   587960 2023-12-08 18:07:26.710483 abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/nv.d3.js
+-rw-r--r--   0        0        0     4047 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/requirejs/domReady.js
+-rw-r--r--   0        0        0    86482 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/requirejs/require.js
+-rw-r--r--   0        0        0     4858 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      939 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/LICENSE
+-rw-r--r--   0        0        0     4727 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/README.md
+-rw-r--r--   0        0        0      206 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/bower.json
+-rw-r--r--   0        0        0     1732 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/component.json
+-rw-r--r--   0        0        0      637 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/composer.json
+-rw-r--r--   0        0        0      678 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/package.json
+-rwxr-xr-x   0        0        0     1490 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/release.sh
+-rw-r--r--   0        0        0    16890 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2-bootstrap.css
+-rw-r--r--   0        0        0     1849 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2-spinner.gif
+-rw-r--r--   0        0        0    19457 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.css
+-rw-r--r--   0        0        0     1030 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.jquery.json
+-rw-r--r--   0        0        0   148536 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.js
+-rw-r--r--   0        0        0    66596 2023-12-08 18:07:26.711090 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.min.js
+-rw-r--r--   0        0        0      529 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.png
+-rw-r--r--   0        0        0     1389 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ar.js
+-rw-r--r--   0        0        0     1003 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_az.js
+-rw-r--r--   0        0        0     1081 2023-12-08 18:07:26.711330 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_bg.js
+-rw-r--r--   0        0        0      952 2023-12-08 18:07:26.711571 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ca.js
+-rw-r--r--   0        0        0     1988 2023-12-08 18:07:26.711836 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_cs.js
+-rw-r--r--   0        0        0      853 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_da.js
+-rw-r--r--   0        0        0     1014 2023-12-08 18:07:26.712200 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_de.js
+-rw-r--r--   0        0        0     1128 2023-12-08 18:07:26.712422 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_el.js
+-rw-r--r--   0        0        0     1102 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_en.js.template
+-rw-r--r--   0        0        0     1177 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_es.js
+-rw-r--r--   0        0        0      886 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_et.js
+-rw-r--r--   0        0        0     1313 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_eu.js
+-rw-r--r--   0        0        0     1207 2023-12-08 18:07:26.712658 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fa.js
+-rw-r--r--   0        0        0      940 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fi.js
+-rw-r--r--   0        0        0     1077 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fr.js
+-rw-r--r--   0        0        0     1339 2023-12-08 18:07:26.712886 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_gl.js
+-rw-r--r--   0        0        0      885 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_he.js
+-rw-r--r--   0        0        0     1002 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_hr.js
+-rw-r--r--   0        0        0      802 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_hu.js
+-rw-r--r--   0        0        0      891 2023-12-08 18:07:26.713117 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_id.js
+-rw-r--r--   0        0        0      855 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_is.js
+-rw-r--r--   0        0        0      866 2023-12-08 18:07:26.713388 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_it.js
+-rw-r--r--   0        0        0      812 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ja.js
+-rw-r--r--   0        0        0     1078 2023-12-08 18:07:26.713638 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ka.js
+-rw-r--r--   0        0        0      871 2023-12-08 18:07:26.713909 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ko.js
+-rw-r--r--   0        0        0     1144 2023-12-08 18:07:26.714151 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_lt.js
+-rw-r--r--   0        0        0      999 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_lv.js
+-rw-r--r--   0        0        0     1064 2023-12-08 18:07:26.714300 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_mk.js
+-rw-r--r--   0        0        0      836 2023-12-08 18:07:26.714533 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ms.js
+-rw-r--r--   0        0        0     1145 2023-12-08 18:07:26.714857 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_nb.js
+-rw-r--r--   0        0        0      846 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_nl.js
+-rw-r--r--   0        0        0     2015 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pl.js
+-rw-r--r--   0        0        0      969 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pt-BR.js
+-rw-r--r--   0        0        0      891 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pt-PT.js
+-rw-r--r--   0        0        0      902 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ro.js
+-rw-r--r--   0        0        0     1058 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_rs.js
+-rw-r--r--   0        0        0     1171 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ru.js
+-rw-r--r--   0        0        0     1948 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_sk.js
+-rw-r--r--   0        0        0      847 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_sv.js
+-rw-r--r--   0        0        0     1063 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_th.js
+-rw-r--r--   0        0        0      831 2023-12-08 18:07:26.715096 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_tr.js
+-rw-r--r--   0        0        0      904 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ug-CN.js
+-rw-r--r--   0        0        0     1415 2023-12-08 18:07:26.715322 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_uk.js
+-rw-r--r--   0        0        0      959 2023-12-08 18:07:26.715543 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_vi.js
+-rw-r--r--   0        0        0      762 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_zh-CN.js
+-rw-r--r--   0        0        0      774 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_zh-TW.js
+-rw-r--r--   0        0        0      700 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2x2.png
+-rw-r--r--   0        0        0    15246 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/hogan-2.0.0.js
+-rw-r--r--   0        0        0    49022 2023-12-08 18:07:26.715929 abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js
+-rw-r--r--   0        0        0     1394 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.css
+-rw-r--r--   0        0        0      736 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.less
+-rw-r--r--   0        0        0    21804 2023-12-08 18:07:26.716267 abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.min.js
+-rw-r--r--   0        0        0      646 2024-04-22 07:49:45.045295 abilian_sbe-1.1.9/src/abilian/web/search/__init__.py
+-rw-r--r--   0        0        0     7183 2024-04-22 07:49:45.045624 abilian_sbe-1.1.9/src/abilian/web/search/criterion.py
+-rw-r--r--   0        0        0      318 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/search/templates/search/_base.html
+-rw-r--r--   0        0        0     4163 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/search/templates/search/search.html
+-rw-r--r--   0        0        0     5804 2024-02-07 15:10:35.387923 abilian_sbe-1.1.9/src/abilian/web/search/views.py
+-rw-r--r--   0        0        0      277 2024-04-22 07:49:45.046196 abilian_sbe-1.1.9/src/abilian/web/tags/__init__.py
+-rw-r--r--   0        0        0     9266 2024-03-23 14:15:18.718464 abilian_sbe-1.1.9/src/abilian/web/tags/admin.py
+-rw-r--r--   0        0        0     2463 2024-04-22 07:49:45.046500 abilian_sbe-1.1.9/src/abilian/web/tags/criterion.py
+-rw-r--r--   0        0        0     4193 2024-03-23 14:15:18.719515 abilian_sbe-1.1.9/src/abilian/web/tags/extension.py
+-rw-r--r--   0        0        0     2692 2024-03-25 13:17:52.075808 abilian_sbe-1.1.9/src/abilian/web/tags/forms.py
+-rw-r--r--   0        0        0      758 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/tags/templates/admin/tags.html
+-rw-r--r--   0        0        0     2322 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/tags/templates/admin/tags_ns.html
+-rw-r--r--   0        0        0     3470 2024-03-25 13:17:52.075979 abilian_sbe-1.1.9/src/abilian/web/tags/views.py
+-rw-r--r--   0        0        0     4537 2024-03-25 13:17:52.076246 abilian_sbe-1.1.9/src/abilian/web/templates/abilian_base.html
+-rw-r--r--   0        0        0     2634 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/abilian_init.js
+-rw-r--r--   0        0        0       35 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/base.html
+-rw-r--r--   0        0        0      160 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/breadcrumbs.html
+-rw-r--r--   0        0        0      826 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/actions_panel.html
+-rw-r--r--   0        0        0     1292 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/indexing_panel.html
+-rw-r--r--   0        0        0     1179 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/security_info_panel.html
+-rw-r--r--   0        0        0     1196 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/signals_panel.html
+-rw-r--r--   0        0        0      457 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/default/avatar.svg
+-rw-r--r--   0        0        0     3846 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/default/list_view.html
+-rw-r--r--   0        0        0      397 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/default/object_edit.html
+-rw-r--r--   0        0        0      715 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/default/object_view.html
+-rw-r--r--   0        0        0     2768 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/default/single_view.html
+-rw-r--r--   0        0        0      242 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/error403.html
+-rw-r--r--   0        0        0      222 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/error404.html
+-rw-r--r--   0        0        0      261 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/error500.html
+-rw-r--r--   0        0        0      459 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/flash-messages.html
+-rw-r--r--   0        0        0      157 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/index.html
+-rw-r--r--   0        0        0      902 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/activity.html
+-rw-r--r--   0        0        0      697 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/attachment.html
+-rw-r--r--   0        0        0     2887 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/attachment_default.html
+-rw-r--r--   0        0        0     2394 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/audit.html
+-rw-r--r--   0        0        0     2028 2022-04-04 15:58:58.324607 abilian_sbe-1.1.9/src/abilian/web/templates/macros/box.html
+-rw-r--r--   0        0        0      295 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/buttons.html
+-rw-r--r--   0        0        0     2628 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/comment.html
+-rw-r--r--   0        0        0     4520 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/form.html
+-rw-r--r--   0        0        0      536 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/recent.html
+-rw-r--r--   0        0        0      492 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/table.html
+-rw-r--r--   0        0        0     1399 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/tag.html
+-rw-r--r--   0        0        0      544 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/macros/user.html
+-rw-r--r--   0        0        0     2206 2022-04-12 15:39:37.791321 abilian_sbe-1.1.9/src/abilian/web/templates/navbar.html
+-rw-r--r--   0        0        0      587 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/preferences/_base.html
+-rw-r--r--   0        0        0     1094 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/preferences/user.html
+-rw-r--r--   0        0        0      335 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/fieldlist.html
+-rw-r--r--   0        0        0       90 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/fieldlist_view.html
+-rw-r--r--   0        0        0     1152 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/file_input.html
+-rw-r--r--   0        0        0      542 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/frontend_action_delete_confim.html
+-rw-r--r--   0        0        0      450 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/horizontal_table.html
+-rw-r--r--   0        0        0     1740 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/image_input.html
+-rw-r--r--   0        0        0      505 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/model_fieldlist.html
+-rw-r--r--   0        0        0      281 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/model_widget_edit.html
+-rw-r--r--   0        0        0      226 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/model_widget_view.html
+-rw-r--r--   0        0        0     2652 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_ajax_table.html
+-rw-r--r--   0        0        0     2515 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_for_edit.html
+-rw-r--r--   0        0        0     1194 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_single.html
+-rw-r--r--   0        0        0     1727 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_table.html
+-rw-r--r--   0        0        0      340 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/richtext.html
+-rw-r--r--   0        0        0      219 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/select2ajax.html
+-rw-r--r--   0        0        0      887 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/tabular_fieldlist_widget.html
+-rw-r--r--   0        0        0      357 2021-09-16 12:23:36.000000 abilian_sbe-1.1.9/src/abilian/web/templates/widgets/timepicker.html
+-rw-r--r--   0        0        0        0 2021-09-16 12:23:35.000000 abilian_sbe-1.1.9/src/abilian/web/tools/__init__.py
+-rw-r--r--   0        0        0     3656 2024-02-07 15:10:35.389493 abilian_sbe-1.1.9/src/abilian/web/tools/debug_toolbar.py
+-rw-r--r--   0        0        0      196 2024-03-23 14:15:18.709905 abilian_sbe-1.1.9/src/abilian/web/uploads/__init__.py
+-rw-r--r--   0        0        0     6607 2024-03-25 13:17:52.076414 abilian_sbe-1.1.9/src/abilian/web/uploads/extension.py
+-rw-r--r--   0        0        0     3122 2024-04-22 09:26:28.623044 abilian_sbe-1.1.9/src/abilian/web/uploads/views.py
+-rw-r--r--   0        0        0     1483 2024-03-25 13:17:52.076803 abilian_sbe-1.1.9/src/abilian/web/util.py
+-rw-r--r--   0        0        0      535 2024-02-07 15:10:35.390562 abilian_sbe-1.1.9/src/abilian/web/views/__init__.py
+-rw-r--r--   0        0        0     3502 2024-03-25 13:17:52.077071 abilian_sbe-1.1.9/src/abilian/web/views/base.py
+-rw-r--r--   0        0        0     4434 2024-03-23 14:15:18.741263 abilian_sbe-1.1.9/src/abilian/web/views/files.py
+-rw-r--r--   0        0        0     7141 2024-03-25 13:17:52.077244 abilian_sbe-1.1.9/src/abilian/web/views/images.py
+-rw-r--r--   0        0        0    20078 2024-03-23 14:15:18.743288 abilian_sbe-1.1.9/src/abilian/web/views/object.py
+-rw-r--r--   0        0        0     4820 2023-12-08 09:38:30.290727 abilian_sbe-1.1.9/src/abilian/web/views/registry.py
+-rw-r--r--   0        0        0        0 2021-09-16 12:00:44.000000 abilian_sbe-1.1.9/src/extranet/__init__.py
+-rw-r--r--   0        0        0     4698 2024-03-27 08:36:58.869181 abilian_sbe-1.1.9/src/extranet/app.py
+-rw-r--r--   0        0        0      939 2023-11-02 14:44:40.650969 abilian_sbe-1.1.9/src/extranet/config.py
+-rw-r--r--   0        0        0      164 2024-03-25 13:17:52.077774 abilian_sbe-1.1.9/src/extranet/wsgi.py
+-rw-r--r--   0        0        0     7020 1970-01-01 00:00:00.000000 abilian_sbe-1.1.9/PKG-INFO
```

### Comparing `abilian_sbe-1.1.8/LICENCE.txt` & `abilian_sbe-1.1.9/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/README.md` & `abilian_sbe-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/pyproject.toml` & `abilian_sbe-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abilian-sbe"
-version = "1.1.8"
+version = "1.1.9"
 description = "Social Business platform (entreprise collaboration and information management)"
 authors = ["Abilian SAS"]
 license = "LGPL-2.0-or-later"
 readme = "README.md"
 repository = "https://github.com/abilian/abilian-sbe"
 
 packages = [
```

### Comparing `abilian_sbe-1.1.8/src/abilian/app.py` & `abilian_sbe-1.1.9/src/abilian/app.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/cli/base.py` & `abilian_sbe-1.1.9/src/abilian/cli/base.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/cli/config.py` & `abilian_sbe-1.1.9/src/abilian/cli/config.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/cli/indexing.py` & `abilian_sbe-1.1.9/src/abilian/cli/indexing.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/config.py` & `abilian_sbe-1.1.9/src/abilian/config.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/dramatiq/scheduler.py` & `abilian_sbe-1.1.9/src/abilian/core/dramatiq/scheduler.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/dramatiq/setup.py` & `abilian_sbe-1.1.9/src/abilian/core/dramatiq/setup.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/entities.py` & `abilian_sbe-1.1.9/src/abilian/core/entities.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/__init__.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/csrf.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/csrf.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/jinjaext.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/jinjaext.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/login.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/login.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/redis.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/redis.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/extensions/upstream_info.py` & `abilian_sbe-1.1.9/src/abilian/core/extensions/upstream_info.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/logger_patch.py` & `abilian_sbe-1.1.9/src/abilian/core/logger_patch.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/logging.py` & `abilian_sbe-1.1.9/src/abilian/core/logging.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/attachment.py` & `abilian_sbe-1.1.9/src/abilian/core/models/attachment.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/base.py` & `abilian_sbe-1.1.9/src/abilian/core/models/base.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/base_mixin.py` & `abilian_sbe-1.1.9/src/abilian/core/models/base_mixin.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/blob.py` & `abilian_sbe-1.1.9/src/abilian/core/models/blob.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/comment.py` & `abilian_sbe-1.1.9/src/abilian/core/models/comment.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/owned.py` & `abilian_sbe-1.1.9/src/abilian/core/models/owned.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/subjects.py` & `abilian_sbe-1.1.9/src/abilian/core/models/subjects.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/models/tag.py` & `abilian_sbe-1.1.9/src/abilian/core/models/tag.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/signals.py` & `abilian_sbe-1.1.9/src/abilian/core/signals.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/singleton.py` & `abilian_sbe-1.1.9/src/abilian/core/singleton.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/sqlalchemy.py` & `abilian_sbe-1.1.9/src/abilian/core/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/core/util.py` & `abilian_sbe-1.1.9/src/abilian/core/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/i18n.py` & `abilian_sbe-1.1.9/src/abilian/i18n.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/app.py` & `abilian_sbe-1.1.9/src/abilian/sbe/app.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/actions.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/actions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/forms.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/_base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/archives.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/archives.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/event.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/event.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/templates/calendar/index.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/templates/calendar/index.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/calendar/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/calendar/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/actions.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/actions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/blueprint.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/blueprint.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/common.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/common.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/events.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/events.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/forms.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/search.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/search.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/security.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/security.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/_base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/_forumbase.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/_forumbase.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/edit.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/edit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/home.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/home.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members_macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/members_std_macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/members_std_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_add_emails.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_add_emails.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_check_members.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_check_members.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_new_accounts.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_new_accounts.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/templates/community/wizard_users_std_macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/templates/community/wizard_users_std_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/data/community.png` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/data/community.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/communities/views/wizard.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/communities/views/wizard.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/__init__.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/actions.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/actions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cli.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cli.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/atompub.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/atompub.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/parser.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/parser.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/cmis/renderer.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/cmis/renderer.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/lock.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/lock.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/repository.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/repository.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/search.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/search.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/signals.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/signals.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/tasks.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/tasks.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/children.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/children.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/document.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/document.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/feed.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/feed.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/folder.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/folder.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/macros.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/macros.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/service.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/service.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-document.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-document.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-folder.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-folder.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-policy.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-policy.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/type-relationship.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/type-relationship.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/cmis/types.xml` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/cmis/types.xml`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros_audit.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros_audit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_macros_gallery_view.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_macros_gallery_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_delete.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_delete.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_edit.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_edit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_send_by_email.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_send_by_email.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_document_upload_new_version.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_document_upload_new_version.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_change_owner.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_change_owner.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_delete.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_delete.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_edit.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_edit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_move.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_move.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_new.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_new.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_upload.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_folder_upload.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/_modals_roles.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/_modals_roles.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/descendants.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/descendants.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/document.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/document.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/document_viewers.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/document_viewers.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/folder.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/folder.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/folder_gallery_view.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/folder_gallery_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/permissions.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/permissions.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/templates/documents/view_pdf.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/templates/documents/view_pdf.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/documents.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/documents.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/folders.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/folders.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/util.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/views/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/views/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/constants.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/constants.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/documents/webdav/xml.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/documents/webdav/xml.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/__init__.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/actions.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/actions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/cli.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/cli.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/forms.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/tasks.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/tasks.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/_macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/archives.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/archives.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/attachments.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/attachments.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/index.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/index.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.fr.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.fr.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/mail/new_message.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread_attachments.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread_attachments.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/templates/forum/thread_create.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/templates/forum/thread_create.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/forum/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/forum/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/__init__.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/tasks/social.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/tasks/social.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/_base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/_style.css` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/_style.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.fr.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.fr.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/templates/notifications/daily-social-digest.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/notifications/views/social.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/notifications/views/social.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/panels/sbe_notifications.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/panels/sbe_notifications.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/preferences/templates/preferences/sbe_notifications.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/preferences/templates/preferences/sbe_notifications.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/forms.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/restapi.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/restapi.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/_sidebar.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/_sidebar.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/group.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/group.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/groups-new.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/groups-new.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/groups.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/groups.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/invite.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/invite.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/macros.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/user.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/user.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/templates/social/users.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/templates/social/users.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/groups.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/groups.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/invites.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/invites.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/sidebars.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/sidebars.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/social.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/social.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/views/users.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/views/users.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/social/widgets.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/social/widgets.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/presenters.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/presenters.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/templates/wall/_base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/templates/wall/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/templates/wall/files.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/templates/wall/files.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/util.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wall/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wall/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/actions.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/actions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/data/help.txt` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/data/help.txt`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/forms.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/markup.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/markup.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/models.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/_base.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/changes.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/changes.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/edit_conflict_error.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/edit_conflict_error.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/page.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/page.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/templates/wiki/page_readers.html` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/templates/wiki/page_readers.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/apps/wiki/views.py` & `abilian_sbe-1.1.9/src/abilian/sbe/apps/wiki/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/boot.py` & `abilian_sbe-1.1.9/src/abilian/sbe/boot.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/extension.py` & `abilian_sbe-1.1.9/src/abilian/sbe/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/7z.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/7z.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ai.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ai.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/aiff.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/aiff.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/audio.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/audio.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/bz2.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/bz2.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/c.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/c.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cfc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cfc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cfm.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cfm.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/class.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/class.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/conf.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/conf.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cpp.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cpp.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/cs.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/cs.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/css.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/css.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/deb.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/deb.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/divx.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/divx.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/doc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/doc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/docx.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/docx.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/gif.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/gif.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/gz.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/gz.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/htm.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/htm.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/html.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/html.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/image.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/image.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/iso.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/iso.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jar.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jar.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/java.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/java.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jpeg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jpeg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/jpg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/jpg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/js.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/js.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/m.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/m.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mov.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mov.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mp3.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mp3.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/mpg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/mpg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odf.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odf.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odi.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odi.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/odp.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/odp.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ods.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ods.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ogg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ogg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pdf.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pdf.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/php.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/php.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pl.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pl.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/png.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/png.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ppt.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ppt.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/pptx.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/pptx.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/py.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/py.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/ram.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/ram.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rb.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rb.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/rm.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/rm.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sql.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sql.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/swf.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/swf.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxd.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxd.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/sxi.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/sxi.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tar.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tar.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tex.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tex.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/tgz.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/tgz.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/vcf.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/vcf.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/video.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/video.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/vsd.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/vsd.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wav.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wav.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wma.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wma.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/wmv.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/wmv.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xls.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xls.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xlsx.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xlsx.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xpi.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xpi.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/xvid.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/xvid.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/fileicons/zip.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/fileicons/zip.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/arrows.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/arrows.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_disabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_disabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_enabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_enabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/back_enabled_hover.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/back_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/backgrd.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/backgrd.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/eagle.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/eagle.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/error.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/error.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/favicon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/favicon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_disabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_disabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_enabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_enabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/forward_enabled_hover.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/forward_enabled_hover.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/frog.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/frog.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/glyphicons-halflings-white.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/glyphicons-halflings.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/group-icon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/group-icon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/login-background.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/login-background.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/noise_bg.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/noise_bg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/preview_missing.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/preview_missing.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_man.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_man.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_unknown.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_unknown.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/silhouette_woman.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/silhouette_woman.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_asc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_asc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_asc_disabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_asc_disabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_both.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_both.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_desc.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_desc.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/sort_desc_disabled.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/sort_desc_disabled.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/user-icon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/user-icon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/images/valid.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/images/valid.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/avatar140.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/avatar140.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/avatar45.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/avatar45.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/backgrd.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/backgrd.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/error.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/error.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/favicon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/favicon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/glyphicons-halflings-white.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/glyphicons-halflings.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/group-icon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/group-icon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/group64.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/group64.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/login-background.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/login-background.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/me-25x25.jpg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/me-25x25.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/user-icon.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/user-icon.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/img/valid.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/img/valid.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/document_viewer.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/document_viewer.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_edit.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_edit.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_gallery.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_gallery.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/folder_upload.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/folder_upload.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/js/sbe-datatable.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/js/sbe-datatable.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/bootstrap-tagsinput.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/bootstrap-tagsinput.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/communities.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/communities.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/documents.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/documents.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/forum.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/forum.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/misc.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/misc.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/modules/wizard_steps.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/modules/wizard_steps.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/less/overrides.less` & `abilian_sbe-1.1.9/src/abilian/sbe/static/less/overrides.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/moment/moment.min.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/78ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/83pv-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/83pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90ms-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90msp-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/90pv-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Add-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-CNS1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-4.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-4.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-5.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-5.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-GB1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Japan1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Adobe-Korea1-UCS2.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/B5pc-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/B5pc-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS-EUC-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/CNS1-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/CNS1-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETHK-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/ETen-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/Ext-RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GB-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GB-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBK2K-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBKp-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBT-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBT-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBTpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/GBpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdla-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKdlb-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKgccs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm314-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKm471-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/HKscs-B5-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSC-Johab-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCms-UHC-HW-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/KSCpc-EUC-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/LICENSE` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/LICENSE`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/NWP-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/NWP-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/RKSJ-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniCNS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniGB-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF16-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJIS2004-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-HW-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UCS2-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISPro-UTF8-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX0213-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniJISX02132004-UTF32-V.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UCS2-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF16-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF32-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-H.bcmap` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/cmaps/UniKS-UTF8-H.bcmap`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/compatibility.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/compatibility.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/debugger.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/debugger.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-comment.svg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-comment.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-help.svg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-help.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-key.svg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-key.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-note.svg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-note.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/annotation-paragraph.svg` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/annotation-paragraph.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-icon.gif` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-icon.gif`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-small.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-small.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/loading-small@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/loading-small@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-documentProperties@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-handTool@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCcw@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/secondaryToolbarButton-rotateCw@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/texture.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/texture.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-openFile@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-presentationMode@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-search@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-search@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments@2x.png` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/images/toolbarButton-viewAttachments@2x.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/l10n.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/l10n.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/locale/en-US/viewer.properties` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/locale/en-US/viewer.properties`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/locale/fr/viewer.properties` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/locale/fr/viewer.properties`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/pdf.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/pdf.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/pdf.worker.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/pdf.worker.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/viewer.css` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/viewer.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/pdfjs/viewer.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/pdfjs/viewer.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/vendor/bootstrap-tagsinput.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/vendor/bootstrap-tagsinput.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/static/vendor/jquery.fileapi.js` & `abilian_sbe-1.1.9/src/abilian/sbe/static/vendor/jquery.fileapi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/translations/es/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/sbe/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/translations/fr/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/sbe/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/translations/messages.pot` & `abilian_sbe-1.1.9/src/abilian/sbe/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/translations/tr/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/sbe/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/sbe/translations/zh/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/sbe/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/__init__.py` & `abilian_sbe-1.1.9/src/abilian/services/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/activity/models.py` & `abilian_sbe-1.1.9/src/abilian/services/activity/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/activity/service.py` & `abilian_sbe-1.1.9/src/abilian/services/activity/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/antivirus/service.py` & `abilian_sbe-1.1.9/src/abilian/services/antivirus/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/audit/models.py` & `abilian_sbe-1.1.9/src/abilian/services/audit/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/audit/service.py` & `abilian_sbe-1.1.9/src/abilian/services/audit/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/models.py` & `abilian_sbe-1.1.9/src/abilian/services/auth/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/service.py` & `abilian_sbe-1.1.9/src/abilian/services/auth/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/forgotten_password.html` & `abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/forgotten_password.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/login.html` & `abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/login.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/password_reset.fr.html` & `abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/password_reset.fr.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/templates/login/password_reset.html` & `abilian_sbe-1.1.9/src/abilian/services/auth/templates/login/password_reset.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/auth/views.py` & `abilian_sbe-1.1.9/src/abilian/services/auth/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/base.py` & `abilian_sbe-1.1.9/src/abilian/services/base.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/blob_store/service.py` & `abilian_sbe-1.1.9/src/abilian/services/blob_store/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/__init__.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/cache.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/cache.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/mugshot.jpg` & `abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/mugshot.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/onepage.pdf` & `abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/onepage.pdf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/picture.jpg` & `abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/picture.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/dummy_files/rammstein.pdf` & `abilian_sbe-1.1.9/src/abilian/services/conversion/dummy_files/rammstein.pdf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/handler_lock.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/handler_lock.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/handlers.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,14 @@
                                 "Failed to kill process {process}",
                                 process=self._process,
                             )
 
                     raise ConversionError(f"Conversion timeout ({timeout})")
 
                 out_fn = f"{os.path.splitext(in_fn)[0]}.pdf"
-                debug(in_fn, out_fn)
                 converted = open(out_fn, "rb").read()
                 return converted
             finally:
                 if hasattr(self, "_process"):
                     del self._process
```

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/service.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/conversion/util.py` & `abilian_sbe-1.1.9/src/abilian/services/conversion/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/image/__init__.py` & `abilian_sbe-1.1.9/src/abilian/services/image/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/indexing/adapter.py` & `abilian_sbe-1.1.9/src/abilian/services/indexing/adapter.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/indexing/debug_toolbar.py` & `abilian_sbe-1.1.9/src/abilian/services/indexing/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/indexing/schema.py` & `abilian_sbe-1.1.9/src/abilian/services/indexing/schema.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/indexing/service.py` & `abilian_sbe-1.1.9/src/abilian/services/indexing/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/preferences/models.py` & `abilian_sbe-1.1.9/src/abilian/services/preferences/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/preferences/panel.py` & `abilian_sbe-1.1.9/src/abilian/services/preferences/panel.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/preferences/service.py` & `abilian_sbe-1.1.9/src/abilian/services/preferences/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/security/__init__.py` & `abilian_sbe-1.1.9/src/abilian/services/security/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/security/debug_toolbar.py` & `abilian_sbe-1.1.9/src/abilian/services/security/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/security/models.py` & `abilian_sbe-1.1.9/src/abilian/services/security/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/security/service.py` & `abilian_sbe-1.1.9/src/abilian/services/security/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/settings/models.py` & `abilian_sbe-1.1.9/src/abilian/services/settings/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/settings/service.py` & `abilian_sbe-1.1.9/src/abilian/services/settings/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/viewtracker/models.py` & `abilian_sbe-1.1.9/src/abilian/services/viewtracker/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/viewtracker/service.py` & `abilian_sbe-1.1.9/src/abilian/services/viewtracker/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/admin.py` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/admin.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/forms.py` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/models.py` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/models.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/service.py` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/service.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/templates/admin/macros/vocabularies.html` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/templates/admin/macros/vocabularies.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/services/vocabularies/templates/admin/vocabularies.html` & `abilian_sbe-1.1.9/src/abilian/services/vocabularies/templates/admin/vocabularies.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/de_DE/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/en/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/es/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/es_ES/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/es_ES/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/fr/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/fr_FR/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/id_ID/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/id_ID/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/it_IT/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/it_IT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/messages.pot` & `abilian_sbe-1.1.9/src/abilian/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/nl/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/nl_NL/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/nl_NL/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/pt_BR/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/pt_PT/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/pt_PT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/tr_TR/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/tr_TR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/zh_CN/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/translations/zh_TW/LC_MESSAGES/messages.po` & `abilian_sbe-1.1.9/src/abilian/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/access_blueprint.py` & `abilian_sbe-1.1.9/src/abilian/web/access_blueprint.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/action.py` & `abilian_sbe-1.1.9/src/abilian/web/action.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/extension.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panel.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panel.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/audit.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/audit.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/dashboard.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/dashboard.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/ip_country.mmdb` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/ip_country.mmdb`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/ip_country_code.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/ip_country_code.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/geoip/update_ip_country.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/geoip/update_ip_country.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/__init__.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/forms.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/groups/views.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/groups/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/impersonate.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/impersonate.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/login_sessions.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/login_sessions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/settings.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/settings.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/sysinfo.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/sysinfo.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/__init__.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/forms.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/panels/users/views.py` & `abilian_sbe-1.1.9/src/abilian/web/admin/panels/users/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/_base.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/_macros.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/_macros.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/audit.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/audit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/dashboard.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/dashboard.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/group_view.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/group_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/groups.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/groups.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/login_sessions.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/login_sessions.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/settings.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/settings.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/settings_session_lifetime.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/settings_session_lifetime.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/sysinfo.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/sysinfo.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/admin/templates/admin/users.html` & `abilian_sbe-1.1.9/src/abilian/web/admin/templates/admin/users.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/assets/__init__.py` & `abilian_sbe-1.1.9/src/abilian/web/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/assets/filters.py` & `abilian_sbe-1.1.9/src/abilian/web/assets/filters.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/assets/mixin.py` & `abilian_sbe-1.1.9/src/abilian/web/assets/mixin.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/attachments/extension.py` & `abilian_sbe-1.1.9/src/abilian/web/attachments/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/attachments/forms.py` & `abilian_sbe-1.1.9/src/abilian/web/attachments/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/attachments/views.py` & `abilian_sbe-1.1.9/src/abilian/web/attachments/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/comments/extension.py` & `abilian_sbe-1.1.9/src/abilian/web/comments/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/comments/forms.py` & `abilian_sbe-1.1.9/src/abilian/web/comments/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/comments/views.py` & `abilian_sbe-1.1.9/src/abilian/web/comments/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/coreviews/users.py` & `abilian_sbe-1.1.9/src/abilian/web/coreviews/users.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/crm_frontend.py` & `abilian_sbe-1.1.9/src/abilian/web/crm_frontend.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/csrf.py` & `abilian_sbe-1.1.9/src/abilian/web/csrf.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/errors.py` & `abilian_sbe-1.1.9/src/abilian/web/errors.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/filters.py` & `abilian_sbe-1.1.9/src/abilian/web/filters.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/fields.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/fields.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/filters.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/filters.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/form.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/form.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/permissions.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/permissions.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/util.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/validators.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/validators.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/forms/widgets.py` & `abilian_sbe-1.1.9/src/abilian/web/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/frontend.py` & `abilian_sbe-1.1.9/src/abilian/web/frontend.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/jinja.py` & `abilian_sbe-1.1.9/src/abilian/web/jinja.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/nav.py` & `abilian_sbe-1.1.9/src/abilian/web/nav.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/preferences/user.py` & `abilian_sbe-1.1.9/src/abilian/web/preferences/user.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootbox/bootbox.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootbox/bootbox.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.eot` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.svg` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/js/bootstrap.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/js/bootstrap.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/.csscomb.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/.csscomb.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/alerts.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/alerts.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/badges.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/badges.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/bootstrap.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/bootstrap.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/breadcrumbs.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/breadcrumbs.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/button-groups.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/button-groups.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/buttons.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/buttons.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/carousel.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/carousel.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/close.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/close.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/code.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/code.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/component-animations.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/component-animations.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/dropdowns.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/dropdowns.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/forms.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/forms.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/glyphicons.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/glyphicons.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/grid.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/grid.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/input-groups.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/input-groups.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/jumbotron.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/jumbotron.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/labels.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/labels.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/list-group.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/list-group.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/media.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/media.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/buttons.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/buttons.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/clearfix.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/clearfix.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/forms.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/forms.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/gradients.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/gradients.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/grid-framework.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/grid-framework.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/grid.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/grid.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/hide-text.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/hide-text.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/image.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/image.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/list-group.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/list-group.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/panels.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/panels.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/table-row.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/table-row.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins/vendor-prefixes.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins/vendor-prefixes.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/mixins.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/mixins.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/modals.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/modals.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/navbar.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/navbar.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/navs.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/navs.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/normalize.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/normalize.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/pager.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/pager.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/pagination.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/pagination.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/panels.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/panels.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/popovers.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/popovers.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/print.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/print.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/progress-bars.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/progress-bars.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/responsive-embed.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/responsive-embed.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/responsive-utilities.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/responsive-utilities.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/scaffolding.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/scaffolding.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/tables.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/tables.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/theme.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/theme.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/thumbnails.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/thumbnails.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/tooltip.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/tooltip.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/type.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/type.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/utilities.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/utilities.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/variables.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/variables.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap/less/wells.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap/less/wells.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/css/datepicker.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/css/datepicker.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/bootstrap-datepicker.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.bg.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.bg.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cy.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.cy.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.da.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.da.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.de.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.de.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.el.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.el.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.es.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.es.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.et.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.et.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.fr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.gl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.gl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.he.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.he.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.hu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.id.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.id.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.is.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.is.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.it.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.it.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ja.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ja.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ka.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ka.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.kr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.kr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.lv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.mk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.mk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ms.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ms.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl-BE.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl-BE.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.nl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.no.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.no.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt-BR.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt-BR.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.pt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ro.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ro.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs-latin.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs-latin.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.rs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ru.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ru.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sq.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sq.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sw.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.sw.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.th.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.th.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.tr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.tr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ua.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.ua.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.uk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.uk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-CN.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-CN.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-TW.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/js/locales/bootstrap-datepicker.zh-TW.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-datepicker/less/datepicker.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-datepicker/less/datepicker.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/LICENSE` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/LICENSE`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/bootstrap-switch.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/bootstrap-switch.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-switch/less/bootstrap3/bootstrap-switch.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-switch/less/bootstrap3/bootstrap-switch.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.min.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/css/bootstrap-timepicker.min.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/js/bootstrap-timepicker.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/bootstrap-timepicker/less/timepicker.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/bootstrap-timepicker/less/timepicker.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/CHANGES.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/CHANGES.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/LICENSE.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/README.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/README.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/SECURITY.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/SECURITY.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/adapters/jquery.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/adapters/jquery.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/build-config.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/build-config.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/ckeditor.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/ckeditor.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/config.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/config.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/contents.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/contents.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/af.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/af.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/az.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/az.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bg.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bg.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/bs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/bs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/cs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/cs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/cy.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/cy.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/da.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/da.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/de-ch.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/de.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/de.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/el.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/el.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-au.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en-gb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/en.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/en.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/eo.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/eo.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/es-mx.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/es.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/es.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/et.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/et.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/eu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/eu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fa.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fa.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fo.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fo.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fr-ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/fr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/fr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/gl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/gl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/gu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/gu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/he.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/he.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/hu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/hu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/id.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/id.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/is.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/is.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/it.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/it.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ja.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ja.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ka.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ka.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/km.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/km.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ko.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ko.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ku.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ku.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/lt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/lt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/lv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/lv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/mk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/mk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/mn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/mn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ms.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ms.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/nb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/nb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/nl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/nl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/no.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/no.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/oc.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/oc.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pt-br.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/pt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/pt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ro.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ro.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ru.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ru.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/si.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/si.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sq.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sq.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sr-latn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/sv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/sv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/th.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/th.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/tr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/tr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/tt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/tt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/ug.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/ug.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/uk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/uk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/vi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/vi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/zh-cn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/lang/zh.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/lang/zh.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/a11yhelp.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/af.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/az.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/da.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/el.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/et.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fo.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/gu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/he.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/id.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/it.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/km.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/mn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/no.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/si.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/th.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/a11yhelp/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/about.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/about.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/hidpi/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/about/dialogs/logo_ckeditor.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/about/dialogs/logo_ckeditor.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/clipboard/dialogs/paste.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/clipboard/dialogs/paste.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/icons.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/icons.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/icons_hidpi.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/image/dialogs/image.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/image/dialogs/image.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/image/images/noimage.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/image/images/noimage.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/dialogs/anchor.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/dialogs/anchor.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/dialogs/link.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/dialogs/link.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/images/anchor.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/images/anchor.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/link/images/hidpi/anchor.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/link/images/hidpi/anchor.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromgdocs/filter/default.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromgdocs/filter/default.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromlibreoffice/filter/default.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromlibreoffice/filter/default.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastefromword/filter/default.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastefromword/filter/default.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/common.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/common.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/image.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/pastetools/filter/image.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/LICENSE.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/README.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/README.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/options.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/options.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/toolbar.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/scayt/dialogs/toolbar.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/_translationstatus.txt`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/af.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/af.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/az.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/az.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/bg.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/bg.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cy.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/cy.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/da.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/da.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de-ch.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/de.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/el.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/el.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-au.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-au.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en-gb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/en.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eo.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eo.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es-mx.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/es.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/et.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/et.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/eu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fa.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fa.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr-ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/fr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/gl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/gl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/he.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/he.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/hu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/id.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/id.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/it.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/it.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ja.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ja.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/km.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/km.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ko.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ko.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ku.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ku.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/lv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/nl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/no.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/no.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/oc.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/oc.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt-br.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/pt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ro.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ro.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ru.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ru.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/si.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/si.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sq.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sq.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr-latn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/sv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/th.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/th.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/tt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ug.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/ug.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/uk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/uk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/vi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/vi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh-cn.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/lang/zh.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/specialchar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/specialchar/dialogs/specialchar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/table/dialogs/table.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/table/dialogs/table.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/tableselection/styles/tableselection.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/tableselection/styles/tableselection.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/plugins/tabletools/dialogs/tableCell.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/plugins/tabletools/dialogs/tableCell.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/css/samples.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/css/samples.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/header-bg.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/header-bg.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/logo.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/logo.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/logo.svg` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/logo.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/img/navigation-tip.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/img/navigation-tip.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/index.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/index.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/js/sample.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/js/sample.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/js/sf.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/js/sf.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/ajax.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/ajax.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/api.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/api.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/appendto.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/appendto.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/inlineall/logo.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/inlineall/logo.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/outputxhtml/outputxhtml.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/posteddata.php` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/posteddata.php`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/sample.jpg` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/sample.jpg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/assets/uilanguages/languages.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/assets/uilanguages/languages.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/datafiltering.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/datafiltering.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/dialog/assets/my_dialog.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/dialog/assets/my_dialog.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/dialog/dialog.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/dialog/dialog.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/divreplace.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/divreplace.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/enterkey/enterkey.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/enterkey/enterkey.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/htmlwriter/outputhtml.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/htmlwriter/outputhtml.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/index.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/index.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlineall.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlineall.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlinebycode.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlinebycode.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/inlinetextarea.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/inlinetextarea.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/jquery.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/jquery.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/magicline/magicline.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/magicline/magicline.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/readonly.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/readonly.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/replacebyclass.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/replacebyclass.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/replacebycode.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/replacebycode.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/sample_posteddata.php` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/sample_posteddata.php`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/tabindex.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/tabindex.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/toolbar/toolbar.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/toolbar/toolbar.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/uicolor.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/uicolor.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/uilanguages.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/uilanguages.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/wysiwygarea/fullpage.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/wysiwygarea/fullpage.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/old/xhtmlstyle.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/old/xhtmlstyle.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/css/fontello.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/css/fontello.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/config.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/config.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.eot` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.eot`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.svg` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.ttf` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.ttf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.woff` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/font/fontello.woff`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/index.html` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/index.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/abstracttoolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/fulltoolbareditor.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbarmodifier.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/js/toolbartextmodifier.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/LICENSE` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/LICENSE`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/javascript.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/javascript.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/neo.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/neo.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/samples/toolbarconfigurator/lib/codemirror/show-hint.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie8.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_ie8.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_iequirks.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/dialog_iequirks.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_gecko.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_gecko.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie8.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_ie8.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_iequirks.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/editor_iequirks.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons_hidpi.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/icons_hidpi.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/close.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/close.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/close.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/close.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock-open.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/lock.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/refresh.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/hidpi/refresh.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/refresh.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/refresh.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/spinner.gif` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/skins/moono-lisa/readme.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/skins/moono-lisa/readme.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/styles.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/styles.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/ckeditor/vendor/promise.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/ckeditor/vendor/promise.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/css/jquery.dataTables.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/css/jquery.dataTables.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/css/jquery.dataTables_themeroller.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/css/jquery.dataTables_themeroller.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/Sorting icons.psd` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/Sorting icons.psd`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/images/favicon.ico` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/js/jquery.dataTables.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/js/jquery.dataTables.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/datatables/js/jquery.dataTables.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/datatables/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.camera.swf` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.camera.swf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.image.swf` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.image.swf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.flash.swf` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.flash.swf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.html5.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.html5.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.html5.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.html5.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/FileAPI.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/FileAPI.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/LICENSE` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/LICENSE`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/FileAPI.exif.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/FileAPI.exif.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/FileAPI.id3.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/FileAPI.id3.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/caman.full.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/caman.full.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/fileapi/plugins/caman.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/fileapi/plugins/caman.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/css/font-awesome.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/css/font-awesome.min.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/FontAwesome.otf` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.eot` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.svg` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.ttf` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff2` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/animated.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/animated.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/bordered-pulled.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/bordered-pulled.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/icons.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/icons.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/mixins.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/mixins.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/path.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/path.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/rotated-flipped.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/rotated-flipped.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/less/variables.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/less/variables.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_animated.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_animated.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_bordered-pulled.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_bordered-pulled.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_icons.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_icons.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_mixins.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_path.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_path.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_rotated-flipped.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_rotated-flipped.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/font-awesome/scss/_variables.scss` & `abilian_sbe-1.1.9/src/abilian/web/resources/font-awesome/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/highlightjs/default.min.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/highlightjs/default.min.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/highlightjs/highlight.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/highlightjs/highlight.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/img/abilian.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/img/abilian.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/img/avatar-default.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/img/avatar-default.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/img/logo-abilian-32x32.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/img/logo-abilian-32x32.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/img/logo-abilian.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/img/logo-abilian.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/jquery/js/jquery-1.11.3.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/jquery/js/jquery-1.11.3.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/jquery/js/jquery-migrate-1.2.1.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/jquery/js/jquery-migrate-1.2.1.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/abilian-namespace.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/abilian-namespace.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/abilian.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/abilian.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/datatables-advanced-search.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/datatables-advanced-search.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/datatables-setup.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/datatables-setup.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/base.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/base.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/delete.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/delete.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/dynamic-row.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/dynamic-row.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/file.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/file.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/image.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/image.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/richtext.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/richtext.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/select2.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/select2.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/js/widgets/tags.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/js/widgets/tags.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/abilian.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/abilian.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/activities.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/activities.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/admin.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/admin.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/comments.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/comments.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/datatables.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/datatables.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/form.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/form.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/navbar.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/navbar.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/less/print.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/less/print.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/d3.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/d3.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/nv.d3.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/nv.d3.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/nvd3/nv.d3.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/nvd3/nv.d3.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/requirejs/domReady.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/requirejs/domReady.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/requirejs/require.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/requirejs/require.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/CONTRIBUTING.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/LICENSE` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/LICENSE`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/README.md` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/README.md`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/component.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/component.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/composer.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/composer.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/package.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/package.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/release.sh` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/release.sh`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2-bootstrap.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2-bootstrap.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2-spinner.gif` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.jquery.json` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.jquery.json`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ar.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ar.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_az.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_az.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_bg.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_bg.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ca.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ca.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_cs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_cs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_da.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_da.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_de.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_de.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_el.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_el.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_en.js.template` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_en.js.template`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_es.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_es.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_et.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_et.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_eu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_eu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fa.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fa.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_fr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_fr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_gl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_gl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_he.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_he.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_hr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_hr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_hu.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_hu.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_id.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_id.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_is.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_is.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_it.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_it.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ja.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ja.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ka.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ka.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ko.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ko.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_lt.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_lt.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_lv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_lv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_mk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_mk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ms.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ms.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_nb.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_nb.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_nl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_nl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pl.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pl.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pt-BR.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pt-BR.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_pt-PT.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_pt-PT.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ro.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ro.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_rs.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_rs.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ru.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ru.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_sk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_sk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_sv.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_sv.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_th.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_th.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_tr.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_tr.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_ug-CN.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_ug-CN.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_uk.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_uk.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_vi.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_vi.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_zh-CN.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_zh-CN.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2_locale_zh-TW.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2_locale_zh-TW.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/select2/select2x2.png` & `abilian_sbe-1.1.9/src/abilian/web/resources/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/hogan-2.0.0.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/hogan-2.0.0.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.css` & `abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.css`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.less` & `abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.js-bootstrap.less`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/resources/typeahead/typeahead.min.js` & `abilian_sbe-1.1.9/src/abilian/web/resources/typeahead/typeahead.min.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/search/__init__.py` & `abilian_sbe-1.1.9/src/abilian/web/search/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/search/criterion.py` & `abilian_sbe-1.1.9/src/abilian/web/search/criterion.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/search/templates/search/search.html` & `abilian_sbe-1.1.9/src/abilian/web/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/search/views.py` & `abilian_sbe-1.1.9/src/abilian/web/search/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/admin.py` & `abilian_sbe-1.1.9/src/abilian/web/tags/admin.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/criterion.py` & `abilian_sbe-1.1.9/src/abilian/web/tags/criterion.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/extension.py` & `abilian_sbe-1.1.9/src/abilian/web/tags/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/forms.py` & `abilian_sbe-1.1.9/src/abilian/web/tags/forms.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/templates/admin/tags.html` & `abilian_sbe-1.1.9/src/abilian/web/tags/templates/admin/tags.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/templates/admin/tags_ns.html` & `abilian_sbe-1.1.9/src/abilian/web/tags/templates/admin/tags_ns.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tags/views.py` & `abilian_sbe-1.1.9/src/abilian/web/tags/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/abilian_base.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/abilian_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/abilian_init.js` & `abilian_sbe-1.1.9/src/abilian/web/templates/abilian_init.js`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/actions_panel.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/actions_panel.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/indexing_panel.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/indexing_panel.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/security_info_panel.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/security_info_panel.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/debug_panels/signals_panel.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/debug_panels/signals_panel.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/default/list_view.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/default/list_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/default/object_view.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/default/object_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/default/single_view.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/default/single_view.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/activity.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/activity.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/attachment.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/attachment.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/attachment_default.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/attachment_default.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/audit.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/audit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/box.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/box.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/comment.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/comment.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/form.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/form.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/recent.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/recent.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/tag.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/tag.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/macros/user.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/macros/user.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/navbar.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/preferences/_base.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/preferences/_base.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/preferences/user.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/preferences/user.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/file_input.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/file_input.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/frontend_action_delete_confim.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/frontend_action_delete_confim.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/image_input.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/image_input.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_ajax_table.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_ajax_table.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_for_edit.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_for_edit.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_single.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_single.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/render_table.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/render_table.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/templates/widgets/tabular_fieldlist_widget.html` & `abilian_sbe-1.1.9/src/abilian/web/templates/widgets/tabular_fieldlist_widget.html`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/tools/debug_toolbar.py` & `abilian_sbe-1.1.9/src/abilian/web/tools/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/uploads/extension.py` & `abilian_sbe-1.1.9/src/abilian/web/uploads/extension.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/uploads/views.py` & `abilian_sbe-1.1.9/src/abilian/web/uploads/views.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/util.py` & `abilian_sbe-1.1.9/src/abilian/web/util.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/__init__.py` & `abilian_sbe-1.1.9/src/abilian/web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/base.py` & `abilian_sbe-1.1.9/src/abilian/web/views/base.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/files.py` & `abilian_sbe-1.1.9/src/abilian/web/views/files.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/images.py` & `abilian_sbe-1.1.9/src/abilian/web/views/images.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/object.py` & `abilian_sbe-1.1.9/src/abilian/web/views/object.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/abilian/web/views/registry.py` & `abilian_sbe-1.1.9/src/abilian/web/views/registry.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/extranet/app.py` & `abilian_sbe-1.1.9/src/extranet/app.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/src/extranet/config.py` & `abilian_sbe-1.1.9/src/extranet/config.py`

 * *Files identical despite different names*

### Comparing `abilian_sbe-1.1.8/PKG-INFO` & `abilian_sbe-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abilian-sbe
-Version: 1.1.8
+Version: 1.1.9
 Summary: Social Business platform (entreprise collaboration and information management)
 Home-page: https://github.com/abilian/abilian-sbe
 License: LGPL-2.0-or-later
 Author: Abilian SAS
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3
```

