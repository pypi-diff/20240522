# Comparing `tmp/aleksis_app_chronos-4.0.0.dev3.tar.gz` & `tmp/aleksis_app_chronos-4.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_chronos-4.0.0.dev3.tar", max compression
+gzip compressed data, was "aleksis_app_chronos-4.0.0.dev4.tar", max compression
```

## Comparing `aleksis_app_chronos-4.0.0.dev3.tar` & `aleksis_app_chronos-4.0.0.dev4.tar`

### file list

```diff
@@ -1,158 +1,142 @@
--rw-r--r--   0        0        0    10825 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/LICENCE.rst
--rw-r--r--   0        0        0     1835 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/README.rst
--rw-r--r--   0        0        0      153 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__init__.py
--rw-r--r--   0        0        0      447 2024-04-04 15:22:37.692919 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    10080 2024-04-04 15:22:39.480898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0     6047 2024-04-04 15:22:38.516909 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    56706 2024-04-04 15:22:39.380900 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0     3754 2024-04-04 15:22:39.388899 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0     7398 2024-04-04 15:22:39.552898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0    85583 2024-04-04 15:22:39.372900 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     6808 2024-04-04 15:22:39.780895 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     2754 2024-04-04 15:22:39.500898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     5115 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/admin.py
--rw-r--r--   0        0        0     3899 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/apps.py
--rw-r--r--   0        0        0     6090 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/AmendLesson.vue
--rw-r--r--   0        0        0      490 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonEventLinkIterator.vue
--rw-r--r--   0        0        0     1059 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonEventOldNew.vue
--rw-r--r--   0        0        0      947 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonEventSubject.vue
--rw-r--r--   0        0        0      621 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonRelatedObjectChip.vue
--rw-r--r--   0        0        0     1075 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/NoTimetableCard.vue
--rw-r--r--   0        0        0     3062 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/SelectTimetable.vue
--rw-r--r--   0        0        0     5995 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/Timetable.vue
--rw-r--r--   0        0        0     1036 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/amendLesson.graphql
--rw-r--r--   0        0        0     4401 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/details/LessonDetails.vue
--rw-r--r--   0        0        0      414 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/details/SupervisionDetails.vue
--rw-r--r--   0        0        0     3059 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/LessonEventBar.vue
--rw-r--r--   0        0        0      437 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/SupervisionEventBar.vue
--rw-r--r--   0        0        0     2029 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/mixins/lessonEvent.js
--rw-r--r--   0        0        0      333 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/timetableTypes.js
--rw-r--r--   0        0        0      110 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/timetables.graphql
--rw-r--r--   0        0        0      966 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/index.js
--rw-r--r--   0        0        0     1017 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/messages/de.json
--rw-r--r--   0        0        0     1410 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/messages/en.json
--rw-r--r--   0        0        0      446 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/messages/ru.json
--rw-r--r--   0        0        0      426 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/messages/uk.json
--rw-r--r--   0        0        0      463 2024-04-04 15:22:39.944893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19469 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12854 2024-04-04 15:22:39.944893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26924 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      779 2024-04-04 15:22:39.944893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19536 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      513 2024-04-04 15:22:39.936893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19431 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 15:22:39.932893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19287 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16507 2024-04-04 15:22:39.940893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27803 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2024-04-04 15:22:39.936893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19287 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16023 2024-04-04 15:22:39.936893 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    29893 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    34862 2024-04-04 15:21:41.221558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/managers.py
--rw-r--r--   0        0        0    37171 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0001_initial.py
--rw-r--r--   0        0        0     8186 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0002_school_term_validity.py
--rw-r--r--   0        0        0      877 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py
--rw-r--r--   0        0        0     1609 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py
--rw-r--r--   0        0        0     1002 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0005_add_permissions.py
--rw-r--r--   0        0        0     2450 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0006_indexes.py
--rw-r--r--   0        0        0      679 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0007_more_permissions.py
--rw-r--r--   0        0        0     3711 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0008_unique_constraints.py
--rw-r--r--   0        0        0     1555 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0009_automaticplan.py
--rw-r--r--   0        0        0      343 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0010_remove_subject_unique_name_per_site.py
--rw-r--r--   0        0        0     2141 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0011_exam.py
--rw-r--r--   0        0        0      733 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py
--rw-r--r--   0        0        0     1958 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0013_move_room_to_core.py
--rw-r--r--   0        0        0     4621 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0014_add_managed_by_app_label.py
--rw-r--r--   0        0        0     5327 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0015_drop_site.py
--rw-r--r--   0        0        0     3842 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0016_lessonevent.py
--rw-r--r--   0        0        0        0 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/__init__.py
--rw-r--r--   0        0        0     1762 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/mixins.py
--rw-r--r--   0        0        0     4933 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/model_extensions.py
--rw-r--r--   0        0        0    55618 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/models.py
--rw-r--r--   0        0        0     4260 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/preferences.py
--rw-r--r--   0        0        0     2589 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/rules.py
--rw-r--r--   0        0        0     5701 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/schema/__init__.py
--rw-r--r--   0        0        0     2478 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/css/chronos/timetable.css
--rw-r--r--   0        0        0      519 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/css/chronos/timetable_print.css
--rw-r--r--   0        0        0      449 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/js/chronos/date_select.js
--rw-r--r--   0        0        0      579 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/js/chronos/week_select.js
--rw-r--r--   0        0        0      368 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/lesson_event_description.txt
--rw-r--r--   0        0        0     1016 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/datepicker.html
--rw-r--r--   0        0        0      619 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/elements.html
--rw-r--r--   0        0        0     1271 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/event.html
--rw-r--r--   0        0        0      989 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html
--rw-r--r--   0        0        0      115 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/group.html
--rw-r--r--   0        0        0      359 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/groups.html
--rw-r--r--   0        0        0      397 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/groups_part.html
--rw-r--r--   0        0        0     2274 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/headerbox.html
--rw-r--r--   0        0        0       83 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/holiday.html
--rw-r--r--   0        0        0     4401 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/lesson.html
--rw-r--r--   0        0        0      883 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html
--rw-r--r--   0        0        0      538 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/period_time.html
--rw-r--r--   0        0        0      207 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/room.html
--rw-r--r--   0        0        0      135 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subject.html
--rw-r--r--   0        0        0      200 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subject_colour.html
--rw-r--r--   0        0        0      233 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/badge.html
--rw-r--r--   0        0        0      278 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/colour.html
--rw-r--r--   0        0        0      106 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/comment.html
--rw-r--r--   0        0        0      264 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/groups.html
--rw-r--r--   0        0        0      708 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/period.html
--rw-r--r--   0        0        0     1643 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/room.html
--rw-r--r--   0        0        0     1250 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html
--rw-r--r--   0        0        0     1227 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html
--rw-r--r--   0        0        0     1347 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/supervision.html
--rw-r--r--   0        0        0      284 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/teachers.html
--rw-r--r--   0        0        0      101 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/today.html
--rw-r--r--   0        0        0     1734 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/week_select.html
--rw-r--r--   0        0        0     2644 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html
--rw-r--r--   0        0        0     2899 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/substitutions_print.html
--rw-r--r--   0        0        0      109 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/supervision_event_description.txt
--rw-r--r--   0        0        0     1532 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/timetable_print.html
--rw-r--r--   0        0        0        0 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templatetags/__init__.py
--rw-r--r--   0        0        0      797 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templatetags/common.py
--rw-r--r--   0        0        0     1346 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templatetags/week_helpers.py
--rw-r--r--   0        0        0      189 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/urls.py
--rw-r--r--   0        0        0    15656 2024-04-04 15:22:39.504898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/build.cpython-311.pyc
--rw-r--r--   0        0        0     9625 2024-04-04 15:22:39.392899 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/change_tracker.cpython-311.pyc
--rw-r--r--   0        0        0    12110 2024-04-04 15:22:39.504898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/chronos_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     2020 2024-04-04 15:22:39.384899 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/date.cpython-311.pyc
--rw-r--r--   0        0        0     1384 2024-04-04 15:22:39.392899 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/format.cpython-311.pyc
--rw-r--r--   0        0        0      743 2024-04-04 15:22:39.504898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/js.cpython-311.pyc
--rw-r--r--   0        0        0    11071 2024-04-04 15:22:39.556897 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     4090 2024-04-04 15:22:39.500898 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0    17614 2024-04-04 15:21:41.225558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/build.py
--rw-r--r--   0        0        0     5625 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/change_tracker.py
--rw-r--r--   0        0        0     7752 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/chronos_helpers.py
--rw-r--r--   0        0        0     1038 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/date.py
--rw-r--r--   0        0        0      493 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/format.py
--rw-r--r--   0        0        0      234 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/js.py
--rw-r--r--   0        0        0     8309 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/notifications.py
--rw-r--r--   0        0        0     2368 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/predicates.py
--rw-r--r--   0        0        0      750 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/views.py
--rw-r--r--   0        0        0      581 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/Makefile
--rw-r--r--   0        0        0   126772 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/_static/all_timetables.png
--rw-r--r--   0        0        0   134225 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/_static/class_timetable.png
--rw-r--r--   0        0        0   112498 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/_static/daily_lessons.png
--rw-r--r--   0        0        0   115275 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/_static/my_timetable.png
--rw-r--r--   0        0        0   121926 2024-04-04 15:21:41.229558 aleksis_app_chronos-4.0.0.dev3/docs/_static/print_timetable.png
--rw-r--r--   0        0        0    64368 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/_static/substitution_edit.png
--rw-r--r--   0        0        0   100602 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/_static/substitutions.png
--rw-r--r--   0        0        0   135003 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/_static/substitutions_print.png
--rw-r--r--   0        0        0      142 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/admin/00_index.rst
--rw-r--r--   0        0        0      472 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/admin/10_managing_data.rst
--rw-r--r--   0        0        0     1330 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/admin/11_notifications.rst
--rw-r--r--   0        0        0     1139 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/admin/40_preferences.rst
--rw-r--r--   0        0        0     6405 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/conf.py
--rw-r--r--   0        0        0      526 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/index.rst
--rw-r--r--   0        0        0      787 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/make.bat
--rw-r--r--   0        0        0      124 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/00_index.rst
--rw-r--r--   0        0        0     3219 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/01_using_timetables.rst
--rw-r--r--   0        0        0      797 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/10_substitution_plan.rst
--rw-r--r--   0        0        0      536 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/11_notifications.rst
--rw-r--r--   0        0        0      815 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/15_manage_substitutions.rst
--rw-r--r--   0        0        0      384 2024-04-04 15:21:41.233558 aleksis_app_chronos-4.0.0.dev3/docs/user/40_preferences.rst
--rw-r--r--   0        0        0     2934 2024-04-04 15:21:58.525362 aleksis_app_chronos-4.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     2180 2024-04-04 15:21:41.241558 aleksis_app_chronos-4.0.0.dev3/tox.ini
--rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 aleksis_app_chronos-4.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0    10825 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/LICENCE.rst
+-rw-r--r--   0        0        0     1835 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/README.rst
+-rw-r--r--   0        0        0      153 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/__init__.py
+-rw-r--r--   0        0        0     5115 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/admin.py
+-rw-r--r--   0        0        0     3899 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/apps.py
+-rw-r--r--   0        0        0     6090 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/AmendLesson.vue
+-rw-r--r--   0        0        0      490 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonEventLinkIterator.vue
+-rw-r--r--   0        0        0     1059 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonEventOldNew.vue
+-rw-r--r--   0        0        0      947 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonEventSubject.vue
+-rw-r--r--   0        0        0      621 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonRelatedObjectChip.vue
+-rw-r--r--   0        0        0     1075 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/NoTimetableCard.vue
+-rw-r--r--   0        0        0     3062 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/SelectTimetable.vue
+-rw-r--r--   0        0        0      437 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/Timetable.vue
+-rw-r--r--   0        0        0     6721 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/TimetableWrapper.vue
+-rw-r--r--   0        0        0     1036 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/amendLesson.graphql
+-rw-r--r--   0        0        0     4401 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/details/LessonDetails.vue
+-rw-r--r--   0        0        0      414 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/details/SupervisionDetails.vue
+-rw-r--r--   0        0        0     3059 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/LessonEventBar.vue
+-rw-r--r--   0        0        0      437 2024-05-22 12:25:08.603540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/SupervisionEventBar.vue
+-rw-r--r--   0        0        0     2029 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/mixins/lessonEvent.js
+-rw-r--r--   0        0        0      333 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/timetableTypes.js
+-rw-r--r--   0        0        0      110 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/timetables.graphql
+-rw-r--r--   0        0        0      912 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/index.js
+-rw-r--r--   0        0        0     1497 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/messages/de.json
+-rw-r--r--   0        0        0     1410 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/messages/en.json
+-rw-r--r--   0        0        0      662 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/messages/ru.json
+-rw-r--r--   0        0        0      642 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/messages/uk.json
+-rw-r--r--   0        0        0      463 2024-05-22 12:26:15.327085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19469 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12854 2024-05-22 12:26:15.335085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26924 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      779 2024-05-22 12:26:15.339085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19536 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      513 2024-05-22 12:26:15.331085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19431 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-05-22 12:26:15.331085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19287 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16507 2024-05-22 12:26:15.335085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27803 2024-05-22 12:25:08.607540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2024-05-22 12:26:15.339085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19287 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16023 2024-05-22 12:26:15.327085 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    29893 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    35287 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/managers.py
+-rw-r--r--   0        0        0    37171 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0001_initial.py
+-rw-r--r--   0        0        0     8186 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0002_school_term_validity.py
+-rw-r--r--   0        0        0      877 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py
+-rw-r--r--   0        0        0     1609 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py
+-rw-r--r--   0        0        0     1002 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0005_add_permissions.py
+-rw-r--r--   0        0        0     2450 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0006_indexes.py
+-rw-r--r--   0        0        0      679 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0007_more_permissions.py
+-rw-r--r--   0        0        0     3711 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0008_unique_constraints.py
+-rw-r--r--   0        0        0     1555 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0009_automaticplan.py
+-rw-r--r--   0        0        0      343 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0010_remove_subject_unique_name_per_site.py
+-rw-r--r--   0        0        0     2141 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0011_exam.py
+-rw-r--r--   0        0        0      733 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py
+-rw-r--r--   0        0        0     1958 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0013_move_room_to_core.py
+-rw-r--r--   0        0        0     4621 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0014_add_managed_by_app_label.py
+-rw-r--r--   0        0        0     5327 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0015_drop_site.py
+-rw-r--r--   0        0        0     3842 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0016_lessonevent.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:25:09.059537 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-22 12:25:08.611540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/mixins.py
+-rw-r--r--   0        0        0     4933 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/model_extensions.py
+-rw-r--r--   0        0        0    55719 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/models.py
+-rw-r--r--   0        0        0     4766 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/preferences.py
+-rw-r--r--   0        0        0     2589 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/rules.py
+-rw-r--r--   0        0        0     5661 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/schema/__init__.py
+-rw-r--r--   0        0        0     2478 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/css/chronos/timetable.css
+-rw-r--r--   0        0        0      519 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/css/chronos/timetable_print.css
+-rw-r--r--   0        0        0      449 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/js/chronos/date_select.js
+-rw-r--r--   0        0        0      579 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/js/chronos/week_select.js
+-rw-r--r--   0        0        0      368 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/lesson_event_description.txt
+-rw-r--r--   0        0        0     1016 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/datepicker.html
+-rw-r--r--   0        0        0      619 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/elements.html
+-rw-r--r--   0        0        0     1271 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/event.html
+-rw-r--r--   0        0        0      989 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html
+-rw-r--r--   0        0        0      115 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/group.html
+-rw-r--r--   0        0        0      359 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/groups.html
+-rw-r--r--   0        0        0      397 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/groups_part.html
+-rw-r--r--   0        0        0     2274 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/headerbox.html
+-rw-r--r--   0        0        0       83 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/holiday.html
+-rw-r--r--   0        0        0     4401 2024-05-22 12:25:08.615540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/lesson.html
+-rw-r--r--   0        0        0      883 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html
+-rw-r--r--   0        0        0      538 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/period_time.html
+-rw-r--r--   0        0        0      207 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/room.html
+-rw-r--r--   0        0        0      135 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subject.html
+-rw-r--r--   0        0        0      200 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subject_colour.html
+-rw-r--r--   0        0        0      233 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/badge.html
+-rw-r--r--   0        0        0      278 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/colour.html
+-rw-r--r--   0        0        0      106 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/comment.html
+-rw-r--r--   0        0        0      264 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/groups.html
+-rw-r--r--   0        0        0      708 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/period.html
+-rw-r--r--   0        0        0     1643 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/room.html
+-rw-r--r--   0        0        0     1250 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html
+-rw-r--r--   0        0        0     1227 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html
+-rw-r--r--   0        0        0     1347 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/supervision.html
+-rw-r--r--   0        0        0      284 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/teachers.html
+-rw-r--r--   0        0        0      101 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/today.html
+-rw-r--r--   0        0        0     1734 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/week_select.html
+-rw-r--r--   0        0        0     2644 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html
+-rw-r--r--   0        0        0     2899 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/substitutions_print.html
+-rw-r--r--   0        0        0      109 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/supervision_event_description.txt
+-rw-r--r--   0        0        0     1532 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/timetable_print.html
+-rw-r--r--   0        0        0        0 2024-05-22 12:25:09.059537 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templatetags/__init__.py
+-rw-r--r--   0        0        0      797 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templatetags/common.py
+-rw-r--r--   0        0        0     1346 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templatetags/week_helpers.py
+-rw-r--r--   0        0        0      189 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/urls.py
+-rw-r--r--   0        0        0    17614 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/build.py
+-rw-r--r--   0        0        0     5625 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/change_tracker.py
+-rw-r--r--   0        0        0     7810 2024-05-22 12:25:08.619540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/chronos_helpers.py
+-rw-r--r--   0        0        0     1038 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/date.py
+-rw-r--r--   0        0        0      493 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/format.py
+-rw-r--r--   0        0        0      234 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/js.py
+-rw-r--r--   0        0        0     8309 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/notifications.py
+-rw-r--r--   0        0        0     2366 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/predicates.py
+-rw-r--r--   0        0        0      750 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/views.py
+-rw-r--r--   0        0        0      581 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/docs/Makefile
+-rw-r--r--   0        0        0   126772 2024-05-22 12:25:08.623540 aleksis_app_chronos-4.0.0.dev4/docs/_static/all_timetables.png
+-rw-r--r--   0        0        0   134225 2024-05-22 12:25:08.627540 aleksis_app_chronos-4.0.0.dev4/docs/_static/class_timetable.png
+-rw-r--r--   0        0        0   112498 2024-05-22 12:25:08.627540 aleksis_app_chronos-4.0.0.dev4/docs/_static/daily_lessons.png
+-rw-r--r--   0        0        0   115275 2024-05-22 12:25:08.627540 aleksis_app_chronos-4.0.0.dev4/docs/_static/my_timetable.png
+-rw-r--r--   0        0        0   121926 2024-05-22 12:25:08.627540 aleksis_app_chronos-4.0.0.dev4/docs/_static/print_timetable.png
+-rw-r--r--   0        0        0    64368 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/_static/substitution_edit.png
+-rw-r--r--   0        0        0   100602 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/_static/substitutions.png
+-rw-r--r--   0        0        0   135003 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/_static/substitutions_print.png
+-rw-r--r--   0        0        0      142 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/admin/00_index.rst
+-rw-r--r--   0        0        0      472 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/admin/10_managing_data.rst
+-rw-r--r--   0        0        0     1330 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/admin/11_notifications.rst
+-rw-r--r--   0        0        0     1139 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/admin/40_preferences.rst
+-rw-r--r--   0        0        0     6405 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/conf.py
+-rw-r--r--   0        0        0      526 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/index.rst
+-rw-r--r--   0        0        0      787 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/make.bat
+-rw-r--r--   0        0        0      124 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/user/00_index.rst
+-rw-r--r--   0        0        0     3219 2024-05-22 12:25:08.631540 aleksis_app_chronos-4.0.0.dev4/docs/user/01_using_timetables.rst
+-rw-r--r--   0        0        0      797 2024-05-22 12:25:08.635540 aleksis_app_chronos-4.0.0.dev4/docs/user/10_substitution_plan.rst
+-rw-r--r--   0        0        0      536 2024-05-22 12:25:08.635540 aleksis_app_chronos-4.0.0.dev4/docs/user/11_notifications.rst
+-rw-r--r--   0        0        0      815 2024-05-22 12:25:08.635540 aleksis_app_chronos-4.0.0.dev4/docs/user/15_manage_substitutions.rst
+-rw-r--r--   0        0        0      384 2024-05-22 12:25:08.635540 aleksis_app_chronos-4.0.0.dev4/docs/user/40_preferences.rst
+-rw-r--r--   0        0        0     2934 2024-05-22 12:25:27.435412 aleksis_app_chronos-4.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     2180 2024-05-22 12:25:08.659540 aleksis_app_chronos-4.0.0.dev4/tox.ini
+-rw-r--r--   0        0        0     3140 1970-01-01 00:00:00.000000 aleksis_app_chronos-4.0.0.dev4/PKG-INFO
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/CHANGELOG.rst` & `aleksis_app_chronos-4.0.0.dev4/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/LICENCE.rst` & `aleksis_app_chronos-4.0.0.dev4/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/README.rst` & `aleksis_app_chronos-4.0.0.dev4/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/admin.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/apps.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/AmendLesson.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/AmendLesson.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonEventOldNew.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonEventOldNew.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonEventSubject.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonEventSubject.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/LessonRelatedObjectChip.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/LessonRelatedObjectChip.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/NoTimetableCard.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/NoTimetableCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/SelectTimetable.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/SelectTimetable.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/Timetable.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/TimetableWrapper.vue`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <script>
 import { gqlAvailableTimetables } from "./timetables.graphql";
 import NoTimetableCard from "./NoTimetableCard.vue";
 import SelectTimetable from "./SelectTimetable.vue";
 import timetableTypes from "./timetableTypes";
 
 export default {
-  name: "Timetable",
+  name: "TimetableWrapper",
   components: { NoTimetableCard, SelectTimetable },
   apollo: {
     availableTimetables: {
       query: gqlAvailableTimetables,
       result() {
         if (
           !this.selected &&
@@ -33,16 +33,27 @@
       selected: null,
       search: "",
       selectedTypes: ["GROUP", "TEACHER", "ROOM"],
       types: timetableTypes,
       selectDialog: false,
     };
   },
+  props: {
+    onSelected: {
+      type: Function,
+      required: false,
+      default: null,
+    },
+  },
   watch: {
     selected(selected) {
+      if (this.onSelected) {
+        this.onSelected(selected);
+        return;
+      }
       // Align navigation with currently selected timetable
       if (!selected) {
         this.$router.push({ name: "chronos.timetable" });
       } else if (
         selected.objId !== this.$route.params.id ||
         selected.type.toLowerCase() !== this.$route.params.type
       ) {
@@ -103,28 +114,41 @@
         v-model="selectDialog"
         fullscreen
         hide-overlay
         transition="dialog-bottom-transition"
       >
         <v-card>
           <v-toolbar dark color="primary">
+            <v-btn icon dark @click="selectDialog = false">
+              <v-icon>mdi-close</v-icon>
+            </v-btn>
             <v-toolbar-title>{{
               $t("chronos.timetable.select")
             }}</v-toolbar-title>
             <v-spacer></v-spacer>
           </v-toolbar>
+          <slot
+            name="additionalSelect"
+            :selected="selected"
+            :mobile="true"
+          ></slot>
           <select-timetable
             v-model="selected"
             @input="selectDialog = false"
             :available-timetables="availableTimetables"
           />
         </v-card>
       </v-dialog>
 
       <v-col md="3" lg="3" xl="3" v-if="$vuetify.breakpoint.lgAndUp">
+        <slot
+          name="additionalSelect"
+          :selected="selected"
+          :mobile="false"
+        ></slot>
         <v-card>
           <select-timetable
             v-model="selected"
             :available-timetables="availableTimetables"
           />
         </v-card>
       </v-col>
@@ -160,19 +184,29 @@
                 @click="selectTimetable(nextTimetable)"
                 :title="$t('chronos.timetable.next')"
                 class="ml-1 float-right"
               >
                 <v-icon>mdi-chevron-right</v-icon>
               </v-btn>
             </v-card-title>
+            <slot
+              name="additionalButton"
+              :selected="selected"
+              :mobile="true"
+            ></slot>
           </div>
 
           <div class="d-flex flex-wrap justify-space-between mb-2" v-else>
             <v-card-title>
               {{ selected.name }}
+              <slot
+                name="additionalButton"
+                :selected="selected"
+                :mobile="false"
+              ></slot>
             </v-card-title>
             <div class="pa-2 mt-1">
               <v-btn
                 icon
                 :disabled="!prevTimetable"
                 @click="selectTimetable(prevTimetable)"
                 :title="$t('chronos.timetable.prev')"
@@ -188,16 +222,13 @@
                 @click="selectTimetable(nextTimetable)"
                 :title="$t('chronos.timetable.next')"
               >
                 <v-icon>mdi-chevron-right</v-icon>
               </v-btn>
             </div>
           </div>
-          <calendar-with-controls
-            :calendar-feeds="[{ name: 'lesson' }, { name: 'supervision' }]"
-            :params="{ type: selected.type, id: selected.objId }"
-          />
+          <slot :selected="selected"></slot>
         </v-card>
       </v-col>
     </v-row>
   </div>
 </template>
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/amendLesson.graphql` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/amendLesson.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/details/LessonDetails.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/details/LessonDetails.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/LessonEventBar.vue` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/event_bar/LessonEventBar.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/components/calendar_feeds/mixins/lessonEvent.js` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/components/calendar_feeds/mixins/lessonEvent.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/index.js` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/index.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -7,24 +7,22 @@
     meta: {
         inMenu: true,
         titleKey: "chronos.menu_title",
         icon: "mdi-school-outline",
         iconActive: "mdi-school",
         validators: [hasPersonValidator],
     },
-    props: {
-        byTheGreatnessOfTheAlmightyAleksolotlISwearIAmWorthyOfUsingTheLegacyBaseTemplate: true,
-    },
     children: [{
         path: "timetable/",
         component: Timetable,
         name: "chronos.timetable",
         meta: {
             inMenu: true,
             titleKey: "chronos.timetable.menu_title",
+            toolbarTitle: "chronos.timetable.menu_title",
             icon: "mdi-grid",
             permission: "chronos.view_timetable_overview_rule",
             fullWidth: true,
         },
     }, {
         path: "timetable/:type/:id/",
         component: Timetable,
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/frontend/messages/en.json` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/managers.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -872,14 +872,23 @@
     def for_teacher(self, teacher: Union[int, Person]) -> "LessonEventQuerySet":
         """Get all lesson events for a certain person as teacher (including amends)."""
         amended = self.filter(Q(amended_by__isnull=False) & (Q(teachers=teacher))).values_list(
             "amended_by__pk", flat=True
         )
         return self.filter(Q(teachers=teacher) | Q(pk__in=amended)).distinct()
 
+    def for_participant(self, person: Union[int, Person]) -> "LessonEventQuerySet":
+        """Get all lesson events the person participates in (including amends)."""
+        amended = self.filter(
+            Q(amended_by__isnull=False) | Q(groups__members=person)
+        ).values_list("amended_by__pk", flat=True)
+        return self.filter(
+            Q(groups__members=person) | Q(pk__in=amended)
+        ).distinct()
+
     def for_group(self, group: Union[int, Group]) -> "LessonEventQuerySet":
         """Get all lesson events for a certain group (including amends/as parent group)."""
         amended = self.filter(
             Q(amended_by__isnull=False) & (Q(groups=group) | Q(groups__parent_groups=group))
         ).values_list("amended_by__pk", flat=True)
         return self.filter(
             Q(groups=group) | Q(groups__parent_groups=group) | Q(pk__in=amended)
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0001_initial.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0002_school_term_validity.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0002_school_term_validity.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0003_school_term_validity_fixes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0004_substitution_extra_lesson_year.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0005_add_permissions.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0005_add_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0006_indexes.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0006_indexes.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0007_more_permissions.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0007_more_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0008_unique_constraints.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0008_unique_constraints.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0009_automaticplan.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0009_automaticplan.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0011_exam.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0011_exam.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0012_add_supervision_global_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0013_move_room_to_core.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0013_move_room_to_core.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0014_add_managed_by_app_label.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0014_add_managed_by_app_label.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0015_drop_site.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0015_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/migrations/0016_lessonevent.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/migrations/0016_lessonevent.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/mixins.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/model_extensions.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/model_extensions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/models.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1551,14 +1551,16 @@
                     objs = objs.for_person(request.user.person)
                 else:
                     objs = objs.related_to_person(request.user.person)
 
             if type_ and obj_id:
                 if type_ == "TEACHER":
                     return objs.for_teacher(obj_id)
+                elif type_ == "PARTICIPANT":
+                    return objs.for_participant(obj_id)
                 elif type_ == "GROUP":
                     return objs.for_group(obj_id)
                 elif type_ == "ROOM":
                     return objs.for_room(obj_id)
                 elif type_ == "COURSE":
                     return objs.for_course(obj_id)
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/preferences.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/preferences.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from django.utils.translation import gettext_lazy as _
 
 from colorfield.widgets import ColorWidget
 from dynamic_preferences.preferences import Section
 from dynamic_preferences.types import (
     BooleanPreference,
     IntegerPreference,
+    ModelMultipleChoicePreference,
     StringPreference,
     TimePreference,
 )
 
+from aleksis.core.models import GroupType
 from aleksis.core.registries import person_preferences_registry, site_preferences_registry
 
 chronos = Section("chronos", verbose_name=_("Timetables"))
 
 
 @site_preferences_registry.register
 class UseParentGroups(BooleanPreference):
@@ -112,14 +114,28 @@
     section = chronos
     name = "send_notifications"
     default = True
     verbose_name = _("Send notifications for current timetable changes")
 
 
 @site_preferences_registry.register
+class GroupTypesTimetables(ModelMultipleChoicePreference):
+    section = chronos
+    name = "group_types_timetables"
+    required = False
+    default = []
+    model = GroupType
+    verbose_name = _("Group types to show in timetables")
+    help_text = _("If you leave it empty, all groups will be shown.")
+
+    def get_queryset(self):
+        return GroupType.objects.managed_and_unmanaged()
+
+
+@site_preferences_registry.register
 class LessonEventFeedColor(StringPreference):
     """Color for the lesson calendar feed."""
 
     section = chronos
     name = "lesson_color"
     default = "#a7ffeb"
     verbose_name = _("Lesson calendar feed color")
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/rules.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/schema/__init__.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/schema/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     DjangoBatchDeleteMutation,
     DjangoBatchPatchMutation,
 )
 
 from aleksis.core.models import Group, Person, Room
 
 from ..models import LessonEvent
-from ..util.chronos_helpers import get_classes, get_rooms, get_teachers
+from ..util.chronos_helpers import get_groups, get_rooms, get_teachers
 
 
 class TimetablePersonType(DjangoObjectType):
     class Meta:
         model = Person
         fields = ("id", "first_name", "last_name", "short_name")
         skip_registry = True
@@ -145,33 +145,32 @@
     timetable_rooms = graphene.List(TimetableRoomType)
     available_timetables = graphene.List(TimetableObjectType)
 
     def resolve_timetable_teachers(self, info, **kwargs):
         return get_teachers(info.context.user)
 
     def resolve_timetable_groups(self, info, **kwargs):
-        return get_classes(info.context.user)
+        return get_groups(info.context.user)
 
     def resolve_timetable_rooms(self, info, **kwargs):
         return get_rooms(info.context.user)
 
     def resolve_available_timetables(self, info, **kwargs):
         all_timetables = []
-        for group in get_classes(info.context.user):
+        for group in get_groups(info.context.user):
             all_timetables.append(
                 TimetableObjectType(
                     id=group.id,
                     name=group.name,
                     short_name=group.short_name,
                     type=TimetableType.GROUP,
                 )
             )
 
         for teacher in get_teachers(info.context.user):
-            print(teacher.full_name)
             all_timetables.append(
                 TimetableObjectType(
                     id=teacher.id,
                     name=teacher.full_name,
                     short_name=teacher.short_name,
                     type=TimetableType.TEACHER,
                 )
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/css/chronos/timetable.css` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/css/chronos/timetable.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/css/chronos/timetable_print.css` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/css/chronos/timetable_print.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/static/js/chronos/week_select.js` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/static/js/chronos/week_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/datepicker.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/datepicker.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/elements.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/elements.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/event.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/event.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/extra_lesson.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/headerbox.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/headerbox.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/lesson.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/lesson.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/lessons_col.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/period_time.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/period_time.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/period.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/period.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/room.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/room.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/subject.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/subs/teachers.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/supervision.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/supervision.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/week_select.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/week_select.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/partials/week_timetable.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/substitutions_print.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/substitutions_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templates/chronos/timetable_print.html` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templates/chronos/timetable_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templatetags/common.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templatetags/common.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/templatetags/week_helpers.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/templatetags/week_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/build.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/build.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/change_tracker.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/change_tracker.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/chronos_helpers.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/chronos_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,14 @@
     User = get_user_model()  # noqa
 
 
 def get_el_by_pk(
     request: HttpRequest,
     type_: str,
     pk: int,
-    year: Optional[int] = None,
-    week: Optional[int] = None,
-    regular: Optional[str] = None,
     prefetch: bool = False,
     *args,
     **kwargs,
 ):
     if type_ == TimetableType.GROUP.value:
         return get_object_or_404(
             Group.objects.prefetch_related("owners", "parent_groups") if prefetch else Group,
@@ -92,46 +89,52 @@
         teachers = teachers.filter(Q(pk=user.person.pk) | Q(pk__in=wanted_teachers))
 
     teachers = teachers.distinct()
 
     return teachers
 
 
-def get_classes(user: "User"):
-    """Get the classes whose timetables are allowed to be seen by current user."""
+def get_groups(user: "User"):
+    """Get the groups whose timetables are allowed to be seen by current user."""
     checker = ObjectPermissionChecker(user)
 
-    classes = (
+    groups = (
         Group.objects.for_current_school_term_or_all()
         .annotate(
             lessons_count=Count("lesson_events"),
             child_lessons_count=Count("child_groups__lesson_events"),
         )
         .filter(Q(lessons_count__gt=0) | Q(child_lessons_count__gt=0))
-        .order_by("short_name", "name")
     )
 
+    group_types = get_site_preferences()["chronos__group_types_timetables"]
+
+    if group_types:
+        groups = groups.filter(group_type__in=group_types)
+
+    groups = groups.order_by("short_name", "name")
+
     if not check_global_permission(user, "chronos.view_all_group_timetables"):
-        checker.prefetch_perms(classes)
+        checker.prefetch_perms(groups)
 
         wanted_classes = set()
 
-        for _class in classes:
+        for _class in groups:
             if checker.has_perm("core.view_group_timetable", _class):
                 wanted_classes.add(_class.pk)
 
-        classes = classes.filter(
+        groups = groups.filter(
             Q(pk__in=wanted_classes) | Q(members=user.person) | Q(owners=user.person)
         )
         if user.person.primary_group:
-            classes = classes.filter(Q(pk=user.person.primary_group.pk))
+            groups = groups.filter(Q(pk=user.person.primary_group.pk))
 
-    classes = classes.distinct()
+    groups = groups.distinct()
 
-    return classes
+    return groups
 
 
 def get_rooms(user: "User"):
     """Get the rooms whose timetables are allowed to be seen by current user."""
     checker = ObjectPermissionChecker(user)
 
     rooms = (
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/date.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/date.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/notifications.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/util/predicates.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/util/predicates.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.db.models import Model
 
 from rules import predicate
 
 from aleksis.core.models import Group, Person, Room
 from aleksis.core.util.predicates import has_global_perm, has_object_perm
 
-from .chronos_helpers import get_classes, get_rooms, get_teachers
+from .chronos_helpers import get_groups, get_rooms, get_teachers
 
 
 @predicate
 def has_timetable_perm(user: User, obj: Model) -> bool:
     """
     Check if can access timetable.
 
@@ -71,8 +71,8 @@
         "core.view_room_timetable"
     )(user, obj)
 
 
 @predicate
 def has_any_timetable_object(user: User) -> bool:
     """Predicate which checks whether there are any timetables the user is allowed to access."""
-    return get_classes(user).exists() or get_rooms(user).exists() or get_teachers(user).exists()
+    return get_groups(user).exists() or get_rooms(user).exists() or get_teachers(user).exists()
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/aleksis/apps/chronos/views.py` & `aleksis_app_chronos-4.0.0.dev4/aleksis/apps/chronos/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/Makefile` & `aleksis_app_chronos-4.0.0.dev4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/all_timetables.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/all_timetables.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/class_timetable.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/class_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/daily_lessons.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/daily_lessons.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/my_timetable.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/my_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/print_timetable.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/print_timetable.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/substitution_edit.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/substitution_edit.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/substitutions.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/substitutions.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/_static/substitutions_print.png` & `aleksis_app_chronos-4.0.0.dev4/docs/_static/substitutions_print.png`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/admin/11_notifications.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/admin/11_notifications.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/admin/40_preferences.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/admin/40_preferences.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/conf.py` & `aleksis_app_chronos-4.0.0.dev4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/index.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/make.bat` & `aleksis_app_chronos-4.0.0.dev4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/user/01_using_timetables.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/user/01_using_timetables.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/user/10_substitution_plan.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/user/10_substitution_plan.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/user/11_notifications.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/user/11_notifications.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/docs/user/15_manage_substitutions.rst` & `aleksis_app_chronos-4.0.0.dev4/docs/user/15_manage_substitutions.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/pyproject.toml` & `aleksis_app_chronos-4.0.0.dev4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Chronos"
-version = "4.0.0.dev3"
+version = "4.0.0.dev4"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
```

### Comparing `aleksis_app_chronos-4.0.0.dev3/tox.ini` & `aleksis_app_chronos-4.0.0.dev4/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_chronos-4.0.0.dev3/PKG-INFO` & `aleksis_app_chronos-4.0.0.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlekSIS-App-Chronos
-Version: 4.0.0.dev3
+Version: 4.0.0.dev4
 Summary: AlekSIS (School Information System) — App Χρόνος (digital timetables)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,timetable,plans
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
```

