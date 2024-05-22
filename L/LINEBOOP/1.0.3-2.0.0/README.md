# Comparing `tmp/LINEBOOP-1.0.3.tar.gz` & `tmp/LINEBOOP-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LINEBOOP-1.0.3.tar", last modified: Mon May 20 06:24:32 2024, max compression
+gzip compressed data, was "LINEBOOP-2.0.0.tar", last modified: Wed May 22 17:25:56 2024, max compression
```

## Comparing `LINEBOOP-1.0.3.tar` & `LINEBOOP-2.0.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.878485 LINEBOOP-1.0.3/
--rw-rw-rw-   0        0        0     1545 2024-02-10 18:24:20.000000 LINEBOOP-1.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.479249 LINEBOOP-1.0.3/LINEBOOP/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.499544 LINEBOOP-1.0.3/LINEBOOP/BIZ/
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.509371 LINEBOOP-1.0.3/LINEBOOP/BIZ/TL/
--rw-rw-rw-   0        0        0     6497 2024-02-10 18:09:22.000000 LINEBOOP-1.0.3/LINEBOOP/BIZ/TL/ST.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.3/LINEBOOP/BIZ/TL/__init__.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.3/LINEBOOP/BIZ/__init__.py
--rw-rw-rw-   0        0        0      251 2024-05-20 06:22:27.000000 LINEBOOP-1.0.3/LINEBOOP/__init__.py
--rw-rw-rw-   0        0        0    26521 2024-05-20 06:19:35.000000 LINEBOOP-1.0.3/LINEBOOP/api.py
--rw-rw-rw-   0        0        0     5833 2024-02-11 09:02:59.000000 LINEBOOP-1.0.3/LINEBOOP/client.py
--rw-rw-rw-   0        0        0     9317 2024-04-09 11:22:18.000000 LINEBOOP-1.0.3/LINEBOOP/config.py
--rw-rw-rw-   0        0        0     1842 2024-02-10 18:10:19.000000 LINEBOOP-1.0.3/LINEBOOP/cube.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.528527 LINEBOOP-1.0.3/LINEBOOP/dyher/
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.3/LINEBOOP/dyher/__init__.py
--rw-rw-rw-   0        0        0     7763 2024-02-10 18:09:21.000000 LINEBOOP-1.0.3/LINEBOOP/dyher/conn.py
--rw-rw-rw-   0        0        0    15544 2024-02-11 09:01:28.000000 LINEBOOP-1.0.3/LINEBOOP/dyher/connManager.py
--rw-rw-rw-   0        0        0    17273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.3/LINEBOOP/e2ee.py
--rw-rw-rw-   0        0        0      982 2024-02-10 18:10:20.000000 LINEBOOP-1.0.3/LINEBOOP/exceptions.py
--rw-rw-rw-   0        0        0    15273 2024-02-10 18:10:19.000000 LINEBOOP-1.0.3/LINEBOOP/helpers.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.561030 LINEBOOP-1.0.3/LINEBOOP/hksc/
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.3/LINEBOOP/hksc/__init__.py
--rw-rw-rw-   0        0        0     3439 2024-02-10 18:09:19.000000 LINEBOOP-1.0.3/LINEBOOP/hksc/database.py
--rw-rw-rw-   0        0        0      335 2024-02-10 18:09:19.000000 LINEBOOP-1.0.3/LINEBOOP/hksc/events.py
--rw-rw-rw-   0        0        0     6220 2024-02-10 18:09:17.000000 LINEBOOP-1.0.3/LINEBOOP/hksc/types.py
--rw-rw-rw-   0        0        0     2494 2024-02-10 18:09:17.000000 LINEBOOP-1.0.3/LINEBOOP/hksc/utility.py
--rw-rw-rw-   0        0        0     4110 2024-02-10 18:10:41.000000 LINEBOOP-1.0.3/LINEBOOP/hooks.py
--rw-rw-rw-   0        0        0    39147 2024-02-10 18:09:50.000000 LINEBOOP-1.0.3/LINEBOOP/models.py
--rw-rw-rw-   0        0        0    29790 2024-04-09 11:22:18.000000 LINEBOOP-1.0.3/LINEBOOP/object.py
--rw-rw-rw-   0        0        0     2426 2024-02-10 18:10:18.000000 LINEBOOP-1.0.3/LINEBOOP/poll.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.570467 LINEBOOP-1.0.3/LINEBOOP/serializers/
--rw-rw-rw-   0        0        0     2300 2024-02-10 18:09:15.000000 LINEBOOP-1.0.3/LINEBOOP/serializers/DummyProtocol.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-1.0.3/LINEBOOP/serializers/__init__.py
--rw-rw-rw-   0        0        0     2760 2024-02-10 18:10:20.000000 LINEBOOP-1.0.3/LINEBOOP/server.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.659585 LINEBOOP-1.0.3/LINEBOOP/services/
--rw-rw-rw-   0        0        0      933 2024-02-10 18:09:56.000000 LINEBOOP-1.0.3/LINEBOOP/services/AccessTokenRefreshService.py
--rw-rw-rw-   0        0        0     2425 2024-02-10 18:10:01.000000 LINEBOOP-1.0.3/LINEBOOP/services/AccountAuthFactorEapConnectService.py
--rw-rw-rw-   0        0        0    13334 2024-02-10 18:09:55.000000 LINEBOOP-1.0.3/LINEBOOP/services/AuthService.py
--rw-rw-rw-   0        0        0      467 2024-02-11 09:03:35.000000 LINEBOOP-1.0.3/LINEBOOP/services/BaseService.py
--rw-rw-rw-   0        0        0     1285 2024-02-10 18:10:19.000000 LINEBOOP-1.0.3/LINEBOOP/services/BotExternalService.py
--rw-rw-rw-   0        0        0    11397 2024-02-10 18:09:54.000000 LINEBOOP-1.0.3/LINEBOOP/services/BuddyService.py
--rw-rw-rw-   0        0        0    11695 2024-02-10 18:09:57.000000 LINEBOOP-1.0.3/LINEBOOP/services/CallService.py
--rw-rw-rw-   0        0        0    13827 2024-02-10 18:09:53.000000 LINEBOOP-1.0.3/LINEBOOP/services/ChannelService.py
--rw-rw-rw-   0        0        0      975 2024-02-10 18:10:01.000000 LINEBOOP-1.0.3/LINEBOOP/services/ChatAppService.py
--rw-rw-rw-   0        0        0     1509 2024-02-10 18:10:01.000000 LINEBOOP-1.0.3/LINEBOOP/services/E2EEKeyBackupService.py
--rw-rw-rw-   0        0        0     2037 2024-02-10 18:10:02.000000 LINEBOOP-1.0.3/LINEBOOP/services/HomeSafetyCheckService.py
--rw-rw-rw-   0        0        0     1946 2024-02-10 18:10:16.000000 LINEBOOP-1.0.3/LINEBOOP/services/InterlockService.py
--rw-rw-rw-   0        0        0     2651 2024-02-10 18:09:53.000000 LINEBOOP-1.0.3/LINEBOOP/services/LiffService.py
--rw-rw-rw-   0        0        0     2570 2024-02-11 09:01:42.000000 LINEBOOP-1.0.3/LINEBOOP/services/LoginService.py
--rw-rw-rw-   0        0        0     2513 2024-02-10 18:10:18.000000 LINEBOOP-1.0.3/LINEBOOP/services/OaMembershipService.py
--rw-rw-rw-   0        0        0     9898 2024-02-10 18:09:54.000000 LINEBOOP-1.0.3/LINEBOOP/services/PrimaryAccountInitService.py
--rw-rw-rw-   0        0        0      899 2024-02-10 18:10:02.000000 LINEBOOP-1.0.3/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py
--rw-rw-rw-   0        0        0     1132 2024-02-10 18:10:02.000000 LINEBOOP-1.0.3/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py
--rw-rw-rw-   0        0        0     1400 2024-02-10 18:10:18.000000 LINEBOOP-1.0.3/LINEBOOP/services/PwlessPrimaryRegistrationService.py
--rw-rw-rw-   0        0        0     5773 2024-02-10 18:10:17.000000 LINEBOOP-1.0.3/LINEBOOP/services/RelationService.py
--rw-rw-rw-   0        0        0     6045 2024-02-10 18:10:18.000000 LINEBOOP-1.0.3/LINEBOOP/services/SearchService.py
--rw-rw-rw-   0        0        0      937 2024-02-10 18:10:00.000000 LINEBOOP-1.0.3/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py
--rw-rw-rw-   0        0        0     3207 2024-02-10 18:10:00.000000 LINEBOOP-1.0.3/LINEBOOP/services/SecondaryPwlessLoginService.py
--rw-rw-rw-   0        0        0     3908 2024-02-10 18:09:55.000000 LINEBOOP-1.0.3/LINEBOOP/services/SettingsService.py
--rw-rw-rw-   0        0        0      311 2024-02-10 18:10:17.000000 LINEBOOP-1.0.3/LINEBOOP/services/ShopAuthService.py
--rw-rw-rw-   0        0        0    57050 2024-02-10 18:09:51.000000 LINEBOOP-1.0.3/LINEBOOP/services/ShopService.py
--rw-rw-rw-   0        0        0      413 2024-02-10 18:10:01.000000 LINEBOOP-1.0.3/LINEBOOP/services/SquareBotService.py
--rw-rw-rw-   0        0        0    12199 2024-02-11 09:01:34.000000 LINEBOOP-1.0.3/LINEBOOP/services/SquareLiveTalkService.py
--rw-rw-rw-   0        0        0    45459 2024-02-11 09:02:15.000000 LINEBOOP-1.0.3/LINEBOOP/services/SquareService.py
--rw-rw-rw-   0        0        0   226578 2024-02-10 18:09:50.000000 LINEBOOP-1.0.3/LINEBOOP/services/TalkService.py
--rw-rw-rw-   0        0        0      732 2024-02-10 18:10:02.000000 LINEBOOP-1.0.3/LINEBOOP/services/TestService.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:22.000000 LINEBOOP-1.0.3/LINEBOOP/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.819762 LINEBOOP-1.0.3/LINEBOOP/services/thrift/
--rw-rw-rw-   0        0        0     8674 2024-02-10 18:09:50.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/AccessTokenRefreshService.py
--rw-rw-rw-   0        0        0     8916 2024-02-10 18:09:50.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/BuddyService.py
--rw-rw-rw-   0        0        0     8811 2024-02-10 18:09:49.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/CallService.py
--rw-rw-rw-   0        0        0     9240 2024-02-10 18:09:41.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/E2EEKeyBackupService.py
--rw-rw-rw-   0        0        0    19853 2024-02-10 18:09:40.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/HomeSafetyCheckService.py
--rw-rw-rw-   0        0        0    14578 2024-02-10 18:09:39.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py
--rw-rw-rw-   0        0        0   171508 2024-02-10 18:09:39.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/SquareLiveTalkService.py
--rw-rw-rw-   0        0        0   108217 2024-02-10 18:09:38.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/SquareService.py
--rw-rw-rw-   0        0        0     7671 2024-02-10 18:09:38.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/SyncService.py
--rw-rw-rw-   0        0        0   546935 2024-02-10 18:09:37.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/TalkService.py
--rw-rw-rw-   0        0        0      248 2024-02-10 18:09:37.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.872956 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/
--rw-rw-rw-   0        0        0     2909 2024-02-10 18:09:24.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TBase.py
--rw-rw-rw-   0        0        0     9403 2024-02-10 18:09:24.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TBinaryProtocol.py
--rw-rw-rw-   0        0        0    15223 2024-02-10 18:09:24.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TCompactProtocol.py
--rw-rw-rw-   0        0        0    13780 2024-02-10 18:09:23.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TProtocol.py
--rw-rw-rw-   0        0        0     1781 2024-02-10 18:09:23.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TProtocolDecorator.py
--rw-rw-rw-   0        0        0        0 2024-02-10 18:08:23.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/__init__.py
--rw-rw-rw-   0        0        0      419 2024-02-10 18:09:25.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/compat.py
--rw-rw-rw-   0        0        0      380 2024-02-10 18:09:41.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/constants.py
--rw-rw-rw-   0        0        0  1144513 2024-02-10 18:09:37.000000 LINEBOOP-1.0.3/LINEBOOP/services/thrift/ttypes.py
--rw-rw-rw-   0        0        0    39544 2024-02-10 18:10:17.000000 LINEBOOP-1.0.3/LINEBOOP/thrift.py
--rw-rw-rw-   0        0        0    68112 2024-02-10 18:10:18.000000 LINEBOOP-1.0.3/LINEBOOP/timeline.py
--rw-rw-rw-   0        0        0     3531 2024-02-10 18:10:19.000000 LINEBOOP-1.0.3/LINEBOOP/timelineBiz.py
-drwxrwxrwx   0        0        0        0 2024-05-20 06:24:32.875469 LINEBOOP-1.0.3/LINEBOOP.egg-info/
--rw-rw-rw-   0        0        0      713 2024-05-20 06:24:32.000000 LINEBOOP-1.0.3/LINEBOOP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3023 2024-05-20 06:24:32.000000 LINEBOOP-1.0.3/LINEBOOP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 06:24:32.000000 LINEBOOP-1.0.3/LINEBOOP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      129 2024-05-20 06:24:32.000000 LINEBOOP-1.0.3/LINEBOOP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-20 06:24:32.000000 LINEBOOP-1.0.3/LINEBOOP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      713 2024-05-20 06:24:32.876481 LINEBOOP-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      114 2024-02-10 18:16:30.000000 LINEBOOP-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-20 06:24:32.878485 LINEBOOP-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      862 2024-02-10 18:15:11.000000 LINEBOOP-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.089003 LINEBOOP-2.0.0/
+-rw-rw-rw-   0        0        0     1545 2024-02-10 18:24:20.000000 LINEBOOP-2.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:55.986732 LINEBOOP-2.0.0/LINEBOOP/
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:55.998192 LINEBOOP-2.0.0/LINEBOOP/BIZ/
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.000192 LINEBOOP-2.0.0/LINEBOOP/BIZ/TL/
+-rw-rw-rw-   0        0        0     6497 2024-02-10 18:09:22.000000 LINEBOOP-2.0.0/LINEBOOP/BIZ/TL/ST.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-2.0.0/LINEBOOP/BIZ/TL/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-2.0.0/LINEBOOP/BIZ/__init__.py
+-rw-rw-rw-   0        0        0      251 2024-05-22 17:25:14.000000 LINEBOOP-2.0.0/LINEBOOP/__init__.py
+-rw-rw-rw-   0        0        0    26561 2024-05-22 17:13:34.000000 LINEBOOP-2.0.0/LINEBOOP/api.py
+-rw-rw-rw-   0        0        0     5833 2024-02-11 09:02:59.000000 LINEBOOP-2.0.0/LINEBOOP/client.py
+-rw-rw-rw-   0        0        0     9317 2024-05-22 17:15:02.000000 LINEBOOP-2.0.0/LINEBOOP/config.py
+-rw-rw-rw-   0        0        0     1842 2024-02-10 18:10:19.000000 LINEBOOP-2.0.0/LINEBOOP/cube.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.003761 LINEBOOP-2.0.0/LINEBOOP/dyher/
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-2.0.0/LINEBOOP/dyher/__init__.py
+-rw-rw-rw-   0        0        0     7763 2024-02-10 18:09:21.000000 LINEBOOP-2.0.0/LINEBOOP/dyher/conn.py
+-rw-rw-rw-   0        0        0    15544 2024-02-11 09:01:28.000000 LINEBOOP-2.0.0/LINEBOOP/dyher/connManager.py
+-rw-rw-rw-   0        0        0    17273 2024-02-10 18:10:19.000000 LINEBOOP-2.0.0/LINEBOOP/e2ee.py
+-rw-rw-rw-   0        0        0      982 2024-02-10 18:10:20.000000 LINEBOOP-2.0.0/LINEBOOP/exceptions.py
+-rw-rw-rw-   0        0        0    15273 2024-02-10 18:10:19.000000 LINEBOOP-2.0.0/LINEBOOP/helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.009764 LINEBOOP-2.0.0/LINEBOOP/hksc/
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-2.0.0/LINEBOOP/hksc/__init__.py
+-rw-rw-rw-   0        0        0     3439 2024-02-10 18:09:19.000000 LINEBOOP-2.0.0/LINEBOOP/hksc/database.py
+-rw-rw-rw-   0        0        0      335 2024-02-10 18:09:19.000000 LINEBOOP-2.0.0/LINEBOOP/hksc/events.py
+-rw-rw-rw-   0        0        0     6220 2024-02-10 18:09:17.000000 LINEBOOP-2.0.0/LINEBOOP/hksc/types.py
+-rw-rw-rw-   0        0        0     2494 2024-02-10 18:09:17.000000 LINEBOOP-2.0.0/LINEBOOP/hksc/utility.py
+-rw-rw-rw-   0        0        0     4110 2024-02-10 18:10:41.000000 LINEBOOP-2.0.0/LINEBOOP/hooks.py
+-rw-rw-rw-   0        0        0    39147 2024-02-10 18:09:50.000000 LINEBOOP-2.0.0/LINEBOOP/models.py
+-rw-rw-rw-   0        0        0    29790 2024-04-09 11:22:18.000000 LINEBOOP-2.0.0/LINEBOOP/object.py
+-rw-rw-rw-   0        0        0     2426 2024-02-10 18:10:18.000000 LINEBOOP-2.0.0/LINEBOOP/poll.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.013065 LINEBOOP-2.0.0/LINEBOOP/serializers/
+-rw-rw-rw-   0        0        0     2300 2024-02-10 18:09:15.000000 LINEBOOP-2.0.0/LINEBOOP/serializers/DummyProtocol.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:21.000000 LINEBOOP-2.0.0/LINEBOOP/serializers/__init__.py
+-rw-rw-rw-   0        0        0     2760 2024-02-10 18:10:20.000000 LINEBOOP-2.0.0/LINEBOOP/server.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.054149 LINEBOOP-2.0.0/LINEBOOP/services/
+-rw-rw-rw-   0        0        0      933 2024-02-10 18:09:56.000000 LINEBOOP-2.0.0/LINEBOOP/services/AccessTokenRefreshService.py
+-rw-rw-rw-   0        0        0     2425 2024-02-10 18:10:01.000000 LINEBOOP-2.0.0/LINEBOOP/services/AccountAuthFactorEapConnectService.py
+-rw-rw-rw-   0        0        0    13334 2024-02-10 18:09:55.000000 LINEBOOP-2.0.0/LINEBOOP/services/AuthService.py
+-rw-rw-rw-   0        0        0      467 2024-02-11 09:03:35.000000 LINEBOOP-2.0.0/LINEBOOP/services/BaseService.py
+-rw-rw-rw-   0        0        0     1285 2024-02-10 18:10:19.000000 LINEBOOP-2.0.0/LINEBOOP/services/BotExternalService.py
+-rw-rw-rw-   0        0        0    11397 2024-05-22 17:16:51.000000 LINEBOOP-2.0.0/LINEBOOP/services/BuddyService.py
+-rw-rw-rw-   0        0        0    11695 2024-02-10 18:09:57.000000 LINEBOOP-2.0.0/LINEBOOP/services/CallService.py
+-rw-rw-rw-   0        0        0    13827 2024-02-10 18:09:53.000000 LINEBOOP-2.0.0/LINEBOOP/services/ChannelService.py
+-rw-rw-rw-   0        0        0      975 2024-05-22 17:14:01.000000 LINEBOOP-2.0.0/LINEBOOP/services/ChatAppService.py
+-rw-rw-rw-   0        0        0     1509 2024-02-10 18:10:01.000000 LINEBOOP-2.0.0/LINEBOOP/services/E2EEKeyBackupService.py
+-rw-rw-rw-   0        0        0     2037 2024-02-10 18:10:02.000000 LINEBOOP-2.0.0/LINEBOOP/services/HomeSafetyCheckService.py
+-rw-rw-rw-   0        0        0     1946 2024-02-10 18:10:16.000000 LINEBOOP-2.0.0/LINEBOOP/services/InterlockService.py
+-rw-rw-rw-   0        0        0     2651 2024-05-22 17:14:01.000000 LINEBOOP-2.0.0/LINEBOOP/services/LiffService.py
+-rw-rw-rw-   0        0        0     2570 2024-02-11 09:01:42.000000 LINEBOOP-2.0.0/LINEBOOP/services/LoginService.py
+-rw-rw-rw-   0        0        0     2513 2024-02-10 18:10:18.000000 LINEBOOP-2.0.0/LINEBOOP/services/OaMembershipService.py
+-rw-rw-rw-   0        0        0     9898 2024-02-10 18:09:54.000000 LINEBOOP-2.0.0/LINEBOOP/services/PrimaryAccountInitService.py
+-rw-rw-rw-   0        0        0      899 2024-02-10 18:10:02.000000 LINEBOOP-2.0.0/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py
+-rw-rw-rw-   0        0        0     1132 2024-02-10 18:10:02.000000 LINEBOOP-2.0.0/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py
+-rw-rw-rw-   0        0        0     1400 2024-02-10 18:10:18.000000 LINEBOOP-2.0.0/LINEBOOP/services/PwlessPrimaryRegistrationService.py
+-rw-rw-rw-   0        0        0     5773 2024-02-10 18:10:17.000000 LINEBOOP-2.0.0/LINEBOOP/services/RelationService.py
+-rw-rw-rw-   0        0        0     6045 2024-02-10 18:10:18.000000 LINEBOOP-2.0.0/LINEBOOP/services/SearchService.py
+-rw-rw-rw-   0        0        0      937 2024-02-10 18:10:00.000000 LINEBOOP-2.0.0/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py
+-rw-rw-rw-   0        0        0     3207 2024-02-10 18:10:00.000000 LINEBOOP-2.0.0/LINEBOOP/services/SecondaryPwlessLoginService.py
+-rw-rw-rw-   0        0        0     3908 2024-02-10 18:09:55.000000 LINEBOOP-2.0.0/LINEBOOP/services/SettingsService.py
+-rw-rw-rw-   0        0        0      311 2024-02-10 18:10:17.000000 LINEBOOP-2.0.0/LINEBOOP/services/ShopAuthService.py
+-rw-rw-rw-   0        0        0    57050 2024-05-22 17:18:47.000000 LINEBOOP-2.0.0/LINEBOOP/services/ShopService.py
+-rw-rw-rw-   0        0        0      413 2024-02-10 18:10:01.000000 LINEBOOP-2.0.0/LINEBOOP/services/SquareBotService.py
+-rw-rw-rw-   0        0        0    12199 2024-02-11 09:01:34.000000 LINEBOOP-2.0.0/LINEBOOP/services/SquareLiveTalkService.py
+-rw-rw-rw-   0        0        0    45459 2024-02-11 09:02:15.000000 LINEBOOP-2.0.0/LINEBOOP/services/SquareService.py
+-rw-rw-rw-   0        0        0   226578 2024-05-22 17:17:22.000000 LINEBOOP-2.0.0/LINEBOOP/services/TalkService.py
+-rw-rw-rw-   0        0        0      732 2024-02-10 18:10:02.000000 LINEBOOP-2.0.0/LINEBOOP/services/TestService.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:22.000000 LINEBOOP-2.0.0/LINEBOOP/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.073683 LINEBOOP-2.0.0/LINEBOOP/services/thrift/
+-rw-rw-rw-   0        0        0     8674 2024-02-10 18:09:50.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/AccessTokenRefreshService.py
+-rw-rw-rw-   0        0        0     8916 2024-02-10 18:09:50.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/BuddyService.py
+-rw-rw-rw-   0        0        0     8811 2024-02-10 18:09:49.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/CallService.py
+-rw-rw-rw-   0        0        0     9240 2024-02-10 18:09:41.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/E2EEKeyBackupService.py
+-rw-rw-rw-   0        0        0    19853 2024-02-10 18:09:40.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/HomeSafetyCheckService.py
+-rw-rw-rw-   0        0        0    14578 2024-02-10 18:09:39.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py
+-rw-rw-rw-   0        0        0   171508 2024-02-10 18:09:39.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/SquareLiveTalkService.py
+-rw-rw-rw-   0        0        0   108217 2024-02-10 18:09:38.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/SquareService.py
+-rw-rw-rw-   0        0        0     7671 2024-02-10 18:09:38.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/SyncService.py
+-rw-rw-rw-   0        0        0   546935 2024-02-10 18:09:37.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/TalkService.py
+-rw-rw-rw-   0        0        0      248 2024-02-10 18:09:37.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.084003 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/
+-rw-rw-rw-   0        0        0     2909 2024-02-10 18:09:24.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TBase.py
+-rw-rw-rw-   0        0        0     9403 2024-02-10 18:09:24.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TBinaryProtocol.py
+-rw-rw-rw-   0        0        0    15223 2024-02-10 18:09:24.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TCompactProtocol.py
+-rw-rw-rw-   0        0        0    13780 2024-02-10 18:09:23.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TProtocol.py
+-rw-rw-rw-   0        0        0     1781 2024-02-10 18:09:23.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TProtocolDecorator.py
+-rw-rw-rw-   0        0        0        0 2024-02-10 18:08:23.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/__init__.py
+-rw-rw-rw-   0        0        0      419 2024-02-10 18:09:25.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/compat.py
+-rw-rw-rw-   0        0        0      380 2024-02-10 18:09:41.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/constants.py
+-rw-rw-rw-   0        0        0  1144513 2024-02-10 18:09:37.000000 LINEBOOP-2.0.0/LINEBOOP/services/thrift/ttypes.py
+-rw-rw-rw-   0        0        0    39544 2024-02-10 18:10:17.000000 LINEBOOP-2.0.0/LINEBOOP/thrift.py
+-rw-rw-rw-   0        0        0    68112 2024-05-22 17:16:47.000000 LINEBOOP-2.0.0/LINEBOOP/timeline.py
+-rw-rw-rw-   0        0        0     3531 2024-02-10 18:10:19.000000 LINEBOOP-2.0.0/LINEBOOP/timelineBiz.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:25:56.086003 LINEBOOP-2.0.0/LINEBOOP.egg-info/
+-rw-rw-rw-   0        0        0      713 2024-05-22 17:25:55.000000 LINEBOOP-2.0.0/LINEBOOP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3023 2024-05-22 17:25:55.000000 LINEBOOP-2.0.0/LINEBOOP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:25:55.000000 LINEBOOP-2.0.0/LINEBOOP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      129 2024-05-22 17:25:55.000000 LINEBOOP-2.0.0/LINEBOOP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 17:25:55.000000 LINEBOOP-2.0.0/LINEBOOP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      713 2024-05-22 17:25:56.087004 LINEBOOP-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      114 2024-02-10 18:16:30.000000 LINEBOOP-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:25:56.089003 LINEBOOP-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      862 2024-02-10 18:15:11.000000 LINEBOOP-2.0.0/setup.py
```

### Comparing `LINEBOOP-1.0.3/LICENSE` & `LINEBOOP-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/BIZ/TL/ST.py` & `LINEBOOP-2.0.0/LINEBOOP/BIZ/TL/ST.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/api.py` & `LINEBOOP-2.0.0/LINEBOOP/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     def __init__(self, forwardedIp=None, proxy_string=None):                    
         self.server = Server()
         if proxy_string is None:
             self.req = requests.session()
         else:
             self.req = requests.session()
             self.req.proxies = {
-                "http": proxy_string
+                "http": proxy_string,
+                "https": proxy_string
             }
             
         self.req_h2 = httpx.Client(http2=True)
         self.server.Headers = {
             "x-line-application": self.APP_NAME,
             "x-le": self.le,
             "x-lap": "5",
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/client.py` & `LINEBOOP-2.0.0/LINEBOOP/client.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/config.py` & `LINEBOOP-2.0.0/LINEBOOP/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     LINE_LAN_ANDROID_URL = "https://lan.line.me/v1/line/android/notification"
     LINE_LAN_IOS_URL = "https://lan.line.me/v1/line/ios/notification"
     LINE_MUSIC_WEBAPP_URL = "https://music.line.me/webapp"
     LINE_AMP_LOG_URL = "https://log1-amp.line-apps.com/log"
     LINE_SECONDYARY_REGISTER_API_URL = "https://w.line.me/lrs/r"
 
     LINE_LANGUAGE = "th_TH"
-    LINE_SERVICE_REGION = "TW"
+    LINE_SERVICE_REGION = "TH"
 
     APP_TYPE = "CHROMEOS"
     APP_VER = "11.19.2"
     SYSTEM_NAME = "DeachSword"
     SYSTEM_VER = "12.1.4"
     IP_ADDR = "8.8.8.8"
     EMAIL_REGEX = re.compile(r"[^@]+@[^@]+\.[^@]+")
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/cube.py` & `LINEBOOP-2.0.0/LINEBOOP/cube.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/dyher/conn.py` & `LINEBOOP-2.0.0/LINEBOOP/dyher/conn.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/dyher/connManager.py` & `LINEBOOP-2.0.0/LINEBOOP/dyher/connManager.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/e2ee.py` & `LINEBOOP-2.0.0/LINEBOOP/e2ee.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/exceptions.py` & `LINEBOOP-2.0.0/LINEBOOP/exceptions.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/helpers.py` & `LINEBOOP-2.0.0/LINEBOOP/helpers.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/hksc/database.py` & `LINEBOOP-2.0.0/LINEBOOP/hksc/database.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/hksc/types.py` & `LINEBOOP-2.0.0/LINEBOOP/hksc/types.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/hksc/utility.py` & `LINEBOOP-2.0.0/LINEBOOP/hksc/utility.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/hooks.py` & `LINEBOOP-2.0.0/LINEBOOP/hooks.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/models.py` & `LINEBOOP-2.0.0/LINEBOOP/models.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/object.py` & `LINEBOOP-2.0.0/LINEBOOP/object.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/poll.py` & `LINEBOOP-2.0.0/LINEBOOP/poll.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/serializers/DummyProtocol.py` & `LINEBOOP-2.0.0/LINEBOOP/serializers/DummyProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/server.py` & `LINEBOOP-2.0.0/LINEBOOP/server.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/AccessTokenRefreshService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/AccessTokenRefreshService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/AccountAuthFactorEapConnectService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/AccountAuthFactorEapConnectService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/AuthService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/AuthService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/BotExternalService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/BotExternalService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/BuddyService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/BuddyService.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     BuddyService_REQ_TYPE = 3
     BuddyService_RES_TYPE = 3
     BuddyService_API_PATH = None
 
     def __init__(self):
         self.BuddyService_API_PATH = self.LINE_BUDDY_ENDPOINT
 
-    def getPromotedBuddyContacts(self, language="zh_TW", country="TW"):
+    def getPromotedBuddyContacts(self, language="th_TH", country="TH"):
         METHOD_NAME = "getPromotedBuddyContacts"
         sqrd = [128, 1, 0, 1] + \
             self.getStringBytes(METHOD_NAME) + [0, 0, 0, 0]
         sqrd += [11, 0, 2] + self.getStringBytes(language)
         sqrd += [11, 0, 3] + self.getStringBytes(country)
         sqrd += [0]
         return self.postPackDataAndGetUnpackRespData(self.LINE_BUDDY_ENDPOINT, sqrd, readWith=f"BuddyService.{METHOD_NAME}")
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/CallService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/CallService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/ChannelService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/ChannelService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/ChatAppService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/ChatAppService.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 class ChatAppService(object):
     CAPP_REQ_TYPE = 4
     CAPP_RES_TYPE = 4
     
     def __init__(self):
         pass
 
-    def getChatapp(self, chatappId: str, language: str = 'zh_TW'):
+    def getChatapp(self, chatappId: str, language: str = 'th_TH'):
         params = [
             [12, 1, [
                 [11, 1, chatappId],
                 [11, 2, language]
             ]]
         ]
         sqrd = self.generateDummyProtocol('getChatapp', params, self.CAPP_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_CHAT_APP_ENDPOINT, sqrd, self.CAPP_RES_TYPE)
 
-    def getMyChatapps(self, language: str = 'zh_TW', continuationToken: str = None):
+    def getMyChatapps(self, language: str = 'th_TH', continuationToken: str = None):
         params = [
             [12, 1, [
                 [11, 1, language],
                 [11, 2, None]
             ]]
         ]
         sqrd = self.generateDummyProtocol('getMyChatapps', params, self.CAPP_REQ_TYPE)
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/E2EEKeyBackupService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/E2EEKeyBackupService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/HomeSafetyCheckService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/HomeSafetyCheckService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/InterlockService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/InterlockService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/LiffService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/LiffService.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class LiffService(object):
     LIFF_REQ_TYPE = 4
     LIFF_RES_TYPE = 4
 
     def __init__(self):
         pass
         
-    def issueLiffView(self, chatMid, liffId="1562242036-RW04okm", lang='zh_TW', deviceSetting=None):
+    def issueLiffView(self, chatMid, liffId="1562242036-RW04okm", lang='th_TH', deviceSetting=None):
         context = [12, 1, []]
         if chatMid is not None:
             chat = [11, 1, chatMid]
             if chatMid[0] in ['u', 'c', 'r']:
                 chatType = 2
             else:
                 chatType = 3
@@ -38,15 +38,15 @@
         sqrd += b.getFieldHeader(12, 1)
         c = self.TCompactProtocol()
         sqrd += c.getFieldHeader(8, 1)
         sqrd += self.getStringBytes(liffId, isCompact=True)
         sqrd += [0, 0]
         return self.postPackDataAndGetUnpackRespData(self.LINE_LIFF_ENDPOINT ,sqrd, ttype=4)
         
-    def issueSubLiffView(self, chatMid, msit, liffId="1562242036-RW04okm", lang='zh_TW', deviceSetting=None):
+    def issueSubLiffView(self, chatMid, msit, liffId="1562242036-RW04okm", lang='th_TH', deviceSetting=None):
         b = self.TCompactProtocol()
         sqrd = [130, 33, 00] + self.getStringBytes('issueSubLiffView', isCompact=True)
         sqrd += b.getFieldHeader(12, 1)
         c = self.TCompactProtocol()
         sqrd += c.getFieldHeader(8, 1)
         sqrd += self.getStringBytes(liffId, isCompact=True)
         sqrd += c.getFieldHeader(8, 3) + self.getStringBytes(lang, isCompact=True)
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/LoginService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/LoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/OaMembershipService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/OaMembershipService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/PrimaryAccountInitService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/PrimaryAccountInitService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/PrimaryQrCodeMigrationLongPollingService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/PrimaryQrCodeMigrationPreparationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/PwlessPrimaryRegistrationService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/PwlessPrimaryRegistrationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/RelationService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/RelationService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SearchService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SearchService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SecondaryPwlessLoginPermitNoticeService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SecondaryPwlessLoginService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SecondaryPwlessLoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SettingsService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SettingsService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/ShopService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/ShopService.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class ShopService(object):
     ShopService_REQ_TYPE = 3
     ShopService_RES_TYPE = 3
 
     def __init__(self):
         pass
 
-    def getProduct(self, shopId, productId, language="zh-TW", country="TW"):
+    def getProduct(self, shopId, productId, language="th-TH", country="TH"):
         sqrd = [128, 1, 0, 1, 0, 0, 0, 10, 103, 101, 116,
                 80, 114, 111, 100, 117, 99, 116, 0, 0, 0, 0]
         sqrd += [11, 0, 2, 0, 0, 0, len(shopId)]  # e.g. stickershop
         for value in shopId:
             sqrd.append(ord(value))
         sqrd += [11, 0, 3, 0, 0, 0, len(productId)]
         for value in productId:
@@ -48,22 +48,22 @@
 
     def canReceivePresent(self, shopId, productId, recipientMid):
         sqrd = [128, 1, 0, 1] + \
             self.getStringBytes('canReceivePresent') + [0, 0, 0, 0]
         sqrd += [11, 0, 2] + self.getStringBytes(shopId)
         sqrd += [11, 0, 3] + self.getStringBytes(productId)
         sqrd += [12, 0, 4]
-        sqrd += [11, 0, 1] + self.getStringBytes('zh_TW')  # language
-        sqrd += [11, 0, 2] + self.getStringBytes('TW')  # country
+        sqrd += [11, 0, 1] + self.getStringBytes('th_TH')  # language
+        sqrd += [11, 0, 2] + self.getStringBytes('TH')  # country
         sqrd += [0]
         sqrd += [11, 0, 5] + self.getStringBytes(recipientMid)
         sqrd += [0]
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd)
 
-    def getOwnedProductSummaries(self, shopId, offset=0, limit=200, language='zh_TW', country='TW'):
+    def getOwnedProductSummaries(self, shopId, offset=0, limit=200, language='th_TH', country='TH'):
         sqrd = [128, 1, 0, 1] + \
             self.getStringBytes('getOwnedProductSummaries') + [0, 0, 0, 0]
         sqrd += [11, 0, 2] + self.getStringBytes(shopId)
         sqrd += [8, 0, 3] + self.getIntBytes(offset)
         sqrd += [8, 0, 4] + self.getIntBytes(limit)
         sqrd += [12, 0, 5]
         sqrd += [11, 0, 1] + self.getStringBytes(language)
@@ -107,29 +107,29 @@
                 [2, 4, saveBrowsingHistory],
             ]]
         ]
         sqrd = self.generateDummyProtocol(
             'getProductV2', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getProductByVersion(self, shopId: str, productId: str, productVersion: int, language: str = 'zh_TW', country: str = 'TW'):
+    def getProductByVersion(self, shopId: str, productId: str, productVersion: int, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [11, 3, productId],
             [10, 4, productVersion],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getProductByVersion', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def placePurchaseOrderForFreeProduct(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'zh_TW', country: str = 'TW', presentAttributes: dict = {}):
+    def placePurchaseOrderForFreeProduct(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'th_TH', country: str = 'TH', presentAttributes: dict = {}):
         params = [
             [12, 2, [
                 [11, 1, shopId],
                 [11, 2, productId],
                 [11, 5, recipientMid],
                 [12, 11, [
                     [11, 1, price],
@@ -144,15 +144,15 @@
                 [13, 31, [11, 11, presentAttributes]],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'placePurchaseOrderForFreeProduct', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def placePurchaseOrderWithLineCoin(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'zh_TW', country: str = 'TW', presentAttributes: dict = {}):
+    def placePurchaseOrderWithLineCoin(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'th_TH', country: str = 'TH', presentAttributes: dict = {}):
         params = [
             [12, 2, [
                 [11, 1, shopId],
                 [11, 2, productId],
                 [11, 5, recipientMid],
                 [12, 11, [
                     [11, 1, price],
@@ -167,15 +167,15 @@
                 [13, 31, [11, 11, presentAttributes]],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'placePurchaseOrderWithLineCoin', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def placePurchaseOrderWithIAP(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'zh_TW', country: str = 'TW', presentAttributes: dict = {}):
+    def placePurchaseOrderWithIAP(self, shopId: str, productId: str, recipientMid: str, price: str, amount: str, priceString: str, enableLinePointAutoExchange: bool = True, language: str = 'th_TH', country: str = 'TH', presentAttributes: dict = {}):
         params = [
             [12, 2, [
                 [11, 1, shopId],
                 [11, 2, productId],
                 [11, 5, recipientMid],
                 [12, 11, [
                     [11, 1, price],
@@ -190,57 +190,57 @@
                 [13, 31, [11, 11, presentAttributes]],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'placePurchaseOrderWithIAP', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getOwnedProducts(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', country: str = 'TW'):
+    def getOwnedProducts(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [8, 3, offset],
             [8, 4, limit],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getOwnedProducts', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getPurchasedProducts(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', country: str = 'TW'):
+    def getPurchasedProducts(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [8, 3, offset],
             [8, 4, limit],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getPurchasedProducts', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getReceivedPresents(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', country: str = 'TW'):
+    def getReceivedPresents(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [8, 3, offset],
             [8, 4, limit],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getReceivedPresents', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getSentPresents(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', country: str = 'TW'):
+    def getSentPresents(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [8, 3, offset],
             [8, 4, limit],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
@@ -285,28 +285,28 @@
                 [11, 10, authCode]
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'validateProduct', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getProductsByBillingItemId(self, shopId: str, billingItemIds: list, language: str = 'zh_TW', country: str = 'TW'):
+    def getProductsByBillingItemId(self, shopId: str, billingItemIds: list, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [15, 3, [11, billingItemIds]],
             [12, 4, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getProductsByBillingItemId', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getUpdates(self, shopId: str, language: str = 'zh_TW', country: str = 'TW'):
+    def getUpdates(self, shopId: str, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [12, 3, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
@@ -391,29 +391,29 @@
                 [15, 2, [12, showcaseRequests]],  # Shop_ShowcaseRequest
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getAggregatedShowcaseV4', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getRecommendationForUser(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', country: str = 'TW'):
+    def getRecommendationForUser(self, shopId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', country: str = 'TH'):
         params = [
             [11, 2, shopId],
             [8, 3, offset],
             [8, 4, limit],
             [12, 5, [
                 [11, 1, language],
                 [11, 2, country],
             ]],
         ]
         sqrd = self.generateDummyProtocol(
             'getRecommendationForUser', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getRecommendationList(self, productType: int, recommendationType: int, productId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', continuationToken: str = None, shouldShuffle: bool = False, includeStickerIds: bool = True):
+    def getRecommendationList(self, productType: int, recommendationType: int, productId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', continuationToken: str = None, shouldShuffle: bool = False, includeStickerIds: bool = True):
         params = [
             [12, 2, [
                 [11, 1, continuationToken],
                 [8, 2, limit],
                 [8, 3, productType],
                 [8, 4, recommendationType],
                 [11, 5, productId],
@@ -423,15 +423,15 @@
                 # [12, 9, shopFilter],
             ]]
         ]
         sqrd = self.generateDummyProtocol(
             'getRecommendationList', params, self.ShopService_REQ_TYPE)
         return self.postPackDataAndGetUnpackRespData(self.LINE_UNIFIED_SHOP_ENDPOINT, sqrd, self.ShopService_RES_TYPE)
 
-    def getCategories(self, productType: int, recommendationType: int, productId: str, offset: int = 0, limit: int = 20, language: str = 'zh_TW', continuationToken: str = None, shouldShuffle: bool = False, includeStickerIds: bool = True):
+    def getCategories(self, productType: int, recommendationType: int, productId: str, offset: int = 0, limit: int = 20, language: str = 'th_TH', continuationToken: str = None, shouldShuffle: bool = False, includeStickerIds: bool = True):
         params = [
             [12, 2, [
                 [11, 1, continuationToken],
                 [8, 2, limit],
                 [8, 3, productType],
                 [8, 4, recommendationType],
                 [11, 5, productId],
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SquareLiveTalkService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SquareLiveTalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/SquareService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/SquareService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/TalkService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/TalkService.py`

 * *Files 0% similar despite different names*

```diff
@@ -2316,15 +2316,15 @@
             ]
         ]
         sqrd = self.generateDummyProtocol("createChat", params, 4)
         return self.postPackDataAndGetUnpackRespData(
             self.LINE_NORMAL_ENDPOINT, sqrd, readWith=f"TalkService.{METHOD_NAME}"
         )
 
-    def updateRegion(self, region="TW"):
+    def updateRegion(self, region="TH"):
         raise Exception("updateRegion is not implemented")
         params = [[11, 4, region]]
         sqrd = self.generateDummyProtocol("updateRegion", params, 4)
         return self.postPackDataAndGetUnpackRespData(
             self.LINE_NORMAL_ENDPOINT, sqrd, readWith=f"TalkService.{METHOD_NAME}"
         )
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/TestService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/TestService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/AccessTokenRefreshService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/AccessTokenRefreshService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/BuddyService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/BuddyService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/CallService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/CallService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/E2EEKeyBackupService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/E2EEKeyBackupService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/HomeSafetyCheckService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/HomeSafetyCheckService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/SecondaryQrCodeLoginService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/SquareLiveTalkService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/SquareLiveTalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/SquareService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/SquareService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/SyncService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/SyncService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/TalkService.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/TalkService.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TBase.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TBase.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TBinaryProtocol.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TBinaryProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TCompactProtocol.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TCompactProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TProtocol.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TProtocol.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ap/TProtocolDecorator.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ap/TProtocolDecorator.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/services/thrift/ttypes.py` & `LINEBOOP-2.0.0/LINEBOOP/services/thrift/ttypes.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/thrift.py` & `LINEBOOP-2.0.0/LINEBOOP/thrift.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP/timeline.py` & `LINEBOOP-2.0.0/LINEBOOP/timeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -452,15 +452,15 @@
                     },
                 },
                 "STORY": {"version": "v6"},
             }
         }
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
-            {"x-lhm": "POST", "Content-type": "application/json", "x-lsr": "TW"},
+            {"x-lhm": "POST", "Content-type": "application/json", "x-lsr": "TH"},
         )
         r = self.server.postContent(url, headers=hr, data=json.dumps(data))
         result = r.json()
         if result["message"] == "success":
             return result["result"]
         else:
             return False
@@ -836,15 +836,15 @@
             params["scrollId"] = scrollId
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
                 "x-lhm": "GET",
                 "Content-type": "application/json",
                 "x-lpv": "1",
-                "x-lsr": "TW",
+                "x-lsr": "TH",
             },
         )
         url = self.server.urlEncode(
             self.LINE_HOST_DOMAIN, "/mh/api/v57/comment/getList.json", params
         )
         r = self.server.postContent(url, headers=hr)
         return r.json()
@@ -912,15 +912,15 @@
             params["filterType"] = filterType  # eg. 1003 for GROUPED
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
                 "x-lhm": "GET",
                 "Content-type": "application/json",
                 "x-lpv": "1",
-                "x-lsr": "TW",
+                "x-lsr": "TH",
             },
         )
         url = self.server.urlEncode(
             self.LINE_HOST_DOMAIN, "/mh/api/v41/like/getList.json", params
         )
         r = self.server.postContent(url, headers=hr)
         return r.json()
@@ -1061,15 +1061,15 @@
         params = {"homeId": mid}
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
                 "x-lhm": "PUT",
                 "Content-type": "application/json",
                 "x-lpv": "1",  # needless
-                "x-lsr": "TW",  # needless
+                "x-lsr": "TH",  # needless
                 "x-u": "",  # needless
             },
         )
         url = self.server.urlEncode(
             self.LINE_HOST_DOMAIN, "/ext/album/api/v3/album/%s" % albumId, params
         )
         r = self.server.postContent(url, data=data, headers=hr)
@@ -1081,15 +1081,15 @@
         params = {"homeId": mid}
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
                 "x-lhm": "DELETE",
                 "Content-type": "application/json",
                 "x-lpv": "1",  # needless
-                "x-lsr": "TW",  # needless
+                "x-lsr": "TH",  # needless
                 "x-u": "",  # needless
             },
         )
         url = self.server.urlEncode(
             self.LINE_HOST_DOMAIN, "/ext/album/api/v4/album/%s" % albumId, params
         )
         r = self.server.postContent(url, headers=hr)
@@ -1754,15 +1754,15 @@
     @loggedIn
     def getYouTubeVideosWithPopular(self, pageToken=None):
         params = {}
         data = {
             "chart": "mostPopular",
             "part": "snippet,contentDetails,id,liveStreamingDetails,status,statistics",
             "fields": "items(snippet(publishedAt,title,thumbnails(default,high,medium),channelTitle,liveBroadcastContent),contentDetails(duration,contentRating),id,liveStreamingDetails(concurrentViewers,scheduledStartTime),status(embeddable),statistics(viewCount))",
-            "regionCode": "TW",
+            "regionCode": "TH",
             "maxResults": 50,
         }
         if pageToken is not None:
             data["pageToken"] = pageToken
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
@@ -1782,15 +1782,15 @@
     @loggedIn
     def getYouTubeVideosWithPlaylists(self, ids, pageToken=None):
         params = {}
         data = {
             "id": ",".join(ids),
             "part": "id,contentDetails, snippet",
             "fields": "items(contentDetails,id,snippet)",
-            "regionCode": "TW",
+            "regionCode": "TH",
             "maxResults": 50,
         }
         if pageToken is not None:
             data["pageToken"] = pageToken
         hr = self.server.additionalHeaders(
             self.server.timelineHeaders,
             {
@@ -1952,15 +1952,15 @@
         url = self.LINE_HOST_DOMAIN + "/ex/ya/am/v1/share"
         r = self.server.postContent(url, headers=hr, json=data)
         return r.json()
 
     """ Translate Service """
 
     @loggedIn
-    def translate(self, originalText: str, sLang: str = "auto", tLang: str = "tw"):
+    def translate(self, originalText: str, sLang: str = "auto", tLang: str = "th"):
         data = {
             "originalText": originalText,
             "sLang": sLang,
             "tLang": tLang,
             "xMode": 0,
             "id": str(uuid.uuid1()),
             "service": "talk",
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP/timelineBiz.py` & `LINEBOOP-2.0.0/LINEBOOP/timelineBiz.py`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/LINEBOOP.egg-info/PKG-INFO` & `LINEBOOP-2.0.0/LINEBOOP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LINEBOOP
-Version: 1.0.3
+Version: 2.0.0
 Summary: LINE API! Upgrade Proxy
 Home-page: https://github.com/DeachSword/CHRLINE
 Author: DeachSword
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome==3.9.8
```

### Comparing `LINEBOOP-1.0.3/LINEBOOP.egg-info/SOURCES.txt` & `LINEBOOP-2.0.0/LINEBOOP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LINEBOOP-1.0.3/PKG-INFO` & `LINEBOOP-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LINEBOOP
-Version: 1.0.3
+Version: 2.0.0
 Summary: LINE API! Upgrade Proxy
 Home-page: https://github.com/DeachSword/CHRLINE
 Author: DeachSword
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pycryptodome==3.9.8
```

### Comparing `LINEBOOP-1.0.3/setup.py` & `LINEBOOP-2.0.0/setup.py`

 * *Files identical despite different names*

