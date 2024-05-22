# Comparing `tmp/aa_ledger-0.3.8.tar.gz` & `tmp/aa_ledger-0.3.8a1.tar.gz`

## Comparing `aa_ledger-0.3.8.tar` & `aa_ledger-0.3.8a1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/__init__.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/admin.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/app_settings.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/apps.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/auth_hooks.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/decorators.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/errors.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/hooks.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/providers.py
--rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/tasks.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/urls.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/__init__.py
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/helpers.py
--rw-r--r--   0        0        0    21348 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/ledgermanager.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/schema.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/templatemanager.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/character/__init__.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/character/ledger.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/character/template.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/corporation/__init__.py
--rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/corporation/ledger.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/api/corporation/template.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/managers/charaudit_manager.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/managers/corpaudit_manager.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/managers/general_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/migrations/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/models/__init__.py
--rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/models/characteraudit.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/models/corporationaudit.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/models/events.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/models/general.py
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/css/billboards_dark.css
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/css/cards.css
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/css/custom.css
--rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-1.png
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-2.png
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-3.png
--rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/js/charledger.js
--rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/js/corpledger.js
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/static/ledger/js/img.js
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/task_helpers/__init__.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/task_helpers/char_helpers.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/task_helpers/core_helpers.py
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/task_helpers/corp_helpers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/task_helpers/etag_helpers.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/base.html
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/error.html
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/bundles/ledger-css.html
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/base.html
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/index.html
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/menu.html
--rw-r--r--   0        0        0     3305 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/char_ledger.html
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/month.html
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/year.html
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/month.html
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/year.html
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/modals/modal-full.html
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/modals/modal-xl.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/modals/modal.html
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/modals/modal_dialog.html
--rw-r--r--   0        0        0    17968 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templates/ledger/modals/pve/view_character_content.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templatetags/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/templatetags/ledger.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/view_helpers/__init__.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/view_helpers/core.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/__init__.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/pve.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/character/char_audit.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/corporation/corp_audit.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/corporation/corp_events.py
--rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/ledger/views/corporation/corp_tax.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/LICENSE
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/README.md
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     8312 2020-02-02 00:00:00.000000 aa_ledger-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/__init__.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/admin.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/app_settings.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/apps.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/auth_hooks.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/decorators.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/errors.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/hooks.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/providers.py
+-rw-r--r--   0        0        0     4956 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/tasks.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/urls.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/__init__.py
+-rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/helpers.py
+-rw-r--r--   0        0        0    21348 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/ledgermanager.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/schema.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/templatemanager.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/__init__.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/ledger.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/character/template.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/__init__.py
+-rw-r--r--   0        0        0     3953 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/ledger.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/api/corporation/template.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/charaudit_manager.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/corpaudit_manager.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/managers/general_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/migrations/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/__init__.py
+-rw-r--r--   0        0        0     5771 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/characteraudit.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/corporationaudit.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/events.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/models/general.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/billboards_dark.css
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/cards.css
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/css/custom.css
+-rw-r--r--   0        0        0   236145 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-1.png
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-2.png
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-3.png
+-rw-r--r--   0        0        0    43262 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0    22096 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/charledger.js
+-rw-r--r--   0        0        0    18853 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/corpledger.js
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/static/ledger/js/img.js
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/__init__.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/char_helpers.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/core_helpers.py
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/corp_helpers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/task_helpers/etag_helpers.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/base.html
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/error.html
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/bundles/ledger-css.html
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/base.html
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/index.html
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/menu.html
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/char_ledger.html
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/month.html
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/year.html
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/corp_ledger.html
+-rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/month.html
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/year.html
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-full.html
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-xl.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal.html
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal_dialog.html
+-rw-r--r--   0        0        0    17677 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templates/ledger/modals/pve/view_character_content.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templatetags/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/templatetags/ledger.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/view_helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/view_helpers/core.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/__init__.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/pve.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/character/char_audit.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_audit.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_events.py
+-rw-r--r--   0        0        0     8919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/ledger/views/corporation/corp_tax.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/LICENSE
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/README.md
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/pyproject.toml
+-rw-r--r--   0        0        0     8314 2020-02-02 00:00:00.000000 aa_ledger-0.3.8a1/PKG-INFO
```

### Comparing `aa_ledger-0.3.8/ledger/admin.py` & `aa_ledger-0.3.8a1/ledger/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/app_settings.py` & `aa_ledger-0.3.8a1/ledger/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/auth_hooks.py` & `aa_ledger-0.3.8a1/ledger/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/decorators.py` & `aa_ledger-0.3.8a1/ledger/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/hooks.py` & `aa_ledger-0.3.8a1/ledger/hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/tasks.py` & `aa_ledger-0.3.8a1/ledger/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/urls.py` & `aa_ledger-0.3.8a1/ledger/urls.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/__init__.py` & `aa_ledger-0.3.8a1/ledger/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/helpers.py` & `aa_ledger-0.3.8a1/ledger/api/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/ledgermanager.py` & `aa_ledger-0.3.8a1/ledger/api/ledgermanager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/schema.py` & `aa_ledger-0.3.8a1/ledger/api/schema.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/templatemanager.py` & `aa_ledger-0.3.8a1/ledger/api/templatemanager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/character/ledger.py` & `aa_ledger-0.3.8a1/ledger/api/character/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/character/template.py` & `aa_ledger-0.3.8a1/ledger/api/character/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/corporation/ledger.py` & `aa_ledger-0.3.8a1/ledger/api/corporation/ledger.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/api/corporation/template.py` & `aa_ledger-0.3.8a1/ledger/api/corporation/template.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/managers/charaudit_manager.py` & `aa_ledger-0.3.8a1/ledger/managers/charaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/managers/corpaudit_manager.py` & `aa_ledger-0.3.8a1/ledger/managers/corpaudit_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/managers/general_manager.py` & `aa_ledger-0.3.8a1/ledger/managers/general_manager.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/models/characteraudit.py` & `aa_ledger-0.3.8a1/ledger/models/characteraudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/models/corporationaudit.py` & `aa_ledger-0.3.8a1/ledger/models/corporationaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/models/events.py` & `aa_ledger-0.3.8a1/ledger/models/events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/models/general.py` & `aa_ledger-0.3.8a1/ledger/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/css/billboards_dark.css` & `aa_ledger-0.3.8a1/ledger/static/ledger/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/css/cards.css` & `aa_ledger-0.3.8a1/ledger/static/ledger/css/cards.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/css/custom.css` & `aa_ledger-0.3.8a1/ledger/static/ledger/css/custom.css`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-1.png` & `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-1.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-2.png` & `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-2.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/guides/ledger-3.png` & `aa_ledger-0.3.8a1/ledger/static/ledger/guides/ledger-3.png`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/images/Spinner-1s-64px-dark.gif` & `aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/images/Spinner-1s-64px-light.gif` & `aa_ledger-0.3.8a1/ledger/static/ledger/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/js/charledger.js` & `aa_ledger-0.3.8a1/ledger/static/ledger/js/charledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/js/corpledger.js` & `aa_ledger-0.3.8a1/ledger/static/ledger/js/corpledger.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/static/ledger/js/img.js` & `aa_ledger-0.3.8a1/ledger/static/ledger/js/img.js`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/task_helpers/char_helpers.py` & `aa_ledger-0.3.8a1/ledger/task_helpers/char_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/task_helpers/core_helpers.py` & `aa_ledger-0.3.8a1/ledger/task_helpers/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/task_helpers/corp_helpers.py` & `aa_ledger-0.3.8a1/ledger/task_helpers/corp_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/task_helpers/etag_helpers.py` & `aa_ledger-0.3.8a1/ledger/task_helpers/etag_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/base.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/base.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-{% extends 'allianceauth/base-bs5.html' %}
-{% load i18n %}
-{% load ledger %}
-{% block main_css %}
-{% endblock main_css %}
-{% block extra_css %}
-{% endblock extra_css %}
-
-{% block page_title %}Ledger{% endblock %}
-
-{% block header_nav_brand %}
-    Ledger
-{% endblock header_nav_brand %}
-
-{% block header_nav_collapse_left %}
-
-{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
-
-{% endblock header_nav_collapse_left %}
-
-{% block content %}
-
-{% include 'ledger/bundles/ledger-css.html' %}
-{% include 'bundles/datatables-css-bs5.html' %}
-
-<div class="allianceauth-ledger-plugin card">
-    {% block page_topic %}<h1 class="page-header text-center">Ledger</h1>{% endblock page_topic %}
-    <br>
-    <div class="container-fluid" id="vow_block">
-    {% block vow_block %}{% endblock %}
-    </div>
-    <br>
-</div>
-
-{% endblock %}
-
-{% block extra_javascript %}
-{% endblock %}
-
-{% block extra_script %}
-{% endblock %}
+{% extends 'allianceauth/base-bs5.html' %}
+{% load i18n %}
+{% load ledger %}
+{% block main_css %}
+{% endblock main_css %}
+{% block extra_css %}
+{% endblock extra_css %}
+
+{% block page_title %}Ledger{% endblock %}
+
+{% block header_nav_brand %}
+    Ledger
+{% endblock header_nav_brand %}
+
+{% block header_nav_collapse_left %}
+
+{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
+
+{% endblock header_nav_collapse_left %}
+
+{% block content %}
+
+{% include 'ledger/bundles/ledger-css.html' %}
+{% include 'bundles/datatables-css-bs5.html' %}
+
+<div class="allianceauth-ledger-plugin card">
+    {% block page_topic %}<h1 class="page-header text-center">Ledger</h1>{% endblock page_topic %}
+    <br>
+    <div class="container-fluid" id="vow_block">
+    {% block vow_block %}{% endblock %}
+    </div>
+    <br>
+</div>
+
+{% endblock %}
+
+{% block extra_javascript %}
+{% endblock %}
+
+{% block extra_script %}
+{% endblock %}
```

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/error.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/error.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/base.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/base.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-{% extends 'allianceauth/base-bs5.html' %}
-{% load i18n %}
-{% load ledger %}
-{% block main_css %}
-{% endblock main_css %}
-{% block extra_css %}
-{% endblock extra_css %}
-
-{% block page_title %}Ledger{% endblock %}
-
-{% block header_nav_brand %}
-    Ledger
-{% endblock header_nav_brand %}
-
-{% block header_nav_collapse_left %}
-
-{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
-
-{% endblock header_nav_collapse_left %}
-
-{% block content %}
-
-{% include 'ledger/bundles/ledger-css.html' %}
-{% include 'bundles/datatables-css-bs5.html' %}
-
-<div class="allianceauth-ledger-plugin card">
-    {% block page_topic %}<h1 class="page-header text-center">Ledger</h1>{% endblock page_topic %}
-    <br>
-    <div class="container-fluid" id="vow_block">
-    {% block vow_block %}{% endblock %}
-    </div>
-    <br>
-</div>
-
-{% endblock %}
-
-{% block extra_javascript %}
-{% endblock %}
-
-{% block extra_script %}
-{% endblock %}
+{% extends 'allianceauth/base-bs5.html' %}
+{% load i18n %}
+{% load ledger %}
+{% block main_css %}
+{% endblock main_css %}
+{% block extra_css %}
+{% endblock extra_css %}
+
+{% block page_title %}Ledger{% endblock %}
+
+{% block header_nav_brand %}
+    Ledger
+{% endblock header_nav_brand %}
+
+{% block header_nav_collapse_left %}
+
+{% block vow_menu %}{% include 'ledger/ledger/menu.html' %}{% endblock %}
+
+{% endblock header_nav_collapse_left %}
+
+{% block content %}
+
+{% include 'ledger/bundles/ledger-css.html' %}
+{% include 'bundles/datatables-css-bs5.html' %}
+
+<div class="allianceauth-ledger-plugin card">
+    {% block page_topic %}<h1 class="page-header text-center">Ledger</h1>{% endblock page_topic %}
+    <br>
+    <div class="container-fluid" id="vow_block">
+    {% block vow_block %}{% endblock %}
+    </div>
+    <br>
+</div>
+
+{% endblock %}
+
+{% block extra_javascript %}
+{% endblock %}
+
+{% block extra_script %}
+{% endblock %}
```

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/index.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/index.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/menu.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/menu.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/char_ledger.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/char_ledger.html`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-{% extends 'ledger/ledger/base.html' %}
-{% load i18n %}
-{% load humanize %}
-{% load static %}
-{% load ledger %}
-
-{% block page_title %}Character Ledger{% endblock %}
-{% block page_topic %}<h1 class="page-header text-center">{% translate "Character Ledger" %}</h1>{% endblock page_topic %}
-
-{% block vow_block %}
-<div class="container-fluid">
-    <div class="rounded-top" style="--bs-bg-opacity: .5;">
-        <ul class="nav nav-tabs rounded-top bg-primary" id="ledger-ratting" role="tablist">
-            <li class="nav-item">
-                <a id="currentMonthLink" class="nav-link active" href="#tab-current_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-current_month">
-                    Month - {% now "F" %}
-                </a>
-            </li>
-            <li class="nav-item">
-                <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
-                    Year - {% now "Y" %}
-                </a>
-            </li>
-        </ul>
-        <div class="tab-content rounded-bottom">
-            <div class="tab-content">
-                {% include 'ledger/ledger/charledger/month.html' %}
-                {% include 'ledger/ledger/charledger/year.html' %}
-            </div>
-        </div>
-    </div>
-</div>
-
-<!-- Tab Session -->
-{% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
-{% endblock %}
-{% block extra_css %}
-<style>
-@media all {
-    #ratting th, #ratting_year th,
-    #ratting td, #ratting_year td {
-        padding: 0.75rem;
-        vertical-align: top;
-        border-top: 1px solid #dee2e6;
-    }
-
-    #ratting thead th, #ratting_year thead th {
-        vertical-align: bottom;
-        border-bottom: 2px solid #dee2e6;
-    }
-
-    #ratting tbody td:nth-child(5), #ratting_year tbody td:nth-child(5) {
-        text-align: right;
-    }
-
-    #ratting tfoot th:nth-child(5), #ratting_year tfoot th:nth-child(5) {
-        text-align: right;
-    }
-
-    #ratting tr, #ratting_year tr {
-        border-bottom: 1px solid #dee2e6;
-    }
-
-}
-</style>
-{% endblock %}
-{% block extra_javascript %}
-<link rel="stylesheet" type="text/css" href="{% static 'ledger/css/billboards_dark.css' %}">
-<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js" integrity="sha512-vc58qvvBdrDR4etbxMdlTt4GBQk1qjvyORR2nrsPsFPyrs+/u5c3+1Ct6upOgdZoIl7eq6k3a1UPDSNAQi/32A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/billboard.js/3.11.3/billboard.min.js" integrity="sha512-rW9pOtBGPL12EGH9SeJmQWtVRvMImYHFGcYmTG/f9UIEO8I/nl2BxUQ41+t0ieqRdTF3PawVUVBXC7Jnb3AGnA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-{% include 'bundles/datatables-js-bs5.html' %}
-<script type="application/javascript">
-    $('#modalViewCharacterContainer').on('show.bs.modal', function (event) {
-        let button = $(event.relatedTarget)
-        let ajax_url = button.data('ajax_url');
-
-        $("#modalViewCharacterContent").load(ajax_url)
-    });
-</script>
-<script type="text/javascript" src="{% static 'ledger/js/charledger.js' %}"></script>
-{% endblock extra_javascript %}
-{% block extra_script %}
-{% endblock extra_script %}
+{% extends 'ledger/ledger/base.html' %}
+{% load i18n %}
+{% load humanize %}
+{% load static %}
+{% load ledger %}
+
+{% block page_title %}Character Ledger{% endblock %}
+{% block page_topic %}<h1 class="page-header text-center">{% translate "Character Ledger" %}</h1>{% endblock page_topic %}
+
+{% block vow_block %}
+<div class="container-fluid">
+    <div class="rounded-top" style="--bs-bg-opacity: .5;">
+        <ul class="nav nav-tabs rounded-top bg-primary" id="ledger-ratting" role="tablist">
+            <li class="nav-item">
+                <a id="currentMonthLink" class="nav-link active" href="#tab-current_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-current_month">
+                    Month - {% now "F" %}
+                </a>
+            </li>
+            <li class="nav-item">
+                <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
+                    Year - {% now "Y" %}
+                </a>
+            </li>
+        </ul>
+        <div class="tab-content rounded-bottom">
+            <div class="tab-content">
+                {% include 'ledger/ledger/charledger/month.html' %}
+                {% include 'ledger/ledger/charledger/year.html' %}
+            </div>
+        </div>
+    </div>
+</div>
+
+<!-- Tab Session -->
+{% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
+{% endblock %}
+{% block extra_css %}
+<style>
+@media all {
+    #ratting th, #ratting_year th,
+    #ratting td, #ratting_year td {
+        padding: 0.75rem;
+        vertical-align: top;
+        border-top: 1px solid #dee2e6;
+    }
+
+    #ratting thead th, #ratting_year thead th {
+        vertical-align: bottom;
+        border-bottom: 2px solid #dee2e6;
+    }
+
+    #ratting tbody td:nth-child(5), #ratting_year tbody td:nth-child(5) {
+        text-align: right;
+    }
+
+    #ratting tfoot th:nth-child(5), #ratting_year tfoot th:nth-child(5) {
+        text-align: right;
+    }
+
+    #ratting tr, #ratting_year tr {
+        border-bottom: 1px solid #dee2e6;
+    }
+
+}
+</style>
+{% endblock %}
+{% block extra_javascript %}
+<link rel="stylesheet" type="text/css" href="{% static 'ledger/css/billboards_dark.css' %}">
+<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js" integrity="sha512-vc58qvvBdrDR4etbxMdlTt4GBQk1qjvyORR2nrsPsFPyrs+/u5c3+1Ct6upOgdZoIl7eq6k3a1UPDSNAQi/32A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/billboard.js/3.11.3/billboard.min.js" integrity="sha512-rW9pOtBGPL12EGH9SeJmQWtVRvMImYHFGcYmTG/f9UIEO8I/nl2BxUQ41+t0ieqRdTF3PawVUVBXC7Jnb3AGnA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+{% include 'bundles/datatables-js-bs5.html' %}
+<script type="application/javascript">
+    $('#modalViewCharacterContainer').on('show.bs.modal', function (event) {
+        let button = $(event.relatedTarget)
+        let ajax_url = button.data('ajax_url');
+
+        $("#modalViewCharacterContent").load(ajax_url)
+    });
+</script>
+<script type="text/javascript" src="{% static 'ledger/js/charledger.js' %}"></script>
+{% endblock extra_javascript %}
+{% block extra_script %}
+{% endblock extra_script %}
```

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/month.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/charledger/year.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/charledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/corp_ledger.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/corp_ledger.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-{% extends 'ledger/ledger/base.html' %}
-{% load i18n %}
-{% load humanize %}
-{% load static %}
-{% load ledger %}
-
-{% block page_title %}Corporation Ledger{% endblock %}
-{% block page_topic %}<h1 class="page-header text-center">{% translate "Corporation Ledger" %}</h1>{% endblock page_topic %}
-
-{% block vow_block %}
-<div class="container-fluid">
-    <div class="rounded-top" style="--bs-bg-opacity: .5;">
-        <ul class="nav nav-tabs rounded-top bg-primary" id="ledger-ratting" role="tablist">
-            <li class="nav-item">
-                <a id="currentMonthLink" class="nav-link active" href="#tab-current_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-current_month">
-                    Month - {% now "F" %}
-                </a>
-            </li>
-            <li class="nav-item">
-                <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
-                    Year - {% now "Y" %}
-                </a>
-            </li>
-        </ul>
-        <div class="tab-content rounded-bottom">
-            <div class="tab-content">
-                {% include 'ledger/ledger/corpledger/month.html' %}
-                {% include 'ledger/ledger/corpledger/year.html' %}
-            </div>
-        </div>
-    </div>
-</div>
-
-<!-- Tab Session -->
-{% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
-{% endblock %}
-{% block extra_css %}
-<style>
-@media all {
-    #ratting th, #ratting_year th,
-    #ratting td, #ratting_year td {
-        padding: 0.75rem;
-        vertical-align: top;
-        border-top: 1px solid #dee2e6;
-    }
-
-    #ratting thead th, #ratting_year thead th {
-        vertical-align: bottom;
-        border-bottom: 2px solid #dee2e6;
-    }
-
-    #ratting tbody td:nth-child(5), #ratting_year tbody td:nth-child(5) {
-        text-align: right;
-    }
-
-    #ratting tfoot th:nth-child(5), #ratting_year tfoot th:nth-child(5) {
-        text-align: right;
-    }
-
-    #ratting tr, #ratting_year tr {
-        border-bottom: 1px solid #dee2e6;
-    }
-
-}
-</style>
-{% endblock %}
-{% block extra_javascript %}
-<link rel="stylesheet" type="text/css" href="{% static 'ledger/css/billboards_dark.css' %}">
-<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js" integrity="sha512-vc58qvvBdrDR4etbxMdlTt4GBQk1qjvyORR2nrsPsFPyrs+/u5c3+1Ct6upOgdZoIl7eq6k3a1UPDSNAQi/32A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/billboard.js/3.11.3/billboard.min.js" integrity="sha512-rW9pOtBGPL12EGH9SeJmQWtVRvMImYHFGcYmTG/f9UIEO8I/nl2BxUQ41+t0ieqRdTF3PawVUVBXC7Jnb3AGnA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-{% include 'bundles/datatables-js-bs5.html' %}
-<script type="application/javascript">
-    $('#modalViewCharacterContainer').on('show.bs.modal', function (event) {
-        let button = $(event.relatedTarget)
-        let ajax_url = button.data('ajax_url');
-
-        $("#modalViewCharacterContent").load(ajax_url)
-    });
-</script>
-<script type="text/javascript" src="{% static 'ledger/js/corpledger.js' %}"></script>
-{% endblock extra_javascript %}
-{% block extra_script %}
-{% endblock extra_script %}
+{% extends 'ledger/ledger/base.html' %}
+{% load i18n %}
+{% load humanize %}
+{% load static %}
+{% load ledger %}
+
+{% block page_title %}Corporation Ledger{% endblock %}
+{% block page_topic %}<h1 class="page-header text-center">{% translate "Corporation Ledger" %}</h1>{% endblock page_topic %}
+
+{% block vow_block %}
+<div class="container-fluid">
+    <div class="rounded-top" style="--bs-bg-opacity: .5;">
+        <ul class="nav nav-tabs rounded-top bg-primary" id="ledger-ratting" role="tablist">
+            <li class="nav-item">
+                <a id="currentMonthLink" class="nav-link active" href="#tab-current_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-current_month">
+                    Month - {% now "F" %}
+                </a>
+            </li>
+            <li class="nav-item">
+                <a id="currentYearLink" class="nav-link" href="#tab-all_month" data-bs-toggle="tab" role="tab" data-bs-target="#tab-all_month">
+                    Year - {% now "Y" %}
+                </a>
+            </li>
+        </ul>
+        <div class="tab-content rounded-bottom">
+            <div class="tab-content">
+                {% include 'ledger/ledger/corpledger/month.html' %}
+                {% include 'ledger/ledger/corpledger/year.html' %}
+            </div>
+        </div>
+    </div>
+</div>
+
+<!-- Tab Session -->
+{% include 'ledger/modals/modal_dialog.html' with name="ViewCharacter" %}
+{% endblock %}
+{% block extra_css %}
+<style>
+@media all {
+    #ratting th, #ratting_year th,
+    #ratting td, #ratting_year td {
+        padding: 0.75rem;
+        vertical-align: top;
+        border-top: 1px solid #dee2e6;
+    }
+
+    #ratting thead th, #ratting_year thead th {
+        vertical-align: bottom;
+        border-bottom: 2px solid #dee2e6;
+    }
+
+    #ratting tbody td:nth-child(5), #ratting_year tbody td:nth-child(5) {
+        text-align: right;
+    }
+
+    #ratting tfoot th:nth-child(5), #ratting_year tfoot th:nth-child(5) {
+        text-align: right;
+    }
+
+    #ratting tr, #ratting_year tr {
+        border-bottom: 1px solid #dee2e6;
+    }
+
+}
+</style>
+{% endblock %}
+{% block extra_javascript %}
+<link rel="stylesheet" type="text/css" href="{% static 'ledger/css/billboards_dark.css' %}">
+<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/7.9.0/d3.min.js" integrity="sha512-vc58qvvBdrDR4etbxMdlTt4GBQk1qjvyORR2nrsPsFPyrs+/u5c3+1Ct6upOgdZoIl7eq6k3a1UPDSNAQi/32A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/billboard.js/3.11.3/billboard.min.js" integrity="sha512-rW9pOtBGPL12EGH9SeJmQWtVRvMImYHFGcYmTG/f9UIEO8I/nl2BxUQ41+t0ieqRdTF3PawVUVBXC7Jnb3AGnA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+{% include 'bundles/datatables-js-bs5.html' %}
+<script type="application/javascript">
+    $('#modalViewCharacterContainer').on('show.bs.modal', function (event) {
+        let button = $(event.relatedTarget)
+        let ajax_url = button.data('ajax_url');
+
+        $("#modalViewCharacterContent").load(ajax_url)
+    });
+</script>
+<script type="text/javascript" src="{% static 'ledger/js/corpledger.js' %}"></script>
+{% endblock extra_javascript %}
+{% block extra_script %}
+{% endblock extra_script %}
```

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/month.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/month.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/ledger/corpledger/year.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/ledger/corpledger/year.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/modals/modal-full.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-full.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/modals/modal-xl.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal-xl.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/modals/modal.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/modals/modal_dialog.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/modal_dialog.html`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/templates/ledger/modals/pve/view_character_content.html` & `aa_ledger-0.3.8a1/ledger/templates/ledger/modals/pve/view_character_content.html`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,291 +1,291 @@
-{% load i18n %}
-{% load static %}
-{% load humanize %}
-{% load ledger %}
-<div class="modal-content">
-    <button type="button" class="btn-close py-3 px-3" data-bs-dismiss="modal" aria-label="Close"><span aria-hidden="true"></button>
-    <div class="modal-header">
-        <h4 class="modal-title" id="modalTitle"><img src="{{ character.main_id|portrait }}" class="img-circle" alt="{{ data.main_name }}"> {{character.main_name}} - {{character.date}}</h4>
-    </div>
-    <div class="card-body">
-        <div class="row description-row">
-            <h4 id="character-title"></h4>
-        </div>
-        {% if character %}
-        <div>
-            <ul class="nav nav-tabs" role="tablist">
-                <li class="nav-item">
-                    <button class="nav-link active" href="#tab-summary" data-bs-toggle="tab">Summary</button>
-                </li>
-                <li>
-                    <button class="nav-link" href="#tab-daily" data-bs-toggle="tab">Daily</button>
-                </li>
-                <li>
-                    <button class="nav-link" href="#tab-hourly" data-bs-toggle="tab">Hourly</button>
-                </li>
-            </ul>
-            <div class="border border-secondary rounded-bottom tab-content px-2">
-                <div class="tab-pane panel panel-default active" id="tab-summary">
-                    <div class="card-body modal-tab">
-                        <div class="row description-row">
-                            <div class="col-sm-6">Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Stolen ESS:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        {% if character.mining %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Mining:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        {% if character.transaction %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Trading:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Trading Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        {% if character.contract %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Contracts:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        {% if character.donation %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Donations:<br>
-                            <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
-                            </div>
-                            <div class='col-sm-6'>
-                                <span style="color: green">
-                                    {{ character.donation.total_amount|format_currency }}
-                                </span> ISK
-                                    <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
-                            </div>
-                        </div>
-                        {% endif %}
-                        {% if character.production_cost %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Production Cost:</div>
-                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Summary:</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|format_currency }}</span> ISK</div>
-                        </div>
-                    </div>
-                </div>
-                <!--##############################DAILY#######################-->
-                <div class="tab-pane panel panel-default" id="tab-daily">
-                    <div class="card-body modal-tab">
-                        {% if character.bounty.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Ratting:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Ratting per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        <hr>
-
-                        {% if character.ess.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - ESS:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Stolen ESS:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. ESS per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Stolen per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% if character.mining %}
-                        <hr>
-                        {% if character.mining.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Mining:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Mining per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.transaction %}
-                        <hr>
-                        {% if character.transaction.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Trading:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Trading Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.contract %}
-                        <hr>
-                        {% if character.contract.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Contracts:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Contracts per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.donation %}
-                        <hr>
-                        {% if character.donation.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Donations:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Donations per Day:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.production_cost %}
-                        <hr>
-                        {% if character.production_cost.total_amount_day %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Current Day - Production Cost:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Production Cost per Day:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        {% if character.date %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Summary Day</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                    </div>
-                </div>
-                <!--############################## HOURLY #######################-->
-                <div class="tab-pane panel panel-default" id="tab-hourly">
-                    <div class="card-body modal-tab">
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Ratting per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. ESS per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Stolen per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-
-                        {% if character.mining %}
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Mining per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.transaction %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.contract %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Contracts per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.donation %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Donations per Hour:</div>
-                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-
-                        {% if character.production_cost %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Avg. Production Cost per Hour:</div>
-                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                        {% if character.date %}
-                        <hr>
-                        <div class="row description-row">
-                            <div class="col-sm-6">Summary Hour</div>
-                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|format_currency }}</span> ISK</div>
-                        </div>
-                        {% endif %}
-                    </div>
-                </div>
-            </div>
-        </div>
-        {% else %}
-        No ratting data found...
-        {% endif %}
-    </div>
-
-    <div class="modal-footer">
-        </div>
-</div>
+{% load i18n %}
+{% load static %}
+{% load humanize %}
+{% load ledger %}
+<div class="modal-content">
+    <button type="button" class="btn-close py-3 px-3" data-bs-dismiss="modal" aria-label="Close"><span aria-hidden="true"></button>
+    <div class="modal-header">
+        <h4 class="modal-title" id="modalTitle"><img src="{{ character.main_id|portrait }}" class="img-circle" alt="{{ data.main_name }}"> {{character.main_name}} - {{character.date}}</h4>
+    </div>
+    <div class="card-body">
+        <div class="row description-row">
+            <h4 id="character-title"></h4>
+        </div>
+        {% if character %}
+        <div>
+            <ul class="nav nav-tabs" role="tablist">
+                <li class="nav-item">
+                    <button class="nav-link active" href="#tab-summary" data-bs-toggle="tab">Summary</button>
+                </li>
+                <li>
+                    <button class="nav-link" href="#tab-daily" data-bs-toggle="tab">Daily</button>
+                </li>
+                <li>
+                    <button class="nav-link" href="#tab-hourly" data-bs-toggle="tab">Hourly</button>
+                </li>
+            </ul>
+            <div class="border border-secondary rounded-bottom tab-content px-2">
+                <div class="tab-pane panel panel-default active" id="tab-summary">
+                    <div class="card-body modal-tab">
+                        <div class="row description-row">
+                            <div class="col-sm-6">Ratting:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">ESS:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Stolen ESS:</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.stolen.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        {% if character.mining %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Mining:</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.mining.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.transaction %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Trading:</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.transaction.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Trading Cost:</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.market_cost.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.contract %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Contracts:</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.contract.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.donation %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Donations:<br>
+                            <span style="color: #FFBF00"><!--<i class="fas fa-exclamation-triangle"></i> Excluded from summary <i class="fas fa-exclamation-triangle"></i>--></span>
+                            </div>
+                            <div class='col-sm-6'>
+                                <span style="color: green">
+                                    {{ character.donation.total_amount|format_currency }}
+                                </span> ISK
+                                    <br><span style="color: #3483eb"><!--<i class="fas fa-info-circle"></i> Exluded registered chars <i class="fas fa-info-circle"></i>--></span>
+                            </div>
+                        </div>
+                        {% endif %}
+                        {% if character.production_cost %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Production Cost:</div>
+                            <div class='col-sm-6'><span style="color: red">{{ character.production_cost.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Summary:</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount|format_currency }}</span> ISK</div>
+                        </div>
+                    </div>
+                </div>
+                <!--##############################DAILY#######################-->
+                <div class="tab-pane panel panel-default" id="tab-daily">
+                    <div class="card-body modal-tab">
+                        {% if character.bounty.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Ratting:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Ratting per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        <hr>
+
+                        {% if character.ess.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - ESS:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Stolen ESS:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. ESS per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.ess.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Stolen per Day:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% if character.mining %}
+                        <hr>
+                        {% if character.mining.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Mining:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Mining per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.transaction %}
+                        <hr>
+                        {% if character.transaction.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Trading:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Trading Cost:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Trading per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Trading Cost per Day:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.contract %}
+                        <hr>
+                        {% if character.contract.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Contracts:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Contracts per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.donation %}
+                        <hr>
+                        {% if character.donation.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Donations:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Donations per Day:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.production_cost %}
+                        <hr>
+                        {% if character.production_cost.total_amount_day %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Current Day - Production Cost:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Production Cost per Day:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.date %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Summary Day</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_day|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                    </div>
+                </div>
+                <!--############################## HOURLY #######################-->
+                <div class="tab-pane panel panel-default" id="tab-hourly">
+                    <div class="card-body modal-tab">
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Ratting per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. ESS per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.bounty.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Stolen per Hour:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.stolen.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+
+                        {% if character.mining %}
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Mining per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.mining.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.transaction %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Trading per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.transaction.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Trading Cost per Hour:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.market_cost.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.contract %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Contracts per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.contract.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.donation %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Donations per Hour:</div>
+                            <div class='col-sm-4'><span style="color: green">{{ character.donation.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+
+                        {% if character.production_cost %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Avg. Production Cost per Hour:</div>
+                            <div class='col-sm-4'><span style="color: red">{{ character.production_cost.average_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                        {% if character.date %}
+                        <hr>
+                        <div class="row description-row">
+                            <div class="col-sm-6">Summary Hour</div>
+                            <div class='col-sm-6'><span style="color: green">{{ character.summary.total_amount_hour|format_currency }}</span> ISK</div>
+                        </div>
+                        {% endif %}
+                    </div>
+                </div>
+            </div>
+        </div>
+        {% else %}
+        No ratting data found...
+        {% endif %}
+    </div>
+
+    <div class="modal-footer">
+        </div>
+</div>
```

### Comparing `aa_ledger-0.3.8/ledger/view_helpers/core.py` & `aa_ledger-0.3.8a1/ledger/view_helpers/core.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/views/pve.py` & `aa_ledger-0.3.8a1/ledger/views/pve.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/views/character/char_audit.py` & `aa_ledger-0.3.8a1/ledger/views/character/char_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/views/corporation/corp_audit.py` & `aa_ledger-0.3.8a1/ledger/views/corporation/corp_audit.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/views/corporation/corp_events.py` & `aa_ledger-0.3.8a1/ledger/views/corporation/corp_events.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/ledger/views/corporation/corp_tax.py` & `aa_ledger-0.3.8a1/ledger/views/corporation/corp_tax.py`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/LICENSE` & `aa_ledger-0.3.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/README.md` & `aa_ledger-0.3.8a1/README.md`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/pyproject.toml` & `aa_ledger-0.3.8a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ledger-0.3.8/PKG-INFO` & `aa_ledger-0.3.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ledger
-Version: 0.3.8
+Version: 0.3.8a1
 Summary: EVE Online - Character/Corporation Ledger
 Project-URL: Changelog, https://github.com/Geuthur/aa-ledger/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/Geuthur/aa-ledger
 Project-URL: Source, https://github.com/Geuthur/aa-ledger
 Project-URL: Tracker, https://github.com/Geuthur/aa-ledger/issues
 Author-email: Geuthur <devgeuthur@gmail.com>
 License: MIT License
```

