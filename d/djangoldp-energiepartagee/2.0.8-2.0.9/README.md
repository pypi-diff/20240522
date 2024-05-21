# Comparing `tmp/djangoldp_energiepartagee-2.0.8.tar.gz` & `tmp/djangoldp_energiepartagee-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_energiepartagee-2.0.8.tar", last modified: Wed May  1 18:09:23 2024, max compression
+gzip compressed data, was "dist/djangoldp_energiepartagee-2.0.9.tar", last modified: Fri May  3 08:38:35 2024, max compression
```

## Comparing `djangoldp_energiepartagee-2.0.8.tar` & `djangoldp_energiepartagee-2.0.9.tar`

### file list

```diff
@@ -1,235 +1,237 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2608 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2608 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    12893 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/
--rw-rw-rw-   0 root         (0) root         (0)    51152 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10086 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2232 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/oidc_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     3630 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/actor_update.html
--rw-rw-rw-   0 root         (0) root         (0)     2455 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/new_join_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3839 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
--rw-rw-rw-   0 root         (0) root         (0)     2615 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html
--rw-rw-rw-   0 root         (0) root         (0)     3196 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
--rw-rw-rw-   0 root         (0) root         (0)      277 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/waiting_reminder.txt
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/new_join_request.txt
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/join_actor_denied.txt
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/join_actor_validated.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/oidc_provider/authorize.html
--rw-rw-rw-   0 root         (0) root         (0)     1161 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/registration_complete.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/pdf/
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html
--rw-rw-rw-   0 root         (0) root         (0)     7355 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/pdf/contribution_call.html
--rw-rw-rw-   0 root         (0) root         (0)     2711 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-01 18:09:20.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/related_actor_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/contribution_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     4344 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/registration.css
--rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/css_ep.css
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/css_amorce.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   224744 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2
--rw-rw-rw-   0 root         (0) root         (0)   240240 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    12656 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/img/Amorcelogo.svg
--rw-rw-rw-   0 root         (0) root         (0)     4916 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/img/EPlogo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/
--rw-rw-rw-   0 root         (0) root         (0)    18245 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/export_contributions_all.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_call.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/generate_pdf_receipt.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/plain_text_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_reminder.py
--rw-rw-rw-   0 root         (0) root         (0)    18367 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/export_contributions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/utils/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/utils/render_to_pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     5917 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/waiting_members_action.py
--rw-rw-rw-   0 root         (0) root         (0)    12008 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions.py
--rw-rw-rw-   0 root         (0) root         (0)     3051 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_ventilation.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_actor_update.py
--rw-rw-rw-   0 root         (0) root         (0)     2361 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/generate_pdf_call.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_related_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_contribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1233 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_regional_admin.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/auth/
--rw-rw-rw-   0 root         (0) root         (0)     1810 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/auth/backends.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      903 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0065_auto_20220302_1533.py
--rw-rw-rw-   0 root         (0) root         (0)      724 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0039_auto_20210216_1732.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
--rw-rw-rw-   0 root         (0) root         (0)     5894 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py
--rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0093_citizenproject_fundraising_url.py
--rw-rw-rw-   0 root         (0) root         (0)    19750 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      510 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0043_auto_20210219_1412.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0092_alter_region_admins.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py
--rw-rw-rw-   0 root         (0) root         (0)    10724 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0068_contribution_discount.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
--rw-rw-rw-   0 root         (0) root         (0)     4527 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py
--rw-rw-rw-   0 root         (0) root         (0)      740 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0073_relatedactor_reminderdate.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0084_citizenproject_postcode.py
--rw-rw-rw-   0 root         (0) root         (0)     2177 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0096_remove_earneddistinction_production_sites_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
--rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0051_auto_20210323_1356.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0077_alter_discount_options.py
--rw-rw-rw-   0 root         (0) root         (0)     5837 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0003_profile_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py
--rw-rw-rw-   0 root         (0) root         (0)     1518 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1392 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0090_region_admins.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0044_auto_20210219_1415.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0057_actor_visible.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0041_regionalnetwork_nationale.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0049_actor_updatedate.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0017_actor_iban.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py
--rw-rw-rw-   0 root         (0) root         (0)      746 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py
--rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py
--rw-rw-rw-   0 root         (0) root         (0)    54205 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      597 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py
--rw-rw-rw-   0 root         (0) root         (0)    11607 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0075_alter_actor_visible.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0069_region_acronym.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0046_auto_20210223_1052.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0091_merge_0090_productionsite_postcode_0090_region_admins.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0094_remove_energybuyer_contract_type_and_more.py
--rw-rw-rw-   0 root         (0) root         (0)     2185 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0095_rename_type_contracttype_name.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 18:09:23.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/
--rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/communication_profile.py
--rw-rw-rw-   0 root         (0) root         (0)    10065 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/actor.py
--rw-rw-rw-   0 root         (0) root         (0)     7080 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/contribution.py
--rw-rw-rw-   0 root         (0) root         (0)     4965 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/production_site.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/college.py
--rw-rw-rw-   0 root         (0) root         (0)     2993 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/capital_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/production_site_distinction.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/region.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_buyer_type.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/college_epa.py
--rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/regional_network.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_production.py
--rw-rw-rw-   0 root         (0) root         (0)     5092 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/citizen_project.py
--rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/testimony.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/intervention_zone.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/citizen_project_distinction.py
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_buyer.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/shareholder.py
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/legal_structure.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner_type.py
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/related_actor.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner_link.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1120 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_type.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/payment_method.py
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/discount.py
--rw-rw-rw-   0 root         (0) root         (0)     6891 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/integration_step.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-01 18:09:01.000000 djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/context_processors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2608 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    13075 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    51152 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10086 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2232 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/oidc_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     3630 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/actor_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/new_join_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3839 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
+-rw-rw-rw-   0 root         (0) root         (0)     2615 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html
+-rw-rw-rw-   0 root         (0) root         (0)     3196 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
+-rw-rw-rw-   0 root         (0) root         (0)      277 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/waiting_reminder.txt
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/new_join_request.txt
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/join_actor_denied.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/join_actor_validated.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/oidc_provider/authorize.html
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2662 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/registration_complete.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html
+-rw-rw-rw-   0 root         (0) root         (0)     7355 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/pdf/contribution_call.html
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2074 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-03 08:38:33.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/related_actor_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/contribution_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/registration.css
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/css_ep.css
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/css_amorce.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   224744 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   240240 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    12656 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/img/Amorcelogo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4916 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/img/EPlogo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/
+-rw-rw-rw-   0 root         (0) root         (0)    18245 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/export_contributions_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_call.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/generate_pdf_receipt.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/plain_text_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_reminder.py
+-rw-rw-rw-   0 root         (0) root         (0)    18367 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/export_contributions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/utils/render_to_pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5917 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/waiting_members_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    12008 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_ventilation.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_actor_update.py
+-rw-rw-rw-   0 root         (0) root         (0)     2361 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/generate_pdf_call.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_related_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_contribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1233 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_regional_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/auth/
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/auth/backends.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      903 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
+-rw-rw-rw-   0 root         (0) root         (0)      498 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0065_auto_20220302_1533.py
+-rw-rw-rw-   0 root         (0) root         (0)      724 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0039_auto_20210216_1732.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py
+-rw-rw-rw-   0 root         (0) root         (0)      484 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0093_citizenproject_fundraising_url.py
+-rw-rw-rw-   0 root         (0) root         (0)    19750 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      510 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0043_auto_20210219_1412.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0092_alter_region_admins.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py
+-rw-rw-rw-   0 root         (0) root         (0)    10724 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0068_contribution_discount.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0073_relatedactor_reminderdate.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0084_citizenproject_postcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2177 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0096_remove_earneddistinction_production_sites_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
+-rw-rw-rw-   0 root         (0) root         (0)      560 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0051_auto_20210323_1356.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0097_alter_earneddistinction_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0077_alter_discount_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     5837 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0003_profile_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0098_alter_energyproduction_installed_capacity_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0090_region_admins.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0044_auto_20210219_1415.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0057_actor_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0041_regionalnetwork_nationale.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0049_actor_updatedate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0017_actor_iban.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py
+-rw-rw-rw-   0 root         (0) root         (0)    54205 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py
+-rw-rw-rw-   0 root         (0) root         (0)    11607 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0075_alter_actor_visible.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0069_region_acronym.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0046_auto_20210223_1052.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0091_merge_0090_productionsite_postcode_0090_region_admins.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0094_remove_energybuyer_contract_type_and_more.py
+-rw-rw-rw-   0 root         (0) root         (0)     2185 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0095_rename_type_contracttype_name.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:38:35.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/communication_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)    10065 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7080 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/contribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     4965 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/production_site.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/college.py
+-rw-rw-rw-   0 root         (0) root         (0)     2993 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/capital_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/production_site_distinction.py
+-rw-rw-rw-   0 root         (0) root         (0)      851 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/region.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_buyer_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/college_epa.py
+-rw-rw-rw-   0 root         (0) root         (0)     3642 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/regional_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     3617 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_production.py
+-rw-rw-rw-   0 root         (0) root         (0)     5092 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/citizen_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     1166 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/testimony.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/intervention_zone.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/citizen_project_distinction.py
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_buyer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/shareholder.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/legal_structure.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/related_actor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1650 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/payment_method.py
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/discount.py
+-rw-rw-rw-   0 root         (0) root         (0)     6891 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/integration_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-05-03 08:38:15.000000 djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/context_processors.py
```

### Comparing `djangoldp_energiepartagee-2.0.8/README.md` & `djangoldp_energiepartagee-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/setup.cfg` & `djangoldp_energiepartagee-2.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/PKG-INFO` & `djangoldp_energiepartagee-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp_energiepartagee
-Version: 2.0.8
+Version: 2.0.9
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/PKG-INFO` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp-energiepartagee
-Version: 2.0.8
+Version: 2.0.9
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee.egg-info/SOURCES.txt` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,16 @@
 djangoldp_energiepartagee/migrations/0090_region_admins.py
 djangoldp_energiepartagee/migrations/0091_merge_0090_productionsite_postcode_0090_region_admins.py
 djangoldp_energiepartagee/migrations/0092_alter_region_admins.py
 djangoldp_energiepartagee/migrations/0093_citizenproject_fundraising_url.py
 djangoldp_energiepartagee/migrations/0094_remove_energybuyer_contract_type_and_more.py
 djangoldp_energiepartagee/migrations/0095_rename_type_contracttype_name.py
 djangoldp_energiepartagee/migrations/0096_remove_earneddistinction_production_sites_and_more.py
+djangoldp_energiepartagee/migrations/0097_alter_earneddistinction_options_and_more.py
+djangoldp_energiepartagee/migrations/0098_alter_energyproduction_installed_capacity_and_more.py
 djangoldp_energiepartagee/migrations/__init__.py
 djangoldp_energiepartagee/models/__init__.py
 djangoldp_energiepartagee/models/actor.py
 djangoldp_energiepartagee/models/capital_distribution.py
 djangoldp_energiepartagee/models/citizen_project.py
 djangoldp_energiepartagee/models/citizen_project_distinction.py
 djangoldp_energiepartagee/models/college.py
```

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/tests_permissions.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/tests_post.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/tests/runner.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/oidc_settings.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/oidc_settings.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/password_reset_form.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/registration/login.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/waiting_reminder.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/actor_update.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/actor_update.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/new_join_request.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/new_join_request.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_call.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/join_actor_validated.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/html/join_actor_denied.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/actor_update.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/oidc_provider/authorize.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/base.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/activation_complete.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/django_registration/registration_form.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/pdf/contribution_receipt.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/templates/pdf/contribution_call.html` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/templates/pdf/contribution_call.html`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/admin.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/djangoldp_urls.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/related_actor_filter_backend.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/related_actor_filter_backend.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/filters/contribution_filter_backend.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/filters/contribution_filter_backend.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/registration.css` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/registration.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/css_ep.css` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/css_ep.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/css/css_amorce.css` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/css/css_amorce.css`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/fonts/Inter-roman.var.woff2`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/fonts/Inter-italic.var.woff2`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/img/Amorcelogo.svg` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/img/Amorcelogo.svg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/static/img/EPlogo.svg` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/static/img/EPlogo.svg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/export_contributions_all.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/export_contributions_all.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_call.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_call.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/generate_pdf_receipt.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/generate_pdf_receipt.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_reminder.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_reminder.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/export_contributions.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/export_contributions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/utils/render_to_pdf.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/utils/render_to_pdf.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/waiting_members_action.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/waiting_members_action.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_ventilation.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_ventilation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/contributions_actor_update.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/contributions_actor_update.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/views/generate_pdf_call.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/views/generate_pdf_call.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_related_actor.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_related_actor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_contribution.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_contribution.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_actor.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_actor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/permissions/ep_regional_admin.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/permissions/ep_regional_admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/auth/backends.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/auth/backends.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0045_auto_20210222_2353.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0082_alter_capitaldistribution_actor_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0055_auto_20210421_1500.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0001_initial.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0076_alter_actor_options_alter_college_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0092_alter_region_admins.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0092_alter_region_admins.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0050_contribution_usercontact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0081_alter_citizenproject_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0068_contribution_discount.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0068_contribution_discount.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0072_alter_relatedactor_role.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0086_alter_productionsite_total_development_budget_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0088_alter_energyproduction_consumption_equivalence_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0087_alter_productionsite_progress_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0070_contribution_updatereminderdate_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0058_auto_20211108_1909.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0059_auto_20220114_1050.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0090_productionsite_postcode.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0096_remove_earneddistinction_production_sites_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0096_remove_earneddistinction_production_sites_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0048_auto_20210225_1136.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0085_citizenproject_wp_project_url_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0071_relatedactor_createdate.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0062_auto_20220128_1047.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0052_auto_20210323_1424.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0003_profile_user.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0003_profile_user.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0053_auto_20210402_1014.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0040_auto_20210216_2227.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0061_auto_20220114_1140.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0089_rename_effective_commissionning_yearl_productionsite_effective_commissionning_year_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0060_auto_20220114_1113.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0080_alter_citizenproject_status.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0090_region_admins.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0090_region_admins.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0067_discount_actor_villageoise.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0035_auto_20210215_1329.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0047_auto_20210223_1059.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0038_auto_20210216_1721.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0063_auto_20220128_1051.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0078_citizen_project_communication_profile_contract_type_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0066_alter_actor_options_alter_college_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0036_auto_20210216_1714.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0056_auto_20210430_1127.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0079_rename_capital_distribution_capitaldistribution_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0037_auto_20210216_1717.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0083_alter_actor_options_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0064_auto_20220203_1721.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0074_alter_relatedactor_role.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0042_auto_20210219_1409.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0094_remove_energybuyer_contract_type_and_more.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0094_remove_energybuyer_contract_type_and_more.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/migrations/0054_auto_20210419_2106.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/communication_profile.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/communication_profile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/actor.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/actor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/contribution.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/contribution.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/production_site.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/production_site.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/college.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/college.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/capital_distribution.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/capital_distribution.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/production_site_distinction.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/production_site_distinction.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/__init__.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/__init__.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/region.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/region.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_buyer_type.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_buyer_type.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/college_epa.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/college_epa.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/regional_network.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/regional_network.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_production.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_production.py`

 * *Files 26% similar despite different names*

```diff
@@ -47,45 +47,64 @@
     )
     reference_unit = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Unité de référence"
     )
     estimated_capacity = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Puissance estimée"
     )
-    installed_capacity = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Puissance installée"
+    installed_capacity = models.IntegerField(
+        blank=True, null=True, verbose_name="Puissance installée"
     )
     consumption_equivalence = models.CharField(
         max_length=50,
         blank=True,
         null=True,
         verbose_name="Equivalence en nombre de foyers",
     )
-    yearly_production = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Production annuelle"
-    )
-    estimated_yearly_production = models.CharField(
-        max_length=50, blank=True, null=True, verbose_name="Production annuelle estimée"
+    yearly_production = models.IntegerField(
+        blank=True, null=True, verbose_name="Production annuelle"
     )
     technology_used = models.CharField(
         max_length=50, blank=True, null=True, verbose_name="Technologie utilisée"
     )
     estimated_injection_capacity = models.CharField(
         max_length=50,
         blank=True,
         null=True,
         verbose_name="Capacité d'injection estimée",
     )
 
+    @property
+    def estimated_yearly_production(self):
+        if self.yearly_production and self.installed_capacity:
+            return self.installed_capacity / self.yearly_production
+        else:
+            return 0
+
     class Meta(Model.Meta):
         ordering = ["pk"]
         permission_classes = [InheritPermissions]
         inherit_permissions = ["production_site"]
         rdf_type = "energiepartagee:energy_production"
         verbose_name = _("Énergie produite")
         verbose_name_plural = _("Énergies produites")
+        serializer_fields = [
+            "energy_buyer",
+            "contract_type",
+            "energy_type",
+            "energy_contract",
+            "reference_unit",
+            "estimated_capacity",
+            "installed_capacity",
+            "consumption_equivalence",
+            "yearly_production",
+            "technology_used",
+            "estimated_injection_capacity",
+            "estimated_yearly_production"
+        ]
+        depth = 1
 
     def __str__(self):
         if self.production_site.name:
             return self.production_site.name
         else:
             return self.urlid
```

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/citizen_project.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/citizen_project.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/testimony.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/testimony.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/intervention_zone.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/intervention_zone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/citizen_project_distinction.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/citizen_project_distinction.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_buyer.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_buyer.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/shareholder.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/shareholder.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/legal_structure.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/legal_structure.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner_type.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner_type.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/related_actor.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/related_actor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner_link.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner_link.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/profile.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/profile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/partner.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/partner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/energy_type.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/energy_type.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/payment_method.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/discount.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/discount.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/signals.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/signals.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-2.0.8/djangoldp_energiepartagee/models/integration_step.py` & `djangoldp_energiepartagee-2.0.9/djangoldp_energiepartagee/models/integration_step.py`

 * *Files identical despite different names*

