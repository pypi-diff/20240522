# Comparing `tmp/aleksis_core-4.0.0.dev8.tar.gz` & `tmp/aleksis_core-4.0.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-4.0.0.dev8.tar", max compression
+gzip compressed data, was "aleksis_core-4.0.0.dev9.tar", max compression
```

## Comparing `aleksis_core-4.0.0.dev8.tar` & `aleksis_core-4.0.0.dev9.tar`

### file list

```diff
@@ -1,580 +1,557 @@
--rw-r--r--   0        0        0    42717 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/LICENCE.rst
--rw-r--r--   0        0        0     3786 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/README.rst
--rw-r--r--   0        0        0      194 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2024-05-07 10:13:50.121524 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2024-05-07 10:13:50.869516 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2168 2024-05-07 10:13:53.029493 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    11656 2024-05-07 10:13:51.829506 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2024-05-07 10:13:50.153524 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2024-05-07 10:13:53.097492 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    23254 2024-05-07 10:13:52.769496 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2024-05-07 10:13:53.105492 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0    10749 2024-05-07 10:13:52.809495 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    40416 2024-05-07 10:13:52.793495 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0   103996 2024-05-07 10:13:52.425499 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    25279 2024-05-07 10:13:53.269490 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1144 2024-05-07 10:13:51.845506 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    18560 2024-05-07 10:13:53.049493 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    44148 2024-05-07 10:13:50.881516 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2024-05-07 10:13:52.813495 aleksis_core-4.0.0.dev8/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0     1002 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/admin.py
--rw-r--r--   0        0        0     8751 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/celery.py
--rw-r--r--   0        0        0     2759 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/checks.py
--rw-r--r--   0        0        0    14836 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5506 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/filters.py
--rw-r--r--   0        0        0    30667 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/forms.py
--rw-r--r--   0        0        0     3178 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0     1757 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0     1091 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     4682 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2412 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0    10484 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1471 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     4635 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      748 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      412 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      329 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     2568 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
--rw-r--r--   0        0        0     1894 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
--rw-r--r--   0        0        0      220 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
--rw-r--r--   0        0        0       84 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
--rw-r--r--   0        0        0     3564 2024-05-07 10:12:56.578103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
--rw-r--r--   0        0        0     1190 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
--rw-r--r--   0        0        0    13721 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/Calendar.vue
--rw-r--r--   0        0        0      624 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
--rw-r--r--   0        0        0      309 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
--rw-r--r--   0        0        0     5903 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarOverview.vue
--rw-r--r--   0        0        0     2072 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarSelect.vue
--rw-r--r--   0        0        0      364 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
--rw-r--r--   0        0        0     1521 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
--rw-r--r--   0        0        0     1560 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
--rw-r--r--   0        0        0      318 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
--rw-r--r--   0        0        0      405 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
--rw-r--r--   0        0        0      386 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
--rw-r--r--   0        0        0      426 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendar.graphql
--rw-r--r--   0        0        0      154 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
--rw-r--r--   0        0        0      561 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendarMixin.js
--rw-r--r--   0        0        0     1096 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
--rw-r--r--   0        0        0     9850 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
--rw-r--r--   0        0        0     1021 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
--rw-r--r--   0        0        0       93 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
--rw-r--r--   0        0        0      715 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
--rw-r--r--   0        0        0     5242 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
--rw-r--r--   0        0        0      434 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
--rw-r--r--   0        0        0     3611 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     2806 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0     3009 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ActionSelect.vue
--rw-r--r--   0        0        0      655 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      823 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0    13623 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDBar.vue
--rw-r--r--   0        0        0     5044 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDIterator.vue
--rw-r--r--   0        0        0     7047 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDList.vue
--rw-r--r--   0        0        0     1559 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
--rw-r--r--   0        0        0     1359 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/DateSelectFooter.vue
--rw-r--r--   0        0        0      981 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0     1483 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/FilterBar.vue
--rw-r--r--   0        0        0     5289 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/InlineCRUDList.vue
--rw-r--r--   0        0        0      435 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0     3319 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/SlideIterator.vue
--rw-r--r--   0        0        0      269 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0      292 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/TableLink.vue
--rw-r--r--   0        0        0     2017 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/UpdateIndicator.vue
--rw-r--r--   0        0        0      716 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
--rw-r--r--   0        0        0      456 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
--rw-r--r--   0        0        0     1229 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue
--rw-r--r--   0        0        0      361 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
--rw-r--r--   0        0        0      370 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
--rw-r--r--   0        0        0      357 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/EditButton.vue
--rw-r--r--   0        0        0     1139 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
--rw-r--r--   0        0        0      335 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
--rw-r--r--   0        0        0      357 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
--rw-r--r--   0        0        0      427 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
--rw-r--r--   0        0        0      440 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
--rw-r--r--   0        0        0     1273 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
--rw-r--r--   0        0        0     3269 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
--rw-r--r--   0        0        0     5971 2024-05-07 10:12:56.582103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
--rw-r--r--   0        0        0     2244 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
--rw-r--r--   0        0        0     1038 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
--rw-r--r--   0        0        0     1360 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/ColorField.vue
--rw-r--r--   0        0        0     2622 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/DateField.vue
--rw-r--r--   0        0        0     2401 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
--rw-r--r--   0        0        0     3229 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
--rw-r--r--   0        0        0     1006 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
--rw-r--r--   0        0        0     4834 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
--rw-r--r--   0        0        0      695 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/SexSelect.vue
--rw-r--r--   0        0        0     2390 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/TimeField.vue
--rw-r--r--   0        0        0     1267 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
--rw-r--r--   0        0        0      355 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group/GroupChip.vue
--rw-r--r--   0        0        0      706 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     2125 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group_type/GroupType.vue
--rw-r--r--   0        0        0      696 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group_type/groupType.graphql
--rw-r--r--   0        0        0     2697 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
--rw-r--r--   0        0        0      742 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/holiday/holiday.graphql
--rw-r--r--   0        0        0     2966 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2616 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      207 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1252 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     3389 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      862 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonChip.vue
--rw-r--r--   0        0        0      759 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     2482 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonList.vue
--rw-r--r--   0        0        0     9873 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      301 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      345 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/personList.graphql
--rw-r--r--   0        0        0      589 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     1488 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/room/RoomInlineList.vue
--rw-r--r--   0        0        0      630 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/room/room.graphql
--rw-r--r--   0        0        0     2516 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/SchoolTermField.vue
--rw-r--r--   0        0        0     2952 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
--rw-r--r--   0        0        0      742 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/schoolTerm.graphql
--rw-r--r--   0        0        0     3859 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1490 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      422 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2841 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0    15236 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0    14328 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0    18225 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/ru.json
--rw-r--r--   0        0        0    17582 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     3052 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0     1060 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/calendarFeedDetails.js
--rw-r--r--   0        0        0      386 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/calendarFeedEventBar.js
--rw-r--r--   0        0        0     2695 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/createOrPatchMixin.js
--rw-r--r--   0        0        0      938 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/deepSearchMixin.js
--rw-r--r--   0        0        0     1540 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/deleteMixin.js
--rw-r--r--   0        0        0      538 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/error404.js
--rw-r--r--   0        0        0     2419 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/formRulesMixin.js
--rw-r--r--   0        0        0      490 2024-05-07 10:12:56.586103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/loadingMixin.js
--rw-r--r--   0        0        0     3450 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     3296 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/mutateMixin.js
--rw-r--r--   0        0        0     2256 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0      762 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/permissions.js
--rw-r--r--   0        0        0     3060 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/queryMixin.js
--rw-r--r--   0        0        0     2154 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0      524 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/sexChoiceMixin.js
--rw-r--r--   0        0        0      766 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/syncSortMixin.js
--rw-r--r--   0        0        0     1684 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     7148 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    34409 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2024-05-07 10:13:53.521488 aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74550 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2024-05-07 10:13:53.529487 aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    64425 2024-05-07 10:13:53.521488 aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   127576 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2024-05-07 10:13:53.509488 aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2024-05-07 10:13:53.513488 aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    78337 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2024-05-07 10:13:53.509488 aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2510 2024-05-07 10:13:53.505488 aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    84014 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-05-07 10:13:53.497488 aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-05-07 10:13:53.505488 aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74480 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-05-07 10:13:53.501488 aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    79209 2024-05-07 10:13:53.525488 aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   137668 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-05-07 10:13:53.509488 aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-05-07 10:13:53.521488 aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74420 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-05-07 10:13:53.521488 aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2024-05-07 10:12:56.590103 aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    78198 2024-05-07 10:13:53.533487 aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   135337 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2024-05-07 10:13:53.525488 aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2024-05-07 10:12:56.710101 aleksis_core-4.0.0.dev8/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0     1082 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     5688 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/managers.py
--rw-r--r--   0        0        0    49187 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2198 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1207 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     1936 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2073 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1341 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2116 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1924 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2024-05-07 10:12:56.594103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2024-05-07 10:12:56.598103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2510 2024-05-07 10:12:56.598103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2024-05-07 10:12:56.602103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0      533 2024-05-07 10:12:56.602103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
--rw-r--r--   0        0        0     6221 2024-05-07 10:12:56.602103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0050_managed_by_app_label.py
--rw-r--r--   0        0        0     5606 2024-05-07 10:12:56.602103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0051_calendarevent_and_holiday.py
--rw-r--r--   0        0        0   909270 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0052_site_related_name.py
--rw-r--r--   0        0        0      914 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0053_freebusy.py
--rw-r--r--   0        0        0     1994 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0054_create_organisation_model.py
--rw-r--r--   0        0        0     1738 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0055_customevent.py
--rw-r--r--   0        0        0      332 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0056_rename_customevent_personalevent.py
--rw-r--r--   0        0        0      505 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0057_drop_otp_yubikey.py
--rw-r--r--   0        0        0      720 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0058_migrate_preferences_to_global.py
--rw-r--r--   0        0        0     5514 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0059_drop_site.py
--rw-r--r--   0        0        0     1165 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0060_person_unique_short_name_email.py
--rw-r--r--   0        0        0      500 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/migrations/0061_remove_group_additional_fields.py
--rw-r--r--   0        0        0        0 2024-05-07 10:12:56.718101 aleksis_core-4.0.0.dev8/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    25176 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/mixins.py
--rw-r--r--   0        0        0    64648 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/models.py
--rw-r--r--   0        0        0    15497 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/preferences.py
--rw-r--r--   0        0        0      611 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/registries.py
--rw-r--r--   0        0        0    17710 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/rules.py
--rw-r--r--   0        0        0    11074 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0     7649 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     4023 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/calendar.py
--rw-r--r--   0        0        0     3049 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0     2005 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1309 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/group_type.py
--rw-r--r--   0        0        0     1430 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/holiday.py
--rw-r--r--   0        0        0     1743 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/message.py
--rw-r--r--   0        0        0     1296 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0     1145 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/oauth.py
--rw-r--r--   0        0        0      554 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0    10056 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/person.py
--rw-r--r--   0        0        0     3382 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/personal_event.py
--rw-r--r--   0        0        0     1270 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/room.py
--rw-r--r--   0        0        0     2147 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2024-05-07 10:12:56.606103 aleksis_core-4.0.0.dev8/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1697 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      829 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39858 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4351 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2581 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15749 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     5408 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      918 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2024-05-07 10:12:56.610103 aleksis_core-4.0.0.dev8/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0      525 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/email/email_confirmation_message.txt
--rw-r--r--   0        0        0     1255 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0     1182 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0     1377 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0     1053 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1212 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3879 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2024-05-07 10:12:56.718101 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0     2504 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6832 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2358 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      927 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2024-05-07 10:12:56.614103 aleksis_core-4.0.0.dev8/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1162 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      887 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1660 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0     1014 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1102 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/invitation.email
--rw-r--r--   0        0        0     1461 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6686 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3050 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2024-05-07 10:12:56.722102 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1611 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1543 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0      761 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/managers/test_aleksisbasemanager.py
--rw-r--r--   0        0        0     1607 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/mixins/test_registry_object.py
--rw-r--r--   0        0        0     6596 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     1520 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2024-05-07 10:12:56.618103 aleksis_core-4.0.0.dev8/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    17541 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2024-05-07 10:12:56.726101 aleksis_core-4.0.0.dev8/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2024-05-07 10:13:50.433521 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14949 2024-05-07 10:13:51.849506 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2024-05-07 10:13:52.813495 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    29144 2024-05-07 10:13:50.433521 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2024-05-07 10:13:50.821517 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2024-05-07 10:13:52.825495 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5811 2024-05-07 10:13:52.813495 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9909 2024-05-07 10:13:53.049493 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2024-05-07 10:13:51.869505 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      657 2024-05-07 10:13:51.869505 aleksis_core-4.0.0.dev8/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    11018 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     6617 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    18985 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2901 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3818 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5801 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/search.py
--rw-r--r--   0        0        0      125 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    52594 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/views.py
--rw-r--r--   0        0        0    12147 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       44 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/conftest.py
--rw-r--r--   0        0        0      581 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/docs/Makefile
--rw-r--r--   0        0        0   127432 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2024-05-07 10:12:56.622103 aleksis_core-4.0.0.dev8/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2024-05-07 10:12:56.626103 aleksis_core-4.0.0.dev8/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8109 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     2086 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2024-05-07 10:12:56.630102 aleksis_core-4.0.0.dev8/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6392 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/conf.py
--rw-r--r--   0        0        0      132 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4058 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/index.rst
--rw-r--r--   0        0        0      787 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/make.bat
--rw-r--r--   0        0        0       95 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     5570 2024-05-07 10:13:21.525833 aleksis_core-4.0.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-05-07 10:12:56.634102 aleksis_core-4.0.0.dev8/tox.ini
--rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0    42991 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/LICENCE.rst
+-rw-r--r--   0        0        0     3786 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/README.rst
+-rw-r--r--   0        0        0      194 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/__main__.py
+-rw-r--r--   0        0        0     1002 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8751 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2759 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/checks.py
+-rw-r--r--   0        0        0    14836 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5506 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/filters.py
+-rw-r--r--   0        0        0    30667 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3178 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0     1757 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0     1091 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     4682 2024-05-22 09:16:02.335845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2412 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0    10484 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1471 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     4635 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      748 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      412 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      329 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     2568 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue
+-rw-r--r--   0        0        0     1894 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue
+-rw-r--r--   0        0        0      220 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/accessTokens.graphql
+-rw-r--r--   0        0        0       84 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/revokeOauthToken.graphql
+-rw-r--r--   0        0        0     3564 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue
+-rw-r--r--   0        0        0     1190 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0    13721 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/Calendar.vue
+-rw-r--r--   0        0        0      624 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarControlBar.vue
+-rw-r--r--   0        0        0      309 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarDownloadAllButton.vue
+-rw-r--r--   0        0        0     5903 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarOverview.vue
+-rw-r--r--   0        0        0     2072 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarSelect.vue
+-rw-r--r--   0        0        0      364 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarStatusChip.vue
+-rw-r--r--   0        0        0     1521 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue
+-rw-r--r--   0        0        0     1560 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarWithControls.vue
+-rw-r--r--   0        0        0      318 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CancelledCalendarStatusChip.vue
+-rw-r--r--   0        0        0      405 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/GenericCalendarFeedDetails.vue
+-rw-r--r--   0        0        0      386 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/GenericCalendarFeedEventBar.vue
+-rw-r--r--   0        0        0      426 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendar.graphql
+-rw-r--r--   0        0        0      154 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendarFeeds.graphql
+-rw-r--r--   0        0        0      561 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendarMixin.js
+-rw-r--r--   0        0        0     1096 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js
+-rw-r--r--   0        0        0     9850 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue
+-rw-r--r--   0        0        0     1021 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql
+-rw-r--r--   0        0        0       93 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/setCalendarStatus.graphql
+-rw-r--r--   0        0        0      715 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue
+-rw-r--r--   0        0        0     5242 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue
+-rw-r--r--   0        0        0      434 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar_feeds/event_bar/BirthdaysEventBar.vue
+-rw-r--r--   0        0        0     3611 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     2806 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0     3009 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ActionSelect.vue
+-rw-r--r--   0        0        0      655 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      823 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0    13623 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDBar.vue
+-rw-r--r--   0        0        0     5044 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDIterator.vue
+-rw-r--r--   0        0        0     7047 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDList.vue
+-rw-r--r--   0        0        0     1559 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue
+-rw-r--r--   0        0        0     1359 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/DateSelectFooter.vue
+-rw-r--r--   0        0        0      981 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0     1483 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/FilterBar.vue
+-rw-r--r--   0        0        0     5289 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/InlineCRUDList.vue
+-rw-r--r--   0        0        0      435 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0     3319 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/SlideIterator.vue
+-rw-r--r--   0        0        0      269 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0      292 2024-05-22 09:16:02.339845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/TableLink.vue
+-rw-r--r--   0        0        0     2017 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/UpdateIndicator.vue
+-rw-r--r--   0        0        0      716 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/BaseButton.vue
+-rw-r--r--   0        0        0      456 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/CancelButton.vue
+-rw-r--r--   0        0        0     1229 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue
+-rw-r--r--   0        0        0      361 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/CreateButton.vue
+-rw-r--r--   0        0        0      370 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/DeleteButton.vue
+-rw-r--r--   0        0        0      357 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/EditButton.vue
+-rw-r--r--   0        0        0     1139 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/FilterButton.vue
+-rw-r--r--   0        0        0      335 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/PrimaryActionButton.vue
+-rw-r--r--   0        0        0      357 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/SaveButton.vue
+-rw-r--r--   0        0        0      427 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/SecondaryActionButton.vue
+-rw-r--r--   0        0        0      309 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/chips/CounterChip.vue
+-rw-r--r--   0        0        0      440 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/ClosableSnackbar.vue
+-rw-r--r--   0        0        0     1273 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue
+-rw-r--r--   0        0        0     3269 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue
+-rw-r--r--   0        0        0     5971 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue
+-rw-r--r--   0        0        0     2244 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue
+-rw-r--r--   0        0        0     1038 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue
+-rw-r--r--   0        0        0     1360 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/ColorField.vue
+-rw-r--r--   0        0        0     2622 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/DateField.vue
+-rw-r--r--   0        0        0     2401 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/DateTimeField.vue
+-rw-r--r--   0        0        0     3229 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue
+-rw-r--r--   0        0        0     1006 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue
+-rw-r--r--   0        0        0     4834 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue
+-rw-r--r--   0        0        0      695 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/SexSelect.vue
+-rw-r--r--   0        0        0     2390 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/TimeField.vue
+-rw-r--r--   0        0        0     1267 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/WeekDayField.vue
+-rw-r--r--   0        0        0      355 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group/GroupChip.vue
+-rw-r--r--   0        0        0      706 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     2125 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group_type/GroupType.vue
+-rw-r--r--   0        0        0      696 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group_type/groupType.graphql
+-rw-r--r--   0        0        0     2697 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/holiday/HolidayInlineList.vue
+-rw-r--r--   0        0        0      742 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/holiday/holiday.graphql
+-rw-r--r--   0        0        0     2966 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2616 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      207 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1252 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     3389 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      862 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonChip.vue
+-rw-r--r--   0        0        0      759 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     2482 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonList.vue
+-rw-r--r--   0        0        0     9873 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      301 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      345 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/personList.graphql
+-rw-r--r--   0        0        0      589 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     1488 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/room/RoomInlineList.vue
+-rw-r--r--   0        0        0      630 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/room/room.graphql
+-rw-r--r--   0        0        0     2516 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/SchoolTermField.vue
+-rw-r--r--   0        0        0     2952 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue
+-rw-r--r--   0        0        0      742 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/schoolTerm.graphql
+-rw-r--r--   0        0        0     3859 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1490 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      422 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2841 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0    15236 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0    14328 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0    18225 2024-05-22 09:16:02.343845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/ru.json
+-rw-r--r--   0        0        0    17582 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     3052 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0     1060 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/calendarFeedDetails.js
+-rw-r--r--   0        0        0      386 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/calendarFeedEventBar.js
+-rw-r--r--   0        0        0     2695 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/createOrPatchMixin.js
+-rw-r--r--   0        0        0      938 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/deepSearchMixin.js
+-rw-r--r--   0        0        0     1540 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/deleteMixin.js
+-rw-r--r--   0        0        0      538 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/error404.js
+-rw-r--r--   0        0        0     2419 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/formRulesMixin.js
+-rw-r--r--   0        0        0      490 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/loadingMixin.js
+-rw-r--r--   0        0        0     3450 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     3477 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/mutateMixin.js
+-rw-r--r--   0        0        0     2256 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0      762 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/permissions.js
+-rw-r--r--   0        0        0      409 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/personOverviewCardMixin.js
+-rw-r--r--   0        0        0     3060 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/queryMixin.js
+-rw-r--r--   0        0        0     2154 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0      524 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/sexChoiceMixin.js
+-rw-r--r--   0        0        0      766 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/syncSortMixin.js
+-rw-r--r--   0        0        0     1684 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     7148 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    34409 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2024-05-22 09:17:02.363417 aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74550 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2024-05-22 09:17:02.359417 aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    64425 2024-05-22 09:17:02.411416 aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   127576 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2024-05-22 09:17:02.371417 aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2024-05-22 09:17:02.395417 aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    78337 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-05-22 09:17:02.391417 aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2510 2024-05-22 09:17:02.395417 aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    84014 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-05-22 09:17:02.391417 aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-05-22 09:17:02.395417 aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74480 2024-05-22 09:16:02.347845 aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-05-22 09:17:02.379417 aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    79209 2024-05-22 09:17:02.383417 aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   137668 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-05-22 09:17:02.363417 aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-05-22 09:17:02.375417 aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74420 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-05-22 09:17:02.371417 aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    78198 2024-05-22 09:17:02.403416 aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   135337 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2024-05-22 09:17:02.379417 aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2024-05-22 09:16:02.439844 aleksis_core-4.0.0.dev9/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0     1082 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     5688 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/managers.py
+-rw-r--r--   0        0        0    49187 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2198 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1207 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     1936 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2073 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1341 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2116 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1924 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2024-05-22 09:16:02.351845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2510 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0      533 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py
+-rw-r--r--   0        0        0     6221 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0050_managed_by_app_label.py
+-rw-r--r--   0        0        0     5606 2024-05-22 09:16:02.355845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0051_calendarevent_and_holiday.py
+-rw-r--r--   0        0        0   909270 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0052_site_related_name.py
+-rw-r--r--   0        0        0      914 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0053_freebusy.py
+-rw-r--r--   0        0        0     1994 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0054_create_organisation_model.py
+-rw-r--r--   0        0        0     1738 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0055_customevent.py
+-rw-r--r--   0        0        0      332 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0056_rename_customevent_personalevent.py
+-rw-r--r--   0        0        0      505 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0057_drop_otp_yubikey.py
+-rw-r--r--   0        0        0      720 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0058_migrate_preferences_to_global.py
+-rw-r--r--   0        0        0     5514 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0059_drop_site.py
+-rw-r--r--   0        0        0     1165 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0060_person_unique_short_name_email.py
+-rw-r--r--   0        0        0      500 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0061_remove_group_additional_fields.py
+-rw-r--r--   0        0        0     1238 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/migrations/0062_oauth_update.py
+-rw-r--r--   0        0        0        0 2024-05-22 09:16:02.439844 aleksis_core-4.0.0.dev9/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    25176 2024-05-22 09:16:02.359845 aleksis_core-4.0.0.dev9/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    65089 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/models.py
+-rw-r--r--   0        0        0    15497 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      611 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/registries.py
+-rw-r--r--   0        0        0    17710 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/rules.py
+-rw-r--r--   0        0        0    11074 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0     7656 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     4023 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/calendar.py
+-rw-r--r--   0        0        0     3049 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2005 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1309 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/group_type.py
+-rw-r--r--   0        0        0     1430 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/holiday.py
+-rw-r--r--   0        0        0     1743 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1296 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0     1145 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/oauth.py
+-rw-r--r--   0        0        0      554 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0    10056 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0     3382 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/personal_event.py
+-rw-r--r--   0        0        0     1270 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/room.py
+-rw-r--r--   0        0        0     2147 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1697 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      829 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39858 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2024-05-22 09:16:02.363845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4351 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2581 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15749 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     5408 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      918 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0      525 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/email/email_confirmation_message.txt
+-rw-r--r--   0        0        0     1255 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0     1182 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0     1377 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0     1053 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1212 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3879 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2024-05-22 09:16:02.447844 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0     2504 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6832 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1636 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2024-05-22 09:16:02.367845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2358 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      927 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1162 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      887 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1660 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0     1014 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1102 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/invitation.email
+-rw-r--r--   0        0        0     1461 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6686 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3050 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2024-05-22 09:16:02.455844 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1611 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1543 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2024-05-22 09:16:02.371845 aleksis_core-4.0.0.dev9/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0      761 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/managers/test_aleksisbasemanager.py
+-rw-r--r--   0        0        0     1607 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/mixins/test_registry_object.py
+-rw-r--r--   0        0        0     6596 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     1520 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    17541 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2024-05-22 09:16:02.455844 aleksis_core-4.0.0.dev9/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0    11018 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     6617 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    18985 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2901 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3818 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5801 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      125 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    52594 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/views.py
+-rw-r--r--   0        0        0    12147 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       44 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/conftest.py
+-rw-r--r--   0        0        0      581 2024-05-22 09:16:02.375845 aleksis_core-4.0.0.dev9/docs/Makefile
+-rw-r--r--   0        0        0   127432 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2024-05-22 09:16:02.379845 aleksis_core-4.0.0.dev9/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2024-05-22 09:16:02.383845 aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8109 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     2086 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6392 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/conf.py
+-rw-r--r--   0        0        0      132 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4058 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/index.rst
+-rw-r--r--   0        0        0      787 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/make.bat
+-rw-r--r--   0        0        0       95 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     5570 2024-05-22 09:16:22.459701 aleksis_core-4.0.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-05-22 09:16:02.387845 aleksis_core-4.0.0.dev9/tox.ini
+-rw-r--r--   0        0        0     8737 1970-01-01 00:00:00.000000 aleksis_core-4.0.0.dev9/PKG-INFO
```

### Comparing `aleksis_core-4.0.0.dev8/CHANGELOG.rst` & `aleksis_core-4.0.0.dev9/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,28 +44,32 @@
 Changed
 ~~~~~~~
 
 * Management of school terms was migrated to new frontend.
 * [Dev] Child groups are exposed in the GraphQL type for groups.
 * Content width on different screen sizes is more consistent.
 * Room model icon changed from the default to a specific one.
+* Show only short name, if available, in announcement recipients
 
 Fixed
 ~~~~~
 
 * Persons could not be edited by non-superusers with global person editing permission.
 * GraphQL mutations did not return errors in case of exceptions.
 * Make email field unique over all persons.
 * Third-party login buttons now directly open external login page.
 * Opening group details wasn't possible without permissions for all person details.
 * [Dev] Foreign keys to ExtensiblePolymorphicModel types were using the wrong manager.
 * [Dev] Allow activating more frequent polling for Celery task progress.
 * [OIDC] Custom additional claims were not present in userinfo 
 * Synchronisation of AlekSIS and Django groups caused permissions issues
 * Permission checks for dashboard widget creation and person invitations were invalid
+* New Persons were not added to selected primary group on creation
+* Announcements without any recipient had a line to display recipients
+* In some browsers, AlekSIS was not categorised as an installable PWA.
 
 Removed
 ~~~~~~~
 
 * Yubikey support (not WebAuthn) was removed
 * [Dev] `_recursive` methods for groups have been removed.
   Developers relying on parent groups need to account for recursion themselves.
```

### Comparing `aleksis_core-4.0.0.dev8/LICENCE.rst` & `aleksis_core-4.0.0.dev9/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/README.rst` & `aleksis_core-4.0.0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/admin.py` & `aleksis_core-4.0.0.dev9/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/apps.py` & `aleksis_core-4.0.0.dev9/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/celery.py` & `aleksis_core-4.0.0.dev9/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/checks.py` & `aleksis_core-4.0.0.dev9/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/data_checks.py` & `aleksis_core-4.0.0.dev9/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/decorators.py` & `aleksis_core-4.0.0.dev9/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/filters.py` & `aleksis_core-4.0.0.dev9/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/forms.py` & `aleksis_core-4.0.0.dev9/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/apollo.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplication.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/authorized_oauth_applications/AuthorizedApplications.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/BaseCalendarFeedDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/BaseCalendarFeedEventBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/Calendar.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/Calendar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarControlBar.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarControlBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarOverview.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarSelect.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarTypeSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/CalendarWithControls.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/CalendarWithControls.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendarMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendarMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/calendarSelectedFeedsMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/personal_event/PersonalEventDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar/personal_event/personalEvent.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar_feeds/details/BirthdaysDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/calendar_feeds/details/PersonalDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ActionSelect.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ActionSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDBar.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDIterator.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDIterator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CRUDList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CRUDList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/CopyToClipboardButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/DateSelectFooter.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/DateSelectFooter.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/FilterBar.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/FilterBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/InlineCRUDList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/InlineCRUDList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/SlideIterator.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/SlideIterator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/UpdateIndicator.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/UpdateIndicator.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/BaseButton.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/BaseButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/CollapseTriggerButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/buttons/FilterButton.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/buttons/FilterButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/ConfirmDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/DeleteDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/DialogObjectForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/FilterDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/dialogs/MobileFullscreenDialog.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/ColorField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/ColorField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/DateField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/DateField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/DateTimeField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/DateTimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/ForeignKeyField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/PositiveSmallIntegerField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/RecurrenceField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/SexSelect.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/SexSelect.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/TimeField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/TimeField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/generic/forms/WeekDayField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/generic/forms/WeekDayField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group_type/GroupType.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group_type/GroupType.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/group_type/groupType.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/group_type/groupType.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/holiday/HolidayInlineList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/holiday/HolidayInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/holiday/holiday.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/holiday/holiday.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonChip.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/room/RoomInlineList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/room/RoomInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/room/room.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/room/room.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/SchoolTermField.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/SchoolTermField.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/SchoolTermInlineList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/school_term/schoolTerm.graphql` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/school_term/schoolTerm.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/index.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/de.json` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/en.json` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/ru.json` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/ru.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/messages/uk.json` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/calendarFeedDetails.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/calendarFeedDetails.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/createOrPatchMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/createOrPatchMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/deepSearchMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/deepSearchMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/deleteMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/deleteMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/error404.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/error404.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/formRulesMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/formRulesMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/mutateMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/mutateMixin.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -50,16 +50,22 @@
          *
          * Provide updateStore to update the cached data for affectedQuery with
          * the incoming data.
          *
          * @param {Object} mutation
          * @param {Object} variables
          * @param {Function} updateStore
+         * @param {Object} additionalArgs additional arguments passed to apollo mutate function options
          */
-        mutate(mutation, variables, updateStore = (cached, incoming) => {}) {
+        mutate(
+            mutation,
+            variables,
+            updateStore = (cached, incoming) => {},
+            additionalArgs = {},
+        ) {
             this.handleLoading(true);
             this.$apollo
                 .mutate({
                     mutation: mutation,
                     variables: variables,
                     update: (store, data) => {
                         // TODO: Is data transformed properly?
@@ -92,14 +98,15 @@
                          * updateStore was not provided
                          *
                          * @property {object} store
                          * @property {object} updated object
                          */
                         this.$emit("update", store, data);
                     },
+                    ...additionalArgs,
                 })
                 .then((data) => {
                     /**
                      * Emits the data of a successful graphQL mutation
                      *
                      * @property {object} data
                      */
```

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/permissions.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/permissions.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/queryMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/queryMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/sexChoiceMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/sexChoiceMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/syncSortMixin.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/syncSortMixin.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/frontend/routes.js` & `aleksis_core-4.0.0.dev9/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/health_checks.py` & `aleksis_core-4.0.0.dev9/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-4.0.0.dev9/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-4.0.0.dev9/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/management/commands/vite.py` & `aleksis_core-4.0.0.dev9/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/managers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0001_initial.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0049_oauthapplication_post_logout_redirect_uris.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0050_managed_by_app_label.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0050_managed_by_app_label.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0051_calendarevent_and_holiday.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0051_calendarevent_and_holiday.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0052_site_related_name.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0052_site_related_name.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0053_freebusy.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0053_freebusy.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0054_create_organisation_model.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0054_create_organisation_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0055_customevent.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0055_customevent.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0058_migrate_preferences_to_global.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0058_migrate_preferences_to_global.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0059_drop_site.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0059_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/migrations/0060_person_unique_short_name_email.py` & `aleksis_core-4.0.0.dev9/aleksis/core/migrations/0060_person_unique_short_name_email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/mixins.py` & `aleksis_core-4.0.0.dev9/aleksis/core/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/models.py` & `aleksis_core-4.0.0.dev9/aleksis/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,17 @@
 
     def save(self, *args, **kwargs):
         # Determine all fields that were changed since last load
         changed = self.user_info_tracker.changed()
 
         super().save(*args, **kwargs)
 
+        if self.primary_group:
+            self.member_of.add(self.primary_group)
+
         if self.pk is None or bool(changed):
             if "user_id" in changed:
                 # Clear groups of previous Django user
                 previous_user = changed["user_id"]
                 if previous_user is not None:
                     get_user_model().objects.get(pk=previous_user).groups.clear()
 
@@ -835,14 +838,20 @@
         """
         if isinstance(self.recipient, Person):
             return [self.recipient]
         else:
             return getattr(self.recipient, "announcement_recipients", [])
 
     def __str__(self):
+        if hasattr(self.recipient, "short_name") and self.recipient.short_name:
+            return self.recipient.short_name
+        elif hasattr(self.recipient, "name") and self.recipient.name:
+            return self.recipient.name
+        elif hasattr(self.recipient, "full_name") and self.recipient.full_name:
+            return self.recipient.full_name
         return str(self.recipient)
 
     class Meta:
         verbose_name = _("Announcement recipient")
         verbose_name_plural = _("Announcement recipients")
```

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/preferences.py` & `aleksis_core-4.0.0.dev9/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/registries.py` & `aleksis_core-4.0.0.dev9/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/rules.py` & `aleksis_core-4.0.0.dev9/aleksis/core/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/__init__.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/base.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
     """Mixin for creating revision for mutation."""
 
     @classmethod
     def mutate(cls, root, info, *args, **kwargs):
         with reversion.create_revision():
             set_user(info.context.user)
             set_comment(cls.__name__)
-            super().mutate(root, info, *args, **kwargs)
+            return super().mutate(root, info, *args, **kwargs)
 
 
 class BaseBatchCreateMutation(MutateWithRevisionMixin, DjangoBatchCreateMutation):
     class Meta:
         abstract = True
```

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/calendar.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/calendar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/celery_progress.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/custom_menu.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/group.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/group_type.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/group_type.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/holiday.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/holiday.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/installed_apps.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/notification.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/oauth.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/pdf.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/person.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/person.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/personal_event.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/personal_event.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/room.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/room.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/school_term.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/search.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/site_preferences.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/system_properties.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/two_factor.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/schema/user.py` & `aleksis_core-4.0.0.dev9/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/settings.py` & `aleksis_core-4.0.0.dev9/aleksis/core/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/fallback.png` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/img/hero.svg` & `aleksis_core-4.0.0.dev9/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/helper.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/main.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/multi_select.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/search.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/js/serviceworker.js` & `aleksis_core-4.0.0.dev9/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/print.css` & `aleksis_core-4.0.0.dev9/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-4.0.0.dev9/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/public/style.scss` & `aleksis_core-4.0.0.dev9/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/static/public/theme.scss` & `aleksis_core-4.0.0.dev9/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tables.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tasks.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/403.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/404.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/500.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/email/email_confirmation_message.txt` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/email/email_confirmation_message.txt`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_change.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/signup.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/components/chips.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/components/pagination.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base_print.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/edit.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/full.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/group/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/index.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/announcements.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             {% endblocktrans %}
           {% endif %}
         </em>
       {% endif %}
 
       <i class="material-icons iconify left" data-icon="mdi:message-alert-outline"></i>
 
-      {% if show_recipients and announcement.recipients %}
+      {% if show_recipients and announcement.recipients.all %}
         <p>
           {{ announcement.recipients.all|join:", " }}:
         </p>
       {% endif %}
 
       <figcaption>{{ announcement.title }}</figcaption>
       <p>
```

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/perms/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/create.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/edit.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/person/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/core/vue_index.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/enter.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/offline.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/search/search.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/base.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/email.css` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/invitation.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/invitation.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-4.0.0.dev9/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/managers/test_aleksisbasemanager.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/managers/test_aleksisbasemanager.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/mixins/test_registry_object.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/mixins/test_registry_object.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test.pdf` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_notification.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/tests/views/test_account.py` & `aleksis_core-4.0.0.dev9/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/urls.py` & `aleksis_core-4.0.0.dev9/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/apps.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/auth_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/celery_progress.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/core_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/email.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/forms.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/frontend_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/ldap.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/licenses.json` & `aleksis_core-4.0.0.dev9/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/messages.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/middlewares.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/model_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/notifications.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/pdf.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/predicates.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/sass_helpers.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/search.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/util/tables.py` & `aleksis_core-4.0.0.dev9/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/views.py` & `aleksis_core-4.0.0.dev9/aleksis/core/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         prefs = get_site_preferences()
         pwa_imgs = get_pwa_icons()
 
         icons = [
             {
                 "src": favicon_img.faviconImage.url,
                 "sizes": f"{favicon_img.size}x{favicon_img.size}",
-                "purpose": "maskable any" if prefs["theme__pwa_icon_maskable"] else "any",
+                "purpose": "any maskable" if prefs["theme__pwa_icon_maskable"] else "any",
             }
             for favicon_img in pwa_imgs
         ]
 
         manifest = {
             "name": prefs["general__title"],
             "short_name": prefs["general__title"],
```

### Comparing `aleksis_core-4.0.0.dev8/aleksis/core/vite.config.js` & `aleksis_core-4.0.0.dev9/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/Makefile` & `aleksis_core-4.0.0.dev9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/2fa.png` & `aleksis_core-4.0.0.dev9/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/accept_invite.png` & `aleksis_core-4.0.0.dev9/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/create_dashboard_widget.png` & `aleksis_core-4.0.0.dev9/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/create_social_application.png` & `aleksis_core-4.0.0.dev9/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/dashboard.png` & `aleksis_core-4.0.0.dev9/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/dashboard_widgets.png` & `aleksis_core-4.0.0.dev9/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/data_checks.png` & `aleksis_core-4.0.0.dev9/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/edit_dashboard.png` & `aleksis_core-4.0.0.dev9/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/edit_default_dashboard.png` & `aleksis_core-4.0.0.dev9/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/invitations.png` & `aleksis_core-4.0.0.dev9/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/invite_existing.png` & `aleksis_core-4.0.0.dev9/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-4.0.0.dev9/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/pwa_mobile_safari.png` & `aleksis_core-4.0.0.dev9/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/_static/signup.png` & `aleksis_core-4.0.0.dev9/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/01_core_concepts.rst` & `aleksis_core-4.0.0.dev9/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/10_install.rst` & `aleksis_core-4.0.0.dev9/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/15_config_files.rst` & `aleksis_core-4.0.0.dev9/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/16_config_options.rst` & `aleksis_core-4.0.0.dev9/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/17_storage.rst` & `aleksis_core-4.0.0.dev9/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/18_mail.rst` & `aleksis_core-4.0.0.dev9/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/21_ldap.rst` & `aleksis_core-4.0.0.dev9/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/22_registration.rst` & `aleksis_core-4.0.0.dev9/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/23_socialaccounts.rst` & `aleksis_core-4.0.0.dev9/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/31_monitoring.rst` & `aleksis_core-4.0.0.dev9/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/32_tasks.rst` & `aleksis_core-4.0.0.dev9/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/33_data_checks.rst` & `aleksis_core-4.0.0.dev9/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/admin/50_dashboard.rst` & `aleksis_core-4.0.0.dev9/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/conf.py` & `aleksis_core-4.0.0.dev9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/01_setup.rst` & `aleksis_core-4.0.0.dev9/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/02_install_apps.rst` & `aleksis_core-4.0.0.dev9/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/03_run_tests.rst` & `aleksis_core-4.0.0.dev9/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/04_materialize_templates.rst` & `aleksis_core-4.0.0.dev9/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/06_merging_app_settings.rst` & `aleksis_core-4.0.0.dev9/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-4.0.0.dev9/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/index.rst` & `aleksis_core-4.0.0.dev9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/make.bat` & `aleksis_core-4.0.0.dev9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/ref/core/09_utils.rst` & `aleksis_core-4.0.0.dev9/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/user/01_registration.rst` & `aleksis_core-4.0.0.dev9/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/user/02_personal_account.rst` & `aleksis_core-4.0.0.dev9/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/user/10_dashboard.rst` & `aleksis_core-4.0.0.dev9/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/docs/user/20_pwa.rst` & `aleksis_core-4.0.0.dev9/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/pyproject.toml` & `aleksis_core-4.0.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "4.0.0.dev8"
+version = "4.0.0.dev9"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -61,26 +61,26 @@
 django-tables2 = "^2.1"  # Legacy
 django-phonenumber-field = {version = "^6.1", extras = ["phonenumbers"]}
 django-sass-processor = "1.2.2"  # Legacy
 libsass = "^0.22.0"  # Legacy
 colour = "^0.1.5"
 dynaconf = {version = "^3.1", extras = ["yaml", "toml", "ini"]}
 django-auth-ldap = { version = "^4.0", optional = true }
-django-maintenance-mode = "^0.20.0"
-django-ipware = "^6.0"
+django-maintenance-mode = "^0.21.0"
+django-ipware = "^7.0"
 django-impersonate = "^1.4"
 psycopg2 = "^2.8"
 django_select2 = "^8.0"  # Legacy
 django-two-factor-auth = { version = "^1.15.1", extras = [ "phonenumbers", "call", "sms", "webauthn" ] }
 django-yarnpkg = "^6.1.2"
 django-material = "^1.6.0"  # Legacy
 django-dynamic-preferences = "^1.11"
 django-filter = "^2.2.0"
 django-templated-email = "^3.0.0"
-html2text = "^2020.0.0"
+html2text = "^2024.0.0"
 django-ckeditor = "^6.0.0"  # Legacy
 calendarweek = "^0.5.0"
 Celery = {version="^5.2", extras=["django", "redis"]}
 django-celery-results = "^2.5.1"
 django-celery-beat = "^2.2.0"
 django-celery-email = "^3.0.0"
 django-polymorphic = "^3.0.0"
@@ -97,15 +97,15 @@
 django-favicon-plus-reloaded = "^1.1.5"  # Legacy
 django-health-check = "^3.12.1"
 psutil = "^5.7.0"
 celery-progress = "^0.1.0"
 django-cachalot = "^2.5.3"
 django-prometheus = "^2.1.0"
 django-model-utils = "^4.0.0"
-bs4 = "^0.0.1"
+bs4 = "^0.0.2"
 django-invitations = "^2.0.0"
 django-cleavejs = "^0.1.0"
 django-allauth = "^0.56.0"
 django-uwsgi-ng = "^2.0"
 django-extensions = "^3.1.1"
 ipython = "^8.0.0"
 django-oauth-toolkit = "^2.0.0"
@@ -113,21 +113,21 @@
 boto3 = {version = "^1.34.52", optional = true}
 django-cleanup = "^8.0.0"
 djangorestframework = "^3.12.4"
 Whoosh = "^2.7.4"
 django-titofisto = "^1.0.0"
 haystack-redis = "^0.0.1"
 python-gnupg = "^0.5.0"
-sentry-sdk = {version = "^1.4.3", optional = true}
+sentry-sdk = {version = "^2.0.0", optional = true}
 pycountry = "^23.0.0"
 django-iconify = "^0.3"
 customidenticon = "^0.1.5"
 graphene-django = ">=3.0.0, <=3.1.5"
 selenium = "^4.4.3"
-django-vite = "^2.0.2"
+django-vite = "^3.0.0"
 graphene-django-cud = "^0.11.0"
 django-ical = "^1.9.2"
 django-recurrence = "^1.11.1"
 recurring-ical-events = "^2.0.2"
 django-timezone-field = "^6.0"
 uwsgi = "^2.0.21"
 tqdm = "^4.66.1"
```

### Comparing `aleksis_core-4.0.0.dev8/tox.ini` & `aleksis_core-4.0.0.dev9/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-4.0.0.dev8/PKG-INFO` & `aleksis_core-4.0.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlekSIS-Core
-Version: 4.0.0.dev8
+Version: 4.0.0.dev9
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -27,15 +27,15 @@
 Provides-Extra: ldap
 Provides-Extra: s3
 Provides-Extra: sentry
 Requires-Dist: Celery[django,redis] (>=5.2,<6.0)
 Requires-Dist: Django (>=4.1,<5.0)
 Requires-Dist: Whoosh (>=2.7.4,<3.0.0)
 Requires-Dist: boto3 (>=1.34.52,<2.0.0)
-Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: calendarweek (>=0.5.0,<0.6.0)
 Requires-Dist: celery-haystack-ng (>=2.0,<3.0)
 Requires-Dist: celery-progress (>=0.1.0,<0.2.0)
 Requires-Dist: colour (>=0.1.5,<0.2.0)
 Requires-Dist: customidenticon (>=0.1.5,<0.2.0)
 Requires-Dist: django-allauth (>=0.56.0,<0.57.0)
 Requires-Dist: django-any-js (>=1.1,<2.0)
@@ -58,16 +58,16 @@
 Requires-Dist: django-guardian (>=2.2.0,<3.0.0)
 Requires-Dist: django-haystack (>=3.1,<4.0)
 Requires-Dist: django-health-check (>=3.12.1,<4.0.0)
 Requires-Dist: django-ical (>=1.9.2,<2.0.0)
 Requires-Dist: django-iconify (>=0.3,<0.4)
 Requires-Dist: django-impersonate (>=1.4,<2.0)
 Requires-Dist: django-invitations (>=2.0.0,<3.0.0)
-Requires-Dist: django-ipware (>=6.0,<7.0)
-Requires-Dist: django-maintenance-mode (>=0.20.0,<0.21.0)
+Requires-Dist: django-ipware (>=7.0,<8.0)
+Requires-Dist: django-maintenance-mode (>=0.21.0,<0.22.0)
 Requires-Dist: django-material (>=1.6.0,<2.0.0)
 Requires-Dist: django-model-utils (>=4.0.0,<5.0.0)
 Requires-Dist: django-oauth-toolkit (>=2.0.0,<3.0.0)
 Requires-Dist: django-phonenumber-field[phonenumbers] (>=6.1,<7.0)
 Requires-Dist: django-polymorphic (>=3.0.0,<4.0.0)
 Requires-Dist: django-prometheus (>=2.1.0,<3.0.0)
 Requires-Dist: django-recurrence (>=1.11.1,<2.0.0)
@@ -76,34 +76,34 @@
 Requires-Dist: django-storages (>=1.14.2,<2.0.0) ; extra == "s3"
 Requires-Dist: django-tables2 (>=2.1,<3.0)
 Requires-Dist: django-templated-email (>=3.0.0,<4.0.0)
 Requires-Dist: django-timezone-field (>=6.0,<7.0)
 Requires-Dist: django-titofisto (>=1.0.0,<2.0.0)
 Requires-Dist: django-two-factor-auth[call,phonenumbers,sms,webauthn] (>=1.15.1,<2.0.0)
 Requires-Dist: django-uwsgi-ng (>=2.0,<3.0)
-Requires-Dist: django-vite (>=2.0.2,<3.0.0)
+Requires-Dist: django-vite (>=3.0.0,<4.0.0)
 Requires-Dist: django-yarnpkg (>=6.1.2,<7.0.0)
 Requires-Dist: django_select2 (>=8.0,<9.0)
 Requires-Dist: djangorestframework (>=3.12.4,<4.0.0)
 Requires-Dist: dynaconf[ini,toml,yaml] (>=3.1,<4.0)
 Requires-Dist: graphene-django (>=3.0.0,<=3.1.5)
 Requires-Dist: graphene-django-cud (>=0.11.0,<0.12.0)
 Requires-Dist: haystack-redis (>=0.0.1,<0.0.2)
-Requires-Dist: html2text (>=2020.0.0,<2021.0.0)
+Requires-Dist: html2text (>=2024.0.0,<2025.0.0)
 Requires-Dist: ipython (>=8.0.0,<9.0.0)
 Requires-Dist: libsass (>=0.22.0,<0.23.0)
 Requires-Dist: license-expression (>=30.0,<31.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: psycopg2 (>=2.8,<3.0)
 Requires-Dist: pycountry (>=23.0.0,<24.0.0)
 Requires-Dist: python-gnupg (>=0.5.0,<0.6.0)
 Requires-Dist: recurring-ical-events (>=2.0.2,<3.0.0)
 Requires-Dist: rules (>=3.0,<4.0)
 Requires-Dist: selenium (>=4.4.3,<5.0.0)
-Requires-Dist: sentry-sdk (>=1.4.3,<2.0.0) ; extra == "sentry"
+Requires-Dist: sentry-sdk (>=2.0.0,<3.0.0) ; extra == "sentry"
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Requires-Dist: uwsgi (>=2.0.21,<3.0.0)
 Project-URL: Documentation, https://aleksis.org/AlekSIS-Core/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-Core
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — Core (Core functionality and app framework)
```

