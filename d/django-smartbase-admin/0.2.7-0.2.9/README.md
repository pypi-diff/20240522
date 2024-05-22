# Comparing `tmp/django_smartbase_admin-0.2.7.tar.gz` & `tmp/django_smartbase_admin-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_smartbase_admin-0.2.7.tar", max compression
+gzip compressed data, was "django_smartbase_admin-0.2.9.tar", max compression
```

## Comparing `django_smartbase_admin-0.2.7.tar` & `django_smartbase_admin-0.2.9.tar`

### file list

```diff
@@ -1,630 +1,633 @@
--rw-r--r--   0        0        0     1078 2024-04-05 11:44:03.377751 django_smartbase_admin-0.2.7/LICENSE.md
--rw-r--r--   0        0        0       65 2024-04-05 11:44:03.377751 django_smartbase_admin-0.2.7/README.md
--rw-r--r--   0        0        0      586 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/actions/__init__.py
--rw-r--r--   0        0        0    12723 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/actions/admin_action_list.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/__init__.py
--rw-r--r--   0        0        0    31150 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/admin_base.py
--rw-r--r--   0        0        0     6783 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/site.py
--rw-r--r--   0        0        0    12138 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/widgets.py
--rw-r--r--   0        0        0      479 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/apps.py
--rw-r--r--   0        0        0      342 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/compilemessages.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/__init__.py
--rw-r--r--   0        0        0      658 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/actions.py
--rw-r--r--   0        0        0    21953 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_base_view.py
--rw-r--r--   0        0        0      624 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_entrypoint_view.py
--rw-r--r--   0        0        0     4238 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_view.py
--rw-r--r--   0        0        0     5985 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/configuration.py
--rw-r--r--   0        0        0     1942 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/const.py
--rw-r--r--   0        0        0    23660 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/dashboard.py
--rw-r--r--   0        0        0     4630 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/fake_inline.py
--rw-r--r--   0        0        0     8795 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/field.py
--rw-r--r--   0        0        0     1294 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/field_formatter.py
--rw-r--r--   0        0        0    18605 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/filter_widgets.py
--rw-r--r--   0        0        0      249 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/global_filter_form.py
--rw-r--r--   0        0        0     2936 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/menu_item.py
--rw-r--r--   0        0        0     2588 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/request.py
--rw-r--r--   0        0        0    14647 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15583 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      381 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/makemessages.py
--rw-r--r--   0        0        0     1154 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0001_initial.py
--rw-r--r--   0        0        0      631 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py
--rw-r--r--   0        0        0      552 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py
--rw-r--r--   0        0        0      648 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/__init__.py
--rw-r--r--   0        0        0      743 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/models.py
--rw-r--r--   0        0        0      833 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py
--rw-r--r--   0        0        0      385 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/querysets.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/__init__.py
--rw-r--r--   0        0        0      712 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/configuration.py
--rw-r--r--   0        0        0      156 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/data.py
--rw-r--r--   0        0        0      642 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/thread_local.py
--rw-r--r--   0        0        0     5606 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/translations.py
--rw-r--r--   0        0        0     7338 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/views.py
--rw-r--r--   0        0        0     8911 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/xlsx_export.py
--rw-r--r--   0        0        0      610 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js
--rw-r--r--   0        0        0     2369 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js
--rw-r--r--   0        0        0     1015 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js
--rw-r--r--   0        0        0      342 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/screens.js
--rw-r--r--   0        0        0     1341 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js
--rw-r--r--   0        0        0      851 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js
--rw-r--r--   0        0        0      247 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/webpack.analyze.js
--rw-r--r--   0        0        0     2540 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js
--rw-r--r--   0        0        0      176 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/webpack.dev.js
--rw-r--r--   0        0        0      294 2024-04-05 11:44:03.393751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/webpack.prod.js
--rw-r--r--   0        0        0     6037 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css
--rw-r--r--   0        0        0     1646 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css
--rw-r--r--   0        0        0   204560 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/chart.js
--rw-r--r--   0        0        0      257 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/chart.js.LICENSE.txt
--rw-r--r--   0        0        0   375193 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main.js
--rw-r--r--   0        0        0     5600 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt
--rw-r--r--   0        0        0   145596 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main_style.css
--rw-r--r--   0        0        0        0 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main_style.js
--rw-r--r--   0        0        0   457051 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/table.js
--rw-r--r--   0        0        0      125 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/table.js.LICENSE.txt
--rw-r--r--   0        0        0      567 2024-04-05 11:44:37.465676 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/translations.js
--rw-r--r--   0        0        0    18172 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png
--rw-r--r--   0        0        0    50085 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png
--rw-r--r--   0        0        0     7398 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png
--rw-r--r--   0        0        0      261 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/browserconfig.xml
--rw-r--r--   0        0        0     1213 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png
--rw-r--r--   0        0        0     2044 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png
--rw-r--r--   0        0        0    15086 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico
--rw-r--r--   0        0        0     3716 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png
--rw-r--r--   0        0        0     3914 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png
--rw-r--r--   0        0        0     4332 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png
--rw-r--r--   0        0        0     8565 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png
--rw-r--r--   0        0        0     2781 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png
--rw-r--r--   0        0        0     4925 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg
--rw-r--r--   0        0        0      456 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/site.webmanifest
--rw-r--r--   0        0        0    56968 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2
--rw-r--r--   0        0        0    37924 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2
--rw-r--r--   0        0        0       43 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/blank.gif
--rw-r--r--   0        0        0      364 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ad.png
--rw-r--r--   0        0        0      333 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ae.png
--rw-r--r--   0        0        0      478 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/af.png
--rw-r--r--   0        0        0      827 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png
--rw-r--r--   0        0        0      843 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png
--rw-r--r--   0        0        0      614 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/al.png
--rw-r--r--   0        0        0      269 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/am.png
--rw-r--r--   0        0        0      503 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/an.png
--rw-r--r--   0        0        0      497 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ao.png
--rw-r--r--   0        0        0      383 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ar.png
--rw-r--r--   0        0        0      308 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/at.png
--rw-r--r--   0        0        0      877 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/au.png
--rw-r--r--   0        0        0      419 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/aw.png
--rw-r--r--   0        0        0      323 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ax.png
--rw-r--r--   0        0        0      367 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/az.png
--rw-r--r--   0        0        0      600 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png
--rw-r--r--   0        0        0      509 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bb.png
--rw-r--r--   0        0        0      516 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png
--rw-r--r--   0        0        0      275 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/be.png
--rw-r--r--   0        0        0      437 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bf.png
--rw-r--r--   0        0        0      306 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bg.png
--rw-r--r--   0        0        0      393 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bh.png
--rw-r--r--   0        0        0      826 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png
--rw-r--r--   0        0        0      309 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bj.png
--rw-r--r--   0        0        0      870 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png
--rw-r--r--   0        0        0      709 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png
--rw-r--r--   0        0        0      275 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bo.png
--rw-r--r--   0        0        0      863 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/br.png
--rw-r--r--   0        0        0      618 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png
--rw-r--r--   0        0        0      365 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bt.png
--rw-r--r--   0        0        0      280 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bw.png
--rw-r--r--   0        0        0      362 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/by.png
--rw-r--r--   0        0        0      685 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png
--rw-r--r--   0        0        0      494 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ca.png
--rw-r--r--   0        0        0      616 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png
--rw-r--r--   0        0        0      793 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png
--rw-r--r--   0        0        0     1067 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png
--rw-r--r--   0        0        0      783 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png
--rw-r--r--   0        0        0      569 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png
--rw-r--r--   0        0        0      665 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png
--rw-r--r--   0        0        0      313 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ch.png
--rw-r--r--   0        0        0      326 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ci.png
--rw-r--r--   0        0        0      454 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cl.png
--rw-r--r--   0        0        0      446 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cm.png
--rw-r--r--   0        0        0      585 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png
--rw-r--r--   0        0        0      721 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png
--rw-r--r--   0        0        0      276 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/co.png
--rw-r--r--   0        0        0      914 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png
--rw-r--r--   0        0        0      309 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cr.png
--rw-r--r--   0        0        0      463 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cs.png
--rw-r--r--   0        0        0      567 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png
--rw-r--r--   0        0        0      599 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png
--rw-r--r--   0        0        0      594 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png
--rw-r--r--   0        0        0      688 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png
--rw-r--r--   0        0        0      463 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cz.png
--rw-r--r--   0        0        0      278 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/de.png
--rw-r--r--   0        0        0      583 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png
--rw-r--r--   0        0        0      327 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dk.png
--rw-r--r--   0        0        0      677 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png
--rw-r--r--   0        0        0      446 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/do.png
--rw-r--r--   0        0        0      738 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png
--rw-r--r--   0        0        0      491 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ec.png
--rw-r--r--   0        0        0      314 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ee.png
--rw-r--r--   0        0        0      427 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/eg.png
--rw-r--r--   0        0        0     1025 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/en.png
--rw-r--r--   0        0        0      821 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/er.png
--rw-r--r--   0        0        0      473 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/es.png
--rw-r--r--   0        0        0      579 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/et.png
--rw-r--r--   0        0        0      582 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png
--rw-r--r--   0        0        0      326 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fi.png
--rw-r--r--   0        0        0      900 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png
--rw-r--r--   0        0        0      949 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png
--rw-r--r--   0        0        0      599 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png
--rw-r--r--   0        0        0      330 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fr.png
--rw-r--r--   0        0        0      273 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ga.png
--rw-r--r--   0        0        0     1025 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png
--rw-r--r--   0        0        0      806 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png
--rw-r--r--   0        0        0      397 2024-04-05 11:44:03.397751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ge.png
--rw-r--r--   0        0        0      539 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png
--rw-r--r--   0        0        0      393 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gh.png
--rw-r--r--   0        0        0      472 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gi.png
--rw-r--r--   0        0        0      279 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gm.png
--rw-r--r--   0        0        0      278 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gn.png
--rw-r--r--   0        0        0      574 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png
--rw-r--r--   0        0        0      453 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gr.png
--rw-r--r--   0        0        0      491 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gt.png
--rw-r--r--   0        0        0      453 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gw.png
--rw-r--r--   0        0        0      677 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png
--rw-r--r--   0        0        0      657 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png
--rw-r--r--   0        0        0      419 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hn.png
--rw-r--r--   0        0        0      638 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png
--rw-r--r--   0        0        0      568 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png
--rw-r--r--   0        0        0      308 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hu.png
--rw-r--r--   0        0        0      295 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/id.png
--rw-r--r--   0        0        0      328 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ie.png
--rw-r--r--   0        0        0      527 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/il.png
--rw-r--r--   0        0        0      642 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/im.png
--rw-r--r--   0        0        0      375 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/in.png
--rw-r--r--   0        0        0      428 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/iq.png
--rw-r--r--   0        0        0      553 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png
--rw-r--r--   0        0        0      328 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/is.png
--rw-r--r--   0        0        0      329 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/it.png
--rw-r--r--   0        0        0     1133 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/je.png
--rw-r--r--   0        0        0      779 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png
--rw-r--r--   0        0        0      602 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png
--rw-r--r--   0        0        0      614 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png
--rw-r--r--   0        0        0      573 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png
--rw-r--r--   0        0        0      725 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png
--rw-r--r--   0        0        0      459 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kh.png
--rw-r--r--   0        0        0      729 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/km.png
--rw-r--r--   0        0        0     1020 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png
--rw-r--r--   0        0        0      512 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png
--rw-r--r--   0        0        0      845 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png
--rw-r--r--   0        0        0      474 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kw.png
--rw-r--r--   0        0        0      931 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png
--rw-r--r--   0        0        0      883 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png
--rw-r--r--   0        0        0      411 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/la.png
--rw-r--r--   0        0        0      442 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lb.png
--rw-r--r--   0        0        0      542 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png
--rw-r--r--   0        0        0      263 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/li.png
--rw-r--r--   0        0        0      799 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png
--rw-r--r--   0        0        0      659 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png
--rw-r--r--   0        0        0      401 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ls.png
--rw-r--r--   0        0        0      274 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lt.png
--rw-r--r--   0        0        0      314 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lu.png
--rw-r--r--   0        0        0      285 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lv.png
--rw-r--r--   0        0        0      352 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ly.png
--rw-r--r--   0        0        0      513 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png
--rw-r--r--   0        0        0      295 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mc.png
--rw-r--r--   0        0        0      375 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/md.png
--rw-r--r--   0        0        0      810 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/me.png
--rw-r--r--   0        0        0      334 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mg.png
--rw-r--r--   0        0        0     1071 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png
--rw-r--r--   0        0        0      277 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ml.png
--rw-r--r--   0        0        0      548 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png
--rw-r--r--   0        0        0      390 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mn.png
--rw-r--r--   0        0        0      620 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png
--rw-r--r--   0        0        0      579 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png
--rw-r--r--   0        0        0      900 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png
--rw-r--r--   0        0        0      438 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mt.png
--rw-r--r--   0        0        0      279 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mu.png
--rw-r--r--   0        0        0      506 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mv.png
--rw-r--r--   0        0        0      389 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mw.png
--rw-r--r--   0        0        0      523 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png
--rw-r--r--   0        0        0      686 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/my.png
--rw-r--r--   0        0        0      590 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png
--rw-r--r--   0        0        0      897 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/na.png
--rw-r--r--   0        0        0      380 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ne.png
--rw-r--r--   0        0        0      317 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ng.png
--rw-r--r--   0        0        0      405 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ni.png
--rw-r--r--   0        0        0      307 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/nl.png
--rw-r--r--   0        0        0      402 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/no.png
--rw-r--r--   0        0        0      866 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/np.png
--rw-r--r--   0        0        0      784 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png
--rw-r--r--   0        0        0      473 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/om.png
--rw-r--r--   0        0        0      604 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png
--rw-r--r--   0        0        0      319 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pe.png
--rw-r--r--   0        0        0      534 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png
--rw-r--r--   0        0        0      754 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png
--rw-r--r--   0        0        0      629 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png
--rw-r--r--   0        0        0      682 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png
--rw-r--r--   0        0        0      290 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pl.png
--rw-r--r--   0        0        0      678 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png
--rw-r--r--   0        0        0      545 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png
--rw-r--r--   0        0        0      508 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pw.png
--rw-r--r--   0        0        0      371 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/py.png
--rw-r--r--   0        0        0      392 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/qa.png
--rw-r--r--   0        0        0      273 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ro.png
--rw-r--r--   0        0        0      525 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png
--rw-r--r--   0        0        0      306 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ru.png
--rw-r--r--   0        0        0      385 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/rw.png
--rw-r--r--   0        0        0      676 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png
--rw-r--r--   0        0        0     1126 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png
--rw-r--r--   0        0        0      974 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png
--rw-r--r--   0        0        0      523 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png
--rw-r--r--   0        0        0      284 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/se.png
--rw-r--r--   0        0        0      592 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png
--rw-r--r--   0        0        0     1253 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png
--rw-r--r--   0        0        0      430 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/si.png
--rw-r--r--   0        0        0      772 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png
--rw-r--r--   0        0        0      308 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sl.png
--rw-r--r--   0        0        0      503 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sm.png
--rw-r--r--   0        0        0      404 2024-04-05 11:44:03.401751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sn.png
--rw-r--r--   0        0        0      506 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/so.png
--rw-r--r--   0        0        0      446 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sr.png
--rw-r--r--   0        0        0      650 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/st.png
--rw-r--r--   0        0        0      438 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sv.png
--rw-r--r--   0        0        0      495 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sy.png
--rw-r--r--   0        0        0      535 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png
--rw-r--r--   0        0        0      919 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png
--rw-r--r--   0        0        0      274 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/td.png
--rw-r--r--   0        0        0      481 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tg.png
--rw-r--r--   0        0        0      307 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/th.png
--rw-r--r--   0        0        0      399 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tj.png
--rw-r--r--   0        0        0      739 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png
--rw-r--r--   0        0        0      786 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png
--rw-r--r--   0        0        0      678 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png
--rw-r--r--   0        0        0      522 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/to.png
--rw-r--r--   0        0        0      649 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png
--rw-r--r--   0        0        0     1025 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png
--rw-r--r--   0        0        0      423 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tw.png
--rw-r--r--   0        0        0      767 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png
--rw-r--r--   0        0        0      260 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ua.png
--rw-r--r--   0        0        0      598 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png
--rw-r--r--   0        0        0      627 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/us.png
--rw-r--r--   0        0        0      588 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png
--rw-r--r--   0        0        0      494 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/uz.png
--rw-r--r--   0        0        0      485 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vc.png
--rw-r--r--   0        0        0      364 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ve.png
--rw-r--r--   0        0        0      997 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png
--rw-r--r--   0        0        0      503 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vn.png
--rw-r--r--   0        0        0      666 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png
--rw-r--r--   0        0        0      428 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ws.png
--rw-r--r--   0        0        0      744 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png
--rw-r--r--   0        0        0      308 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ye.png
--rw-r--r--   0        0        0      802 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/za.png
--rw-r--r--   0        0        0      501 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/zm.png
--rw-r--r--   0        0        0      620 2024-04-05 11:44:03.405751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png
--rw-r--r--   0        0        0  1664449 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/login.jpg
--rw-r--r--   0        0        0    92962 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/login.webp
--rw-r--r--   0        0        0     6363 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/logo.svg
--rw-r--r--   0        0        0     2354 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/sk.svg
--rw-r--r--   0        0        0   170535 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js
--rw-r--r--   0        0        0     4819 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js
--rw-r--r--   0        0        0     1323 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js
--rw-r--r--   0        0        0    39433 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js
--rw-r--r--   0        0        0    87461 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js
--rw-r--r--   0        0        0     3063 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js
--rw-r--r--   0        0        0     7770 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js
--rw-r--r--   0        0        0     1698 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js
--rw-r--r--   0        0        0     1914 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/prices.js
--rw-r--r--   0        0        0      932 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/remove-me.js
--rw-r--r--   0        0        0   387673 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js
--rw-r--r--   0        0        0      527 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg
--rw-r--r--   0        0        0      682 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg
--rw-r--r--   0        0        0      386 2024-04-05 11:44:03.409751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-one.svg
--rw-r--r--   0        0        0      826 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg
--rw-r--r--   0        0        0      444 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-three.svg
--rw-r--r--   0        0        0      477 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Aiming.svg
--rw-r--r--   0        0        0      677 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg
--rw-r--r--   0        0        0      732 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg
--rw-r--r--   0        0        0      734 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg
--rw-r--r--   0        0        0     1138 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg
--rw-r--r--   0        0        0     1238 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg
--rw-r--r--   0        0        0     1209 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg
--rw-r--r--   0        0        0      509 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-down.svg
--rw-r--r--   0        0        0      522 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg
--rw-r--r--   0        0        0      524 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg
--rw-r--r--   0        0        0      511 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-up.svg
--rw-r--r--   0        0        0      737 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg
--rw-r--r--   0        0        0      988 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg
--rw-r--r--   0        0        0      538 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg
--rw-r--r--   0        0        0      524 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg
--rw-r--r--   0        0        0      304 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card.svg
--rw-r--r--   0        0        0      622 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg
--rw-r--r--   0        0        0      532 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg
--rw-r--r--   0        0        0      824 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg
--rw-r--r--   0        0        0      540 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg
--rw-r--r--   0        0        0      583 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg
--rw-r--r--   0        0        0      979 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg
--rw-r--r--   0        0        0      281 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-small.svg
--rw-r--r--   0        0        0      280 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check.svg
--rw-r--r--   0        0        0      544 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg
--rw-r--r--   0        0        0      318 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-small.svg
--rw-r--r--   0        0        0      318 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close.svg
--rw-r--r--   0        0        0      429 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Column.svg
--rw-r--r--   0        0        0      361 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-left.svg
--rw-r--r--   0        0        0      347 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-right.svg
--rw-r--r--   0        0        0     1231 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg
--rw-r--r--   0        0        0     2040 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg
--rw-r--r--   0        0        0      611 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg
--rw-r--r--   0        0        0      454 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete.svg
--rw-r--r--   0        0        0      439 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-down.svg
--rw-r--r--   0        0        0      433 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-left.svg
--rw-r--r--   0        0        0      430 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-right.svg
--rw-r--r--   0        0        0      439 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-up.svg
--rw-r--r--   0        0        0      504 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-c.svg
--rw-r--r--   0        0        0      296 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-small.svg
--rw-r--r--   0        0        0      280 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down.svg
--rw-r--r--   0        0        0      984 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg
--rw-r--r--   0        0        0      386 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download.svg
--rw-r--r--   0        0        0      898 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg
--rw-r--r--   0        0        0      529 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg
--rw-r--r--   0        0        0      442 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Excel-one.svg
--rw-r--r--   0        0        0      636 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg
--rw-r--r--   0        0        0     1432 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg
--rw-r--r--   0        0        0      683 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg
--rw-r--r--   0        0        0      575 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg
--rw-r--r--   0        0        0      527 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg
--rw-r--r--   0        0        0      570 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg
--rw-r--r--   0        0        0      264 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Hamburger-button.svg
--rw-r--r--   0        0        0      653 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg
--rw-r--r--   0        0        0     1300 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg
--rw-r--r--   0        0        0      536 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg
--rw-r--r--   0        0        0      756 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg
--rw-r--r--   0        0        0     1039 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg
--rw-r--r--   0        0        0      501 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-c.svg
--rw-r--r--   0        0        0      247 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-down.svg
--rw-r--r--   0        0        0      235 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-up.svg
--rw-r--r--   0        0        0      301 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small.svg
--rw-r--r--   0        0        0      272 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left.svg
--rw-r--r--   0        0        0      852 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg
--rw-r--r--   0        0        0      856 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg
--rw-r--r--   0        0        0      714 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg
--rw-r--r--   0        0        0      566 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg
--rw-r--r--   0        0        0      403 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lock.svg
--rw-r--r--   0        0        0      381 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Login.svg
--rw-r--r--   0        0        0      376 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Logout.svg
--rw-r--r--   0        0        0      887 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg
--rw-r--r--   0        0        0      574 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg
--rw-r--r--   0        0        0      666 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg
--rw-r--r--   0        0        0      647 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg
--rw-r--r--   0        0        0      418 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail.svg
--rw-r--r--   0        0        0     1757 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg
--rw-r--r--   0        0        0      555 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg
--rw-r--r--   0        0        0      487 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus-the-top.svg
--rw-r--r--   0        0        0      148 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus.svg
--rw-r--r--   0        0        0      541 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg
--rw-r--r--   0        0        0      810 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg
--rw-r--r--   0        0        0      771 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg
--rw-r--r--   0        0        0      547 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg
--rw-r--r--   0        0        0     1528 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg
--rw-r--r--   0        0        0      638 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg
--rw-r--r--   0        0        0      874 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg
--rw-r--r--   0        0        0      656 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg
--rw-r--r--   0        0        0      940 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg
--rw-r--r--   0        0        0      891 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg
--rw-r--r--   0        0        0     1485 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg
--rw-r--r--   0        0        0      242 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Plus.svg
--rw-r--r--   0        0        0     2587 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg
--rw-r--r--   0        0        0      938 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg
--rw-r--r--   0        0        0     2362 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg
--rw-r--r--   0        0        0      745 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg
--rw-r--r--   0        0        0      362 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Reduce-one.svg
--rw-r--r--   0        0        0      899 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg
--rw-r--r--   0        0        0      507 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Return.svg
--rw-r--r--   0        0        0      299 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora Filled.svg
--rw-r--r--   0        0        0      504 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora.svg
--rw-r--r--   0        0        0      501 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-c.svg
--rw-r--r--   0        0        0      280 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-down.svg
--rw-r--r--   0        0        0      243 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-up.svg
--rw-r--r--   0        0        0      294 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small.svg
--rw-r--r--   0        0        0      272 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right.svg
--rw-r--r--   0        0        0      687 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg
--rw-r--r--   0        0        0      461 2024-04-05 11:44:03.413751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Search.svg
--rw-r--r--   0        0        0      534 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg
--rw-r--r--   0        0        0      328 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-config.svg
--rw-r--r--   0        0        0     2761 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg
--rw-r--r--   0        0        0     1380 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg
--rw-r--r--   0        0        0     2218 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg
--rw-r--r--   0        0        0      812 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg
--rw-r--r--   0        0        0      940 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg
--rw-r--r--   0        0        0      497 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort Alt.svg
--rw-r--r--   0        0        0      311 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-down.svg
--rw-r--r--   0        0        0      334 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-up.svg
--rw-r--r--   0        0        0      360 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-one.svg
--rw-r--r--   0        0        0      479 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-three.svg
--rw-r--r--   0        0        0      809 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg
--rw-r--r--   0        0        0     1175 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg
--rw-r--r--   0        0        0     1876 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg
--rw-r--r--   0        0        0      323 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Switch.svg
--rw-r--r--   0        0        0      525 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg
--rw-r--r--   0        0        0      806 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg
--rw-r--r--   0        0        0      485 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag.svg
--rw-r--r--   0        0        0      490 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tips-one.svg
--rw-r--r--   0        0        0      312 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/To-top.svg
--rw-r--r--   0        0        0      476 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Transfer-data.svg
--rw-r--r--   0        0        0     2485 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg
--rw-r--r--   0        0        0     1003 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg
--rw-r--r--   0        0        0      860 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg
--rw-r--r--   0        0        0     1074 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg
--rw-r--r--   0        0        0      592 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg
--rw-r--r--   0        0        0      393 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Unlock.svg
--rw-r--r--   0        0        0      504 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-c.svg
--rw-r--r--   0        0        0      299 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-small.svg
--rw-r--r--   0        0        0      279 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up.svg
--rw-r--r--   0        0        0      988 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg
--rw-r--r--   0        0        0      385 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload.svg
--rw-r--r--   0        0        0      777 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg
--rw-r--r--   0        0        0      888 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg
--rw-r--r--   0        0        0      680 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg
--rw-r--r--   0        0        0      584 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg
--rw-r--r--   0        0        0      490 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-out.svg
--rw-r--r--   0        0        0     1840 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_base.css
--rw-r--r--   0        0        0     1889 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css
--rw-r--r--   0        0        0     2825 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css
--rw-r--r--   0        0        0    11118 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_components.css
--rw-r--r--   0        0        0    14025 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css
--rw-r--r--   0        0        0     4096 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css
--rw-r--r--   0        0        0     5587 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css
--rw-r--r--   0        0        0    18294 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css
--rw-r--r--   0        0        0       58 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_tailwind_base.css
--rw-r--r--   0        0        0      901 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css
--rw-r--r--   0        0        0     4665 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css
--rw-r--r--   0        0        0     1763 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css
--rw-r--r--   0        0        0    10276 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css
--rw-r--r--   0        0        0     4316 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css
--rw-r--r--   0        0        0      719 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css
--rw-r--r--   0        0        0    10087 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css
--rw-r--r--   0        0        0     2388 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css
--rw-r--r--   0        0        0     2485 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css
--rw-r--r--   0        0        0      361 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/style.css
--rw-r--r--   0        0        0    12215 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js
--rw-r--r--   0        0        0     4736 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/chart.js
--rw-r--r--   0        0        0     4615 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/choices.js
--rw-r--r--   0        0        0      486 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/code.js
--rw-r--r--   0        0        0    14259 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js
--rw-r--r--   0        0        0     9131 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/main.js
--rw-r--r--   0        0        0     3354 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js
--rw-r--r--   0        0        0     1733 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/range.js
--rw-r--r--   0        0        0     1570 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js
--rw-r--r--   0        0        0     1186 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js
--rw-r--r--   0        0        0     9972 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table.js
--rw-r--r--   0        0        0      507 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/base_module.js
--rw-r--r--   0        0        0    10561 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js
--rw-r--r--   0        0        0      929 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js
--rw-r--r--   0        0        0      686 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js
--rw-r--r--   0        0        0     4016 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js
--rw-r--r--   0        0        0     7694 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js
--rw-r--r--   0        0        0     6403 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js
--rw-r--r--   0        0        0    11157 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js
--rw-r--r--   0        0        0     2383 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js
--rw-r--r--   0        0        0      954 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/translations.js
--rw-r--r--   0        0        0     4245 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/utils.js
--rw-r--r--   0        0        0    10987 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html
--rw-r--r--   0        0        0     3200 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html
--rw-r--r--   0        0        0      272 2024-04-05 11:44:03.417751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/dashboard.html
--rw-r--r--   0        0        0     3205 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html
--rw-r--r--   0        0        0     2248 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html
--rw-r--r--   0        0        0     9442 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/list.html
--rw-r--r--   0        0        0      122 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/media.html
--rw-r--r--   0        0        0     1905 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html
--rw-r--r--   0        0        0      109 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/partials/open_modal_attrs.html
--rw-r--r--   0        0        0      857 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html
--rw-r--r--   0        0        0     4549 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html
--rw-r--r--   0        0        0      587 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html
--rw-r--r--   0        0        0      334 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations-list.html
--rw-r--r--   0        0        0     1285 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations.html
--rw-r--r--   0        0        0       50 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/auth/user/add_form.html
--rw-r--r--   0        0        0     2398 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/login.html
--rw-r--r--   0        0        0      864 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html
--rw-r--r--   0        0        0      496 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/logout.html
--rw-r--r--   0        0        0      485 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_done.html
--rw-r--r--   0        0        0     1905 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html
--rw-r--r--   0        0        0      503 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_complete.html
--rw-r--r--   0        0        0     1310 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html
--rw-r--r--   0        0        0      666 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html
--rw-r--r--   0        0        0      621 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html
--rw-r--r--   0        0        0     1397 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html
--rw-r--r--   0        0        0       76 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/blank_base.html
--rw-r--r--   0        0        0     1982 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/buttons.html
--rw-r--r--   0        0        0      959 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/columns.html
--rw-r--r--   0        0        0     2654 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/filters.html
--rw-r--r--   0        0        0    10938 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/inputs.html
--rw-r--r--   0        0        0     4543 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/config/view.html
--rw-r--r--   0        0        0      900 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html
--rw-r--r--   0        0        0     1096 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html
--rw-r--r--   0        0        0      141 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/list_widget.html
--rw-r--r--   0        0        0      720 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html
--rw-r--r--   0        0        0     1071 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html
--rw-r--r--   0        0        0      548 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html
--rw-r--r--   0        0        0      645 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html
--rw-r--r--   0        0        0      648 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html
--rw-r--r--   0        0        0     1243 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html
--rw-r--r--   0        0        0     1162 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html
--rw-r--r--   0        0        0      614 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html
--rw-r--r--   0        0        0     1212 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html
--rw-r--r--   0        0        0      548 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html
--rw-r--r--   0        0        0     1121 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/fonts.html
--rw-r--r--   0        0        0      165 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/attrs.html
--rw-r--r--   0        0        0      172 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/change_form_title.html
--rw-r--r--   0        0        0    18710 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/components.html
--rw-r--r--   0        0        0      229 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/fieldset.html
--rw-r--r--   0        0        0     2227 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html
--rw-r--r--   0        0        0      287 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/loading.html
--rw-r--r--   0        0        0      304 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/loading_absolute.html
--rw-r--r--   0        0        0      771 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html
--rw-r--r--   0        0        0     7592 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html
--rw-r--r--   0        0        0    15127 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html
--rw-r--r--   0        0        0     3046 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html
--rw-r--r--   0        0        0    18190 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html
--rw-r--r--   0        0        0      308 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/cms/translations_status_row.html
--rw-r--r--   0        0        0     3002 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html
--rw-r--r--   0        0        0    18834 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html
--rw-r--r--   0        0        0     1909 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html
--rw-r--r--   0        0        0    15189 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html
--rw-r--r--   0        0        0     9195 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/navigation.html
--rw-r--r--   0        0        0      825 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html
--rw-r--r--   0        0        0      121 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_close.html
--rw-r--r--   0        0        0      276 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_error.html
--rw-r--r--   0        0        0      268 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_info.html
--rw-r--r--   0        0        0      323 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_success.html
--rw-r--r--   0        0        0      323 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_warning.html
--rw-r--r--   0        0        0     1507 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html
--rw-r--r--   0        0        0      505 2024-04-05 11:44:03.421751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sb_admin_base.html
--rw-r--r--   0        0        0     3253 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html
--rw-r--r--   0        0        0      817 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html
--rw-r--r--   0        0        0    59910 2024-04-05 11:44:25.989702 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg
--rw-r--r--   0        0        0     3254 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/submit_line.html
--rw-r--r--   0        0        0      577 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html
--rw-r--r--   0        0        0     2815 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/array.html
--rw-r--r--   0        0        0      172 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/attrs.html
--rw-r--r--   0        0        0     2434 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html
--rw-r--r--   0        0        0      232 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox.html
--rw-r--r--   0        0        0       51 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_option.html
--rw-r--r--   0        0        0     1578 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html
--rw-r--r--   0        0        0      542 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html
--rw-r--r--   0        0        0     2435 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html
--rw-r--r--   0        0        0      345 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/code.html
--rw-r--r--   0        0        0      160 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/date.html
--rw-r--r--   0        0        0       44 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/datetime.html
--rw-r--r--   0        0        0       43 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/email.html
--rw-r--r--   0        0        0       44 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/file.html
--rw-r--r--   0        0        0       44 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/hidden.html
--rw-r--r--   0        0        0      148 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/includes/field_label.html
--rw-r--r--   0        0        0      148 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/includes/help_text.html
--rw-r--r--   0        0        0      443 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/includes/simple_field_label.html
--rw-r--r--   0        0        0      185 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/input.html
--rw-r--r--   0        0        0      209 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/input_option.html
--rw-r--r--   0        0        0       50 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/multiple_hidden.html
--rw-r--r--   0        0        0      329 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/multiwidget.html
--rw-r--r--   0        0        0      159 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/number.html
--rw-r--r--   0        0        0      585 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/password.html
--rw-r--r--   0        0        0      363 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/radio.html
--rw-r--r--   0        0        0       51 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/radio_option.html
--rw-r--r--   0        0        0      216 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/read_only_password_hash.html
--rw-r--r--   0        0        0      496 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/select.html
--rw-r--r--   0        0        0       50 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/select_date.html
--rw-r--r--   0        0        0      123 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/select_option.html
--rw-r--r--   0        0        0       50 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/splitdatetime.html
--rw-r--r--   0        0        0       50 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/splithiddendatetime.html
--rw-r--r--   0        0        0      160 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/text.html
--rw-r--r--   0        0        0      257 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/textarea.html
--rw-r--r--   0        0        0      160 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/time.html
--rw-r--r--   0        0        0      280 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/toggle.html
--rw-r--r--   0        0        0      160 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/url.html
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templatetags/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templatetags/base.py
--rw-r--r--   0        0        0     4125 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/templatetags/sb_admin_tags.py
--rw-r--r--   0        0        0       17 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/urls.py
--rw-r--r--   0        0        0     1343 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/__init__.py
--rw-r--r--   0        0        0     1495 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/dashboard_view.py
--rw-r--r--   0        0        0      954 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/global_filter_view.py
--rw-r--r--   0        0        0      292 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/media_view.py
--rw-r--r--   0        0        0    20254 2024-04-05 11:44:03.425751 django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/translations_view.py
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 django_smartbase_admin-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-10 08:02:51.090920 django_smartbase_admin-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0       65 2024-04-10 08:02:51.090920 django_smartbase_admin-0.2.9/README.md
+-rw-r--r--   0        0        0      610 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/actions/__init__.py
+-rw-r--r--   0        0        0    12723 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/actions/admin_action_list.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/__init__.py
+-rw-r--r--   0        0        0    31150 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/admin_base.py
+-rw-r--r--   0        0        0     6783 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/site.py
+-rw-r--r--   0        0        0    12138 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/widgets.py
+-rw-r--r--   0        0        0      479 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/apps.py
+-rw-r--r--   0        0        0      342 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/compilemessages.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/__init__.py
+-rw-r--r--   0        0        0      658 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/actions.py
+-rw-r--r--   0        0        0    21953 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_base_view.py
+-rw-r--r--   0        0        0      624 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_entrypoint_view.py
+-rw-r--r--   0        0        0     4238 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_view.py
+-rw-r--r--   0        0        0     5985 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/configuration.py
+-rw-r--r--   0        0        0     1942 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/const.py
+-rw-r--r--   0        0        0    23660 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/dashboard.py
+-rw-r--r--   0        0        0     4630 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/fake_inline.py
+-rw-r--r--   0        0        0     8795 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/field.py
+-rw-r--r--   0        0        0     1294 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/field_formatter.py
+-rw-r--r--   0        0        0    18605 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/filter_widgets.py
+-rw-r--r--   0        0        0      249 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/global_filter_form.py
+-rw-r--r--   0        0        0     2936 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/menu_item.py
+-rw-r--r--   0        0        0     1894 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/modal_view.py
+-rw-r--r--   0        0        0     2588 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/request.py
+-rw-r--r--   0        0        0    14647 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15583 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      381 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/makemessages.py
+-rw-r--r--   0        0        0     1154 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0001_initial.py
+-rw-r--r--   0        0        0      631 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py
+-rw-r--r--   0        0        0      552 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py
+-rw-r--r--   0        0        0      648 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/models.py
+-rw-r--r--   0        0        0      833 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py
+-rw-r--r--   0        0        0      385 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/querysets.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/configuration.py
+-rw-r--r--   0        0        0      156 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/data.py
+-rw-r--r--   0        0        0      642 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/thread_local.py
+-rw-r--r--   0        0        0     5606 2024-04-10 08:02:51.106920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/translations.py
+-rw-r--r--   0        0        0     7338 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/views.py
+-rw-r--r--   0        0        0     8911 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/xlsx_export.py
+-rw-r--r--   0        0        0      610 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js
+-rw-r--r--   0        0        0     2369 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js
+-rw-r--r--   0        0        0     1015 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js
+-rw-r--r--   0        0        0      342 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/screens.js
+-rw-r--r--   0        0        0     1341 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js
+-rw-r--r--   0        0        0      851 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js
+-rw-r--r--   0        0        0      247 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/webpack.analyze.js
+-rw-r--r--   0        0        0     2540 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js
+-rw-r--r--   0        0        0      176 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/webpack.dev.js
+-rw-r--r--   0        0        0      294 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/webpack.prod.js
+-rw-r--r--   0        0        0     6037 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css
+-rw-r--r--   0        0        0     1646 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css
+-rw-r--r--   0        0        0   204560 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/chart.js
+-rw-r--r--   0        0        0      257 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/chart.js.LICENSE.txt
+-rw-r--r--   0        0        0   375310 2024-04-10 08:03:25.487062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main.js
+-rw-r--r--   0        0        0     5600 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt
+-rw-r--r--   0        0        0   145822 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main_style.css
+-rw-r--r--   0        0        0        0 2024-04-10 08:03:25.487062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main_style.js
+-rw-r--r--   0        0        0   457051 2024-04-10 08:03:25.487062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/table.js
+-rw-r--r--   0        0        0      125 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/table.js.LICENSE.txt
+-rw-r--r--   0        0        0      567 2024-04-10 08:03:25.491062 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/translations.js
+-rw-r--r--   0        0        0    18172 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png
+-rw-r--r--   0        0        0    50085 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png
+-rw-r--r--   0        0        0     7398 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png
+-rw-r--r--   0        0        0      261 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/browserconfig.xml
+-rw-r--r--   0        0        0     1213 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png
+-rw-r--r--   0        0        0     2044 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png
+-rw-r--r--   0        0        0    15086 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico
+-rw-r--r--   0        0        0     3716 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png
+-rw-r--r--   0        0        0     3914 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png
+-rw-r--r--   0        0        0     4332 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png
+-rw-r--r--   0        0        0     8565 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png
+-rw-r--r--   0        0        0     2781 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png
+-rw-r--r--   0        0        0     4925 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg
+-rw-r--r--   0        0        0      456 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/site.webmanifest
+-rw-r--r--   0        0        0    56968 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2
+-rw-r--r--   0        0        0    37924 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2
+-rw-r--r--   0        0        0       43 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/blank.gif
+-rw-r--r--   0        0        0      364 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ad.png
+-rw-r--r--   0        0        0      333 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ae.png
+-rw-r--r--   0        0        0      478 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/af.png
+-rw-r--r--   0        0        0      827 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png
+-rw-r--r--   0        0        0      843 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png
+-rw-r--r--   0        0        0      614 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/al.png
+-rw-r--r--   0        0        0      269 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/am.png
+-rw-r--r--   0        0        0      503 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/an.png
+-rw-r--r--   0        0        0      497 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ao.png
+-rw-r--r--   0        0        0      383 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ar.png
+-rw-r--r--   0        0        0      308 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/at.png
+-rw-r--r--   0        0        0      877 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/au.png
+-rw-r--r--   0        0        0      419 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/aw.png
+-rw-r--r--   0        0        0      323 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ax.png
+-rw-r--r--   0        0        0      367 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/az.png
+-rw-r--r--   0        0        0      600 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png
+-rw-r--r--   0        0        0      509 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bb.png
+-rw-r--r--   0        0        0      516 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png
+-rw-r--r--   0        0        0      275 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/be.png
+-rw-r--r--   0        0        0      437 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bf.png
+-rw-r--r--   0        0        0      306 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bg.png
+-rw-r--r--   0        0        0      393 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bh.png
+-rw-r--r--   0        0        0      826 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png
+-rw-r--r--   0        0        0      309 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bj.png
+-rw-r--r--   0        0        0      870 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png
+-rw-r--r--   0        0        0      709 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png
+-rw-r--r--   0        0        0      275 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bo.png
+-rw-r--r--   0        0        0      863 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/br.png
+-rw-r--r--   0        0        0      618 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png
+-rw-r--r--   0        0        0      365 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bt.png
+-rw-r--r--   0        0        0      280 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bw.png
+-rw-r--r--   0        0        0      362 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/by.png
+-rw-r--r--   0        0        0      685 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png
+-rw-r--r--   0        0        0      494 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ca.png
+-rw-r--r--   0        0        0      616 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png
+-rw-r--r--   0        0        0      793 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png
+-rw-r--r--   0        0        0     1067 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png
+-rw-r--r--   0        0        0      783 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png
+-rw-r--r--   0        0        0      569 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png
+-rw-r--r--   0        0        0      665 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png
+-rw-r--r--   0        0        0      313 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ch.png
+-rw-r--r--   0        0        0      326 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ci.png
+-rw-r--r--   0        0        0      454 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cl.png
+-rw-r--r--   0        0        0      446 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cm.png
+-rw-r--r--   0        0        0      585 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png
+-rw-r--r--   0        0        0      721 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png
+-rw-r--r--   0        0        0      276 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/co.png
+-rw-r--r--   0        0        0      914 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png
+-rw-r--r--   0        0        0      309 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cr.png
+-rw-r--r--   0        0        0      463 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cs.png
+-rw-r--r--   0        0        0      567 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png
+-rw-r--r--   0        0        0      599 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png
+-rw-r--r--   0        0        0      594 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png
+-rw-r--r--   0        0        0      688 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png
+-rw-r--r--   0        0        0      463 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cz.png
+-rw-r--r--   0        0        0      278 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/de.png
+-rw-r--r--   0        0        0      583 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png
+-rw-r--r--   0        0        0      327 2024-04-10 08:02:51.110921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dk.png
+-rw-r--r--   0        0        0      677 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png
+-rw-r--r--   0        0        0      446 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/do.png
+-rw-r--r--   0        0        0      738 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png
+-rw-r--r--   0        0        0      491 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ec.png
+-rw-r--r--   0        0        0      314 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ee.png
+-rw-r--r--   0        0        0      427 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/eg.png
+-rw-r--r--   0        0        0     1025 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/en.png
+-rw-r--r--   0        0        0      821 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/er.png
+-rw-r--r--   0        0        0      473 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/es.png
+-rw-r--r--   0        0        0      579 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/et.png
+-rw-r--r--   0        0        0      582 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png
+-rw-r--r--   0        0        0      326 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fi.png
+-rw-r--r--   0        0        0      900 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png
+-rw-r--r--   0        0        0      949 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png
+-rw-r--r--   0        0        0      599 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png
+-rw-r--r--   0        0        0      330 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fr.png
+-rw-r--r--   0        0        0      273 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ga.png
+-rw-r--r--   0        0        0     1025 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png
+-rw-r--r--   0        0        0      806 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png
+-rw-r--r--   0        0        0      397 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ge.png
+-rw-r--r--   0        0        0      539 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png
+-rw-r--r--   0        0        0      393 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gh.png
+-rw-r--r--   0        0        0      472 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gi.png
+-rw-r--r--   0        0        0      279 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gm.png
+-rw-r--r--   0        0        0      278 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gn.png
+-rw-r--r--   0        0        0      574 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png
+-rw-r--r--   0        0        0      453 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gr.png
+-rw-r--r--   0        0        0      491 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gt.png
+-rw-r--r--   0        0        0      453 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gw.png
+-rw-r--r--   0        0        0      677 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png
+-rw-r--r--   0        0        0      657 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png
+-rw-r--r--   0        0        0      419 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hn.png
+-rw-r--r--   0        0        0      638 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png
+-rw-r--r--   0        0        0      568 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png
+-rw-r--r--   0        0        0      308 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hu.png
+-rw-r--r--   0        0        0      295 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/id.png
+-rw-r--r--   0        0        0      328 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ie.png
+-rw-r--r--   0        0        0      527 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/il.png
+-rw-r--r--   0        0        0      642 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/im.png
+-rw-r--r--   0        0        0      375 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/in.png
+-rw-r--r--   0        0        0      428 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/iq.png
+-rw-r--r--   0        0        0      553 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png
+-rw-r--r--   0        0        0      328 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/is.png
+-rw-r--r--   0        0        0      329 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/it.png
+-rw-r--r--   0        0        0     1133 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/je.png
+-rw-r--r--   0        0        0      779 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png
+-rw-r--r--   0        0        0      602 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png
+-rw-r--r--   0        0        0      614 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png
+-rw-r--r--   0        0        0      573 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png
+-rw-r--r--   0        0        0      725 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png
+-rw-r--r--   0        0        0      459 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kh.png
+-rw-r--r--   0        0        0      729 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/km.png
+-rw-r--r--   0        0        0     1020 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png
+-rw-r--r--   0        0        0      512 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png
+-rw-r--r--   0        0        0      845 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png
+-rw-r--r--   0        0        0      474 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kw.png
+-rw-r--r--   0        0        0      931 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png
+-rw-r--r--   0        0        0      883 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png
+-rw-r--r--   0        0        0      411 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/la.png
+-rw-r--r--   0        0        0      442 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lb.png
+-rw-r--r--   0        0        0      542 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png
+-rw-r--r--   0        0        0      263 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/li.png
+-rw-r--r--   0        0        0      799 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png
+-rw-r--r--   0        0        0      659 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png
+-rw-r--r--   0        0        0      401 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ls.png
+-rw-r--r--   0        0        0      274 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lt.png
+-rw-r--r--   0        0        0      314 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lu.png
+-rw-r--r--   0        0        0      285 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lv.png
+-rw-r--r--   0        0        0      352 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ly.png
+-rw-r--r--   0        0        0      513 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png
+-rw-r--r--   0        0        0      295 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mc.png
+-rw-r--r--   0        0        0      375 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/md.png
+-rw-r--r--   0        0        0      810 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/me.png
+-rw-r--r--   0        0        0      334 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mg.png
+-rw-r--r--   0        0        0     1071 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png
+-rw-r--r--   0        0        0      277 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ml.png
+-rw-r--r--   0        0        0      548 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png
+-rw-r--r--   0        0        0      390 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mn.png
+-rw-r--r--   0        0        0      620 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png
+-rw-r--r--   0        0        0      579 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png
+-rw-r--r--   0        0        0      900 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png
+-rw-r--r--   0        0        0      438 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mt.png
+-rw-r--r--   0        0        0      279 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mu.png
+-rw-r--r--   0        0        0      506 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mv.png
+-rw-r--r--   0        0        0      389 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mw.png
+-rw-r--r--   0        0        0      523 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png
+-rw-r--r--   0        0        0      686 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/my.png
+-rw-r--r--   0        0        0      590 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png
+-rw-r--r--   0        0        0      897 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/na.png
+-rw-r--r--   0        0        0      380 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ne.png
+-rw-r--r--   0        0        0      317 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ng.png
+-rw-r--r--   0        0        0      405 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ni.png
+-rw-r--r--   0        0        0      307 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/nl.png
+-rw-r--r--   0        0        0      402 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/no.png
+-rw-r--r--   0        0        0      866 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/np.png
+-rw-r--r--   0        0        0      784 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png
+-rw-r--r--   0        0        0      473 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/om.png
+-rw-r--r--   0        0        0      604 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png
+-rw-r--r--   0        0        0      319 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pe.png
+-rw-r--r--   0        0        0      534 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png
+-rw-r--r--   0        0        0      754 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png
+-rw-r--r--   0        0        0      629 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png
+-rw-r--r--   0        0        0      682 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png
+-rw-r--r--   0        0        0      290 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pl.png
+-rw-r--r--   0        0        0      678 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png
+-rw-r--r--   0        0        0      545 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png
+-rw-r--r--   0        0        0      508 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pw.png
+-rw-r--r--   0        0        0      371 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/py.png
+-rw-r--r--   0        0        0      392 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/qa.png
+-rw-r--r--   0        0        0      273 2024-04-10 08:02:51.114920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ro.png
+-rw-r--r--   0        0        0      525 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png
+-rw-r--r--   0        0        0      306 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ru.png
+-rw-r--r--   0        0        0      385 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/rw.png
+-rw-r--r--   0        0        0      676 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png
+-rw-r--r--   0        0        0     1126 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png
+-rw-r--r--   0        0        0      974 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png
+-rw-r--r--   0        0        0      523 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png
+-rw-r--r--   0        0        0      284 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/se.png
+-rw-r--r--   0        0        0      592 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png
+-rw-r--r--   0        0        0     1253 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png
+-rw-r--r--   0        0        0      430 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/si.png
+-rw-r--r--   0        0        0      772 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png
+-rw-r--r--   0        0        0      308 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sl.png
+-rw-r--r--   0        0        0      503 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sm.png
+-rw-r--r--   0        0        0      404 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sn.png
+-rw-r--r--   0        0        0      506 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/so.png
+-rw-r--r--   0        0        0      446 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sr.png
+-rw-r--r--   0        0        0      650 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/st.png
+-rw-r--r--   0        0        0      438 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sv.png
+-rw-r--r--   0        0        0      495 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sy.png
+-rw-r--r--   0        0        0      535 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png
+-rw-r--r--   0        0        0      919 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png
+-rw-r--r--   0        0        0      274 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/td.png
+-rw-r--r--   0        0        0      481 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tg.png
+-rw-r--r--   0        0        0      307 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/th.png
+-rw-r--r--   0        0        0      399 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tj.png
+-rw-r--r--   0        0        0      739 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png
+-rw-r--r--   0        0        0      786 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png
+-rw-r--r--   0        0        0      678 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png
+-rw-r--r--   0        0        0      522 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/to.png
+-rw-r--r--   0        0        0      649 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png
+-rw-r--r--   0        0        0     1025 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png
+-rw-r--r--   0        0        0      423 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tw.png
+-rw-r--r--   0        0        0      767 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png
+-rw-r--r--   0        0        0      260 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ua.png
+-rw-r--r--   0        0        0      598 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png
+-rw-r--r--   0        0        0      627 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/us.png
+-rw-r--r--   0        0        0      588 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png
+-rw-r--r--   0        0        0      494 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/uz.png
+-rw-r--r--   0        0        0      485 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vc.png
+-rw-r--r--   0        0        0      364 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ve.png
+-rw-r--r--   0        0        0      997 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png
+-rw-r--r--   0        0        0      503 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vn.png
+-rw-r--r--   0        0        0      666 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png
+-rw-r--r--   0        0        0      428 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ws.png
+-rw-r--r--   0        0        0      744 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png
+-rw-r--r--   0        0        0      308 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ye.png
+-rw-r--r--   0        0        0      802 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/za.png
+-rw-r--r--   0        0        0      501 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/zm.png
+-rw-r--r--   0        0        0      620 2024-04-10 08:02:51.118920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png
+-rw-r--r--   0        0        0  1664449 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/login.jpg
+-rw-r--r--   0        0        0    92962 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/login.webp
+-rw-r--r--   0        0        0     6363 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/logo.svg
+-rw-r--r--   0        0        0     2354 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/sk.svg
+-rw-r--r--   0        0        0   170535 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js
+-rw-r--r--   0        0        0     4819 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js
+-rw-r--r--   0        0        0     1323 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js
+-rw-r--r--   0        0        0    39433 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js
+-rw-r--r--   0        0        0    87461 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js
+-rw-r--r--   0        0        0     3063 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js
+-rw-r--r--   0        0        0     7770 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js
+-rw-r--r--   0        0        0     1698 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js
+-rw-r--r--   0        0        0     1914 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/prices.js
+-rw-r--r--   0        0        0      932 2024-04-10 08:02:51.122920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/remove-me.js
+-rw-r--r--   0        0        0   387673 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js
+-rw-r--r--   0        0        0      527 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg
+-rw-r--r--   0        0        0      682 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg
+-rw-r--r--   0        0        0      386 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-one.svg
+-rw-r--r--   0        0        0      826 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg
+-rw-r--r--   0        0        0      444 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-three.svg
+-rw-r--r--   0        0        0      477 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Aiming.svg
+-rw-r--r--   0        0        0      677 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg
+-rw-r--r--   0        0        0      732 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg
+-rw-r--r--   0        0        0      734 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg
+-rw-r--r--   0        0        0     1138 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg
+-rw-r--r--   0        0        0     1238 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg
+-rw-r--r--   0        0        0     1209 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg
+-rw-r--r--   0        0        0      509 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-down.svg
+-rw-r--r--   0        0        0      522 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg
+-rw-r--r--   0        0        0      524 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg
+-rw-r--r--   0        0        0      511 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-up.svg
+-rw-r--r--   0        0        0      737 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg
+-rw-r--r--   0        0        0      988 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg
+-rw-r--r--   0        0        0      538 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg
+-rw-r--r--   0        0        0      524 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg
+-rw-r--r--   0        0        0      304 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card.svg
+-rw-r--r--   0        0        0      622 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg
+-rw-r--r--   0        0        0      532 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg
+-rw-r--r--   0        0        0      824 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg
+-rw-r--r--   0        0        0      540 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg
+-rw-r--r--   0        0        0      583 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg
+-rw-r--r--   0        0        0      979 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg
+-rw-r--r--   0        0        0      281 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-small.svg
+-rw-r--r--   0        0        0      280 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check.svg
+-rw-r--r--   0        0        0      544 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg
+-rw-r--r--   0        0        0      318 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-small.svg
+-rw-r--r--   0        0        0      318 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close.svg
+-rw-r--r--   0        0        0      429 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Column.svg
+-rw-r--r--   0        0        0      361 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-left.svg
+-rw-r--r--   0        0        0      347 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Corner-up-right.svg
+-rw-r--r--   0        0        0     1231 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg
+-rw-r--r--   0        0        0     2040 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg
+-rw-r--r--   0        0        0      611 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg
+-rw-r--r--   0        0        0      454 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete.svg
+-rw-r--r--   0        0        0      439 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-down.svg
+-rw-r--r--   0        0        0      433 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-left.svg
+-rw-r--r--   0        0        0      430 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-right.svg
+-rw-r--r--   0        0        0      439 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Double-up.svg
+-rw-r--r--   0        0        0      504 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-c.svg
+-rw-r--r--   0        0        0      296 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down-small.svg
+-rw-r--r--   0        0        0      280 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Down.svg
+-rw-r--r--   0        0        0      984 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg
+-rw-r--r--   0        0        0      386 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download.svg
+-rw-r--r--   0        0        0      898 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg
+-rw-r--r--   0        0        0      529 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg
+-rw-r--r--   0        0        0      442 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Excel-one.svg
+-rw-r--r--   0        0        0      636 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg
+-rw-r--r--   0        0        0     1432 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg
+-rw-r--r--   0        0        0      683 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg
+-rw-r--r--   0        0        0      575 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg
+-rw-r--r--   0        0        0      527 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg
+-rw-r--r--   0        0        0      570 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg
+-rw-r--r--   0        0        0      264 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Hamburger-button.svg
+-rw-r--r--   0        0        0      653 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg
+-rw-r--r--   0        0        0     1300 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg
+-rw-r--r--   0        0        0      536 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg
+-rw-r--r--   0        0        0      756 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg
+-rw-r--r--   0        0        0     1039 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg
+-rw-r--r--   0        0        0      501 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-c.svg
+-rw-r--r--   0        0        0      247 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-down.svg
+-rw-r--r--   0        0        0      235 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small-up.svg
+-rw-r--r--   0        0        0      301 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left-small.svg
+-rw-r--r--   0        0        0      272 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Left.svg
+-rw-r--r--   0        0        0      852 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg
+-rw-r--r--   0        0        0      856 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg
+-rw-r--r--   0        0        0      714 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg
+-rw-r--r--   0        0        0      566 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg
+-rw-r--r--   0        0        0      403 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lock.svg
+-rw-r--r--   0        0        0      381 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Login.svg
+-rw-r--r--   0        0        0      376 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Logout.svg
+-rw-r--r--   0        0        0      887 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg
+-rw-r--r--   0        0        0      574 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg
+-rw-r--r--   0        0        0      666 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg
+-rw-r--r--   0        0        0      647 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg
+-rw-r--r--   0        0        0      418 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail.svg
+-rw-r--r--   0        0        0     1757 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg
+-rw-r--r--   0        0        0      555 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg
+-rw-r--r--   0        0        0      487 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus-the-top.svg
+-rw-r--r--   0        0        0      148 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Minus.svg
+-rw-r--r--   0        0        0      541 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg
+-rw-r--r--   0        0        0      810 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg
+-rw-r--r--   0        0        0      771 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg
+-rw-r--r--   0        0        0      547 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg
+-rw-r--r--   0        0        0     1528 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg
+-rw-r--r--   0        0        0      638 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg
+-rw-r--r--   0        0        0      874 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg
+-rw-r--r--   0        0        0      656 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg
+-rw-r--r--   0        0        0      940 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg
+-rw-r--r--   0        0        0      891 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg
+-rw-r--r--   0        0        0     1485 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg
+-rw-r--r--   0        0        0      242 2024-04-10 08:02:51.126921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Plus.svg
+-rw-r--r--   0        0        0     2587 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg
+-rw-r--r--   0        0        0      938 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg
+-rw-r--r--   0        0        0     2362 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg
+-rw-r--r--   0        0        0      745 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg
+-rw-r--r--   0        0        0      362 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Reduce-one.svg
+-rw-r--r--   0        0        0      899 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg
+-rw-r--r--   0        0        0      507 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Return.svg
+-rw-r--r--   0        0        0      299 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora Filled.svg
+-rw-r--r--   0        0        0      504 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Rewora.svg
+-rw-r--r--   0        0        0      501 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-c.svg
+-rw-r--r--   0        0        0      280 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-down.svg
+-rw-r--r--   0        0        0      243 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small-up.svg
+-rw-r--r--   0        0        0      294 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right-small.svg
+-rw-r--r--   0        0        0      272 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Right.svg
+-rw-r--r--   0        0        0      687 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg
+-rw-r--r--   0        0        0      461 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Search.svg
+-rw-r--r--   0        0        0      534 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg
+-rw-r--r--   0        0        0      328 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-config.svg
+-rw-r--r--   0        0        0     2761 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg
+-rw-r--r--   0        0        0     1380 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg
+-rw-r--r--   0        0        0     2218 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg
+-rw-r--r--   0        0        0      812 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg
+-rw-r--r--   0        0        0      940 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg
+-rw-r--r--   0        0        0      497 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort Alt.svg
+-rw-r--r--   0        0        0      311 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-down.svg
+-rw-r--r--   0        0        0      334 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-amount-up.svg
+-rw-r--r--   0        0        0      360 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-one.svg
+-rw-r--r--   0        0        0      479 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort-three.svg
+-rw-r--r--   0        0        0      809 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg
+-rw-r--r--   0        0        0     1175 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg
+-rw-r--r--   0        0        0     1876 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg
+-rw-r--r--   0        0        0      323 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Switch.svg
+-rw-r--r--   0        0        0      525 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg
+-rw-r--r--   0        0        0      806 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg
+-rw-r--r--   0        0        0      485 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag.svg
+-rw-r--r--   0        0        0      490 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tips-one.svg
+-rw-r--r--   0        0        0      312 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/To-top.svg
+-rw-r--r--   0        0        0      476 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Transfer-data.svg
+-rw-r--r--   0        0        0     2485 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg
+-rw-r--r--   0        0        0     1003 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg
+-rw-r--r--   0        0        0      860 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg
+-rw-r--r--   0        0        0     1074 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg
+-rw-r--r--   0        0        0      592 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg
+-rw-r--r--   0        0        0      393 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Unlock.svg
+-rw-r--r--   0        0        0      504 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-c.svg
+-rw-r--r--   0        0        0      299 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up-small.svg
+-rw-r--r--   0        0        0      279 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Up.svg
+-rw-r--r--   0        0        0      988 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg
+-rw-r--r--   0        0        0      385 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload.svg
+-rw-r--r--   0        0        0      777 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg
+-rw-r--r--   0        0        0      888 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg
+-rw-r--r--   0        0        0      680 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg
+-rw-r--r--   0        0        0      584 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg
+-rw-r--r--   0        0        0      490 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-out.svg
+-rw-r--r--   0        0        0     1840 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_base.css
+-rw-r--r--   0        0        0     1889 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css
+-rw-r--r--   0        0        0     2825 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css
+-rw-r--r--   0        0        0    11128 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_components.css
+-rw-r--r--   0        0        0    14025 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css
+-rw-r--r--   0        0        0     3928 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css
+-rw-r--r--   0        0        0     5587 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css
+-rw-r--r--   0        0        0    18365 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css
+-rw-r--r--   0        0        0       58 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_tailwind_base.css
+-rw-r--r--   0        0        0      901 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css
+-rw-r--r--   0        0        0     4665 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css
+-rw-r--r--   0        0        0     1763 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css
+-rw-r--r--   0        0        0    10276 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css
+-rw-r--r--   0        0        0     4316 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css
+-rw-r--r--   0        0        0      719 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css
+-rw-r--r--   0        0        0    10087 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css
+-rw-r--r--   0        0        0     2388 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css
+-rw-r--r--   0        0        0     2485 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css
+-rw-r--r--   0        0        0      361 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/style.css
+-rw-r--r--   0        0        0    12215 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js
+-rw-r--r--   0        0        0     4736 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/chart.js
+-rw-r--r--   0        0        0     4615 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/choices.js
+-rw-r--r--   0        0        0      486 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/code.js
+-rw-r--r--   0        0        0    14259 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js
+-rw-r--r--   0        0        0     9299 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/main.js
+-rw-r--r--   0        0        0     3354 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js
+-rw-r--r--   0        0        0     1733 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/range.js
+-rw-r--r--   0        0        0     1570 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js
+-rw-r--r--   0        0        0     1186 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js
+-rw-r--r--   0        0        0     9972 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table.js
+-rw-r--r--   0        0        0      507 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/base_module.js
+-rw-r--r--   0        0        0    10561 2024-04-10 08:02:51.130921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js
+-rw-r--r--   0        0        0      929 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js
+-rw-r--r--   0        0        0      686 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js
+-rw-r--r--   0        0        0     4016 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js
+-rw-r--r--   0        0        0     7694 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js
+-rw-r--r--   0        0        0     6403 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js
+-rw-r--r--   0        0        0    11157 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js
+-rw-r--r--   0        0        0     2383 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js
+-rw-r--r--   0        0        0      954 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/translations.js
+-rw-r--r--   0        0        0     4245 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/utils.js
+-rw-r--r--   0        0        0    11036 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html
+-rw-r--r--   0        0        0     3200 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html
+-rw-r--r--   0        0        0      272 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/dashboard.html
+-rw-r--r--   0        0        0     3205 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html
+-rw-r--r--   0        0        0     2248 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     9511 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/list.html
+-rw-r--r--   0        0        0      122 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/media.html
+-rw-r--r--   0        0        0     1905 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html
+-rw-r--r--   0        0        0      109 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/partials/open_modal_attrs.html
+-rw-r--r--   0        0        0      857 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html
+-rw-r--r--   0        0        0     4549 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html
+-rw-r--r--   0        0        0      587 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html
+-rw-r--r--   0        0        0      334 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations-list.html
+-rw-r--r--   0        0        0     1285 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations.html
+-rw-r--r--   0        0        0       50 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     2398 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/login.html
+-rw-r--r--   0        0        0      864 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html
+-rw-r--r--   0        0        0      496 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/logout.html
+-rw-r--r--   0        0        0      485 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_done.html
+-rw-r--r--   0        0        0     1905 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html
+-rw-r--r--   0        0        0      503 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_complete.html
+-rw-r--r--   0        0        0     1310 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html
+-rw-r--r--   0        0        0      666 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html
+-rw-r--r--   0        0        0      621 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html
+-rw-r--r--   0        0        0     1397 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html
+-rw-r--r--   0        0        0       76 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/blank_base.html
+-rw-r--r--   0        0        0     1982 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/buttons.html
+-rw-r--r--   0        0        0      959 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/columns.html
+-rw-r--r--   0        0        0     2654 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/filters.html
+-rw-r--r--   0        0        0    10938 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/inputs.html
+-rw-r--r--   0        0        0     4543 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/config/view.html
+-rw-r--r--   0        0        0      900 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html
+-rw-r--r--   0        0        0     1096 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html
+-rw-r--r--   0        0        0      141 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/list_widget.html
+-rw-r--r--   0        0        0      720 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html
+-rw-r--r--   0        0        0     1071 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html
+-rw-r--r--   0        0        0      548 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html
+-rw-r--r--   0        0        0      645 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html
+-rw-r--r--   0        0        0      648 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html
+-rw-r--r--   0        0        0     1243 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html
+-rw-r--r--   0        0        0     1162 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html
+-rw-r--r--   0        0        0      614 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html
+-rw-r--r--   0        0        0     1212 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html
+-rw-r--r--   0        0        0      548 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html
+-rw-r--r--   0        0        0     1121 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/fonts.html
+-rw-r--r--   0        0        0      165 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/attrs.html
+-rw-r--r--   0        0        0      172 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/change_form_title.html
+-rw-r--r--   0        0        0    18710 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/components.html
+-rw-r--r--   0        0        0      229 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/fieldset.html
+-rw-r--r--   0        0        0     2227 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html
+-rw-r--r--   0        0        0      287 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/loading.html
+-rw-r--r--   0        0        0      304 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/loading_absolute.html
+-rw-r--r--   0        0        0      771 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html
+-rw-r--r--   0        0        0     1109 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/table_inline_delete_button.html
+-rw-r--r--   0        0        0     7592 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html
+-rw-r--r--   0        0        0    13850 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html
+-rw-r--r--   0        0        0     3046 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html
+-rw-r--r--   0        0        0    18190 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html
+-rw-r--r--   0        0        0      308 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/cms/translations_status_row.html
+-rw-r--r--   0        0        0     3002 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html
+-rw-r--r--   0        0        0    18834 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html
+-rw-r--r--   0        0        0     1909 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html
+-rw-r--r--   0        0        0    15189 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html
+-rw-r--r--   0        0        0     9194 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/navigation.html
+-rw-r--r--   0        0        0      825 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html
+-rw-r--r--   0        0        0      121 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_close.html
+-rw-r--r--   0        0        0      276 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_error.html
+-rw-r--r--   0        0        0      268 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_info.html
+-rw-r--r--   0        0        0      323 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_success.html
+-rw-r--r--   0        0        0      323 2024-04-10 08:02:51.134920 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_warning.html
+-rw-r--r--   0        0        0     1507 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html
+-rw-r--r--   0        0        0     1928 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal_content.html
+-rw-r--r--   0        0        0      543 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sb_admin_base.html
+-rw-r--r--   0        0        0     3253 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html
+-rw-r--r--   0        0        0      817 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html
+-rw-r--r--   0        0        0    59910 2024-04-10 08:03:14.099017 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg
+-rw-r--r--   0        0        0     3254 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/submit_line.html
+-rw-r--r--   0        0        0      577 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html
+-rw-r--r--   0        0        0     2815 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/array.html
+-rw-r--r--   0        0        0      172 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/attrs.html
+-rw-r--r--   0        0        0     2550 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html
+-rw-r--r--   0        0        0      232 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox.html
+-rw-r--r--   0        0        0       51 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_option.html
+-rw-r--r--   0        0        0     1578 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html
+-rw-r--r--   0        0        0      542 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html
+-rw-r--r--   0        0        0     2435 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html
+-rw-r--r--   0        0        0      345 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/code.html
+-rw-r--r--   0        0        0      160 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/date.html
+-rw-r--r--   0        0        0       44 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/datetime.html
+-rw-r--r--   0        0        0       43 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/email.html
+-rw-r--r--   0        0        0       44 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/file.html
+-rw-r--r--   0        0        0       44 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/hidden.html
+-rw-r--r--   0        0        0      148 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/includes/field_label.html
+-rw-r--r--   0        0        0      148 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/includes/help_text.html
+-rw-r--r--   0        0        0      443 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/includes/simple_field_label.html
+-rw-r--r--   0        0        0      185 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/input.html
+-rw-r--r--   0        0        0      209 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/input_option.html
+-rw-r--r--   0        0        0       50 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/multiple_hidden.html
+-rw-r--r--   0        0        0      329 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/multiwidget.html
+-rw-r--r--   0        0        0      159 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/number.html
+-rw-r--r--   0        0        0      585 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/password.html
+-rw-r--r--   0        0        0      363 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/radio.html
+-rw-r--r--   0        0        0       51 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/radio_option.html
+-rw-r--r--   0        0        0      216 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/read_only_password_hash.html
+-rw-r--r--   0        0        0      496 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/select.html
+-rw-r--r--   0        0        0       50 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/select_date.html
+-rw-r--r--   0        0        0      123 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/select_option.html
+-rw-r--r--   0        0        0       50 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/splitdatetime.html
+-rw-r--r--   0        0        0       50 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/splithiddendatetime.html
+-rw-r--r--   0        0        0      160 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/text.html
+-rw-r--r--   0        0        0      257 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/textarea.html
+-rw-r--r--   0        0        0      160 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/time.html
+-rw-r--r--   0        0        0      280 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/toggle.html
+-rw-r--r--   0        0        0      160 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/url.html
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templatetags/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templatetags/base.py
+-rw-r--r--   0        0        0     4179 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/templatetags/sb_admin_tags.py
+-rw-r--r--   0        0        0       17 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/urls.py
+-rw-r--r--   0        0        0     1343 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/__init__.py
+-rw-r--r--   0        0        0     1495 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/dashboard_view.py
+-rw-r--r--   0        0        0      954 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/global_filter_view.py
+-rw-r--r--   0        0        0      292 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/media_view.py
+-rw-r--r--   0        0        0    20254 2024-04-10 08:02:51.138921 django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/translations_view.py
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 django_smartbase_admin-0.2.9/PKG-INFO
```

### Comparing `django_smartbase_admin-0.2.7/LICENSE.md` & `django_smartbase_admin-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/pyproject.toml` & `django_smartbase_admin-0.2.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-smartbase-admin"
-version = "0.2.7"
+version = "0.2.9"
 description = ""
 authors = ["SmartBase <info@smartbase.sk>"]
 readme = "README.md"
 include = [
     "**/static/sb_admin/dist/**/*"
 ]
 
@@ -14,12 +14,13 @@
 django-ckeditor = "^6.7.1"
 django-admin-inline-paginator = "^0.4.0"
 django-nested-admin = "^4.0.2"
 xlsxwriter = "^3.2.0"
 django-widget-tweaks = "^1.5.0"
 django-filer = "^3.1.1"
 easy-thumbnails = {extras = ["svg"], version = "^2.8.5"}
+django-htmx = "^1.17.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/actions/admin_action_list.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/actions/admin_action_list.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/admin_base.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/admin_base.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/site.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/site.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/admin/widgets.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/actions.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/actions.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_base_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_base_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_entrypoint_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_entrypoint_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/admin_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/admin_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/configuration.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/configuration.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/const.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/const.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/dashboard.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/dashboard.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/fake_inline.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/fake_inline.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/field.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/field.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/field_formatter.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/field_formatter.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/filter_widgets.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/filter_widgets.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/menu_item.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/menu_item.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/engine/request.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/engine/request.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0001_initial.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0002_auto_20230402_2316.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0003_auto_20230402_2328.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/migrations/0004_alter_sbadminlistviewconfiguration_action_and_more.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/models.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/models.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/monkeypatch/fake_inline_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/configuration.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/configuration.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/thread_local.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/thread_local.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/translations.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/translations.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/views.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/views.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/services/xlsx_export.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/services/xlsx_export.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/postcss.config.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/colors.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/spacing.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/tailwind_config_partials/typography.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/build/webpack.common.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/css/codemirror/codemirror.min.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/css/codemirror/dracula.min.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/chart.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/chart.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -13705,15 +13705,15 @@
                 document.body.classList.add("js-ready");
                 [].slice.call(document.querySelectorAll('[data-bs-toggle="tooltip"]')).map((e => {
                     const t = e.closest(".js-tooltip");
                     return t ? new(d())(e, {
                         container: t
                     }) : null
                 })), this.initDropdowns(), document.addEventListener("formset:added", (e => {
-                    this.initDropdowns(e.target), this.initFileInputs(e.target)
+                    this.initDropdowns(e.target), this.initFileInputs(e.target), e.target !== e.target.parentNode.firstChild && e.target.parentNode.insertBefore(e.target, e.target.parentNode.firstChild)
                 })), document.addEventListener("openUrl", (e => {
                     var t;
                     window.open(e.detail.url, (null === (t = e.detail) || void 0 === t ? void 0 : t.target) || "_blank")
                 })), new u, new U, new X, new rn, new fn, new dn, new pn, document.addEventListener("click", (e => {
                     this.closeAlert(e), this.selectAll(e), this.saveState(e), this.fileDownload(e), this.passwordToggleFnc(e)
                 })), this.initFileInputs(), this.initAliasName(), this.handleLocationHashFromTabs()
             }
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/main_style.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/main_style.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.1.8 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}:root{--color-light:#fff;--color-transparent:transparent;--color-dark-900:#111827;--color-dark-800:#1f2937;--color-dark-700:#374151;--color-dark-600:#4b5563;--color-dark:#6b7280;--color-dark-400:#9ca3af;--color-dark-300:#d1d5db;--color-dark-200:#e5e7eb;--color-dark-100:#f3f4f6;--color-dark-50:#f9fafb;--color-dark-a:17 24 39;--color-primary-900:#d3f6f8;--color-primary-800:#003a3d;--color-primary-700:#006166;--color-primary-600:#008188;--color-primary:#00959d;--color-primary-400:#00c2cc;--color-primary-300:#59d3da;--color-primary-200:#99e7eb;--color-primary-100:#d3f6f8;--color-primary-50:#edfafb;--color-secondary-900:#3d2500;--color-secondary-800:#7a4901;--color-secondary-700:#a26201;--color-secondary-600:#cb7a01;--color-secondary:#f18f01;--color-secondary-400:#fea520;--color-secondary-300:#feb548;--color-secondary-200:#fec671;--color-secondary-100:#ffdeae;--color-secondary-50:#fff7eb;--color-success-900:#064e3b;--color-success-800:#065f46;--color-success-700:#047857;--color-success-600:#059669;--color-success:#10b981;--color-success-400:#34d399;--color-success-300:#6ee7b7;--color-success-200:#a7f3d0;--color-success-100:#d1fae5;--color-success-50:#d1fae5;--color-warning-900:#78350f;--color-warning-800:#78350f;--color-warning-700:#b45309;--color-warning-600:#d97706;--color-warning:#f59e0b;--color-warning-400:#fbbf24;--color-warning-300:#fcd34d;--color-warning-200:#fde68a;--color-warning-100:#fef3c7;--color-warning-50:#fffbeb;--color-negative-900:#7f1d1d;--color-negative-800:#991b1b;--color-negative-700:#b91c1c;--color-negative-600:#dc2626;--color-negative:#ef4444;--color-negative-400:#f87171;--color-negative-300:#fca5a5;--color-negative-200:#fecaca;--color-negative-100:#fee2e2;--color-negative-50:#fef2f2;--color-notice-900:#0c4a6e;--color-notice-800:#075985;--color-notice-700:#0369a1;--color-notice-600:#0369a1;--color-notice:#0284c7;--color-notice-400:#0ea5e9;--color-notice-300:#38bdf8;--color-notice-200:#7dd3fc;--color-notice-100:#bae6fd;--color-notice-50:#e0f2fe}html{scroll-behavior:smooth}body{background-color:var(--color-dark-100);color:var(--color-dark);font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol}svg{fill:currentColor;display:inline-flex}label[for]{cursor:pointer}hr{border-color:var(--color-dark-200)}small{font-size:.75rem;line-height:1.25rem}a{cursor:pointer;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}a.link,a[href]:hover{color:var(--color-primary)}a[aria-disabled=true]{cursor:not-allowed;pointer-events:none}select{-webkit-appearance:none;-moz-appearance:none;appearance:none;cursor:pointer}button:disabled{pointer-events:none}input[type=submit]{cursor:pointer}.scrollbar-measure{height:100px;overflow:scroll;position:absolute;top:-9999px;width:100px}.custom-scrollbar::-webkit-scrollbar,.tabulator .tabulator-tableholder::-webkit-scrollbar{height:9px;width:9px}.custom-scrollbar::-webkit-scrollbar-track,.tabulator .tabulator-tableholder::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.custom-scrollbar::-webkit-scrollbar-thumb,.tabulator .tabulator-tableholder::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.custom-scrollbar:hover::-webkit-scrollbar-thumb,.tabulator .tabulator-tableholder:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.outline{outline-style:solid;outline-width:1px}:focus-visible{outline:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.btn{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.btn>span{-webkit-box-orient:vertical;-webkit-line-clamp:2;display:-webkit-box;margin-right:auto;overflow:hidden}.btn>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.btn:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.btn:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);color:var(--color-dark-900)}.btn:focus,.btn:not(:disabled):hover:active{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color)}.btn:focus-visible{outline:none}.btn:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.btn-primary{background-color:var(--color-primary);border-color:var(--color-primary);color:var(--color-light)}.btn-primary:not(:disabled):hover{background-color:var(--color-primary-600);border-color:var(--color-primary-600);color:var(--color-light)}.btn-primary:not(:disabled):hover:active{background-color:var(--color-primary-700);border-color:var(--color-primary-700);color:var(--color-light)}.btn-primary:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-primary:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-primary.btn-empty{background-color:var(--color-primary-50);color:var(--color-primary)}.btn-primary.btn-empty:not(:disabled):hover,.btn-primary.btn-empty:not(:disabled):hover:active{background-color:var(--color-primary-100);color:var(--color-primary)}.btn-primary-light{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-primary-50);border-color:var(--color-transparent);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-primary)}.btn-primary-light:not(:disabled):hover,.btn-primary-light:not(:disabled):hover:active{background-color:var(--color-primary-100);border-color:var(--color-transparent)}.btn-primary-light:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-primary-light:disabled{background-color:var(--color-transparent);border-color:var(--color-transparent)}.btn-secondary{background-color:var(--color-secondary);border-color:var(--color-secondary);color:var(--color-dark-900)}.btn-secondary:not(:disabled):hover{background-color:var(--color-secondary-600);border-color:var(--color-secondary-600);color:var(--color-dark-900)}.btn-secondary:not(:disabled):hover:active{background-color:var(--color-secondary-700);border-color:var(--color-secondary-700)}.btn-secondary:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-secondary:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-destructive{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-negative-300);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-negative)}.btn-destructive:not(:disabled):hover{background-color:var(--color-negative-50);border-color:var(--color-negative-400);color:var(--color-negative)}.btn-destructive:not(:disabled):hover:active{background-color:var(--color-negative-100);border-color:var(--color-negative-400);color:var(--color-negative)}.btn-destructive:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-destructive:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-empty{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent);border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-empty:not(:disabled):hover{background-color:rgb(var(--color-dark-a)/.05)}.btn-empty:not(:disabled):hover:active{background-color:rgb(var(--color-dark-a)/.1)}.btn-empty:disabled{background-color:var(--color-transparent);color:var(--color-dark)}.btn-small{height:2rem;padding-left:.75rem;padding-right:.75rem}.btn-small>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.btn-small>svg{height:1rem;width:1rem}.btn-tiny{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);font-size:.75rem;height:1.5rem;line-height:1rem;padding-left:.5rem;padding-right:.5rem}.btn-tiny>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.btn-tiny>svg{height:1rem;width:1rem}.btn-tiny.btn-destructive{background-color:var(--color-negative-50);border-style:none}.btn-tiny.btn-destructive:not(:disabled):hover,.btn-tiny.btn-destructive:not(:disabled):hover:active{background-color:var(--color-negative-100)}@media (max-width:767px){.btn-icon{justify-content:center!important;padding-left:0;padding-right:0;width:2.5rem}.btn-icon>span{display:none}}.input{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.input~.error{color:var(--color-negative)}.input:hover{border-color:var(--color-dark-400)}.input:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.input:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.input::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.input::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.input.field-valid{border-color:var(--color-success)}.input.field-valid~.success{display:block}.input.field-error{border-color:var(--color-negative)}.input.field-error~.error{display:block}input.input:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.input:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.input:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.input:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.input{height:auto}.input-file{align-items:center;border-color:var(--color-dark-300);border-radius:6px;border-style:dashed;border-width:1px;display:flex;padding:1rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.input-file input[type=file]{cursor:pointer;height:100%;left:0;opacity:0;position:absolute;top:0;width:100%}.input-file .input-file-upload-icon{background-color:var(--color-dark-100);transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.input-file:not(.filled):hover{background-color:var(--color-primary-50);border-color:var(--color-primary)}.input-file:not(.filled):hover .input-file-upload-icon{background-color:var(--color-light);color:var(--color-primary)}.input-file:not(.filled) .js-input-file-filled{display:none}.flatpickr-day.input-file:not(.filled) .js-input-file-filled{visibility:hidden}.input-file:not(.filled) .js-input-file-image{display:none}.flatpickr-day.input-file:not(.filled) .js-input-file-image{visibility:hidden}.input-file.filled{border-style:solid}.input-file.filled input[type=file]{z-index:-1}.input-file.filled .js-input-file-empty{display:none}.flatpickr-day.input-file.filled .js-input-file-empty{visibility:hidden}.checkbox,.radio{opacity:0;position:absolute;top:0;z-index:-1}.checkbox~label,.radio~label{display:flex;font-size:.875rem;line-height:1.25rem;min-height:1.25rem;padding-left:2rem;position:relative}.checkbox~label:after,.checkbox~label:before,.radio~label:after,.radio~label:before{content:"";display:block;position:absolute}.checkbox~label:before,.radio~label:before{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);height:1.25rem;left:0;outline-color:var(--color-transparent);outline-offset:2px;outline-style:solid;outline-width:2px;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:1.25rem}.checkbox:not(:disabled):hover+label:before,.radio:not(:disabled):hover+label:before{border-color:var(--color-dark-400)}.checkbox:not(:disabled):hover+label:after,.radio:not(:disabled):hover+label:after{opacity:1}.checkbox:not(:disabled):focus+label:before,.radio:not(:disabled):focus+label:before{outline-color:var(--color-primary)}.checkbox:disabled+label,.radio:disabled+label{cursor:not-allowed}.checkbox:disabled+label:before,.radio:disabled+label:before{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-300);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.checkbox:checked+label:after,.radio:checked+label:after{opacity:1}.checkbox:checked:not(:disabled)+label:before,.radio:checked:not(:disabled)+label:before{background-color:var(--color-primary);border-color:var(--color-primary)}.checkbox:checked:not(:disabled):hover+label:before,.radio:checked:not(:disabled):hover+label:before{background-color:var(--color-primary-600);border-color:var(--color-primary-600)}.checkbox:checked:not(:disabled):hover+label:after,.radio:checked:not(:disabled):hover+label:after{opacity:1}.checkbox~label:before{border-radius:6px}.checkbox~label:after{height:1.125rem;height:18px;left:1px;opacity:0;top:1px;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);width:1.125rem;width:18px}.checkbox:checked:not(:disabled):hover+label:after,.checkbox~label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m20.707 7.707-10 10a1 1 0 0 1-1.414 0l-5-5 1.414-1.414L10 15.586l9.293-9.293 1.414 1.414Z' fill='%23E5E7EB'/%3E%3C/svg%3E")}.checkbox:indeterminate+label:before{background-color:var(--color-primary);border-color:var(--color-primary)}.checkbox:indeterminate+label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M19.25 13h-14v-2h14v2Z' fill='%23E5E7EB'/%3E%3C/svg%3E");opacity:1}.checkbox:indeterminate:not(:disabled):hover+label:before{background-color:var(--color-primary-600);border-color:var(--color-primary-600)}.checkbox-delete+label{align-items:center;color:var(--color-dark-300);display:flex;height:100%;justify-content:center;padding:.5rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:100%}.checkbox-delete+label:after,.checkbox-delete+label:before{display:none}.flatpickr-day .checkbox-delete+label:after,.flatpickr-day.checkbox-delete+label:before{visibility:hidden}.checkbox-delete+label:hover{color:var(--color-dark-400)}.checkbox-delete:checked+label{color:var(--color-negative)}.radio+label{align-items:center;color:var(--color-dark-900);display:flex;justify-content:space-between;padding:.75rem 1rem}.radio+label:before{display:none}.flatpickr-day.radio+label:before{visibility:hidden}.radio+label:after{display:none;flex-shrink:0;height:1rem;margin-left:1rem;position:relative;width:1rem}.flatpickr-day.radio+label:after{visibility:hidden}.radio+label:after{background:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='%23009FA7' fill-rule='evenodd' clip-rule='evenodd' d='M8.437 17.09 20.794 4.79l1.411 1.418-13.062 13a1 1 0 0 1-1.411 0l-5.938-5.91 1.411-1.417 5.232 5.207Z'/%3E%3C/svg%3E")}.radio:checked+label,.radio:hover+label{background-color:var(--color-dark-100)}.radio:checked+label:after{display:flex}input:not([type=number])::-webkit-inner-spin-button,input:not([type=number])::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.checkbox.checkbox-icon+label{color:var(--color-dark-300);padding-left:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.checkbox.checkbox-icon+label:after,.checkbox.checkbox-icon+label:before{display:none}.flatpickr-day .checkbox.checkbox-icon+label:after,.flatpickr-day.checkbox.checkbox-icon+label:before{visibility:hidden}.checkbox.checkbox-icon+label:hover{color:var(--color-dark-700)}.checkbox.checkbox-icon:not(:checked)+label>svg:last-child{display:none}.flatpickr-day.checkbox.checkbox-icon:not(:checked)+label>svg:last-child{visibility:hidden}.checkbox.checkbox-icon:checked+label>svg:first-child{display:none}.flatpickr-day.checkbox.checkbox-icon:checked+label>svg:first-child{visibility:hidden}input[type=search]{padding-right:0}input[type=search]::-webkit-search-cancel-button{-webkit-appearance:none;background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg width='24' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m12 13.414 4.293 4.293 1.414-1.414L13.414 12l4.293-4.293-1.414-1.414L12 10.586 7.707 6.293 6.293 7.707 10.586 12l-4.293 4.293 1.414 1.414L12 13.414Z' fill='%236B7280'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;cursor:pointer;height:40px;width:40px}select{-webkit-appearance:none;-moz-appearance:none;background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg fill='%236B7280' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M12.64 18.142a.904.904 0 0 1-1.389 0l-3.04-3.649a.904.904 0 0 1 .694-1.482h6.08a.904.904 0 0 1 .695 1.482l-3.04 3.649ZM11.252 5.325a.904.904 0 0 1 1.388 0l3.04 3.648a.904.904 0 0 1-.694 1.482h-6.08a.904.904 0 0 1-.695-1.482l3.04-3.648Z'/%3E%3C/svg%3E");background-position:right 10px top 50%;background-repeat:no-repeat;background-size:1.25rem;cursor:pointer}select.input{padding-right:2rem}.dropdown-menu{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);display:none;font-size:.875rem;left:0;line-height:1.25rem;max-height:18.75rem;position:absolute;top:100%;width:14rem;z-index:20}.flatpickr-day.dropdown-menu{visibility:hidden}.dropdown-menu{flex-direction:column;white-space:normal}.dropdown-menu>ul::-webkit-scrollbar{height:9px;width:9px}.dropdown-menu>ul::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.dropdown-menu>ul::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.dropdown-menu>ul:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.dropdown-menu>ul{overflow-x:hidden;overflow-y:auto}.dropdown-menu:not(.show).transition-width{display:flex;width:0}.dropdown-menu:not(.show).transition-height{display:flex;height:0}.dropdown-menu.show,.dropdown-menu:not(.show).fade{display:flex}.dropdown-menu-link{color:var(--color-dark-700);cursor:pointer;display:flex;padding:.75rem 1rem;transition-duration:.1s;transition-property:color,background-color;transition-timing-function:ease-in;white-space:nowrap}.dropdown-menu-link:hover{background-color:var(--color-dark-100);color:var(--color-dark-900)}.dropdown-menu-link:focus{color:var(--color-primary)}.dropdown-menu hr{border-color:var(--color-dark-200);border-width:1px;margin-bottom:.25rem;margin-top:.25rem}.btn[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.btn[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.btn[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dropdown-menu-datepicker{@appy w-auto h-auto max-w-none max-h-none}.dropdown-menu-datepicker .flatpickr-calendar{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);margin-left:-.75rem;margin-right:-.75rem}input[type=checkbox].toggle{opacity:0;position:absolute;top:0;z-index:-1}input[type=checkbox].toggle~label{color:var(--color-dark-900);display:flex;font-size:.875rem;font-weight:500;line-height:1.25rem;padding-left:3.5rem;position:relative;top:.125rem}input[type=checkbox].toggle+label{background-color:var(--color-dark-200);border-radius:9999px;display:block;height:1.5rem;left:0;outline-color:var(--color-transparent);outline-offset:2px;outline-style:solid;outline-width:2px;padding-left:0;position:absolute;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.75rem}input[type=checkbox].toggle+label:after,input[type=checkbox].toggle+label:before{content:"";display:block;position:absolute}input[type=checkbox].toggle+label:before{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-radius:9999px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);height:1.25rem;left:.125rem;top:.125rem;transition:left .15s ease-in-out;width:1.25rem}input[type=checkbox].toggle+label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m20.707 7.707-10 10a1 1 0 0 1-1.414 0l-5-5 1.414-1.414L10 15.586l9.293-9.293 1.414 1.414Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-size:1rem;height:1.25rem;left:.125rem;opacity:0;top:.125rem;transition:opacity .15s ease-in-out,left .15s ease-in-out;width:1.25rem}input[type=checkbox].toggle:not(:disabled):hover+label{background-color:var(--color-dark-300)}input[type=checkbox].toggle:not(:disabled):focus+label{outline-color:var(--color-primary)}input[type=checkbox].toggle:checked+label{background-color:var(--color-primary)}input[type=checkbox].toggle:checked+label:after,input[type=checkbox].toggle:checked+label:before{left:calc(100% - 1.375rem);opacity:1}input[type=checkbox].toggle:checked:not(:disabled):hover+label{background-color:var(--color-primary-600)}input[type=checkbox].toggle:checked:not(:disabled):hover+label:after{opacity:.5}input[type=checkbox].toggle~p{font-size:.875rem;line-height:1.25rem;margin-top:0;padding-left:3.5rem}.modal{display:none;height:100%;left:0;outline:0;overflow-x:hidden;overflow-y:auto;position:fixed;top:0;width:100%;z-index:1010}.modal-dialog{align-items:center;display:flex;height:100%;min-height:calc(100% - var(--modal-dialog-margin)*2);pointer-events:none;position:relative;width:auto}@media (min-width:576px){.modal-dialog{height:calc(100% - var(--modal-dialog-margin)*2);margin:var(--modal-dialog-margin)}}.modal.fade .modal-dialog{transform:translateY(-50px);transition:transform .15s ease-out}.modal.show .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog .modal-body{overflow-y:auto}.modal-dialog .modal-body::-webkit-scrollbar{height:9px;width:9px}.modal-dialog .modal-body::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.modal-dialog .modal-body::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.modal-dialog .modal-body:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}@media (min-width:576px){.modal-content{border-radius:6px}}.modal-content{background-clip:padding-box;background-color:#fff;display:flex;flex-direction:column;margin:0 auto;max-height:100%;outline:0;overflow:hidden;pointer-events:auto;position:relative;width:100%}@media (max-width:767px){.modal-content{height:100%}}.modal-backdrop{-webkit-backdrop-filter:blur(.5rem);backdrop-filter:blur(.5rem);background-color:rgb(var(--color-dark-a)/.5);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:1000}.modal-backdrop.fade{opacity:0}.modal-backdrop.show{opacity:1}.modal-header{align-items:center;border-bottom-width:1px;border-color:var(--color-dark-200);border-top-left-radius:6px;border-top-right-radius:6px;display:flex;flex-shrink:0;justify-content:space-between;padding:1rem}.modal-body{flex:1 1 auto;padding:1rem;position:relative}.modal-footer{align-items:center;border-bottom-left-radius:6px;border-bottom-right-radius:6px;border-color:var(--color-dark-200);border-top-width:1px;display:flex;flex-shrink:0;flex-wrap:wrap;gap:.5rem;justify-content:flex-end;padding:1rem}@media (min-width:576px){.modal-dialog{height:calc(100% - var(--modal-dialog-margin-y-sm-up)*2);margin:var(--modal-dialog-margin-y-sm-up) auto;max-width:45rem;min-height:calc(100% - var(--modal-dialog-margin-y-sm-up)*2)}.modal.modal-small>.modal-dialog{max-width:23rem}}.tooltip{word-wrap:break-word;display:block;font-size:.75rem;line-height:1rem;opacity:0;padding-bottom:.5rem;padding-top:.5rem;position:absolute;z-index:10}.tooltip.show{opacity:1}.tooltip .tooltip-arrow{display:block;height:.5rem;position:absolute;width:1rem}.tooltip .tooltip-arrow:before{border-color:transparent;border-style:solid;content:"";position:absolute}&[data-popper-placement^=top] .tooltip-arrow,.tooltip.bs-tooltip-top .tooltip-arrow{bottom:0}&[data-popper-placement^=top] .tooltip-arrow:before,.tooltip.bs-tooltip-top .tooltip-arrow:before{border-top-color:rgb(var(--color-dark-a)/90%);border-width:.5rem .5rem 0;top:-1px}&[data-popper-placement^=bottom] .tooltip-arrow,.tooltip.bs-tooltip-bottom .tooltip-arrow{top:0}&[data-popper-placement^=bottom] .tooltip-arrow:before,.tooltip.bs-tooltip-bottom .tooltip-arrow:before{border-bottom-color:rgb(var(--color-dark-a)/90%);border-width:0 .5rem .5rem;bottom:-1px}&[data-popper-placement^=right],.tooltip.bs-tooltip-end{padding:0 .5rem}&[data-popper-placement^=right] .tooltip-arrow,.tooltip.bs-tooltip-end .tooltip-arrow{height:.1rem;left:0;width:.5rem}&[data-popper-placement^=right] .tooltip-arrow:before,.tooltip.bs-tooltip-end .tooltip-arrow:before{border-right-color:rgb(var(--color-dark-a)/90%);border-width:.5rem .5rem .5rem 0;right:-1px}&[data-popper-placement^=left],.tooltip.bs-tooltip-start{padding:0 .5rem}&[data-popper-placement^=left] .tooltip-arrow,.tooltip.bs-tooltip-start .tooltip-arrow{height:.1rem;right:0;width:.5rem}&[data-popper-placement^=left] .tooltip-arrow:before,.tooltip.bs-tooltip-start .tooltip-arrow:before{border-left-color:rgb(var(--color-dark-a)/90%);border-width:.5rem 0 .5rem .5rem;left:-1px}.tooltip-inner{--tw-shadow:0 2px 4px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 2px 4px 0 var(--tw-shadow-color);background-color:rgb(var(--color-dark-a)/.9);border-radius:6px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-light);max-width:200px;padding:.5rem}.card{background-color:var(--color-light);border-color:var(--color-dark-200);border-width:1px;min-width:0;padding:1.25rem}@media (min-width:576px){.card{border-radius:6px}}@media (min-width:768px){.card{padding:1.5rem}}@media (max-width:575px){.card{border-bottom-width:0;padding-bottom:2rem;padding-top:2rem}}.card>header{align-items:center;display:flex;font-size:1.125rem;font-weight:600;line-height:1.25rem;margin-bottom:1.5rem}.column-widget-columns>li{align-items:center;display:flex;padding:.5rem .75rem;position:relative}@media (pointer:fine){.column-widget-columns>li .checkbox.checkbox-icon:not(:checked)+label{opacity:0}}.column-widget-columns>li:hover .checkbox.checkbox-icon+label{opacity:1}.tab-pane:not(.active){display:none}.flatpickr-day.tab-pane:not(.active){visibility:hidden}.collapse-btn,.collapse-horizontal-btn{align-items:center;display:flex;justify-content:space-between}.collapse-btn svg:last-child,.collapse-horizontal-btn svg:last-child{transition:transform .2s}.collapse-btn:not(.collapsed) svg:last-child,.collapse-horizontal-btn:not(.collapsed) svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.collapse-horizontal.collapsed{max-width:0;opacity:0;overflow:hidden;transition:max-width .2s ease-in-out,opacity .2s ease-in}.collapse-horizontal.\!collapsed{max-width:0!important;opacity:0!important;overflow:hidden!important;transition:max-width .2s ease-in-out,opacity .2s ease-in!important}.bg-filter{background-color:rgb(var(--color-dark-a)/.3);height:100vh;opacity:0;transition:opacity .3s ease-in-out,z-index 0s linear .3s;width:100vw;z-index:-1}.bg-filter,.sidebar{left:0;position:fixed;top:0}.sidebar{--tw-translate-x:-100%;height:100%;overflow:hidden;z-index:51}.sidebar,.sidebar.active{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.sidebar.active{--tw-translate-x:0}.sidebar.active+.bg-filter{opacity:1;transition:opacity .3s ease-in-out,z-index 0s linear 0s;z-index:50}.menu-item{border-radius:8px;color:var(--color-dark-900)}.menu-item a,.menu-item>div{display:flex}.menu-item>a:hover svg{color:var(--color-primary)}.menu-item span{display:inline-block;line-height:1.25rem}.menu-item span:first-letter{text-transform:capitalize}.menu-item svg{color:var(--color-dark)}.menu-item .collapse-btn>a{width:calc(100% - 2.25rem)}.menu-item .collapse-btn:hover{color:var(--color-primary)}.menu-item .collapse-btn:not(.collapsed)>a{font-weight:600}.menu-item .collapse-btn:not(.collapsed)>a>svg,.menu-item.active{color:var(--color-primary)}.menu-item.active{background-color:var(--color-light);font-weight:600}.menu-item.active svg{color:var(--color-primary)}.key{display:inline-flex;font-size:.75rem;line-height:1.25rem;margin-bottom:.125rem;padding-left:.375rem;padding-right:.375rem;position:relative}.key,.key:after{border-color:var(--color-dark-300);border-radius:6px;border-width:1px}.key:after{align-items:center;bottom:calc(-1px - .125rem);content:"";display:flex;justify-content:center;left:-1px;position:absolute;right:-1px;top:-1px}.badge{align-items:center;background-color:var(--color-notice-100);border-radius:9999px;color:var(--color-notice-700);display:inline-flex;font-size:.75rem;font-weight:500;line-height:1rem;padding:.125rem .5rem}.badge:before{background-color:currentColor;border-radius:9999px;content:"";height:.25rem;margin-right:.25rem;width:.25rem}.badge-large{padding:.25rem .625rem}.badge-large:before{height:.375rem;margin-right:.5rem;width:.375rem}.badge-simple:before{display:none}.flatpickr-day.badge-simple:before{visibility:hidden}.badge-positive{background-color:var(--color-success-100);color:var(--color-success-700)}.badge-warning{background-color:var(--color-warning-100);color:var(--color-warning-700)}.badge-negative{background-color:var(--color-negative-100);color:var(--color-negative-700)}.badge-neutral{background-color:var(--color-dark-200);color:var(--color-dark-600)}.badge-primary{background-color:var(--color-primary-100);color:var(--color-primary-700)}.nav-tabs{border-bottom-width:1px;border-color:var(--color-dark-200);display:flex;gap:.5rem;overflow-x:auto}.nav-tabs .tab-link{border-bottom:3px solid transparent;display:block;padding-bottom:calc(1rem - 3px);padding-left:1rem;padding-right:1rem;padding-top:1rem;transition-duration:.15s;transition-property:color,border;transition-timing-function:ease-in;white-space:nowrap}.nav-tabs .tab-link:hover{border-color:var(--color-dark-200)}.nav-tabs .tab-link.active{border-color:var(--color-primary);color:var(--color-primary)}.saved-filters{color:var(--color-dark-600);display:flex;font-size:.875rem;font-weight:500;gap:.5rem;line-height:1.25rem}.saved-filters>li button{align-items:center;border-radius:6px;cursor:pointer;display:flex;height:2.5rem;padding:.5rem 1rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.saved-filters>li button:not(:disabled):hover{background-color:var(--color-dark-100)}.saved-filters>li button:not(:disabled).active{background-color:var(--color-primary-100);color:var(--color-primary-600)}.saved-filters>li button:disabled{opacity:0}.saved-filters>li button.changed span:after{content:"*";padding-left:2px}.alert{border-radius:8px;font-size:.875rem;line-height:1.25rem;padding:1rem}#save-view-modal-button:disabled{display:none}.flatpickr-day#save-view-modal-button:disabled{visibility:hidden}#filters-collapse-button:not(.collapsed){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.django-ckeditor-widget{display:block!important;flex:1}.django-ckeditor-widget>.cke{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);width:auto!important}.django-ckeditor-widget>.cke,.django-ckeditor-widget>.cke>.cke_inner{border-radius:6px}.django-ckeditor-widget>.cke>.cke_inner>.cke_top{border-top-left-radius:6px;border-top-right-radius:6px}.django-ckeditor-widget>.cke>.cke_inner>.cke_bottom{border-bottom-left-radius:6px;border-bottom-right-radius:6px}.django-ckeditor-widget>textarea:-moz-read-only+.cke{height:100%}.django-ckeditor-widget>textarea:read-only+.cke{height:100%}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner{height:100%}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner{height:100%}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_bottom,.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_top{display:none}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_bottom,.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_top{display:none}.flatpickr-day .django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_bottom,.flatpickr-day.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_top{visibility:hidden}.flatpickr-day .django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_bottom,.flatpickr-day.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_top{visibility:hidden}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_contents{border-radius:6px;height:100%!important}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_contents{border-radius:6px;height:100%!important}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_contents>.cke_wysiwyg_frame{background-color:var(--color-dark-50)}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_contents>.cke_wysiwyg_frame{background-color:var(--color-dark-50)}.errorlist{color:var(--color-negative);font-size:.75rem;line-height:1rem;margin-top:.5rem}.filter-dropdown-button{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.filter-dropdown-button>span{-webkit-line-clamp:2;margin-right:auto}.filter-dropdown-button>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.filter-dropdown-button:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.filter-dropdown-button:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);color:var(--color-dark-900)}.filter-dropdown-button:focus,.filter-dropdown-button:not(:disabled):hover:active{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color)}.filter-dropdown-button:focus-visible{outline:none}.filter-dropdown-button:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.filter-dropdown-button{height:2rem;padding-left:.75rem;padding-right:.75rem}.filter-dropdown-button>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.filter-dropdown-button>svg{height:1rem;width:1rem}.filter-dropdown-button[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.filter-dropdown-button[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.filter-dropdown-button[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.filter-wrapper>.filter-dropdown-button.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.filter-dropdown-button.empty>svg:not(:last-child){visibility:hidden}.filter-dropdown-button{border-radius:9999px;position:relative}.tabulator-row .tabulator-cell .filter-dropdown-button+.btn{margin-left:.25rem}.djn-table>.djn-tbody td .filter-dropdown-button:not(.input-file-edit-btn){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rules-group-container .rules-group-header .filter-dropdown-button{height:2rem}.query-builder .rules-group-container .group-conditions label.filter-dropdown-button{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.filter-dropdown-button.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container .rule-header .filter-dropdown-button-group .btn{margin-right:0}.query-builder .filter-dropdown-button[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .filter-dropdown-button[data-delete] i{display:none}.flatpickr-day.query-builder .filter-dropdown-button[data-delete] i{visibility:hidden}.query-builder .filter-dropdown-button[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .filter-dropdown-button[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.filter-dropdown-button>svg:not(:last-child){--tw-translate-y:-50%;color:var(--color-dark);position:absolute;right:.75rem;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.filter-dropdown-button>svg:not(:last-child):hover{color:var(--color-dark-900)}.filter-dropdown-button>svg:last-child{visibility:hidden}.filter-dropdown-button.show>svg:not(:last-child){color:var(--color-primary)}.filter-dropdown-button.empty{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button.empty>svg:last-child{display:block;visibility:visible}.filter-dropdown-button.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-dropdown-button.empty>svg:not(:last-child){visibility:hidden}.filter-wrapper>.btn.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.btn.empty>svg:not(:last-child){visibility:hidden}.table-selected-rows-bar{align-items:center;background-color:var(--color-light);display:flex;height:3rem;left:0;margin-top:1px;overflow-x:auto;padding-bottom:.5rem;padding-right:1rem;padding-top:.5rem;position:absolute;right:0;top:100%}.table-selected-rows-bar.show{z-index:1}.copy-translations-button-wrapper{align-items:center;display:flex;margin-right:.75rem;padding-top:1.625rem;position:absolute;right:100%;top:0;z-index:1}.django-ckeditor-widget+.copy-translations-button-wrapper{bottom:0;height:100%}.detail-view-action-bar:before{content:"";display:block;height:4.5rem}.detail-view-action-bar>div{--tw-shadow:0px -4px 16px 0px rgba(17,24,39,.08);--tw-shadow-colored:0px -4px 16px 0px var(--tw-shadow-color);align-items:center;background-color:var(--color-light);bottom:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);display:flex;left:0;padding:1rem 1.5rem;position:fixed;right:0;z-index:1}@media (min-width:1200px){.detail-view-action-bar>div{left:16.25rem}}.translations-status-fieldset{position:relative}.translations-status-fieldset>header{height:2rem}.translations-status-fieldset .translation-status-row:last-child{margin-bottom:0}.translations-status-fieldset:has(.is-empty){display:none}.mermaid .label{color:var(--color-dark-900)!important}.mermaid .node circle,.mermaid .node ellipse,.mermaid .node polygon,.mermaid .node rect{fill:var(--color-primary-100)!important;stroke:var(--color-primary-200)!important}.mermaid .mermaid_purchase_active .label{color:var(--color-light)!important}.cms-pagetree-section:after{clear:both;content:"";display:block}.page-loading{display:none}.page-loading.htmx-request{display:block}.page-loading .loader,.page-loading .loader:after{border-radius:50%;height:42px;width:42px}.page-loading .loader{animation:loading 1.1s linear infinite;border-color:var(--color-primary);border-left-color:var(--color-dark-300);border-width:4px;font-size:10px;text-indent:-9999em;transform:translateZ(0)}@keyframes loading{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.read-only-password-hash a{color:var(--color-primary)}.dropdown-btn.show{background-color:var(--color-dark-200)}.dropdown-menu{padding-bottom:0;padding-top:0}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.visible{visibility:visible}.\!visible{visibility:visible!important}.invisible{visibility:hidden}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{bottom:0;left:0;right:0;top:0}.top-0{top:0}.bottom-0{bottom:0}.left-0{left:0}.top-24{top:1.5rem}.right-24{right:1.5rem}.left-10{left:.625rem}.left-24{left:1.5rem}.right-0{right:0}.top-16{top:1rem}.right-16{right:1rem}.left-260{left:16.25rem}.top-1\/2{top:50%}.right-10{right:.625rem}.left-1\/2{left:50%}.z-1{z-index:1}.z-1000{z-index:1000}.order-1{order:1}.m-auto{margin:auto}.-m-8{margin:-.5rem}.m-10{margin:.625rem}.-my-2{margin-bottom:-.125rem;margin-top:-.125rem}.my-32{margin-bottom:2rem;margin-top:2rem}.mx-auto{margin-left:auto;margin-right:auto}.-mx-32{margin-left:-2rem;margin-right:-2rem}.-mx-24{margin-left:-1.5rem;margin-right:-1.5rem}.my-16{margin-bottom:1rem;margin-top:1rem}.mx-24{margin-left:1.5rem;margin-right:1.5rem}.-my-12{margin-bottom:-.75rem;margin-top:-.75rem}.mr-12{margin-right:.75rem}.ml-auto{margin-left:auto}.mr-8{margin-right:.5rem}.-mb-2{margin-bottom:-.125rem}.mt-2{margin-top:.125rem}.mb-24{margin-bottom:1.5rem}.mt-auto{margin-top:auto}.ml-8{margin-left:.5rem}.mr-16{margin-right:1rem}.-mt-16{margin-top:-1rem}.mt-8{margin-top:.5rem}.mb-16{margin-bottom:1rem}.mb-4{margin-bottom:.25rem}.mt-16{margin-top:1rem}.ml-4{margin-left:.25rem}.mb-8{margin-bottom:.5rem}.ml-2{margin-left:.125rem}.mt-24{margin-top:1.5rem}.ml-24{margin-left:1.5rem}.-mb-24{margin-bottom:-1.5rem}.-mt-8{margin-top:-.5rem}.mr-auto{margin-right:auto}.ml-28{margin-left:1.75rem}.ml-16{margin-left:1rem}.mr-10{margin-right:.625rem}.mb-10{margin-bottom:.625rem}.ml-10{margin-left:.625rem}.mb-30{margin-bottom:1.875rem}.-mr-8{margin-right:-.5rem}.mr-4{margin-right:.25rem}.block{display:block}.\!block{display:block!important}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.\!inline-flex{display:inline-flex!important}.table{display:table}.grid{display:grid}.contents{display:contents}.hidden{display:none}.\!hidden{display:none!important}.h-24{height:1.5rem}.h-32{height:2rem}.h-20{height:1.25rem}.h-full{height:100%}.h-16{height:1rem}.h-10{height:.625rem}.h-18{height:1.125rem}.h-56{height:3.5rem}.h-screen{height:100vh}.h-6{height:.375rem}.h-40{height:2.5rem}.h-12{height:.75rem}.h-64{height:4rem}.h-36{height:2.25rem}.max-h-432{max-height:27rem}.max-h-screen{max-height:100vh}.max-h-40{max-height:2.5rem}.max-h-none{max-height:none}.min-h-56{min-height:3.5rem}.min-h-72{min-height:4.5rem}.min-h-full{min-height:100%}.min-h-screen{min-height:100vh}.min-h-32{min-height:2rem}.min-h-40{min-height:2.5rem}.w-24{width:1.5rem}.w-auto{width:auto}.w-32{width:2rem}.w-260{width:16.25rem}.w-20{width:1.25rem}.w-full{width:100%}.w-16{width:1rem}.w-248{width:15.5rem}.w-1\/2{width:50%}.w-1\/3{width:33.333334%}.w-1\/4{width:25%}.w-1\/5{width:20%}.w-1\/6{width:16.666667%}.w-40{width:2.5rem}.w-10{width:.625rem}.w-56{width:3.5rem}.w-8{width:.5rem}.w-6{width:.375rem}.w-192{width:12rem}.w-12{width:.75rem}.w-64{width:4rem}.\!w-full{width:100%!important}.w-36{width:2.25rem}.w-18{width:1.125rem}.min-w-0{min-width:0}.max-w-1180{max-width:73.75rem}.max-w-370{max-width:23.125rem}.flex-1{flex:1 1 0%}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-y-1\/2{--tw-translate-y:-50%}.-translate-x-1\/2,.-translate-y-1\/2{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.-translate-x-1\/2{--tw-translate-x:-50%}.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.cursor-pointer{cursor:pointer}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-end{align-items:flex-end}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-8{gap:.5rem}.gap-10{gap:.625rem}.gap-24{gap:1.5rem}.gap-4{gap:.25rem}.gap-16{gap:1rem}.gap-x-8{-moz-column-gap:.5rem;column-gap:.5rem}.gap-x-4{-moz-column-gap:.25rem;column-gap:.25rem}.gap-y-12{row-gap:.75rem}.gap-y-8{row-gap:.5rem}.gap-x-16{-moz-column-gap:1rem;column-gap:1rem}.self-end{align-self:flex-end}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-x-auto{overflow-x:auto}.whitespace-normal{white-space:normal}.whitespace-nowrap{white-space:nowrap}.break-words{overflow-wrap:break-word}.rounded-full{border-radius:9999px}.rounded-xs{border-radius:2px}.rounded{border-radius:6px}.rounded-none{border-radius:0}.rounded-r{border-bottom-right-radius:6px;border-top-right-radius:6px}.border{border-width:1px}.border-0{border-width:0}.border-2{border-width:2px}.border-x-0{border-left-width:0;border-right-width:0}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-solid{border-style:solid}.border-dark-200{border-color:var(--color-dark-200)}.border-dark-100{border-color:var(--color-dark-100)}.border-negative-100{border-color:var(--color-negative-100)}.border-transparent{border-color:var(--color-transparent)}.border-notice-100{border-color:var(--color-notice-100)}.border-current{border-color:currentColor}.border-dark-300{border-color:var(--color-dark-300)}.border-success-100{border-color:var(--color-success-100)}.border-warning-100{border-color:var(--color-warning-100)}.bg-light{background-color:var(--color-light)}.bg-dark-300{background-color:var(--color-dark-300)}.bg-dark-100{background-color:var(--color-dark-100)}.bg-success-100{background-color:var(--color-success-100)}.bg-warning-100{background-color:var(--color-warning-100)}.bg-notice-100{background-color:var(--color-notice-100)}.bg-negative-100{background-color:var(--color-negative-100)}.bg-negative-50{background-color:var(--color-negative-50)}.bg-success{background-color:var(--color-success)}.bg-notice-50{background-color:var(--color-notice-50)}.bg-transparent{background-color:var(--color-transparent)}.bg-success-50{background-color:var(--color-success-50)}.bg-warning-50{background-color:var(--color-warning-50)}.bg-primary-50{background-color:var(--color-primary-50)}.object-cover{-o-object-fit:cover;object-fit:cover}.p-12{padding:.75rem}.p-8{padding:.5rem}.p-16{padding:1rem}.p-0{padding:0}.p-24{padding:1.5rem}.p-32{padding:2rem}.px-24{padding-left:1.5rem;padding-right:1.5rem}.py-32{padding-bottom:2rem;padding-top:2rem}.px-16{padding-left:1rem;padding-right:1rem}.py-8{padding-bottom:.5rem;padding-top:.5rem}.py-2{padding-bottom:.125rem;padding-top:.125rem}.py-16{padding-bottom:1rem;padding-top:1rem}.px-32{padding-left:2rem;padding-right:2rem}.px-0{padding-left:0;padding-right:0}.py-24{padding-bottom:1.5rem;padding-top:1.5rem}.py-12{padding-bottom:.75rem;padding-top:.75rem}.px-38{padding-left:2.375rem;padding-right:2.375rem}.px-12{padding-left:.75rem;padding-right:.75rem}.py-20{padding-bottom:1.25rem;padding-top:1.25rem}.px-20{padding-left:1.25rem;padding-right:1.25rem}.px-10{padding-left:.625rem;padding-right:.625rem}.pl-36{padding-left:2.25rem}.pr-8{padding-right:.5rem}.pt-20{padding-top:1.25rem}.\!pl-20{padding-left:1.25rem!important}.pb-24{padding-bottom:1.5rem}.pl-38{padding-left:2.375rem}.pt-8{padding-top:.5rem}.pr-10{padding-right:.625rem}.pr-66{padding-right:4.125rem}.pl-42{padding-left:2.625rem}.pl-26{padding-left:1.625rem}.pl-10{padding-left:.625rem}.pr-38{padding-right:2.375rem}.pt-10{padding-top:.625rem}.pb-0{padding-bottom:0}.pb-8{padding-bottom:.5rem}.text-left{text-align:left}.text-center{text-align:center}.font-heading{font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol}.text-14{font-size:.875rem}.text-12,.text-14{line-height:1.25rem}.text-12{font-size:.75rem}.text-16{font-size:1rem;line-height:1.25rem}.text-24{font-size:1.5rem;line-height:2rem}.text-18{font-size:1.125rem;line-height:1.25rem}.text-30{font-size:1.875rem;line-height:2.75rem}.font-bold{font-weight:700}.font-semibold{font-weight:600}.font-medium{font-weight:500}.font-normal{font-weight:400}.leading-none{line-height:1}.leading-20{line-height:1.25rem}.leading-16{line-height:1rem}.leading-18{line-height:1.125rem}.leading-28{line-height:1.75rem}.text-dark-600{color:var(--color-dark-600)}.text-dark{color:var(--color-dark)}.text-dark-900{color:var(--color-dark-900)}.text-secondary{color:var(--color-secondary)}.text-success-800{color:var(--color-success-800)}.text-warning-800{color:var(--color-warning-800)}.text-notice-800{color:var(--color-notice-800)}.text-negative-800{color:var(--color-negative-800)}.text-negative-900{color:var(--color-negative-900)}.text-negative{color:var(--color-negative)}.text-primary{color:var(--color-primary)}.text-notice-900{color:var(--color-notice-900)}.text-notice{color:var(--color-notice)}.text-dark-400{color:var(--color-dark-400)}.text-dark-300{color:var(--color-dark-300)}.text-light{color:var(--color-light)}.text-success-900{color:var(--color-success-900)}.text-success{color:var(--color-success)}.text-warning-900{color:var(--color-warning-900)}.text-warning{color:var(--color-warning)}.opacity-75{opacity:.75}.shadow-none{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000}.shadow,.shadow-none{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.shadow{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color)}.outline{outline-style:solid}.blur{--tw-blur:blur(8px)}.blur,.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition-transform{transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}.line-clamp-1{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.fade{transition-duration:.15s;transition-property:opacity,visibility;transition-timing-function:cubic-bezier(.4,0,.2,1)}.fade:not(.show){opacity:0;visibility:hidden}.collapse:not(.show){display:none}.flatpickr-day.collapse:not(.show){visibility:hidden}.flex-center{align-items:center;display:flex;justify-content:center}.\!visible,.visible{display:block!important}.active{opacity:1;visibility:visible}.tabulator{font-size:.875rem;line-height:1.25rem;overflow:hidden;position:relative;text-align:left;transform:translateZ(0)}.tabulator[tabulator-layout=fitDataFill] .tabulator-tableholder .tabulator-table{min-width:100%}.tabulator[tabulator-layout=fitDataTable]{display:inline-block}.tabulator .tabulator-header,.tabulator.tabulator-block-select{-webkit-user-select:none;-moz-user-select:none;user-select:none}.tabulator .tabulator-header{background-color:var(--color-dark-100);border-bottom-width:1px;border-color:var(--color-dark-200);box-sizing:border-box;color:var(--color-dark-600);overflow:hidden;position:relative;white-space:nowrap;width:100%}.tabulator .tabulator-header.tabulator-header-hidden{display:none}.tabulator .tabulator-header .tabulator-header-contents{overflow:hidden;position:relative}.tabulator .tabulator-header .tabulator-header-contents .tabulator-headers{display:inline-block}.tabulator .tabulator-header .tabulator-col{background-color:var(--color-dark-100);box-sizing:border-box;color:var(--color-dark-600);display:inline-flex;flex-direction:column;justify-content:flex-start;overflow:hidden;position:relative;text-align:left;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);vertical-align:bottom}.tabulator .tabulator-header .tabulator-col .tabulator-col-content{align-items:center;box-sizing:border-box;display:flex;min-height:3rem;padding:.5rem;position:relative}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title-holder.tabulator-col-sorter-element{position:relative}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title{box-sizing:border-box;overflow:hidden;text-overflow:ellipsis;vertical-align:bottom;white-space:nowrap;width:100%}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title:first-letter{text-transform:capitalize}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title.tabulator-col-title-wrap{text-overflow:clip;white-space:normal}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter{align-items:center;bottom:0;display:flex;position:absolute;right:.125rem;top:0}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow{border:none!important;opacity:0;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:before{border-bottom:4px solid var(--color-dark-400);border-left:4px solid transparent;border-right:4px solid transparent;content:"";display:block}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:after{border-left:4px solid transparent;border-right:4px solid transparent;border-top:4px solid var(--color-dark-400);content:"";display:block;margin-top:.125rem}.tabulator .tabulator-header .tabulator-col.tabulator-sortable{cursor:pointer}.tabulator .tabulator-header .tabulator-col.tabulator-sortable:hover .tabulator-col-content .tabulator-col-title,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-title,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-title{color:var(--color-dark-900)}.tabulator .tabulator-header .tabulator-col.tabulator-sortable:hover .tabulator-col-content .tabulator-col-sorter .tabulator-arrow,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow{opacity:1}.tabulator .tabulator-header .tabulator-col.tabulator-sortable .tabulator-col-title{padding-right:1.25rem}.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:before{border-bottom:4px solid var(--color-dark-800)}.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:after{border-top:4px solid var(--color-dark-800)}.tabulator .tabulator-header .tabulator-col.tabulator-col-vertical .tabulator-col-content .tabulator-col-title{align-items:center;display:flex;justify-content:center;text-orientation:mixed;writing-mode:vertical-rl}.tabulator .tabulator-frozen:before{bottom:0;box-shadow:0 0 8px 0 rgba(17,24,39,.16);content:"";left:0;position:absolute;right:0;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator .tabulator-header .tabulator-frozen{background-color:transparent;left:0;position:sticky;z-index:10}.tabulator .tabulator-header .tabulator-frozen:before{background-color:var(--color-dark-100)}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-left{padding-right:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-left:before{margin-right:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-right{padding-left:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-right:before{margin-left:.5rem}.tabulator .tabulator-header .tabulator-frozen-rows-holder:empty{display:none}.tabulator .tabulator-tableholder{-webkit-overflow-scrolling:touch;overflow:auto;position:relative;white-space:nowrap;width:100%}.tabulator .tabulator-tableholder:focus{outline:none}.tabulator .tabulator-tableholder .tabulator-placeholder{align-items:center;box-sizing:border-box;display:flex;justify-content:center;width:100%}.tabulator .tabulator-tableholder .tabulator-placeholder[tabulator-render-mode=virtual]{min-height:100%;min-width:100%}.tabulator .tabulator-tableholder .tabulator-placeholder .tabulator-placeholder-contents{display:inline-block;font-size:1rem;font-weight:600;line-height:1.25rem;padding:1.5rem;text-align:center;white-space:normal}.tabulator .tabulator-tableholder .tabulator-table{background-color:var(--color-light);color:var(--color-dark-900);display:inline-block;min-width:100%;overflow:visible;position:relative;white-space:nowrap}.tabulator .tabulator-footer{background-color:var(--color-light);border-color:var(--color-dark-200);border-top-width:1px;display:none;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.tabulator .tabulator-footer .tabulator-footer-contents{align-items:center;display:flex;padding:1rem}.tabulator .tabulator-footer .tabulator-footer-contents:empty{display:none}.tabulator-page-counter{margin-left:auto}.tabulator-paginator{display:flex;margin-left:.5rem}@media (min-width:576px){.tabulator-paginator{margin-left:1rem}}.tabulator-pages{display:flex}.tabulator-pages+.tabulator-page{margin-left:-1px}.tabulator-page{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;border-color:var(--color-dark-200);border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:flex;font-weight:500;height:2.5rem;justify-content:center;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.5rem}.tabulator-page.active,.tabulator-page:not(:disabled):not(.disabled):hover{background-color:var(--color-primary-100);border-color:var(--color-primary);cursor:pointer;z-index:1}.tabulator-page.active{color:var(--color-primary)}.tabulator-page+.tabulator-page,.tabulator-page+.tabulator-pages{margin-left:-1px}.tabulator-page[data-page=first],.tabulator-page[data-page=last]{display:none}.tabulator-page[data-page=next],.tabulator-page[data-page=prev]{position:relative;text-indent:-9999px;white-space:nowrap}.tabulator-page[data-page=next]:after,.tabulator-page[data-page=prev]:after{background-position:50%;background-repeat:no-repeat;background-size:24px;bottom:0;content:"";height:100%;left:0;position:absolute;right:0;top:0;width:100%}.tabulator-page:first-child{border-bottom-left-radius:6px;border-top-left-radius:6px}.tabulator-page:last-child{border-bottom-right-radius:6px;border-top-right-radius:6px}.tabulator-page:disabled{color:var(--color-dark-400)}.tabulator-page:disabled:after{opacity:.4}.tabulator-page:disabled:first-child,.tabulator-page:disabled:last-child{border-color:var(--color-dark-100)}@media (max-width:767px){.tabulator-page:not(:first-child):not(:last-child){display:none}}.tabulator .tabulator-col-resize-handle{display:inline-block;margin-left:-3px;margin-right:-3px;position:relative;vertical-align:middle;width:6px;z-index:10}.tabulator .tabulator-col-resize-handle:hover{cursor:ew-resize}.tabulator .tabulator-col-resize-handle:last-of-type{margin-right:0;width:3px}.tabulator .tabulator-alert{align-items:center;background:rgba(0,0,0,.4);display:flex;height:100%;left:0;position:absolute;text-align:center;top:0;width:100%;z-index:100}.tabulator .tabulator-alert .tabulator-alert-msg{background:#fff;border-radius:10px;display:inline-block;font-size:16px;font-weight:700;margin:0 auto;padding:10px 20px}.tabulator .tabulator-alert .tabulator-alert-msg.tabulator-alert-state-msg{border:4px solid #333;color:#000}.tabulator .tabulator-alert .tabulator-alert-msg.tabulator-alert-state-error{border:4px solid #d00;color:#590000}.tabulator-row{background-color:var(--color-light);border-bottom-width:1px;border-color:var(--color-dark-200);box-sizing:border-box;cursor:pointer;min-height:2.5rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator-row.tabulator-selectable:hover{cursor:pointer}.tabulator-row.tabulator-selectable:hover,.tabulator-row.tabulator-selectable:hover>.tabulator-frozen:before{background-color:var(--color-primary-50)}.tabulator-header .row-select-wrapper,.tabulator-row.tabulator-selectable .row-select-wrapper{align-items:center;bottom:0;display:flex;justify-content:center;left:0;padding:.5rem 1rem;position:absolute;right:0;top:0;width:100%}.tabulator-header .row-select-wrapper>label,.tabulator-row.tabulator-selectable .row-select-wrapper>label{height:1.25rem;padding-left:1.25rem}.tabulator-row.tabulator-selectable .row-select-wrapper{height:100%}.tabulator-header .row-select-wrapper{height:3rem}.tabulator-row.tabulator-selected,.tabulator-row.tabulator-selected:hover{background-color:var(--color-primary-50)}.tabulator-row.tabulator-selected:hover{cursor:pointer}.tabulator-row.tabulator-row-moving{background:#fff;border:1px solid #000}.tabulator-row.tabulator-moving{border-bottom:1px solid #aaa;border-top:1px solid #aaa;pointer-events:none;position:absolute;z-index:15}.tabulator-row .tabulator-row-resize-handle{bottom:0;height:5px;left:0;position:absolute;right:0}.tabulator-row .tabulator-row-resize-handle.prev{bottom:auto;top:0}.tabulator-row .tabulator-row-resize-handle:hover{cursor:ns-resize}.tabulator-row .tabulator-responsive-collapse{border-bottom-width:1px;border-color:var(--color-dark-200);border-top-width:1px;box-sizing:border-box;padding:.5rem}.tabulator-row .tabulator-responsive-collapse:empty{display:none}.tabulator-row .tabulator-responsive-collapse table tr td{position:relative}.tabulator-row .tabulator-responsive-collapse table tr td:first-of-type{padding-right:1rem}.tabulator-row .tabulator-cell{align-items:center;box-sizing:border-box;display:inline-flex;min-height:2.5rem;overflow:hidden;padding:.5rem;position:relative;text-overflow:ellipsis;vertical-align:middle;white-space:nowrap}.tabulator-row .tabulator-cell .btn+.btn{margin-left:.25rem}.tabulator-row .tabulator-cell.tabulator-frozen{display:inline-block;left:0;position:sticky;z-index:10}.tabulator-row .tabulator-cell.tabulator-frozen:before{background-color:var(--color-light)}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-left{padding-right:1rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-left:before{margin-right:.5rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-right{padding-left:1rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-right:before{margin-left:.5rem}.tabulator-row .tabulator-cell.tabulator-editable{border-color:var(--color-dark-200);border-left-width:1px;border-right-width:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-editable:hover{background-color:var(--color-dark-50)}.tabulator-row .tabulator-cell.tabulator-editing{border-color:var(--color-primary);border-width:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-editing input,.tabulator-row .tabulator-cell.tabulator-editing select{background:transparent;border:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-validation-fail{border:1px solid #d00}.tabulator-row .tabulator-cell.tabulator-validation-fail input,.tabulator-row .tabulator-cell.tabulator-validation-fail select{background:transparent;border:1px;color:#d00}.tabulator-row .tabulator-cell.tabulator-row-handle{align-items:center;display:inline-flex;justify-content:center;-moz-user-select:none;-khtml-user-select:none;-webkit-user-select:none;-o-user-select:none}.tabulator-row .tabulator-cell.tabulator-row-handle .tabulator-row-handle-box{width:80%}.tabulator-row .tabulator-cell.tabulator-row-handle .tabulator-row-handle-box .tabulator-row-handle-bar{background:#666;height:3px;margin-top:2px;width:100%}.tabulator-row .tabulator-cell .tabulator-data-tree-branch{border-bottom:2px solid #aaa;border-bottom-left-radius:1px;border-left:2px solid #aaa;display:inline-block;height:9px;margin-right:5px;margin-top:-9px;vertical-align:middle;width:7px}.tabulator-row .tabulator-cell .tabulator-data-tree-control{align-items:center;background:rgba(0,0,0,.1);border:1px solid #333;border-radius:2px;display:inline-flex;height:11px;justify-content:center;margin-right:5px;overflow:hidden;vertical-align:middle;width:11px}.tabulator-row .tabulator-cell .tabulator-data-tree-control:hover{background:rgba(0,0,0,.2);cursor:pointer}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-collapse{background:transparent;display:inline-block;height:7px;position:relative;width:1px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-collapse:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-expand{background:#333;display:inline-block;height:7px;position:relative;width:1px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-expand:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-row.tabulator-group{background:#ccc;border-bottom:1px solid #999;border-right:1px solid #aaa;border-top:1px solid #999;box-sizing:border-box;font-weight:700;min-width:100%;padding:5px 5px 5px 10px}.tabulator-row.tabulator-group:hover{background-color:rgba(0,0,0,.1);cursor:pointer}.tabulator-row.tabulator-group.tabulator-group-visible .tabulator-arrow{border-bottom:0;border-left:6px solid transparent;border-right:6px solid transparent;border-top:6px solid #666;margin-right:10px}.tabulator-row.tabulator-group.tabulator-group-level-1{padding-left:30px}.tabulator-row.tabulator-group.tabulator-group-level-2{padding-left:50px}.tabulator-row.tabulator-group.tabulator-group-level-3{padding-left:70px}.tabulator-row.tabulator-group.tabulator-group-level-4{padding-left:90px}.tabulator-row.tabulator-group.tabulator-group-level-5{padding-left:110px}.tabulator-row.tabulator-group .tabulator-group-toggle{display:inline-block}.tabulator-row.tabulator-group .tabulator-arrow{border-bottom:6px solid transparent;border-left:6px solid #666;border-right:0;border-top:6px solid transparent;display:inline-block;height:0;margin-right:16px;vertical-align:middle;width:0}.tabulator-row.tabulator-group span{color:#d00;margin-left:10px}.tabulator-print-table .tabulator-data-tree-branch{border-bottom:2px solid #aaa;border-bottom-left-radius:1px;border-left:2px solid #aaa;display:inline-block;height:9px;margin-right:5px;margin-top:-9px;vertical-align:middle;width:7px}.tabulator-print-table .tabulator-data-tree-control{align-items:center;background:rgba(0,0,0,.1);border:1px solid #333;border-radius:2px;display:inline-flex;height:11px;justify-content:center;margin-right:5px;overflow:hidden;vertical-align:middle;width:11px}.tabulator-print-table .tabulator-data-tree-control:hover{background:rgba(0,0,0,.2);cursor:pointer}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-collapse{background:transparent;display:inline-block;height:7px;position:relative;width:1px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-collapse:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-expand{background:#333;display:inline-block;height:7px;position:relative;width:1px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-expand:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-custom-header{border-bottom-width:1px;border-color:var(--color-dark-200);font-size:.875rem;line-height:1.25rem;position:relative}.tabulator-custom-footer{border-color:var(--color-dark-200);border-top-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;padding:1rem}.tabulator-responsive-collapse table{display:flex;gap:.5rem}.tabulator-responsive-collapse td:first-child{display:none}.tabulator-responsive-collapse tr{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.tabulator-responsive-collapse tr>span{-webkit-line-clamp:2;margin-right:auto}.tabulator-responsive-collapse tr>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.tabulator-responsive-collapse tr:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.tabulator-responsive-collapse tr:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900)}.tabulator-responsive-collapse tr:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.tabulator-responsive-collapse tr:focus-visible{outline:none}.tabulator-responsive-collapse tr:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.tabulator-responsive-collapse tr{height:2rem;padding-left:.75rem;padding-right:.75rem}.tabulator-responsive-collapse tr>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.tabulator-responsive-collapse tr>svg{height:1rem;width:1rem}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.filter-wrapper>.tabulator-responsive-collapse tr.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.tabulator-responsive-collapse tr.empty>svg:not(:last-child){visibility:hidden}.tabulator-responsive-collapse tr{border-radius:9999px;position:relative}.tabulator-row .tabulator-cell .tabulator-responsive-collapse tr+.btn{margin-left:.25rem}.djn-table>.djn-tbody td .tabulator-responsive-collapse tr:not(.input-file-edit-btn){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rules-group-container .rules-group-header .tabulator-responsive-collapse tr{height:2rem}.query-builder .rules-group-container .group-conditions label.tabulator-responsive-collapse tr{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.tabulator-responsive-collapse tr.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container .rule-header .tabulator-responsive-collapse tr-group .btn{margin-right:0}.query-builder .tabulator-responsive-collapse tr[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .tabulator-responsive-collapse tr[data-delete] i{display:none}.flatpickr-day.query-builder .tabulator-responsive-collapse tr[data-delete] i{visibility:hidden}.query-builder .tabulator-responsive-collapse tr[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .tabulator-responsive-collapse tr[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.tabulator-responsive-collapse tr{color:var(--color-dark)}.tabulator-responsive-collapse tr:hover{color:var(--color-dark-900)}.tabulator-responsive-collapse tr .catalog-image{height:1.5rem;width:1.5rem}.flatpickr-calendar{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color);animation:none;background:transparent;background-color:var(--color-light);border:0;border-radius:6px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);box-sizing:border-box;direction:ltr;display:none;opacity:0;padding:0;position:absolute;text-align:center;touch-action:manipulation;visibility:hidden;width:272px}.flatpickr-calendar.inline,.flatpickr-calendar.open{max-height:640px;opacity:1;visibility:visible}.flatpickr-calendar.open{display:inline-block;z-index:99999}.flatpickr-calendar.inline{display:block;position:relative;top:2px}.flatpickr-calendar.static{position:absolute;top:calc(100% + 2px)}.flatpickr-calendar.static.open{display:block;z-index:999}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+1) .flatpickr-day.inRange:nth-child(7n+7){box-shadow:none!important}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+2) .flatpickr-day.inRange:nth-child(7n+1){box-shadow:-2px 0 0 #e6e6e6,5px 0 0 #e6e6e6}.flatpickr-calendar .hasTime .dayContainer,.flatpickr-calendar .hasWeeks .dayContainer{border-bottom:0;border-bottom-left-radius:0;border-bottom-right-radius:0}.flatpickr-calendar .hasWeeks .dayContainer{border-left:0}.flatpickr-calendar.hasTime:not(.noCalendar) .flatpickr-time{padding-top:0}.flatpickr-calendar.noCalendar.hasTime{width:200px}.flatpickr-calendar.noCalendar.hasTime .flatpickr-time{border:0;height:auto}.flatpickr-calendar:focus{outline:0}.flatpickr-wrapper{display:inline-block;position:relative}.flatpickr-months{color:var(--color-dark-900);display:flex;margin-top:.25rem;padding:.5rem .75rem}.flatpickr-months .flatpickr-month{display:flex;justify-content:center;position:relative;width:100%}.flatpickr-months .flatpickr-next-month,.flatpickr-months .flatpickr-prev-month{cursor:pointer;font-size:0}.flatpickr-months .flatpickr-next-month>svg,.flatpickr-months .flatpickr-prev-month>svg{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.flatpickr-months .flatpickr-next-month.flatpickr-disabled,.flatpickr-months .flatpickr-prev-month.flatpickr-disabled{display:none}.flatpickr-months .flatpickr-next-month i,.flatpickr-months .flatpickr-prev-month i{position:relative}.flatpickr-months .flatpickr-next-month:hover,.flatpickr-months .flatpickr-prev-month:hover{color:var(--color-primary)}.numInputWrapper{border-color:var(--color-dark-200);border-radius:6px;border-width:1px;height:auto;padding-left:.25rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.numInputWrapper input,.numInputWrapper span{display:inline-block}.numInputWrapper input{width:100%}.numInputWrapper input::-ms-clear{display:none}.numInputWrapper input::-webkit-inner-spin-button,.numInputWrapper input::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.numInputWrapper span{background-color:var(--color-light);border-color:var(--color-dark-400);border-width:1px;box-sizing:border-box;cursor:pointer;height:calc(50% + 1px);opacity:0;padding:0 4px 0 3px;position:absolute;right:0;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);width:17px}.numInputWrapper span:hover{background-color:var(--color-dark-100)}.numInputWrapper span:active{background-color:var(--color-dark-200)}.numInputWrapper span:after{content:"";display:block;position:absolute}.numInputWrapper span.arrowUp{border-bottom:0;border-top-right-radius:6px;top:0}.numInputWrapper span.arrowUp:after{border-bottom:4px solid var(--color-dark-900);border-left:4px solid transparent;border-right:4px solid transparent;bottom:40%}.numInputWrapper span.arrowDown{border-bottom-right-radius:6px;bottom:0}.numInputWrapper span.arrowDown:after{border-left:4px solid transparent;border-right:4px solid transparent;border-top:4px solid var(--color-dark-900);top:calc(40% - 1px)}.numInputWrapper span svg{height:auto;width:inherit}.numInputWrapper:hover{border-color:var(--color-dark-400)}.numInputWrapper:hover span{opacity:1}.flatpickr-current-month{color:var(--color-dark-900);cursor:pointer;display:flex;font-size:1rem;font-weight:600;gap:.25rem;justify-content:center;line-height:1.5rem;transform:translateZ(0);transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.flatpickr-current-month:hover{color:var(--color-primary)}.flatpickr-current-month span.cur-month{color:inherit;display:inline-block;font-family:inherit;font-weight:700;margin-left:.5ch;padding:0}.flatpickr-current-month span.cur-month:hover{background-color:var(--color-primary-100)}.flatpickr-current-month .numInputWrapper{display:inline-block;width:6ch;width:7ch \0}.flatpickr-current-month .numInputWrapper span.arrowUp:after{border-bottom-color:rgba(0,0,0,.9)}.flatpickr-current-month .numInputWrapper span.arrowDown:after{border-top-color:rgba(0,0,0,.9)}.flatpickr-current-month input.cur-year{-webkit-appearance:textfield;-moz-appearance:textfield;appearance:textfield;background:transparent;border:0;border-radius:0;color:inherit;cursor:text;display:inline-block;font-family:inherit;font-size:inherit;height:auto;line-height:inherit;margin:0;vertical-align:initial}.flatpickr-current-month input.cur-year:focus{outline:0}.flatpickr-current-month input.cur-year[disabled],.flatpickr-current-month input.cur-year[disabled]:hover{background:transparent;color:rgba(0,0,0,.5);font-size:100%;pointer-events:none}.flatpickr-current-month .flatpickr-monthDropdown-months{-webkit-appearance:menulist-button;-moz-appearance:menulist-button;appearance:menulist-button;background-color:transparent;border-color:var(--color-dark-200);border-radius:0;border-radius:6px;border-width:1px;box-sizing:border-box;color:inherit;color:var(--color-dark-900);cursor:pointer;font-family:inherit;font-size:inherit;font-size:1rem;font-weight:600;height:auto;line-height:inherit;line-height:1.5rem;outline:none;padding-left:.25rem;padding-right:.25rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);vertical-align:initial;width:auto}.flatpickr-current-month .flatpickr-monthDropdown-months:active,.flatpickr-current-month .flatpickr-monthDropdown-months:focus{outline:none}.flatpickr-current-month .flatpickr-monthDropdown-months:hover{border-color:var(--color-dark-400)}.flatpickr-current-month .flatpickr-monthDropdown-months .flatpickr-monthDropdown-month{background-color:var(--color-light);outline:none;padding:0}.flatpickr-weekdays{align-items:center;background:transparent;display:flex;overflow:hidden;text-align:center;width:100%}.flatpickr-weekdays .flatpickr-weekdaycontainer{display:flex;flex:1;padding-bottom:.5rem;padding-top:.5rem}span.flatpickr-weekday{background:transparent;cursor:default;display:block;flex:1;margin:0;text-align:center}.dayContainer,.flatpickr-weeks{padding:1px 0 0}.flatpickr-days{align-items:flex-start;display:flex;overflow:hidden;position:relative}.dayContainer,.flatpickr-days:focus{outline:0}.dayContainer{display:flex;flex-wrap:wrap;gap:.25rem;height:100%;opacity:1;text-align:left;transform:translateZ(0);width:100%}.dayContainer+.dayContainer{box-shadow:-1px 0 0 #e6e6e6}.flatpickr-day{align-items:center;background:none;border:1px solid transparent;border-radius:6px;color:var(--color-dark-900);cursor:pointer;display:flex;font-weight:400;height:2rem;justify-content:center;margin:0;position:relative;width:2rem}.flatpickr-day.inRange,.flatpickr-day.nextMonthDay.inRange,.flatpickr-day.nextMonthDay.today.inRange,.flatpickr-day.nextMonthDay:focus,.flatpickr-day.nextMonthDay:hover,.flatpickr-day.prevMonthDay.inRange,.flatpickr-day.prevMonthDay.today.inRange,.flatpickr-day.prevMonthDay:focus,.flatpickr-day.prevMonthDay:hover,.flatpickr-day.today.inRange,.flatpickr-day:focus,.flatpickr-day:hover{background:var(--color-primary-100);border-color:var(--color-primary-100);cursor:pointer;outline:0}.flatpickr-day.today{color:var(--color-primary);font-weight:600}.flatpickr-day.today:focus,.flatpickr-day.today:hover{background:var(--color-primary);border-color:var(--color-primary);color:var(--color-light)}.flatpickr-day.endRange,.flatpickr-day.endRange.inRange,.flatpickr-day.endRange.nextMonthDay,.flatpickr-day.endRange.prevMonthDay,.flatpickr-day.endRange:focus,.flatpickr-day.endRange:hover,.flatpickr-day.selected,.flatpickr-day.selected.inRange,.flatpickr-day.selected.nextMonthDay,.flatpickr-day.selected.prevMonthDay,.flatpickr-day.selected:focus,.flatpickr-day.selected:hover,.flatpickr-day.startRange,.flatpickr-day.startRange.inRange,.flatpickr-day.startRange.nextMonthDay,.flatpickr-day.startRange.prevMonthDay,.flatpickr-day.startRange:focus,.flatpickr-day.startRange:hover{background:var(--color-primary);border-color:var(--color-primary);box-shadow:none;color:var(--color-light)}.flatpickr-day.endRange.startRange,.flatpickr-day.selected.startRange,.flatpickr-day.startRange.startRange{border-radius:50px 0 0 50px}.flatpickr-day.endRange.endRange,.flatpickr-day.selected.endRange,.flatpickr-day.startRange.endRange{border-radius:0 50px 50px 0}.flatpickr-day.endRange.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.selected.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.startRange.startRange+.endRange:not(:nth-child(7n+1)){box-shadow:-10px 0 0 var(--color-primary)}.flatpickr-day.endRange.startRange.endRange,.flatpickr-day.selected.startRange.endRange,.flatpickr-day.startRange.startRange.endRange{border-radius:50px}.flatpickr-day.inRange{border-radius:0;box-shadow:-5px 0 0 var(--color-primary-100),5px 0 0 var(--color-primary-100);color:var(--color-primary-700)}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover,.flatpickr-day.nextMonthDay,.flatpickr-day.notAllowed,.flatpickr-day.notAllowed.nextMonthDay,.flatpickr-day.notAllowed.prevMonthDay,.flatpickr-day.prevMonthDay{background:transparent;border-color:transparent;color:var(--color-dark);cursor:default}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover{color:rgba(57,57,57,.1);cursor:not-allowed}.flatpickr-day.week.selected{border-radius:0;box-shadow:-5px 0 0 #569ff7,5px 0 0 #569ff7}.flatpickr-day.hidden{visibility:hidden}.flatpickr-day.flatpickr-month{height:3.5rem;width:5rem}.flatpickr-day.flatpickr-year{height:3rem;margin-top:0!important;width:100%}.rangeMode .flatpickr-day{margin-top:1px}.flatpickr-weekwrapper{float:left}.flatpickr-weekwrapper .flatpickr-weeks{box-shadow:1px 0 0 #e6e6e6;padding:0 12px}.flatpickr-weekwrapper .flatpickr-weekday{float:none;line-height:28px;width:100%}.flatpickr-weekwrapper span.flatpickr-day,.flatpickr-weekwrapper span.flatpickr-day:hover{background:transparent;border:none;color:rgba(57,57,57,.3);cursor:default;display:block;max-width:none;width:100%}.flatpickr-innerContainer{display:flex;font-size:.75rem;height:17rem;line-height:1rem;overflow:hidden;padding:.5rem .75rem}.flatpickr-rContainer{display:inline-block;padding:0}.flatpickr-time{align-items:center;display:flex;padding:.75rem}.flatpickr-time .numInputWrapper{border:none;display:flex;padding:0}.flatpickr-time .numInputWrapper span.arrowUp:after{border-bottom-color:#393939}.flatpickr-time .numInputWrapper span.arrowDown:after{border-top-color:#393939}.flatpickr-time.hasSeconds .numInputWrapper{width:26%}.flatpickr-time.time24hr .numInputWrapper{width:50%}.flatpickr-time input{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.flatpickr-time input~.error{color:var(--color-negative)}.flatpickr-time input:hover{border-color:var(--color-dark-400)}.flatpickr-time input:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.flatpickr-time input:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.flatpickr-time input::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.flatpickr-time input::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.flatpickr-time input.field-valid{border-color:var(--color-success)}.flatpickr-time input.field-valid~.success{display:block}.flatpickr-time input.field-error{border-color:var(--color-negative)}.flatpickr-time input.field-error~.error{display:block}input.flatpickr-time input:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.flatpickr-time input:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.flatpickr-time input:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.flatpickr-time input:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.flatpickr-time input{height:auto}select.flatpickr-time input{padding-right:2rem}.djn-table>.djn-tbody td .flatpickr-time input:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.flatpickr-time .flatpickr-am-pm,.flatpickr-time .flatpickr-time-separator{align-items:center;display:flex;float:left;font-weight:700;height:inherit;justify-content:center;line-height:inherit;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:1rem}.flatpickr-time .flatpickr-am-pm{cursor:pointer;font-weight:400;outline:0;text-align:center;width:18%}.flatpickr-input[readonly]{cursor:pointer}@keyframes fpFadeInDown{0%{opacity:0;transform:translate3d(0,-20px,0)}to{opacity:1;transform:translateZ(0)}}.flatpickr-shortcuts{margin-bottom:1rem;padding-top:.25rem}.flatpickr-shortcuts>label{padding:0}.flatpickr-footer{padding-bottom:.25rem;text-align:left}.flatpickr-custom-events-overlay{bottom:0;cursor:pointer;left:0;position:absolute;right:0;top:0}.flatpickr-custom-views-wrapper{position:relative;z-index:10}.flatpickr-custom-months-view,.flatpickr-custom-years-view{background-color:var(--color-light);left:0;position:absolute;right:0;width:100%}.flatpickr-back{color:var(--color-primary);cursor:pointer;display:inline-block;font-size:.875rem;line-height:1.25rem;padding:.5rem .75rem;position:absolute;right:0;top:100%}.js-timepicker{max-width:4rem}.noUi-target,.noUi-target *{-webkit-touch-callout:none;-webkit-tap-highlight-color:rgba(0,0,0,0);box-sizing:border-box;touch-action:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}.noUi-target{position:relative}.noUi-base,.noUi-connects{height:100%;position:relative;width:100%;z-index:1}.noUi-connects{overflow:hidden;z-index:0}.noUi-connect,.noUi-origin{height:100%;position:absolute;right:0;top:0;-ms-transform-origin:0 0;-webkit-transform-origin:0 0;transform-origin:0 0;-webkit-transform-style:preserve-3d;transform-style:flat;width:100%;will-change:transform;z-index:1}.noUi-txt-dir-rtl.noUi-horizontal .noUi-origin{left:0;right:auto}.noUi-vertical .noUi-origin{top:-100%;width:0}.noUi-horizontal .noUi-origin{height:0}.noUi-handle{-webkit-backface-visibility:hidden;backface-visibility:hidden;position:absolute}.noUi-touch-area{--tw-translate-x:-50%;--tw-translate-y:-50%;height:1.25rem;left:50%;position:absolute;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));width:1.25rem}.noUi-state-tap .noUi-connect,.noUi-state-tap .noUi-origin{transition:transform .3s}.noUi-state-drag *{cursor:inherit!important}.noUi-horizontal{height:.25rem}.noUi-horizontal .noUi-handle{height:1rem;right:-7px;top:-7px;width:1rem}.noUi-vertical{width:18px}.noUi-vertical .noUi-handle{bottom:-17px;height:34px;right:-6px;width:28px}.noUi-txt-dir-rtl.noUi-horizontal .noUi-handle{left:-17px;right:auto}.noUi-target{background-color:var(--color-dark-200);border-radius:2px}.noUi-connects{border-radius:3px}.noUi-connect{background:#3fb8af}.noUi-draggable{cursor:ew-resize}.noUi-vertical .noUi-draggable{cursor:ns-resize}.noUi-handle{--tw-shadow:0 2px 4px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 2px 4px 0 var(--tw-shadow-color);background-color:var(--color-primary);border:2px solid var(--color-light);border-radius:9999px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);cursor:pointer}.noUi-active{background-color:var(--color-primary-400)}.noUi-vertical .noUi-handle:after,.noUi-vertical .noUi-handle:before{height:1px;left:6px;top:14px;width:14px}.noUi-vertical .noUi-handle:after{top:17px}[disabled] .noUi-connect{background:#b8b8b8}[disabled] .noUi-handle,[disabled].noUi-handle,[disabled].noUi-target{cursor:not-allowed}.noUi-pips,.noUi-pips *{box-sizing:border-box}.noUi-pips{color:#999;position:absolute}.noUi-value{position:absolute;text-align:center;white-space:nowrap}.noUi-value-sub{color:#ccc;font-size:10px}.noUi-marker{background:#ccc;position:absolute}.noUi-marker-large,.noUi-marker-sub{background:#aaa}.noUi-pips-horizontal{height:80px;left:0;padding:10px 0;top:100%;width:100%}.noUi-value-horizontal{transform:translate(-50%,50%)}.noUi-rtl .noUi-value-horizontal{transform:translate(50%,50%)}.noUi-marker-horizontal.noUi-marker{height:5px;margin-left:-1px;width:2px}.noUi-marker-horizontal.noUi-marker-sub{height:10px}.noUi-marker-horizontal.noUi-marker-large{height:15px}.noUi-pips-vertical{height:100%;left:100%;padding:0 10px;top:0}.noUi-value-vertical{padding-left:25px;transform:translateY(-50%)}.noUi-rtl .noUi-value-vertical{transform:translateY(50%)}.noUi-marker-vertical.noUi-marker{height:2px;margin-top:-1px;width:5px}.noUi-marker-vertical.noUi-marker-sub{width:10px}.noUi-marker-vertical.noUi-marker-large{width:15px}.noUi-tooltip{background:#fff;border:1px solid #d9d9d9;border-radius:3px;color:#000;display:block;padding:5px;position:absolute;text-align:center;white-space:nowrap}.noUi-horizontal .noUi-tooltip{bottom:120%;left:50%;transform:translate(-50%)}.noUi-vertical .noUi-tooltip{right:120%;top:50%;transform:translateY(-50%)}.noUi-horizontal .noUi-origin>.noUi-tooltip{bottom:10px;left:auto;transform:translate(50%)}.noUi-vertical .noUi-origin>.noUi-tooltip{right:28px;top:auto;transform:translateY(-18px)}.tabular::-webkit-scrollbar{height:9px;width:9px}.tabular::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.tabular::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.tabular:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.tabular{overflow-x:auto}.djn-table{border-collapse:separate;border-spacing:0;height:100%;min-width:100%;white-space:nowrap}.djn-table>.djn-thead th{background-color:var(--color-dark-100);color:var(--color-dark-600);font-size:.875rem;font-weight:400;height:3rem;line-height:1.25rem;padding:.5rem;text-align:left;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.djn-table>.djn-thead th.original{min-width:2.5rem;width:2.5rem}.djn-table>.djn-thead th.original:not(.is-sortable){display:none}.flatpickr-day.djn-table>.djn-thead th.original:not(.is-sortable){visibility:hidden}.djn-table>.djn-thead th.original:not(.is-sortable)+td{border-left:0}.djn-table>.djn-thead td{font-size:.875rem;font-weight:400;line-height:1.25rem}.djn-table>.djn-tbody td{border-bottom-width:1px;border-color:var(--color-dark-200);min-height:3.5rem;position:relative}.djn-table>.djn-tbody td label:first-child:not(.input-file-edit-btn){display:none}.flatpickr-day.djn-table>.djn-tbody td label:first-child:not(.input-file-edit-btn){visibility:hidden}.djn-table>.djn-tbody td:not(:first-child){border-left-width:1px}.djn-table>.djn-tbody td.original{min-width:2.5rem;width:2.5rem}.djn-table>.djn-tbody td.original:not(.is-sortable){display:none}.flatpickr-day.djn-table>.djn-tbody td.original:not(.is-sortable){visibility:hidden}.djn-table>.djn-tbody td.original:not(.is-sortable)+td{border-left:0}.djn-table>.djn-tbody td.original>p{display:none}.flatpickr-day.djn-table>.djn-tbody td.original>p{visibility:hidden}.djn-table>.djn-tbody td select,.djn-table>.djn-tbody td>input[type=text]{height:100%;min-width:10rem}.djn-table>.djn-tbody td>.autocomplete-data-wrapper+p{display:none}.flatpickr-day.djn-table>.djn-tbody td>.autocomplete-data-wrapper+p{visibility:hidden}.djn-table>.djn-tbody td.field-image{max-width:23.125rem}.djn-table>.djn-tbody td .btn:not(.input-file-edit-btn),.djn-table>.djn-tbody td .input:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.djn-table>.djn-tbody td .toggle~label{margin-left:.5rem}.djn-table>.djn-tbody td .input-file-wrapper>.input-file{border-width:0}.djn-table>.djn-tbody:last-child>tr:last-child>td:first-child{border-bottom-left-radius:6px}.djn-table>.djn-tbody:last-child>tr:last-child>td:last-child{border-bottom-right-radius:6px}.djn-table>.djn-tbody.ui-sortable-placeholder td{background-color:var(--color-primary-50);height:3.5rem}.djn-table>.djn-tbody.has-errors td{vertical-align:top}.djn-table>:nth-last-child(2) td:first-child,.djn-table>:nth-last-child(2) th:first-child{border-bottom-left-radius:6px}.djn-table>:nth-last-child(2) td:last-child,.djn-table>:nth-last-child(2) th:last-child{border-bottom-right-radius:6px}.inline-group .empty-form{display:none!important}.djn-item{position:relative}.djn-drag-handler{--tw-translate-y:-50%;cursor:move;display:flex;left:.5rem;margin-right:.5rem;position:absolute;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.stacked-row .form-row{display:flex;flex-direction:column;margin-bottom:1.5rem}.stacked-row .form-row>div>.help,.stacked-row .form-row>div>label:first-child{display:none}.stacked-row .form-row>.errorlist{order:1}.checkbox-row>label{display:none}fieldset.module>h2{align-items:center;color:var(--color-dark-900);display:flex;font-size:1.125rem;font-weight:600;line-height:1.25rem;margin-bottom:1.5rem}fieldset.module>h2.stacked-inline-heading{font-size:1.5rem;line-height:2rem}@media (max-width:767px){fieldset.module>h2.stacked-inline-heading{padding-left:1.5rem;padding-right:1.5rem}}.djn-group .djn-group.djn-group-nested{border:0;margin:0}.djn-group .djn-group>fieldset>.djn-add-item,.djn-group .djn-group>fieldset>.stacked-inline-heading{padding-left:1.5rem;padding-right:1.5rem}.djn-td input[type=checkbox].toggle+label+label{font-size:0}:root{--modal-dialog-margin:0.5rem;--modal-dialog-margin-y-sm-up:1.75rem}.query-builder input,.query-builder select:not(.select2-hidden-accessible){--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder input~.error,.query-builder select:not(.select2-hidden-accessible)~.error{color:var(--color-negative)}.query-builder input:hover,.query-builder select:not(.select2-hidden-accessible):hover{border-color:var(--color-dark-400)}.query-builder input:not(:disabled):focus,.query-builder select:not(.select2-hidden-accessible):not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder input:disabled,.query-builder select:not(.select2-hidden-accessible):disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder input::-moz-placeholder,.query-builder select:not(.select2-hidden-accessible)::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder input::placeholder,.query-builder select:not(.select2-hidden-accessible)::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder input.field-valid,.query-builder select:not(.select2-hidden-accessible).field-valid{border-color:var(--color-success)}.query-builder input.field-valid~.success,.query-builder select:not(.select2-hidden-accessible).field-valid~.success{display:block}.query-builder input.field-error,.query-builder select:not(.select2-hidden-accessible).field-error{border-color:var(--color-negative)}.query-builder input.field-error~.error,.query-builder select:not(.select2-hidden-accessible).field-error~.error{display:block}input .query-builder input:-moz-read-only,input.query-builder select:not(.select2-hidden-accessible):-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input .query-builder input:read-only,input.query-builder select:not(.select2-hidden-accessible):read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input .query-builder input:not(:disabled):not(:-moz-read-only):focus,input.query-builder select:not(.select2-hidden-accessible):not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input .query-builder input:not(:disabled):not(:read-only):focus,input.query-builder select:not(.select2-hidden-accessible):not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea .query-builder input,textarea.query-builder select:not(.select2-hidden-accessible){height:auto}select .query-builder input,select.query-builder select:not(.select2-hidden-accessible){padding-right:2rem}.query-builder input,.query-builder select:not(.select2-hidden-accessible){width:100%!important}.djn-table>.djn-tbody td .query-builder input:not(.choices__input),.djn-table>.djn-tbody td .query-builder select:not(.select2-hidden-accessible):not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .select2{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative!important;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in!important;width:100%!important}.query-builder .select2~.error{color:var(--color-negative)}.query-builder .select2:hover{border-color:var(--color-dark-400)}.query-builder .select2:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .select2:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .select2::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .select2::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .select2.field-valid{border-color:var(--color-success)}.query-builder .select2.field-valid~.success{display:block!important}.query-builder .select2.field-error{border-color:var(--color-negative)}.query-builder .select2.field-error~.error{display:block!important}input.query-builder .select2:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.query-builder .select2:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.query-builder .select2:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .select2:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .select2{height:auto}select.query-builder .select2{padding-right:2rem}.query-builder .rules-group-container{background-color:var(--color-transparent)!important;border-color:var(--color-dark-200)!important;border-radius:6px!important;margin:0!important;padding:0!important}.query-builder .rules-group-container:after,.query-builder .rules-group-container:before{display:none}.flatpickr-day .query-builder .rules-group-container:after,.flatpickr-day.query-builder .rules-group-container:before{visibility:hidden}.query-builder .rules-group-container .rules-group-header{align-items:center;background-color:var(--color-dark-100);display:flex;flex-wrap:wrap;gap:1rem;margin-bottom:0;padding:1rem}.query-builder .rules-group-container .rules-group-header .drag-handle{order:1}.query-builder .rules-group-container .rules-group-header button[data-not]{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-transparent)!important;border-style:none!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;display:flex;font-weight:600;gap:.375rem;height:1.5rem;margin-right:1rem!important;padding:0!important;position:relative;text-transform:capitalize}@media (min-width:768px){.query-builder .rules-group-container .rules-group-header button[data-not]{font-size:1rem!important;line-height:1.25rem!important}}.query-builder .rules-group-container .rules-group-header button[data-not]:before{background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:9999px;border-width:1px;content:"";display:block;flex-shrink:0;height:1.5rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.75rem}.query-builder .rules-group-container .rules-group-header button[data-not]:after{background-color:var(--color-dark-200);border-radius:9999px;content:"";display:block;flex-shrink:0;height:1.25rem;left:.125rem;position:absolute;top:.125rem;transition:left .15s ease-in-out,background-color .15s ease-in-out;width:1.25rem}.query-builder .rules-group-container .rules-group-header button[data-not]:not(.active):hover:before{border-color:var(--color-dark-400)}.query-builder .rules-group-container .rules-group-header button[data-not].active:before{background-color:var(--color-primary);border-color:var(--color-primary)}.query-builder .rules-group-container .rules-group-header button[data-not].active:after{background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='m13.805 5.138-6.667 6.667a.667.667 0 0 1-.942 0L2.862 8.47l.943-.942 2.862 2.862 6.195-6.196.943.943Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;left:calc(2.75rem - 22px)}.query-builder .rules-group-container .rules-group-header .group-conditions{align-items:center;display:flex;margin-right:auto;order:2}.query-builder .rules-group-container .rules-group-header .group-actions{align-items:center;display:flex;flex-wrap:wrap;order:3;row-gap:.5rem}.query-builder .rules-group-container .rules-group-header .btn{height:2rem}.query-builder .rules-group-container .rules-list{display:flex;flex-direction:column;gap:1rem;margin:1rem;padding-left:0!important}.query-builder .rules-group-container .group-conditions label.btn{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.btn.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container{display:grid;gap:.5rem;grid-template-columns:repeat(18,1fr);grid-template-rows:repeat(2,1fr);margin:0!important;padding-bottom:.5rem!important;padding-top:.5rem!important}@media (min-width:768px){.query-builder .rule-container{padding-bottom:1rem!important;padding-top:1rem!important}}.query-builder .rule-container{background-color:var(--color-dark-100)!important;border-color:var(--color-dark-200)!important;border-radius:6px!important}.query-builder .rule-container:after,.query-builder .rule-container:before{display:none}.flatpickr-day .query-builder .rule-container:after,.flatpickr-day.query-builder .rule-container:before{visibility:hidden}.query-builder .rule-container .drag-handle{display:flex;grid-column-end:2;grid-column-start:1;grid-row-end:3;grid-row-start:1;justify-content:center;margin:auto 0;width:100%}.query-builder .rule-container .drag-handle:before{width:1.25rem}.query-builder .rule-container .rule-filter-container{grid-column-end:18;grid-column-start:2;grid-row-end:2;grid-row-start:1}.query-builder .rule-container .rule-operator-container{grid-column-end:10;grid-column-start:2;grid-row-end:2;grid-row-start:2;margin-right:0!important;width:100%}.query-builder .rule-container .rule-operator-container:empty{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder .rule-container .rule-operator-container:empty~.error{color:var(--color-negative)}.query-builder .rule-container .rule-operator-container:empty:hover{border-color:var(--color-dark-400)}.query-builder .rule-container .rule-operator-container:empty:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .rule-container .rule-operator-container:empty:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .rule-container .rule-operator-container:empty::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-operator-container:empty::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-operator-container:empty.field-valid{border-color:var(--color-success)}.query-builder .rule-container .rule-operator-container:empty.field-valid~.success{display:block}.query-builder .rule-container .rule-operator-container:empty.field-error{border-color:var(--color-negative)}.query-builder .rule-container .rule-operator-container:empty.field-error~.error{display:block}input.query-builder .rule-container .rule-operator-container:empty:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-operator-container:empty:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-operator-container:empty:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .rule-container .rule-operator-container:empty:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .rule-container .rule-operator-container:empty{height:auto}select.query-builder .rule-container .rule-operator-container:empty{padding-right:2rem}.query-builder .rule-container .rule-operator-container:empty{border-style:none;cursor:not-allowed}.djn-table>.djn-tbody td .query-builder .rule-container .rule-operator-container:empty:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rule-container .rule-value-container{grid-column-end:18;grid-column-start:10;grid-row-end:3;grid-row-start:2;margin-right:0!important;width:100%}.query-builder .rule-container .rule-value-container:empty{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder .rule-container .rule-value-container:empty~.error{color:var(--color-negative)}.query-builder .rule-container .rule-value-container:empty:hover{border-color:var(--color-dark-400)}.query-builder .rule-container .rule-value-container:empty:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .rule-container .rule-value-container:empty:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .rule-container .rule-value-container:empty::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-value-container:empty::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-value-container:empty.field-valid{border-color:var(--color-success)}.query-builder .rule-container .rule-value-container:empty.field-valid~.success{display:block}.query-builder .rule-container .rule-value-container:empty.field-error{border-color:var(--color-negative)}.query-builder .rule-container .rule-value-container:empty.field-error~.error{display:block}input.query-builder .rule-container .rule-value-container:empty:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-value-container:empty:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-value-container:empty:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .rule-container .rule-value-container:empty:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .rule-container .rule-value-container:empty{height:auto}select.query-builder .rule-container .rule-value-container:empty{padding-right:2rem}.query-builder .rule-container .rule-value-container:empty{cursor:not-allowed}.djn-table>.djn-tbody td .query-builder .rule-container .rule-value-container:empty:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rule-container .rule-value-container input[type=text]{padding-left:.625rem;padding-right:.625rem}.query-builder .rule-container .rule-header{display:grid;grid-column-end:19;grid-column-start:18;grid-row-end:3;grid-row-start:1;height:100%;margin:auto 0;width:100%}.query-builder .rule-container .rule-header .btn-group{align-items:center;display:flex;justify-content:center}.query-builder .rule-container .rule-header .btn-group .btn{margin-right:0}.query-builder .drag-handle{flex-shrink:0;height:1.25rem;width:1.25rem}@media (max-width:767px){.query-builder .drag-handle{display:none!important}}.query-builder .drag-handle i{display:none}.flatpickr-day.query-builder .drag-handle i{visibility:hidden}.query-builder .drag-handle:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M6.25 5.833a1.667 1.667 0 1 0 0-3.333 1.667 1.667 0 0 0 0 3.333ZM7.916 10a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm0 5.833a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm5.834-10a1.667 1.667 0 1 0 0-3.333 1.667 1.667 0 0 0 0 3.333ZM15.416 10a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm0 5.833a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .rule-header{order:2}.query-builder .btn[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .btn[data-delete] i{display:none}.flatpickr-day.query-builder .btn[data-delete] i{visibility:hidden}.query-builder .btn[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .btn[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.query-builder .rule-filter-container,.query-builder .rule-operator-container{width:100%}@media (min-width:768px){.query-builder .rule-operator-container{width:50%}}.query-builder .rules-list:empty{display:none!important}.query-builder .rule-value-container{border-style:none!important;display:flex;padding-left:0!important}.query-builder .rule-value-container .select2{border-radius:6px;max-width:100%;min-width:0;overflow:hidden;padding:0!important}.query-builder .rule-value-container .select2:hover{border-color:var(--color-dark-400)!important}.query-builder .rule-value-container .select2 .select2-selection{border-style:none!important;height:100%}.query-builder .rule-value-container .select2 .select2-selection>span{align-items:center;display:flex;height:100%;text-overflow:ellipsis}.query-builder .rule-value-container .select2 .select2-selection .select2-selection__arrow{background-color:var(--color-light);right:0!important;top:0!important}.query-builder button[data-add]{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1)!important;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color)!important;align-items:center;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;display:flex;font-size:.875rem!important;font-weight:600;gap:.25rem;line-height:1.25rem!important;padding-left:.75rem!important;padding-right:.75rem!important}.query-builder button[data-add]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='m7.346 8.667-.005 3.999 1.333.002.005-4.001h3.987V7.333H8.681l.005-3.999-1.333-.001-.005 4H3.333v1.334h4.013Z' fill='%23111827'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:inline-block;flex-shrink:0;height:1rem;width:1rem}@media (min-width:768px){.select2-search{padding:.5rem!important}}.select2-search__field{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative!important;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in!important;width:100%!important}.select2-search__field~.error{color:var(--color-negative)}.select2-search__field:hover{border-color:var(--color-dark-400)}.select2-search__field:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.select2-search__field:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.select2-search__field::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.select2-search__field::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.select2-search__field.field-valid{border-color:var(--color-success)}.select2-search__field.field-valid~.success{display:block!important}.select2-search__field.field-error{border-color:var(--color-negative)}.select2-search__field.field-error~.error{display:block!important}input.select2-search__field:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.select2-search__field:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.select2-search__field:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.select2-search__field:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.select2-search__field{height:auto}select.select2-search__field{padding-right:2rem}.select2-search__field{padding-left:.5rem!important;padding-right:.5rem!important}.select2-dropdown{border-color:var(--color-dark-300)!important;border-radius:6px!important;overflow:hidden}.select2-results__option{font-size:.875rem!important;line-height:1.25rem!important}@media (min-width:768px){.select2-results__option{padding:.625rem!important}}.select2-results__option{transition:background-color .05s ease-in-out,color .05s ease-in-out}.select2-results__option--highlighted{background-color:var(--color-primary)!important;color:var(--color-light)!important}.choices{display:flex;flex-direction:column;position:relative}.choices:not(.search-on):not(.search-off){display:none}.flatpickr-day.choices:not(.search-on):not(.search-off){visibility:hidden}.choices.search-on{padding-top:2.5rem}.choices.search-off .choices__inner>label,.choices.search-off .choices__input{display:none}.flatpickr-day .choices.search-off .choices__inner>label,.flatpickr-day.choices.search-off .choices__input{visibility:hidden}.choices.search-off .choices__list.choices__list--dropdown{margin-top:0}.choices__inner{order:1}.choices__input{background-color:transparent;left:0;padding-right:0;position:absolute;top:0;width:100%!important}.choices__input+label,.choices__list.choices__list--single+label{align-items:center;display:flex;height:2.5rem;justify-content:center;position:absolute;right:0;top:0;width:2.5rem;z-index:-1}.choices__input+label>svg,.choices__list.choices__list--single+label>svg{height:1.25rem;width:1.25rem}.choice__item{position:relative}.choices__list[role=listbox]::-webkit-scrollbar{height:9px;width:9px}.choices__list[role=listbox]::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.choices__list[role=listbox]::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.choices__list[role=listbox]:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.choices__list[role=listbox]{max-height:13.5rem;overflow:auto}.choices__list.choices__list--dropdown{margin:.5rem -.75rem .25rem}.choices__list.choices__list--dropdown .choices__item{color:var(--color-dark-900);padding:.5rem .75rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.choices__list.choices__list--dropdown .choices__item:not(.has-no-choices):not(.has-no-results){cursor:pointer}.choices__list.choices__list--dropdown .choices__item:not(.has-no-choices):not(.has-no-results):hover{background-color:var(--color-dark-100)}.choices__list.choices__list--dropdown .choices__item.has-no-choices{padding-bottom:0;padding-top:.25rem}.choices__list.choices__list--single{display:none}.choices__list.choices__list--multiple{display:flex;flex-wrap:wrap;gap:.25rem;margin-left:-.75rem;margin-right:-.75rem;padding-bottom:0;padding-left:.75rem;padding-right:.75rem}.choices__list.choices__list--multiple:not(:empty){border-color:var(--color-dark-200);border-top-width:1px;padding-top:.75rem}.choices__list.choices__list--multiple .choices__item{align-items:center;background-color:var(--color-dark-100);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;color:var(--color-dark-900);display:flex;font-size:.75rem;font-weight:500;line-height:1rem;padding:.25rem .5rem}.choices__list.choices__list--multiple .choices__item svg{color:var(--color-dark);display:flex;height:1rem;margin-left:.25rem;pointer-events:none;width:1rem}.js-ready .sidebar,.js-ready [class*=":sidebar"]{transition-duration:.3s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}.first-letter\:uppercase:first-letter{text-transform:uppercase}.empty\:hidden:empty{display:none}.hover\:rotate-90:hover{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:bg-dark-100:hover{background-color:var(--color-dark-100)}.hover\:text-dark-900:hover{color:var(--color-dark-900)}.hover\:text-notice:hover{color:var(--color-notice)}.hover\:text-dark-400:hover{color:var(--color-dark-400)}.peer:checked~.peer-checked\:border-dark-300{border-color:var(--color-dark-300)}.peer:checked~.peer-checked\:bg-dark-50{background-color:var(--color-dark-50)}@media (min-width:576px){.sm\:-mx-16{margin-left:-1rem;margin-right:-1rem}.sm\:mb-24{margin-bottom:1.5rem}.sm\:min-w-84{min-width:5.25rem}.sm\:flex-1{flex:1 1 0%}.sm\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}.sm\:gap-24{gap:1.5rem}.sm\:p-24{padding:1.5rem}}@media (min-width:768px){.md\:left-40{left:2.5rem}.md\:top-40{top:2.5rem}.md\:mr-8{margin-right:.5rem}.md\:block{display:block}.md\:hidden{display:none}.md\:w-1\/4{width:25%}.md\:max-w-640{max-width:40rem}.md\:grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}.md\:flex-wrap{flex-wrap:wrap}.md\:gap-16{gap:1rem}.md\:gap-x-8{-moz-column-gap:.5rem;column-gap:.5rem}.md\:p-16{padding:1rem}.md\:px-24{padding-left:1.5rem;padding-right:1.5rem}.md\:pb-32{padding-bottom:2rem}.md\:pt-24{padding-top:1.5rem}.md\:text-30{font-size:1.875rem;line-height:2.75rem}}@media (min-width:992px){.lg\:hidden{display:none}.lg\:w-370{width:23.125rem}.lg\:flex-shrink-0{flex-shrink:0}.lg\:gap-24{gap:1.5rem}}@media (min-width:1200px){.xl\:fixed{position:fixed}.xl\:left-260{left:16.25rem}.xl\:\!block{display:block!important}.xl\:hidden{display:none}.xl\:pl-260{padding-left:16.25rem}}@media (max-width:1199px){.max-lg\:sidebar{--tw-translate-x:-100%;height:100%;left:0;overflow:hidden;position:fixed;top:0;z-index:51}.max-lg\:sidebar,.max-lg\:sidebar.active{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.max-lg\:sidebar.active{--tw-translate-x:0}.max-lg\:sidebar.active+.bg-filter{opacity:1;transition:opacity .3s ease-in-out,z-index 0s linear 0s;z-index:50}.max-lg\:py-16{padding-bottom:1rem;padding-top:1rem}}@media (max-width:991px){.max-md\:flex-wrap{flex-wrap:wrap}}@media (max-width:767px){.max-sm\:-order-1{order:-1}.max-sm\:mt-8{margin-top:.5rem}.max-sm\:hidden{display:none}.max-sm\:flex-shrink-0{flex-shrink:0}.max-sm\:flex-wrap{flex-wrap:wrap}.max-sm\:overflow-x-auto{overflow-x:auto}.max-sm\:px-16{padding-left:1rem;padding-right:1rem}.max-sm\:px-24{padding-left:1.5rem;padding-right:1.5rem}}@media (max-width:575px){.max-xs\:hidden{display:none}.max-xs\:w-full{width:100%}.max-xs\:flex-wrap{flex-wrap:wrap}.max-xs\:px-20{padding-left:1.25rem;padding-right:1.25rem}.max-xs\:py-16{padding-bottom:1rem;padding-top:1rem}.max-xs\:text-12{font-size:.75rem;line-height:1.25rem}}
+/*! tailwindcss v3.1.8 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}:root{--color-light:#fff;--color-transparent:transparent;--color-dark-900:#111827;--color-dark-800:#1f2937;--color-dark-700:#374151;--color-dark-600:#4b5563;--color-dark:#6b7280;--color-dark-400:#9ca3af;--color-dark-300:#d1d5db;--color-dark-200:#e5e7eb;--color-dark-100:#f3f4f6;--color-dark-50:#f9fafb;--color-dark-a:17 24 39;--color-primary-900:#d3f6f8;--color-primary-800:#003a3d;--color-primary-700:#006166;--color-primary-600:#008188;--color-primary:#00959d;--color-primary-400:#00c2cc;--color-primary-300:#59d3da;--color-primary-200:#99e7eb;--color-primary-100:#d3f6f8;--color-primary-50:#edfafb;--color-secondary-900:#3d2500;--color-secondary-800:#7a4901;--color-secondary-700:#a26201;--color-secondary-600:#cb7a01;--color-secondary:#f18f01;--color-secondary-400:#fea520;--color-secondary-300:#feb548;--color-secondary-200:#fec671;--color-secondary-100:#ffdeae;--color-secondary-50:#fff7eb;--color-success-900:#064e3b;--color-success-800:#065f46;--color-success-700:#047857;--color-success-600:#059669;--color-success:#10b981;--color-success-400:#34d399;--color-success-300:#6ee7b7;--color-success-200:#a7f3d0;--color-success-100:#d1fae5;--color-success-50:#d1fae5;--color-warning-900:#78350f;--color-warning-800:#78350f;--color-warning-700:#b45309;--color-warning-600:#d97706;--color-warning:#f59e0b;--color-warning-400:#fbbf24;--color-warning-300:#fcd34d;--color-warning-200:#fde68a;--color-warning-100:#fef3c7;--color-warning-50:#fffbeb;--color-negative-900:#7f1d1d;--color-negative-800:#991b1b;--color-negative-700:#b91c1c;--color-negative-600:#dc2626;--color-negative:#ef4444;--color-negative-400:#f87171;--color-negative-300:#fca5a5;--color-negative-200:#fecaca;--color-negative-100:#fee2e2;--color-negative-50:#fef2f2;--color-notice-900:#0c4a6e;--color-notice-800:#075985;--color-notice-700:#0369a1;--color-notice-600:#0369a1;--color-notice:#0284c7;--color-notice-400:#0ea5e9;--color-notice-300:#38bdf8;--color-notice-200:#7dd3fc;--color-notice-100:#bae6fd;--color-notice-50:#e0f2fe}html{scroll-behavior:smooth}body{background-color:var(--color-dark-100);color:var(--color-dark);font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol}svg{fill:currentColor;display:inline-flex}label[for]{cursor:pointer}hr{border-color:var(--color-dark-200)}small{font-size:.75rem;line-height:1.25rem}a{cursor:pointer;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}a.link,a[href]:hover{color:var(--color-primary)}a[aria-disabled=true]{cursor:not-allowed;pointer-events:none}select{-webkit-appearance:none;-moz-appearance:none;appearance:none;cursor:pointer}button:disabled{pointer-events:none}input[type=submit]{cursor:pointer}.scrollbar-measure{height:100px;overflow:scroll;position:absolute;top:-9999px;width:100px}.custom-scrollbar::-webkit-scrollbar,.tabulator .tabulator-tableholder::-webkit-scrollbar{height:9px;width:9px}.custom-scrollbar::-webkit-scrollbar-track,.tabulator .tabulator-tableholder::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.custom-scrollbar::-webkit-scrollbar-thumb,.tabulator .tabulator-tableholder::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.custom-scrollbar:hover::-webkit-scrollbar-thumb,.tabulator .tabulator-tableholder:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.outline{outline-style:solid;outline-width:1px}:focus-visible{outline:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.btn{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.btn>span{-webkit-box-orient:vertical;-webkit-line-clamp:2;display:-webkit-box;margin-right:auto;overflow:hidden}.btn>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.btn:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.btn:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);color:var(--color-dark-900)}.btn:focus,.btn:not(:disabled):hover:active{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color)}.btn:focus-visible{outline:none}.btn:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.btn-primary{background-color:var(--color-primary);border-color:var(--color-primary);color:var(--color-light)}.btn-primary:not(:disabled):hover{background-color:var(--color-primary-600);border-color:var(--color-primary-600);color:var(--color-light)}.btn-primary:not(:disabled):hover:active{background-color:var(--color-primary-700);border-color:var(--color-primary-700);color:var(--color-light)}.btn-primary:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-primary:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-primary.btn-empty{background-color:var(--color-primary-50);color:var(--color-primary)}.btn-primary.btn-empty:not(:disabled):hover,.btn-primary.btn-empty:not(:disabled):hover:active{background-color:var(--color-primary-100);color:var(--color-primary)}.btn-primary-light{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-primary-50);border-color:var(--color-transparent);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-primary)}.btn-primary-light:not(:disabled):hover,.btn-primary-light:not(:disabled):hover:active{background-color:var(--color-primary-100);border-color:var(--color-transparent)}.btn-primary-light:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-primary-light:disabled{background-color:var(--color-transparent);border-color:var(--color-transparent)}.btn-secondary{background-color:var(--color-secondary);border-color:var(--color-secondary);color:var(--color-dark-900)}.btn-secondary:not(:disabled):hover{background-color:var(--color-secondary-600);border-color:var(--color-secondary-600);color:var(--color-dark-900)}.btn-secondary:not(:disabled):hover:active{background-color:var(--color-secondary-700);border-color:var(--color-secondary-700)}.btn-secondary:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-secondary:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-destructive{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-negative-300);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-negative)}.btn-destructive:not(:disabled):hover{background-color:var(--color-negative-50);border-color:var(--color-negative-400);color:var(--color-negative)}.btn-destructive:not(:disabled):hover:active{background-color:var(--color-negative-100);border-color:var(--color-negative-400);color:var(--color-negative)}.btn-destructive:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-destructive:disabled{border-color:rgb(var(--color-dark-a)/.05)}.btn-empty{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent);border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn-empty:not(:disabled):hover{background-color:rgb(var(--color-dark-a)/.05)}.btn-empty:not(:disabled):hover:active{background-color:rgb(var(--color-dark-a)/.1)}.btn-empty:disabled{background-color:var(--color-transparent);color:var(--color-dark)}.btn-small{height:2rem;padding-left:.75rem;padding-right:.75rem}.btn-small>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.btn-small>svg{height:1rem;width:1rem}.btn-tiny{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);font-size:.75rem;height:1.5rem;line-height:1rem;padding-left:.5rem;padding-right:.5rem}.btn-tiny>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.btn-tiny>svg{height:1rem;width:1rem}.btn-tiny.btn-destructive{background-color:var(--color-negative-50);border-style:none}.btn-tiny.btn-destructive:not(:disabled):hover,.btn-tiny.btn-destructive:not(:disabled):hover:active{background-color:var(--color-negative-100)}@media (max-width:767px){.btn-icon{justify-content:center!important;padding-left:0;padding-right:0;width:2.5rem}.btn-icon>span{display:none}}.input{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.input~.error{color:var(--color-negative)}.input:hover{border-color:var(--color-dark-400)}.input:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.input:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.input::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.input::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.input.field-valid{border-color:var(--color-success)}.input.field-valid~.success{display:block}.input.field-error{border-color:var(--color-negative)}.input.field-error~.error{display:block}input.input:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.input:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.input:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.input:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.input{height:auto}.input-file{align-items:center;border-color:var(--color-dark-300);border-radius:6px;border-style:dashed;border-width:1px;display:flex;padding:1rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.input-file input[type=file]{cursor:pointer;height:100%;left:0;opacity:0;position:absolute;top:0;width:100%}.input-file .input-file-upload-icon{background-color:var(--color-dark-100);transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.input-file:not(.filled):hover{background-color:var(--color-primary-50);border-color:var(--color-primary)}.input-file:not(.filled):hover .input-file-upload-icon{background-color:var(--color-light);color:var(--color-primary)}.input-file:not(.filled) .js-input-file-filled{display:none}.flatpickr-day.input-file:not(.filled) .js-input-file-filled{visibility:hidden}.input-file:not(.filled) .js-input-file-image{display:none}.flatpickr-day.input-file:not(.filled) .js-input-file-image{visibility:hidden}.input-file.filled{border-style:solid}.input-file.filled input[type=file]{z-index:-1}.input-file.filled .js-input-file-empty{display:none}.flatpickr-day.input-file.filled .js-input-file-empty{visibility:hidden}.checkbox,.radio{opacity:0;position:absolute;top:0;z-index:-1}.checkbox~label,.radio~label{display:flex;font-size:.875rem;line-height:1.25rem;min-height:1.25rem;padding-left:2rem;position:relative}.checkbox~label:after,.checkbox~label:before,.radio~label:after,.radio~label:before{content:"";display:block;position:absolute}.checkbox~label:before,.radio~label:before{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);height:1.25rem;left:0;outline-color:var(--color-transparent);outline-offset:2px;outline-style:solid;outline-width:2px;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:1.25rem}.checkbox:not(:disabled):hover+label:before,.radio:not(:disabled):hover+label:before{border-color:var(--color-dark-400)}.checkbox:not(:disabled):hover+label:after,.radio:not(:disabled):hover+label:after{opacity:1}.checkbox:not(:disabled):focus+label:before,.radio:not(:disabled):focus+label:before{outline-color:var(--color-primary)}.checkbox:disabled+label,.radio:disabled+label{cursor:not-allowed}.checkbox:disabled+label:before,.radio:disabled+label:before{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-300);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.checkbox:checked+label:after,.radio:checked+label:after{opacity:1}.checkbox:checked:not(:disabled)+label:before,.radio:checked:not(:disabled)+label:before{background-color:var(--color-primary);border-color:var(--color-primary)}.checkbox:checked:not(:disabled):hover+label:before,.radio:checked:not(:disabled):hover+label:before{background-color:var(--color-primary-600);border-color:var(--color-primary-600)}.checkbox:checked:not(:disabled):hover+label:after,.radio:checked:not(:disabled):hover+label:after{opacity:1}.checkbox~label:before{border-radius:6px}.checkbox~label:after{height:1.125rem;height:18px;left:1px;opacity:0;top:1px;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);width:1.125rem;width:18px}.checkbox:checked:not(:disabled):hover+label:after,.checkbox~label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m20.707 7.707-10 10a1 1 0 0 1-1.414 0l-5-5 1.414-1.414L10 15.586l9.293-9.293 1.414 1.414Z' fill='%23E5E7EB'/%3E%3C/svg%3E")}.checkbox:indeterminate+label:before{background-color:var(--color-primary);border-color:var(--color-primary)}.checkbox:indeterminate+label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M19.25 13h-14v-2h14v2Z' fill='%23E5E7EB'/%3E%3C/svg%3E");opacity:1}.checkbox:indeterminate:not(:disabled):hover+label:before{background-color:var(--color-primary-600);border-color:var(--color-primary-600)}.checkbox-delete+label{align-items:center;color:var(--color-dark-300);display:flex;height:100%;justify-content:center;padding:.5rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:100%}.checkbox-delete+label:after,.checkbox-delete+label:before{display:none}.flatpickr-day .checkbox-delete+label:after,.flatpickr-day.checkbox-delete+label:before{visibility:hidden}.checkbox-delete+label:hover{color:var(--color-dark-400)}.checkbox-delete:checked+label{color:var(--color-negative)}.radio+label{align-items:center;color:var(--color-dark-900);display:flex;justify-content:space-between;padding:.75rem 1rem}.radio+label:before{display:none}.flatpickr-day.radio+label:before{visibility:hidden}.radio+label:after{display:none;flex-shrink:0;height:1rem;margin-left:1rem;position:relative;width:1rem}.flatpickr-day.radio+label:after{visibility:hidden}.radio+label:after{background:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath fill='%23009FA7' fill-rule='evenodd' clip-rule='evenodd' d='M8.437 17.09 20.794 4.79l1.411 1.418-13.062 13a1 1 0 0 1-1.411 0l-5.938-5.91 1.411-1.417 5.232 5.207Z'/%3E%3C/svg%3E")}.radio:checked+label,.radio:hover+label{background-color:var(--color-dark-100)}.radio:checked+label:after{display:flex}input:not([type=number])::-webkit-inner-spin-button,input:not([type=number])::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.checkbox.checkbox-icon+label{color:var(--color-dark-300);padding-left:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.checkbox.checkbox-icon+label:after,.checkbox.checkbox-icon+label:before{display:none}.flatpickr-day .checkbox.checkbox-icon+label:after,.flatpickr-day.checkbox.checkbox-icon+label:before{visibility:hidden}.checkbox.checkbox-icon+label:hover{color:var(--color-dark-700)}.checkbox.checkbox-icon:not(:checked)+label>svg:last-child{display:none}.flatpickr-day.checkbox.checkbox-icon:not(:checked)+label>svg:last-child{visibility:hidden}.checkbox.checkbox-icon:checked+label>svg:first-child{display:none}.flatpickr-day.checkbox.checkbox-icon:checked+label>svg:first-child{visibility:hidden}input[type=search]{padding-right:0}input[type=search]::-webkit-search-cancel-button{-webkit-appearance:none;background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg width='24' height='24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m12 13.414 4.293 4.293 1.414-1.414L13.414 12l4.293-4.293-1.414-1.414L12 10.586 7.707 6.293 6.293 7.707 10.586 12l-4.293 4.293 1.414 1.414L12 13.414Z' fill='%236B7280'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;cursor:pointer;height:40px;width:40px}select{-webkit-appearance:none;-moz-appearance:none;background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg fill='%236B7280' viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M12.64 18.142a.904.904 0 0 1-1.389 0l-3.04-3.649a.904.904 0 0 1 .694-1.482h6.08a.904.904 0 0 1 .695 1.482l-3.04 3.649ZM11.252 5.325a.904.904 0 0 1 1.388 0l3.04 3.648a.904.904 0 0 1-.694 1.482h-6.08a.904.904 0 0 1-.695-1.482l3.04-3.648Z'/%3E%3C/svg%3E");background-position:right 10px top 50%;background-repeat:no-repeat;background-size:1.25rem;cursor:pointer}select.input{padding-right:2rem}.dropdown-menu{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);display:none;font-size:.875rem;left:0;line-height:1.25rem;max-height:18.75rem;position:absolute;top:100%;width:14rem;z-index:20}.flatpickr-day.dropdown-menu{visibility:hidden}.dropdown-menu{flex-direction:column;white-space:normal}.dropdown-menu>ul::-webkit-scrollbar{height:9px;width:9px}.dropdown-menu>ul::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.dropdown-menu>ul::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.dropdown-menu>ul:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.dropdown-menu>ul{overflow-x:hidden;overflow-y:auto}.dropdown-menu:not(.show).transition-width{display:flex;width:0}.dropdown-menu:not(.show).transition-height{display:flex;height:0}.dropdown-menu.show,.dropdown-menu:not(.show).fade{display:flex}.dropdown-menu-link{color:var(--color-dark-700);cursor:pointer;display:flex;padding:.75rem 1rem;transition-duration:.1s;transition-property:color,background-color;transition-timing-function:ease-in;white-space:nowrap}.dropdown-menu-link:hover{background-color:var(--color-dark-100);color:var(--color-dark-900)}.dropdown-menu-link:focus{color:var(--color-primary)}.dropdown-menu hr{border-color:var(--color-dark-200);border-width:1px;margin-bottom:.25rem;margin-top:.25rem}.btn[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.btn[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.btn[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.btn[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dropdown-menu-datepicker{@appy w-auto h-auto max-w-none max-h-none}.dropdown-menu-datepicker .flatpickr-calendar{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);margin-left:-.75rem;margin-right:-.75rem}input[type=checkbox].toggle{opacity:0;position:absolute;top:0;z-index:-1}input[type=checkbox].toggle~label{color:var(--color-dark-900);display:flex;font-size:.875rem;font-weight:500;line-height:1.25rem;padding-left:3.5rem;position:relative;top:.125rem}input[type=checkbox].toggle+label{background-color:var(--color-dark-200);border-radius:9999px;display:block;height:1.5rem;left:0;outline-color:var(--color-transparent);outline-offset:2px;outline-style:solid;outline-width:2px;padding-left:0;position:absolute;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.75rem}input[type=checkbox].toggle+label:after,input[type=checkbox].toggle+label:before{content:"";display:block;position:absolute}input[type=checkbox].toggle+label:before{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-radius:9999px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);height:1.25rem;left:.125rem;top:.125rem;transition:left .15s ease-in-out;width:1.25rem}input[type=checkbox].toggle+label:after{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m20.707 7.707-10 10a1 1 0 0 1-1.414 0l-5-5 1.414-1.414L10 15.586l9.293-9.293 1.414 1.414Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-size:1rem;height:1.25rem;left:.125rem;opacity:0;top:.125rem;transition:opacity .15s ease-in-out,left .15s ease-in-out;width:1.25rem}input[type=checkbox].toggle:not(:disabled):hover+label{background-color:var(--color-dark-300)}input[type=checkbox].toggle:not(:disabled):focus+label{outline-color:var(--color-primary)}input[type=checkbox].toggle:checked+label{background-color:var(--color-primary)}input[type=checkbox].toggle:checked+label:after,input[type=checkbox].toggle:checked+label:before{left:calc(100% - 1.375rem);opacity:1}input[type=checkbox].toggle:checked:not(:disabled):hover+label{background-color:var(--color-primary-600)}input[type=checkbox].toggle:checked:not(:disabled):hover+label:after{opacity:.5}input[type=checkbox].toggle~p{font-size:.875rem;line-height:1.25rem;margin-top:0;padding-left:3.5rem}.modal{display:none;height:100%;left:0;outline:0;overflow-x:hidden;overflow-y:auto;position:fixed;top:0;width:100%;z-index:1010}.modal-dialog{align-items:center;display:flex;height:100%;min-height:calc(100% - var(--modal-dialog-margin)*2);pointer-events:none;position:relative;width:auto}@media (min-width:576px){.modal-dialog{height:calc(100% - var(--modal-dialog-margin)*2);margin:var(--modal-dialog-margin)}}.modal.fade .modal-dialog{transform:translateY(-50px);transition:transform .15s ease-out}.modal.show .modal-dialog{transform:none}.modal.modal-static .modal-dialog{transform:scale(1.02)}.modal-dialog .modal-body{overflow-y:auto}.modal-dialog .modal-body::-webkit-scrollbar{height:9px;width:9px}.modal-dialog .modal-body::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.modal-dialog .modal-body::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.modal-dialog .modal-body:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}@media (min-width:576px){.modal-content{border-radius:6px}}.modal-content{background-clip:padding-box;background-color:#fff;display:flex;flex-direction:column;margin:0 auto;max-height:100%;outline:0;overflow:hidden;pointer-events:auto;position:relative;width:100%}@media (max-width:767px){.modal-content{height:100%}}.modal-backdrop{-webkit-backdrop-filter:blur(.5rem);backdrop-filter:blur(.5rem);background-color:rgb(var(--color-dark-a)/.5);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:1000}.modal-backdrop.fade{opacity:0}.modal-backdrop.show{opacity:1}.modal-header{align-items:center;border-bottom-width:1px;border-color:var(--color-dark-200);border-top-left-radius:6px;border-top-right-radius:6px;display:flex;flex-shrink:0;justify-content:space-between;padding:1rem}.modal-body{flex:1 1 auto;padding:1rem;position:relative}.modal-footer{align-items:center;border-bottom-left-radius:6px;border-bottom-right-radius:6px;border-color:var(--color-dark-200);border-top-width:1px;display:flex;flex-shrink:0;flex-wrap:wrap;gap:.5rem;justify-content:flex-end;padding:1rem}@media (min-width:576px){.modal-dialog{height:calc(100% - var(--modal-dialog-margin-y-sm-up)*2);margin:var(--modal-dialog-margin-y-sm-up) auto;max-width:45rem;min-height:calc(100% - var(--modal-dialog-margin-y-sm-up)*2)}.modal.modal-small>.modal-dialog{max-width:23rem}}.tooltip{word-wrap:break-word;display:block;font-size:.75rem;line-height:1rem;opacity:0;padding-bottom:.5rem;padding-top:.5rem;position:absolute;z-index:10}.tooltip.show{opacity:1}.tooltip .tooltip-arrow{display:block;height:.5rem;position:absolute;width:1rem}.tooltip .tooltip-arrow:before{border-color:transparent;border-style:solid;content:"";position:absolute}&[data-popper-placement^=top] .tooltip-arrow,.tooltip.bs-tooltip-top .tooltip-arrow{bottom:0}&[data-popper-placement^=top] .tooltip-arrow:before,.tooltip.bs-tooltip-top .tooltip-arrow:before{border-top-color:rgb(var(--color-dark-a)/90%);border-width:.5rem .5rem 0;top:-1px}&[data-popper-placement^=bottom] .tooltip-arrow,.tooltip.bs-tooltip-bottom .tooltip-arrow{top:0}&[data-popper-placement^=bottom] .tooltip-arrow:before,.tooltip.bs-tooltip-bottom .tooltip-arrow:before{border-bottom-color:rgb(var(--color-dark-a)/90%);border-width:0 .5rem .5rem;bottom:-1px}&[data-popper-placement^=right],.tooltip.bs-tooltip-end{padding:0 .5rem}&[data-popper-placement^=right] .tooltip-arrow,.tooltip.bs-tooltip-end .tooltip-arrow{height:.1rem;left:0;width:.5rem}&[data-popper-placement^=right] .tooltip-arrow:before,.tooltip.bs-tooltip-end .tooltip-arrow:before{border-right-color:rgb(var(--color-dark-a)/90%);border-width:.5rem .5rem .5rem 0;right:-1px}&[data-popper-placement^=left],.tooltip.bs-tooltip-start{padding:0 .5rem}&[data-popper-placement^=left] .tooltip-arrow,.tooltip.bs-tooltip-start .tooltip-arrow{height:.1rem;right:0;width:.5rem}&[data-popper-placement^=left] .tooltip-arrow:before,.tooltip.bs-tooltip-start .tooltip-arrow:before{border-left-color:rgb(var(--color-dark-a)/90%);border-width:.5rem 0 .5rem .5rem;left:-1px}.tooltip-inner{--tw-shadow:0 2px 4px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 2px 4px 0 var(--tw-shadow-color);background-color:rgb(var(--color-dark-a)/.9);border-radius:6px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-light);max-width:200px;padding:.5rem}.card{background-color:var(--color-light);border-color:var(--color-dark-200);border-width:1px;min-width:0;padding:1.25rem}@media (min-width:576px){.card{border-radius:6px}}@media (min-width:768px){.card{padding:1.5rem}}@media (max-width:575px){.card{border-bottom-width:0;padding-bottom:2rem;padding-top:2rem}}.card>header{align-items:center;display:flex;font-size:1.125rem;font-weight:600;line-height:1.25rem;margin-bottom:1.5rem}.column-widget-columns>li{align-items:center;display:flex;padding:.5rem .75rem;position:relative}@media (pointer:fine){.column-widget-columns>li .checkbox.checkbox-icon:not(:checked)+label{opacity:0}}.column-widget-columns>li:hover .checkbox.checkbox-icon+label{opacity:1}.tab-pane:not(.active){display:none}.flatpickr-day.tab-pane:not(.active){visibility:hidden}.collapse-btn,.collapse-horizontal-btn{align-items:center;display:flex;justify-content:space-between}.collapse-btn svg:last-child,.collapse-horizontal-btn svg:last-child{transition:transform .2s}.collapse-btn:not(.collapsed) svg:last-child,.collapse-horizontal-btn:not(.collapsed) svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.collapse-horizontal.collapsed{max-width:0;opacity:0;overflow:hidden;transition:max-width .2s ease-in-out,opacity .2s ease-in}.collapse-horizontal.\!collapsed{max-width:0!important;opacity:0!important;overflow:hidden!important;transition:max-width .2s ease-in-out,opacity .2s ease-in!important}.bg-filter{background-color:rgb(var(--color-dark-a)/.3);height:100vh;opacity:0;transition:opacity .3s ease-in-out,z-index 0s linear .3s;width:100vw;z-index:-1}.bg-filter,.sidebar{left:0;position:fixed;top:0}.sidebar{--tw-translate-x:-100%;height:100%;overflow:hidden;z-index:51}.sidebar,.sidebar.active{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.sidebar.active{--tw-translate-x:0}.sidebar.active+.bg-filter{opacity:1;transition:opacity .3s ease-in-out,z-index 0s linear 0s;z-index:50}.menu-item{border-radius:8px;color:var(--color-dark-900)}.menu-item a,.menu-item>div{display:flex}.menu-item>a:hover svg{color:var(--color-primary)}.menu-item span{display:inline-block;line-height:1.25rem}.menu-item span:first-letter{text-transform:capitalize}.menu-item svg{color:var(--color-dark)}.menu-item .collapse-btn>a{width:calc(100% - 2.25rem)}.menu-item .collapse-btn:hover{color:var(--color-primary)}.menu-item .collapse-btn:not(.collapsed)>a{font-weight:600}.menu-item .collapse-btn:not(.collapsed)>a>svg{color:var(--color-primary)}.menu-item.active{background-color:var(--color-primary-100);color:var(--color-primary-600);font-weight:600}.menu-item.active svg{color:var(--color-primary)}.key{display:inline-flex;font-size:.75rem;line-height:1.25rem;margin-bottom:.125rem;padding-left:.375rem;padding-right:.375rem;position:relative}.key,.key:after{border-color:var(--color-dark-300);border-radius:6px;border-width:1px}.key:after{align-items:center;bottom:calc(-1px - .125rem);content:"";display:flex;justify-content:center;left:-1px;position:absolute;right:-1px;top:-1px}.badge{align-items:center;background-color:var(--color-notice-100);border-radius:9999px;color:var(--color-notice-700);display:inline-flex;font-size:.75rem;font-weight:500;line-height:1rem;padding:.125rem .5rem}.badge:before{background-color:currentColor;border-radius:9999px;content:"";height:.25rem;margin-right:.25rem;width:.25rem}.badge-large{padding:.25rem .625rem}.badge-large:before{height:.375rem;margin-right:.5rem;width:.375rem}.badge-simple:before{display:none}.flatpickr-day.badge-simple:before{visibility:hidden}.badge-positive{background-color:var(--color-success-100);color:var(--color-success-700)}.badge-warning{background-color:var(--color-warning-100);color:var(--color-warning-700)}.badge-negative{background-color:var(--color-negative-100);color:var(--color-negative-700)}.badge-neutral{background-color:var(--color-dark-200);color:var(--color-dark-600)}.badge-primary{background-color:var(--color-primary-100);color:var(--color-primary-700)}.nav-tabs{border-bottom-width:1px;border-color:var(--color-dark-200);display:flex;gap:.5rem;overflow-x:auto}.nav-tabs .tab-link{border-bottom:3px solid transparent;display:block;padding-bottom:calc(1rem - 3px);padding-left:1rem;padding-right:1rem;padding-top:1rem;transition-duration:.15s;transition-property:color,border;transition-timing-function:ease-in;white-space:nowrap}.nav-tabs .tab-link:hover{border-color:var(--color-dark-200)}.nav-tabs .tab-link.active{border-color:var(--color-primary);color:var(--color-primary)}.saved-filters{color:var(--color-dark-600);display:flex;font-size:.875rem;font-weight:500;gap:.5rem;line-height:1.25rem}.saved-filters>li button{align-items:center;border-radius:6px;cursor:pointer;display:flex;height:2.5rem;padding:.5rem 1rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.saved-filters>li button:not(:disabled):hover{background-color:var(--color-dark-100)}.saved-filters>li button:not(:disabled).active{background-color:var(--color-primary-100);color:var(--color-primary-600)}.saved-filters>li button:disabled{opacity:0}.saved-filters>li button.changed span:after{content:"*";padding-left:2px}.alert{border-radius:8px;font-size:.875rem;line-height:1.25rem;padding:1rem}#save-view-modal-button:disabled{display:none}.flatpickr-day#save-view-modal-button:disabled{visibility:hidden}#filters-collapse-button:not(.collapsed){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.django-ckeditor-widget{display:block!important;flex:1}.django-ckeditor-widget>.cke{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);width:auto!important}.django-ckeditor-widget>.cke,.django-ckeditor-widget>.cke>.cke_inner{border-radius:6px}.django-ckeditor-widget>.cke>.cke_inner>.cke_top{border-top-left-radius:6px;border-top-right-radius:6px}.django-ckeditor-widget>.cke>.cke_inner>.cke_bottom{border-bottom-left-radius:6px;border-bottom-right-radius:6px}.django-ckeditor-widget>textarea:-moz-read-only+.cke{height:100%}.django-ckeditor-widget>textarea:read-only+.cke{height:100%}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner{height:100%}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner{height:100%}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_bottom,.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_top{display:none}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_bottom,.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_top{display:none}.flatpickr-day .django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_bottom,.flatpickr-day.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_top{visibility:hidden}.flatpickr-day .django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_bottom,.flatpickr-day.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_top{visibility:hidden}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_contents{border-radius:6px;height:100%!important}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_contents{border-radius:6px;height:100%!important}.django-ckeditor-widget>textarea:-moz-read-only+.cke>.cke_inner>.cke_contents>.cke_wysiwyg_frame{background-color:var(--color-dark-50)}.django-ckeditor-widget>textarea:read-only+.cke>.cke_inner>.cke_contents>.cke_wysiwyg_frame{background-color:var(--color-dark-50)}.errorlist{color:var(--color-negative);font-size:.75rem;line-height:1rem;margin-top:.5rem}.filter-dropdown-button{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.filter-dropdown-button>span{-webkit-line-clamp:2;margin-right:auto}.filter-dropdown-button>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.filter-dropdown-button:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.filter-dropdown-button:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);color:var(--color-dark-900)}.filter-dropdown-button:focus,.filter-dropdown-button:not(:disabled):hover:active{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color)}.filter-dropdown-button:focus-visible{outline:none}.filter-dropdown-button:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.filter-dropdown-button{height:2rem;padding-left:.75rem;padding-right:.75rem}.filter-dropdown-button>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.filter-dropdown-button>svg{height:1rem;width:1rem}.filter-dropdown-button[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.filter-dropdown-button[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.filter-dropdown-button[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.filter-wrapper>.filter-dropdown-button.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.filter-dropdown-button.empty>svg:not(:last-child){visibility:hidden}.filter-dropdown-button{border-radius:9999px;position:relative}.tabulator-row .tabulator-cell .filter-dropdown-button+.btn{margin-left:.25rem}.djn-table>.djn-tbody td .filter-dropdown-button:not(.input-file-edit-btn){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rules-group-container .rules-group-header .filter-dropdown-button{height:2rem}.query-builder .rules-group-container .group-conditions label.filter-dropdown-button{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.filter-dropdown-button.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container .rule-header .filter-dropdown-button-group .btn{margin-right:0}.query-builder .filter-dropdown-button[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .filter-dropdown-button[data-delete] i{display:none}.flatpickr-day.query-builder .filter-dropdown-button[data-delete] i{visibility:hidden}.query-builder .filter-dropdown-button[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .filter-dropdown-button[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.filter-dropdown-button>svg:not(:last-child){--tw-translate-y:-50%;color:var(--color-dark);position:absolute;right:.75rem;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.filter-dropdown-button>svg:not(:last-child):hover{color:var(--color-dark-900)}.filter-dropdown-button>svg:last-child{visibility:hidden}.filter-dropdown-button.show>svg:not(:last-child){color:var(--color-primary)}.filter-dropdown-button.empty{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.filter-dropdown-button.empty>svg:last-child{display:block;visibility:visible}.filter-dropdown-button.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-dropdown-button.empty>svg:not(:last-child){visibility:hidden}.filter-wrapper>.btn.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.btn.empty>svg:not(:last-child){visibility:hidden}.table-selected-rows-bar{align-items:center;background-color:var(--color-light);display:flex;height:3rem;left:0;margin-top:1px;overflow-x:auto;padding-bottom:.5rem;padding-right:1rem;padding-top:.5rem;position:absolute;right:0;top:100%}.table-selected-rows-bar.show{z-index:1}.copy-translations-button-wrapper{align-items:center;display:flex;margin-right:.75rem;padding-top:1.625rem;position:absolute;right:100%;top:0;z-index:1}.django-ckeditor-widget+.copy-translations-button-wrapper{bottom:0;height:100%}.detail-view-action-bar:before{content:"";display:block;height:4.5rem}.detail-view-action-bar>div{--tw-shadow:0px -4px 16px 0px rgba(17,24,39,.08);--tw-shadow-colored:0px -4px 16px 0px var(--tw-shadow-color);align-items:center;background-color:var(--color-light);bottom:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);display:flex;left:0;padding:1rem 1.5rem;position:fixed;right:0;z-index:1}@media (min-width:1200px){.detail-view-action-bar>div{left:16.25rem}}.translations-status-fieldset{position:relative}.translations-status-fieldset>header{height:2rem}.translations-status-fieldset .translation-status-row:last-child{margin-bottom:0}.translations-status-fieldset:has(.is-empty){display:none}.mermaid .label{color:var(--color-dark-900)!important}.mermaid .node circle,.mermaid .node ellipse,.mermaid .node polygon,.mermaid .node rect{fill:var(--color-primary-100)!important;stroke:var(--color-primary-200)!important}.mermaid .mermaid_purchase_active .label{color:var(--color-light)!important}.cms-pagetree-section:after{clear:both;content:"";display:block}.page-loading{display:none}.page-loading.htmx-request{display:block}.page-loading .loader,.page-loading .loader:after{border-radius:50%;height:42px;width:42px}.page-loading .loader{animation:loading 1.1s linear infinite;border-color:var(--color-primary);border-left-color:var(--color-dark-300);border-width:4px;font-size:10px;text-indent:-9999em;transform:translateZ(0)}@keyframes loading{0%{transform:rotate(0deg)}to{transform:rotate(1turn)}}.read-only-password-hash a{color:var(--color-primary)}.dropdown-btn.show{background-color:var(--color-dark-200)}.dropdown-menu{padding-bottom:0;padding-top:0}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.visible{visibility:visible}.\!visible{visibility:visible!important}.invisible{visibility:hidden}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{bottom:0;left:0;right:0;top:0}.top-0{top:0}.bottom-0{bottom:0}.left-0{left:0}.top-24{top:1.5rem}.right-24{right:1.5rem}.left-10{left:.625rem}.left-24{left:1.5rem}.right-0{right:0}.top-16{top:1rem}.right-16{right:1rem}.left-260{left:16.25rem}.top-1\/2{top:50%}.right-10{right:.625rem}.left-1\/2{left:50%}.z-1{z-index:1}.z-1000{z-index:1000}.order-1{order:1}.m-auto{margin:auto}.-m-8{margin:-.5rem}.m-10{margin:.625rem}.-my-2{margin-bottom:-.125rem;margin-top:-.125rem}.my-32{margin-bottom:2rem;margin-top:2rem}.mx-auto{margin-left:auto;margin-right:auto}.-mx-32{margin-left:-2rem;margin-right:-2rem}.-mx-24{margin-left:-1.5rem;margin-right:-1.5rem}.my-16{margin-bottom:1rem;margin-top:1rem}.mx-24{margin-left:1.5rem;margin-right:1.5rem}.-my-12{margin-bottom:-.75rem;margin-top:-.75rem}.mr-12{margin-right:.75rem}.ml-auto{margin-left:auto}.mr-8{margin-right:.5rem}.-mb-2{margin-bottom:-.125rem}.mt-2{margin-top:.125rem}.mb-24{margin-bottom:1.5rem}.mt-auto{margin-top:auto}.ml-8{margin-left:.5rem}.mr-16{margin-right:1rem}.-mt-16{margin-top:-1rem}.mt-8{margin-top:.5rem}.mb-16{margin-bottom:1rem}.mb-4{margin-bottom:.25rem}.mt-16{margin-top:1rem}.ml-4{margin-left:.25rem}.mb-8{margin-bottom:.5rem}.ml-2{margin-left:.125rem}.mt-24{margin-top:1.5rem}.ml-24{margin-left:1.5rem}.-mb-24{margin-bottom:-1.5rem}.-mt-8{margin-top:-.5rem}.mr-auto{margin-right:auto}.ml-28{margin-left:1.75rem}.ml-16{margin-left:1rem}.mr-10{margin-right:.625rem}.mb-10{margin-bottom:.625rem}.ml-10{margin-left:.625rem}.mb-30{margin-bottom:1.875rem}.-mr-8{margin-right:-.5rem}.mr-4{margin-right:.25rem}.block{display:block}.\!block{display:block!important}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.\!inline-flex{display:inline-flex!important}.table{display:table}.grid{display:grid}.contents{display:contents}.hidden{display:none}.\!hidden{display:none!important}.h-24{height:1.5rem}.h-32{height:2rem}.h-20{height:1.25rem}.h-full{height:100%}.h-16{height:1rem}.h-10{height:.625rem}.h-18{height:1.125rem}.h-56{height:3.5rem}.h-screen{height:100vh}.h-6{height:.375rem}.h-40{height:2.5rem}.h-12{height:.75rem}.h-64{height:4rem}.h-36{height:2.25rem}.max-h-432{max-height:27rem}.max-h-screen{max-height:100vh}.max-h-40{max-height:2.5rem}.max-h-none{max-height:none}.min-h-56{min-height:3.5rem}.min-h-72{min-height:4.5rem}.min-h-full{min-height:100%}.min-h-screen{min-height:100vh}.min-h-32{min-height:2rem}.min-h-40{min-height:2.5rem}.w-24{width:1.5rem}.w-auto{width:auto}.w-32{width:2rem}.w-260{width:16.25rem}.w-20{width:1.25rem}.w-full{width:100%}.w-16{width:1rem}.w-248{width:15.5rem}.w-1\/2{width:50%}.w-1\/3{width:33.333334%}.w-1\/4{width:25%}.w-1\/5{width:20%}.w-1\/6{width:16.666667%}.w-40{width:2.5rem}.w-10{width:.625rem}.w-56{width:3.5rem}.w-8{width:.5rem}.w-6{width:.375rem}.w-192{width:12rem}.w-12{width:.75rem}.w-64{width:4rem}.\!w-full{width:100%!important}.w-36{width:2.25rem}.w-18{width:1.125rem}.min-w-0{min-width:0}.max-w-1180{max-width:73.75rem}.max-w-370{max-width:23.125rem}.flex-1{flex:1 1 0%}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-y-1\/2{--tw-translate-y:-50%}.-translate-x-1\/2,.-translate-y-1\/2{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.-translate-x-1\/2{--tw-translate-x:-50%}.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.cursor-pointer{cursor:pointer}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-end{align-items:flex-end}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-8{gap:.5rem}.gap-10{gap:.625rem}.gap-24{gap:1.5rem}.gap-4{gap:.25rem}.gap-16{gap:1rem}.gap-x-8{-moz-column-gap:.5rem;column-gap:.5rem}.gap-x-4{-moz-column-gap:.25rem;column-gap:.25rem}.gap-y-12{row-gap:.75rem}.gap-y-8{row-gap:.5rem}.gap-x-16{-moz-column-gap:1rem;column-gap:1rem}.self-end{align-self:flex-end}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-x-auto{overflow-x:auto}.whitespace-normal{white-space:normal}.whitespace-nowrap{white-space:nowrap}.break-words{overflow-wrap:break-word}.rounded-full{border-radius:9999px}.rounded-xs{border-radius:2px}.rounded{border-radius:6px}.rounded-none{border-radius:0}.rounded-r{border-bottom-right-radius:6px;border-top-right-radius:6px}.border{border-width:1px}.border-0{border-width:0}.border-2{border-width:2px}.border-x-0{border-left-width:0;border-right-width:0}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-solid{border-style:solid}.border-dark-200{border-color:var(--color-dark-200)}.border-dark-100{border-color:var(--color-dark-100)}.border-negative-100{border-color:var(--color-negative-100)}.border-transparent{border-color:var(--color-transparent)}.border-notice-100{border-color:var(--color-notice-100)}.border-current{border-color:currentColor}.border-dark-300{border-color:var(--color-dark-300)}.border-success-100{border-color:var(--color-success-100)}.border-warning-100{border-color:var(--color-warning-100)}.bg-light{background-color:var(--color-light)}.bg-dark-300{background-color:var(--color-dark-300)}.bg-dark-50{background-color:var(--color-dark-50)}.bg-success-100{background-color:var(--color-success-100)}.bg-warning-100{background-color:var(--color-warning-100)}.bg-notice-100{background-color:var(--color-notice-100)}.bg-negative-100{background-color:var(--color-negative-100)}.bg-negative-50{background-color:var(--color-negative-50)}.bg-dark-100{background-color:var(--color-dark-100)}.bg-success{background-color:var(--color-success)}.bg-notice-50{background-color:var(--color-notice-50)}.bg-transparent{background-color:var(--color-transparent)}.bg-success-50{background-color:var(--color-success-50)}.bg-warning-50{background-color:var(--color-warning-50)}.bg-primary-50{background-color:var(--color-primary-50)}.object-cover{-o-object-fit:cover;object-fit:cover}.p-12{padding:.75rem}.p-8{padding:.5rem}.p-16{padding:1rem}.p-0{padding:0}.p-24{padding:1.5rem}.p-32{padding:2rem}.px-24{padding-left:1.5rem;padding-right:1.5rem}.py-32{padding-bottom:2rem;padding-top:2rem}.px-16{padding-left:1rem;padding-right:1rem}.py-8{padding-bottom:.5rem;padding-top:.5rem}.py-2{padding-bottom:.125rem;padding-top:.125rem}.py-16{padding-bottom:1rem;padding-top:1rem}.px-32{padding-left:2rem;padding-right:2rem}.px-0{padding-left:0;padding-right:0}.py-24{padding-bottom:1.5rem;padding-top:1.5rem}.py-12{padding-bottom:.75rem;padding-top:.75rem}.px-38{padding-left:2.375rem;padding-right:2.375rem}.px-12{padding-left:.75rem;padding-right:.75rem}.py-20{padding-bottom:1.25rem;padding-top:1.25rem}.px-20{padding-left:1.25rem;padding-right:1.25rem}.px-10{padding-left:.625rem;padding-right:.625rem}.pl-36{padding-left:2.25rem}.pr-8{padding-right:.5rem}.pt-20{padding-top:1.25rem}.\!pl-20{padding-left:1.25rem!important}.pb-24{padding-bottom:1.5rem}.pl-38{padding-left:2.375rem}.pt-8{padding-top:.5rem}.pr-10{padding-right:.625rem}.pr-66{padding-right:4.125rem}.pl-42{padding-left:2.625rem}.pl-26{padding-left:1.625rem}.pl-10{padding-left:.625rem}.pr-38{padding-right:2.375rem}.pt-10{padding-top:.625rem}.pb-0{padding-bottom:0}.pb-8{padding-bottom:.5rem}.text-left{text-align:left}.text-center{text-align:center}.font-heading{font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica,Arial,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol}.text-14{font-size:.875rem}.text-12,.text-14{line-height:1.25rem}.text-12{font-size:.75rem}.text-16{font-size:1rem;line-height:1.25rem}.text-24{font-size:1.5rem;line-height:2rem}.text-18{font-size:1.125rem;line-height:1.25rem}.text-30{font-size:1.875rem;line-height:2.75rem}.font-bold{font-weight:700}.font-semibold{font-weight:600}.font-medium{font-weight:500}.font-normal{font-weight:400}.leading-none{line-height:1}.leading-20{line-height:1.25rem}.leading-16{line-height:1rem}.leading-18{line-height:1.125rem}.leading-28{line-height:1.75rem}.text-dark-600{color:var(--color-dark-600)}.text-dark{color:var(--color-dark)}.text-dark-900{color:var(--color-dark-900)}.text-secondary{color:var(--color-secondary)}.text-success-800{color:var(--color-success-800)}.text-warning-800{color:var(--color-warning-800)}.text-notice-800{color:var(--color-notice-800)}.text-negative-800{color:var(--color-negative-800)}.text-negative-900{color:var(--color-negative-900)}.text-negative{color:var(--color-negative)}.text-primary{color:var(--color-primary)}.text-notice-900{color:var(--color-notice-900)}.text-notice{color:var(--color-notice)}.text-dark-400{color:var(--color-dark-400)}.text-dark-300{color:var(--color-dark-300)}.text-light{color:var(--color-light)}.text-success-900{color:var(--color-success-900)}.text-success{color:var(--color-success)}.text-warning-900{color:var(--color-warning-900)}.text-warning{color:var(--color-warning)}.opacity-75{opacity:.75}.shadow-none{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000}.shadow,.shadow-none{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.shadow{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color)}.outline{outline-style:solid}.blur{--tw-blur:blur(8px)}.blur,.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition-transform{transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}.line-clamp-1{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.fade{transition-duration:.15s;transition-property:opacity,visibility;transition-timing-function:cubic-bezier(.4,0,.2,1)}.fade:not(.show){opacity:0;visibility:hidden}.collapse:not(.show){display:none}.flatpickr-day.collapse:not(.show){visibility:hidden}.flex-center{align-items:center;display:flex;justify-content:center}.\!visible,.visible{display:block!important}.active{opacity:1;visibility:visible}.tabulator{font-size:.875rem;line-height:1.25rem;overflow:hidden;position:relative;text-align:left;transform:translateZ(0)}.tabulator[tabulator-layout=fitDataFill] .tabulator-tableholder .tabulator-table{min-width:100%}.tabulator[tabulator-layout=fitDataTable]{display:inline-block}.tabulator .tabulator-header,.tabulator.tabulator-block-select{-webkit-user-select:none;-moz-user-select:none;user-select:none}.tabulator .tabulator-header{background-color:var(--color-dark-50);border-bottom-width:1px;border-color:var(--color-dark-200);box-sizing:border-box;color:var(--color-dark-600);overflow:hidden;position:relative;white-space:nowrap;width:100%}.tabulator .tabulator-header.tabulator-header-hidden{display:none}.tabulator .tabulator-header .tabulator-header-contents{overflow:hidden;position:relative}.tabulator .tabulator-header .tabulator-header-contents .tabulator-headers{display:inline-block}.tabulator .tabulator-header .tabulator-col{background-color:var(--color-dark-50);box-sizing:border-box;color:var(--color-dark-600);display:inline-flex;flex-direction:column;justify-content:flex-start;overflow:hidden;position:relative;text-align:left;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);vertical-align:bottom}.tabulator .tabulator-header .tabulator-col .tabulator-col-content{align-items:center;box-sizing:border-box;display:flex;min-height:3rem;padding:.5rem;position:relative}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title-holder{align-items:center;display:flex}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title-holder.tabulator-col-sorter-element{position:relative}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title{box-sizing:border-box;overflow:hidden;text-overflow:ellipsis;vertical-align:bottom;white-space:nowrap;width:100%}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title:first-letter{text-transform:capitalize}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title.tabulator-col-title-wrap{text-overflow:clip;white-space:normal}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter{align-items:center;display:flex}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow{border:none!important;opacity:0;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:before{border-bottom:4px solid var(--color-dark-400);border-left:4px solid transparent;border-right:4px solid transparent;content:"";display:block}.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:after{border-left:4px solid transparent;border-right:4px solid transparent;border-top:4px solid var(--color-dark-400);content:"";display:block;margin-top:.125rem}.tabulator .tabulator-header .tabulator-col.tabulator-sortable{cursor:pointer}.tabulator .tabulator-header .tabulator-col.tabulator-sortable:hover .tabulator-col-content .tabulator-col-title,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-title,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-title{color:var(--color-dark-900)}.tabulator .tabulator-header .tabulator-col.tabulator-sortable:hover .tabulator-col-content .tabulator-col-sorter .tabulator-arrow,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow,.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow{opacity:1}.tabulator .tabulator-header .tabulator-col.tabulator-sortable .tabulator-col-title{padding-right:.625rem}.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=ascending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:before{border-bottom:4px solid var(--color-dark-800)}.tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort=descending] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow:after{border-top:4px solid var(--color-dark-800)}.tabulator .tabulator-header .tabulator-col.tabulator-col-vertical .tabulator-col-content .tabulator-col-title{align-items:center;display:flex;justify-content:center;text-orientation:mixed;writing-mode:vertical-rl}.tabulator .tabulator-frozen:before{bottom:0;box-shadow:0 0 8px 0 rgba(17,24,39,.16);content:"";left:0;position:absolute;right:0;top:0;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator .tabulator-header .tabulator-frozen{background-color:transparent;left:0;position:sticky;z-index:10}.tabulator .tabulator-header .tabulator-frozen:before{background-color:var(--color-dark-100)}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-left{padding-right:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-left:before{margin-right:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-right{padding-left:.5rem}.tabulator .tabulator-header .tabulator-frozen.tabulator-frozen-right:before{margin-left:.5rem}.tabulator .tabulator-header .tabulator-frozen-rows-holder:empty{display:none}.tabulator .tabulator-tableholder{-webkit-overflow-scrolling:touch;overflow:auto;position:relative;white-space:nowrap;width:100%}.tabulator .tabulator-tableholder:focus{outline:none}.tabulator .tabulator-tableholder .tabulator-placeholder{align-items:center;box-sizing:border-box;display:flex;justify-content:center;width:100%}.tabulator .tabulator-tableholder .tabulator-placeholder[tabulator-render-mode=virtual]{min-height:100%;min-width:100%}.tabulator .tabulator-tableholder .tabulator-placeholder .tabulator-placeholder-contents{display:inline-block;font-size:1rem;font-weight:600;line-height:1.25rem;padding:1.5rem;text-align:center;white-space:normal}.tabulator .tabulator-tableholder .tabulator-table{background-color:var(--color-light);color:var(--color-dark-900);display:inline-block;min-width:100%;overflow:visible;position:relative;white-space:nowrap}.tabulator .tabulator-footer{background-color:var(--color-light);border-color:var(--color-dark-200);border-top-width:1px;display:none;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.tabulator .tabulator-footer .tabulator-footer-contents{align-items:center;display:flex;padding:1rem}.tabulator .tabulator-footer .tabulator-footer-contents:empty{display:none}.tabulator-page-counter{margin-left:auto}.tabulator-paginator{display:flex;margin-left:.5rem}@media (min-width:576px){.tabulator-paginator{margin-left:1rem}}.tabulator-pages{display:flex}.tabulator-pages+.tabulator-page{margin-left:-1px}.tabulator-page{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;border-color:var(--color-dark-200);border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:flex;font-weight:500;height:2.5rem;justify-content:center;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.5rem}.tabulator-page.active,.tabulator-page:not(:disabled):not(.disabled):hover{background-color:var(--color-primary-100);border-color:var(--color-primary);cursor:pointer;z-index:1}.tabulator-page.active{color:var(--color-primary)}.tabulator-page+.tabulator-page,.tabulator-page+.tabulator-pages{margin-left:-1px}.tabulator-page[data-page=first],.tabulator-page[data-page=last]{display:none}.tabulator-page[data-page=next],.tabulator-page[data-page=prev]{position:relative;text-indent:-9999px;white-space:nowrap}.tabulator-page[data-page=next]:after,.tabulator-page[data-page=prev]:after{background-position:50%;background-repeat:no-repeat;background-size:24px;bottom:0;content:"";height:100%;left:0;position:absolute;right:0;top:0;width:100%}.tabulator-page:first-child{border-bottom-left-radius:6px;border-top-left-radius:6px}.tabulator-page:last-child{border-bottom-right-radius:6px;border-top-right-radius:6px}.tabulator-page:disabled{color:var(--color-dark-400)}.tabulator-page:disabled:after{opacity:.4}.tabulator-page:disabled:first-child,.tabulator-page:disabled:last-child{border-color:var(--color-dark-100)}@media (max-width:767px){.tabulator-page:not(:first-child):not(:last-child){display:none}}.tabulator .tabulator-col-resize-handle{display:inline-block;margin-left:-3px;margin-right:-3px;position:relative;vertical-align:middle;width:6px;z-index:10}.tabulator .tabulator-col-resize-handle:hover{cursor:ew-resize}.tabulator .tabulator-col-resize-handle:last-of-type{margin-right:0;width:3px}.tabulator .tabulator-alert{align-items:center;background:rgba(0,0,0,.4);display:flex;height:100%;left:0;position:absolute;text-align:center;top:0;width:100%;z-index:100}.tabulator .tabulator-alert .tabulator-alert-msg{background:#fff;border-radius:10px;display:inline-block;font-size:16px;font-weight:700;margin:0 auto;padding:10px 20px}.tabulator .tabulator-alert .tabulator-alert-msg.tabulator-alert-state-msg{border:4px solid #333;color:#000}.tabulator .tabulator-alert .tabulator-alert-msg.tabulator-alert-state-error{border:4px solid #d00;color:#590000}.tabulator-row{background-color:var(--color-light);border-bottom-width:1px;border-color:var(--color-dark-200);box-sizing:border-box;cursor:pointer;min-height:2.5rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.tabulator-row.tabulator-selectable:hover{cursor:pointer}.tabulator-row.tabulator-selectable:hover,.tabulator-row.tabulator-selectable:hover>.tabulator-frozen:before{background-color:var(--color-primary-50)}.tabulator-header .row-select-wrapper,.tabulator-row.tabulator-selectable .row-select-wrapper{align-items:center;bottom:0;display:flex;justify-content:center;left:0;padding:.5rem 1rem;position:absolute;right:0;top:0;width:100%}.tabulator-header .row-select-wrapper>label,.tabulator-row.tabulator-selectable .row-select-wrapper>label{height:1.25rem;padding-left:1.25rem}.tabulator-row.tabulator-selectable .row-select-wrapper{height:100%}.tabulator-header .row-select-wrapper{height:3rem}.tabulator-row.tabulator-selected,.tabulator-row.tabulator-selected:hover{background-color:var(--color-primary-50)}.tabulator-row.tabulator-selected:hover{cursor:pointer}.tabulator-row.tabulator-row-moving{background:#fff;border:1px solid #000}.tabulator-row.tabulator-moving{border-bottom:1px solid #aaa;border-top:1px solid #aaa;pointer-events:none;position:absolute;z-index:15}.tabulator-row .tabulator-row-resize-handle{bottom:0;height:5px;left:0;position:absolute;right:0}.tabulator-row .tabulator-row-resize-handle.prev{bottom:auto;top:0}.tabulator-row .tabulator-row-resize-handle:hover{cursor:ns-resize}.tabulator-row .tabulator-responsive-collapse{border-bottom-width:1px;border-color:var(--color-dark-200);border-top-width:1px;box-sizing:border-box;padding:.5rem}.tabulator-row .tabulator-responsive-collapse:empty{display:none}.tabulator-row .tabulator-responsive-collapse table tr td{position:relative}.tabulator-row .tabulator-responsive-collapse table tr td:first-of-type{padding-right:1rem}.tabulator-row .tabulator-cell{align-items:center;box-sizing:border-box;display:inline-flex;min-height:2.5rem;overflow:hidden;padding:.5rem;position:relative;text-overflow:ellipsis;vertical-align:middle;white-space:nowrap}.tabulator-row .tabulator-cell .btn+.btn{margin-left:.25rem}.tabulator-row .tabulator-cell.tabulator-frozen{display:inline-block;left:0;position:sticky;z-index:10}.tabulator-row .tabulator-cell.tabulator-frozen:before{background-color:var(--color-light)}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-left{padding-right:1rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-left:before{margin-right:.5rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-right{padding-left:1rem}.tabulator-row .tabulator-cell.tabulator-frozen.tabulator-frozen-right:before{margin-left:.5rem}.tabulator-row .tabulator-cell.tabulator-editable{border-color:var(--color-dark-200);border-left-width:1px;border-right-width:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-editable:hover{background-color:var(--color-dark-50)}.tabulator-row .tabulator-cell.tabulator-editing{border-color:var(--color-primary);border-width:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-editing input,.tabulator-row .tabulator-cell.tabulator-editing select{background:transparent;border:1px;outline:none}.tabulator-row .tabulator-cell.tabulator-validation-fail{border:1px solid #d00}.tabulator-row .tabulator-cell.tabulator-validation-fail input,.tabulator-row .tabulator-cell.tabulator-validation-fail select{background:transparent;border:1px;color:#d00}.tabulator-row .tabulator-cell.tabulator-row-handle{align-items:center;display:inline-flex;justify-content:center;-moz-user-select:none;-khtml-user-select:none;-webkit-user-select:none;-o-user-select:none}.tabulator-row .tabulator-cell.tabulator-row-handle .tabulator-row-handle-box{width:80%}.tabulator-row .tabulator-cell.tabulator-row-handle .tabulator-row-handle-box .tabulator-row-handle-bar{background:#666;height:3px;margin-top:2px;width:100%}.tabulator-row .tabulator-cell .tabulator-data-tree-branch{border-bottom:2px solid #aaa;border-bottom-left-radius:1px;border-left:2px solid #aaa;display:inline-block;height:9px;margin-right:5px;margin-top:-9px;vertical-align:middle;width:7px}.tabulator-row .tabulator-cell .tabulator-data-tree-control{align-items:center;background:rgba(0,0,0,.1);border:1px solid #333;border-radius:2px;display:inline-flex;height:11px;justify-content:center;margin-right:5px;overflow:hidden;vertical-align:middle;width:11px}.tabulator-row .tabulator-cell .tabulator-data-tree-control:hover{background:rgba(0,0,0,.2);cursor:pointer}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-collapse{background:transparent;display:inline-block;height:7px;position:relative;width:1px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-collapse:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-expand{background:#333;display:inline-block;height:7px;position:relative;width:1px}.tabulator-row .tabulator-cell .tabulator-data-tree-control .tabulator-data-tree-control-expand:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-row.tabulator-group{background:#ccc;border-bottom:1px solid #999;border-right:1px solid #aaa;border-top:1px solid #999;box-sizing:border-box;font-weight:700;min-width:100%;padding:5px 5px 5px 10px}.tabulator-row.tabulator-group:hover{background-color:rgba(0,0,0,.1);cursor:pointer}.tabulator-row.tabulator-group.tabulator-group-visible .tabulator-arrow{border-bottom:0;border-left:6px solid transparent;border-right:6px solid transparent;border-top:6px solid #666;margin-right:10px}.tabulator-row.tabulator-group.tabulator-group-level-1{padding-left:30px}.tabulator-row.tabulator-group.tabulator-group-level-2{padding-left:50px}.tabulator-row.tabulator-group.tabulator-group-level-3{padding-left:70px}.tabulator-row.tabulator-group.tabulator-group-level-4{padding-left:90px}.tabulator-row.tabulator-group.tabulator-group-level-5{padding-left:110px}.tabulator-row.tabulator-group .tabulator-group-toggle{display:inline-block}.tabulator-row.tabulator-group .tabulator-arrow{border-bottom:6px solid transparent;border-left:6px solid #666;border-right:0;border-top:6px solid transparent;display:inline-block;height:0;margin-right:16px;vertical-align:middle;width:0}.tabulator-row.tabulator-group span{color:#d00;margin-left:10px}.tabulator-print-table .tabulator-data-tree-branch{border-bottom:2px solid #aaa;border-bottom-left-radius:1px;border-left:2px solid #aaa;display:inline-block;height:9px;margin-right:5px;margin-top:-9px;vertical-align:middle;width:7px}.tabulator-print-table .tabulator-data-tree-control{align-items:center;background:rgba(0,0,0,.1);border:1px solid #333;border-radius:2px;display:inline-flex;height:11px;justify-content:center;margin-right:5px;overflow:hidden;vertical-align:middle;width:11px}.tabulator-print-table .tabulator-data-tree-control:hover{background:rgba(0,0,0,.2);cursor:pointer}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-collapse{background:transparent;display:inline-block;height:7px;position:relative;width:1px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-collapse:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-expand{background:#333;display:inline-block;height:7px;position:relative;width:1px}.tabulator-print-table .tabulator-data-tree-control .tabulator-data-tree-control-expand:after{background:#333;content:"";height:1px;left:-3px;position:absolute;top:3px;width:7px}.tabulator-custom-header{border-bottom-width:1px;border-color:var(--color-dark-200);font-size:.875rem;line-height:1.25rem;position:relative}.tabulator-custom-footer{border-color:var(--color-dark-200);border-top-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;padding:1rem}.tabulator-responsive-collapse table{display:flex;gap:.5rem}.tabulator-responsive-collapse td:first-child{display:none}.tabulator-responsive-collapse tr{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);align-items:center;background-color:var(--color-light);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);display:inline-flex;flex-shrink:0;font-size:.875rem;font-weight:500;height:2.5rem;justify-content:center;line-height:1.125rem;overflow:hidden;padding-left:1rem;padding-right:1rem;transition-duration:.1s;transition-property:color,background-color,border,outline,box-shadow;transition-timing-function:ease-in;-webkit-user-select:none;-moz-user-select:none;user-select:none}.tabulator-responsive-collapse tr>span{-webkit-line-clamp:2;margin-right:auto}.tabulator-responsive-collapse tr>svg{flex-shrink:0;height:1.25rem;width:1.25rem}.tabulator-responsive-collapse tr:not(:disabled):hover{background-color:var(--color-dark-100);border-color:var(--color-dark-300);color:var(--color-dark-900)}.tabulator-responsive-collapse tr:not(:disabled):hover:active{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900)}.tabulator-responsive-collapse tr:focus{--tw-shadow:0px 0px 0px 2px #fff,0px 0px 0px 4px #009fa7;--tw-shadow-colored:0px 0px 0px 2px var(--tw-shadow-color),0px 0px 0px 4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.tabulator-responsive-collapse tr:focus-visible{outline:none}.tabulator-responsive-collapse tr:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-light);border-color:var(--color-dark-100);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark);cursor:not-allowed}.tabulator-responsive-collapse tr{height:2rem;padding-left:.75rem;padding-right:.75rem}.tabulator-responsive-collapse tr>span{-webkit-box-orient:vertical;-webkit-line-clamp:1;display:-webkit-box;overflow:hidden}.tabulator-responsive-collapse tr>svg{height:1rem;width:1rem}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown]:focus{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown] svg:last-child{transition:transform .2s}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown].show{background-color:var(--color-primary-50);border-color:var(--color-primary);color:var(--color-primary)}.tabulator-responsive-collapse tr[data-bs-toggle=dropdown].show svg:last-child{--tw-rotate:180deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.filter-wrapper>.tabulator-responsive-collapse tr.empty>svg:not(:last-child){display:none}.flatpickr-day.filter-wrapper>.tabulator-responsive-collapse tr.empty>svg:not(:last-child){visibility:hidden}.tabulator-responsive-collapse tr{border-radius:9999px;position:relative}.tabulator-row .tabulator-cell .tabulator-responsive-collapse tr+.btn{margin-left:.25rem}.djn-table>.djn-tbody td .tabulator-responsive-collapse tr:not(.input-file-edit-btn){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rules-group-container .rules-group-header .tabulator-responsive-collapse tr{height:2rem}.query-builder .rules-group-container .group-conditions label.tabulator-responsive-collapse tr{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.tabulator-responsive-collapse tr.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container .rule-header .tabulator-responsive-collapse tr-group .btn{margin-right:0}.query-builder .tabulator-responsive-collapse tr[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .tabulator-responsive-collapse tr[data-delete] i{display:none}.flatpickr-day.query-builder .tabulator-responsive-collapse tr[data-delete] i{visibility:hidden}.query-builder .tabulator-responsive-collapse tr[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .tabulator-responsive-collapse tr[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.tabulator-responsive-collapse tr{color:var(--color-dark)}.tabulator-responsive-collapse tr:hover{color:var(--color-dark-900)}.tabulator-responsive-collapse tr .catalog-image{height:1.5rem;width:1.5rem}.flatpickr-calendar{--tw-shadow:0 4px 16px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 4px 16px 0 var(--tw-shadow-color);animation:none;background:transparent;background-color:var(--color-light);border:0;border-radius:6px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);box-sizing:border-box;direction:ltr;display:none;opacity:0;padding:0;position:absolute;text-align:center;touch-action:manipulation;visibility:hidden;width:272px}.flatpickr-calendar.inline,.flatpickr-calendar.open{max-height:640px;opacity:1;visibility:visible}.flatpickr-calendar.open{display:inline-block;z-index:99999}.flatpickr-calendar.inline{display:block;position:relative;top:2px}.flatpickr-calendar.static{position:absolute;top:calc(100% + 2px)}.flatpickr-calendar.static.open{display:block;z-index:999}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+1) .flatpickr-day.inRange:nth-child(7n+7){box-shadow:none!important}.flatpickr-calendar.multiMonth .flatpickr-days .dayContainer:nth-child(n+2) .flatpickr-day.inRange:nth-child(7n+1){box-shadow:-2px 0 0 #e6e6e6,5px 0 0 #e6e6e6}.flatpickr-calendar .hasTime .dayContainer,.flatpickr-calendar .hasWeeks .dayContainer{border-bottom:0;border-bottom-left-radius:0;border-bottom-right-radius:0}.flatpickr-calendar .hasWeeks .dayContainer{border-left:0}.flatpickr-calendar.hasTime:not(.noCalendar) .flatpickr-time{padding-top:0}.flatpickr-calendar.noCalendar.hasTime{width:200px}.flatpickr-calendar.noCalendar.hasTime .flatpickr-time{border:0;height:auto}.flatpickr-calendar:focus{outline:0}.flatpickr-wrapper{display:inline-block;position:relative}.flatpickr-months{color:var(--color-dark-900);display:flex;margin-top:.25rem;padding:.5rem .75rem}.flatpickr-months .flatpickr-month{display:flex;justify-content:center;position:relative;width:100%}.flatpickr-months .flatpickr-next-month,.flatpickr-months .flatpickr-prev-month{cursor:pointer;font-size:0}.flatpickr-months .flatpickr-next-month>svg,.flatpickr-months .flatpickr-prev-month>svg{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.flatpickr-months .flatpickr-next-month.flatpickr-disabled,.flatpickr-months .flatpickr-prev-month.flatpickr-disabled{display:none}.flatpickr-months .flatpickr-next-month i,.flatpickr-months .flatpickr-prev-month i{position:relative}.flatpickr-months .flatpickr-next-month:hover,.flatpickr-months .flatpickr-prev-month:hover{color:var(--color-primary)}.numInputWrapper{border-color:var(--color-dark-200);border-radius:6px;border-width:1px;height:auto;padding-left:.25rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.numInputWrapper input,.numInputWrapper span{display:inline-block}.numInputWrapper input{width:100%}.numInputWrapper input::-ms-clear{display:none}.numInputWrapper input::-webkit-inner-spin-button,.numInputWrapper input::-webkit-outer-spin-button{-webkit-appearance:none;margin:0}.numInputWrapper span{background-color:var(--color-light);border-color:var(--color-dark-400);border-width:1px;box-sizing:border-box;cursor:pointer;height:calc(50% + 1px);opacity:0;padding:0 4px 0 3px;position:absolute;right:0;transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1);width:17px}.numInputWrapper span:hover{background-color:var(--color-dark-100)}.numInputWrapper span:active{background-color:var(--color-dark-200)}.numInputWrapper span:after{content:"";display:block;position:absolute}.numInputWrapper span.arrowUp{border-bottom:0;border-top-right-radius:6px;top:0}.numInputWrapper span.arrowUp:after{border-bottom:4px solid var(--color-dark-900);border-left:4px solid transparent;border-right:4px solid transparent;bottom:40%}.numInputWrapper span.arrowDown{border-bottom-right-radius:6px;bottom:0}.numInputWrapper span.arrowDown:after{border-left:4px solid transparent;border-right:4px solid transparent;border-top:4px solid var(--color-dark-900);top:calc(40% - 1px)}.numInputWrapper span svg{height:auto;width:inherit}.numInputWrapper:hover{border-color:var(--color-dark-400)}.numInputWrapper:hover span{opacity:1}.flatpickr-current-month{color:var(--color-dark-900);cursor:pointer;display:flex;font-size:1rem;font-weight:600;gap:.25rem;justify-content:center;line-height:1.5rem;transform:translateZ(0);transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.flatpickr-current-month:hover{color:var(--color-primary)}.flatpickr-current-month span.cur-month{color:inherit;display:inline-block;font-family:inherit;font-weight:700;margin-left:.5ch;padding:0}.flatpickr-current-month span.cur-month:hover{background-color:var(--color-primary-100)}.flatpickr-current-month .numInputWrapper{display:inline-block;width:6ch;width:7ch \0}.flatpickr-current-month .numInputWrapper span.arrowUp:after{border-bottom-color:rgba(0,0,0,.9)}.flatpickr-current-month .numInputWrapper span.arrowDown:after{border-top-color:rgba(0,0,0,.9)}.flatpickr-current-month input.cur-year{-webkit-appearance:textfield;-moz-appearance:textfield;appearance:textfield;background:transparent;border:0;border-radius:0;color:inherit;cursor:text;display:inline-block;font-family:inherit;font-size:inherit;height:auto;line-height:inherit;margin:0;vertical-align:initial}.flatpickr-current-month input.cur-year:focus{outline:0}.flatpickr-current-month input.cur-year[disabled],.flatpickr-current-month input.cur-year[disabled]:hover{background:transparent;color:rgba(0,0,0,.5);font-size:100%;pointer-events:none}.flatpickr-current-month .flatpickr-monthDropdown-months{-webkit-appearance:menulist-button;-moz-appearance:menulist-button;appearance:menulist-button;background-color:transparent;border-color:var(--color-dark-200);border-radius:0;border-radius:6px;border-width:1px;box-sizing:border-box;color:inherit;color:var(--color-dark-900);cursor:pointer;font-family:inherit;font-size:inherit;font-size:1rem;font-weight:600;height:auto;line-height:inherit;line-height:1.5rem;outline:none;padding-left:.25rem;padding-right:.25rem;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);vertical-align:initial;width:auto}.flatpickr-current-month .flatpickr-monthDropdown-months:active,.flatpickr-current-month .flatpickr-monthDropdown-months:focus{outline:none}.flatpickr-current-month .flatpickr-monthDropdown-months:hover{border-color:var(--color-dark-400)}.flatpickr-current-month .flatpickr-monthDropdown-months .flatpickr-monthDropdown-month{background-color:var(--color-light);outline:none;padding:0}.flatpickr-weekdays{align-items:center;background:transparent;display:flex;overflow:hidden;text-align:center;width:100%}.flatpickr-weekdays .flatpickr-weekdaycontainer{display:flex;flex:1;padding-bottom:.5rem;padding-top:.5rem}span.flatpickr-weekday{background:transparent;cursor:default;display:block;flex:1;margin:0;text-align:center}.dayContainer,.flatpickr-weeks{padding:1px 0 0}.flatpickr-days{align-items:flex-start;display:flex;overflow:hidden;position:relative}.dayContainer,.flatpickr-days:focus{outline:0}.dayContainer{display:flex;flex-wrap:wrap;gap:.25rem;height:100%;opacity:1;text-align:left;transform:translateZ(0);width:100%}.dayContainer+.dayContainer{box-shadow:-1px 0 0 #e6e6e6}.flatpickr-day{align-items:center;background:none;border:1px solid transparent;border-radius:6px;color:var(--color-dark-900);cursor:pointer;display:flex;font-weight:400;height:2rem;justify-content:center;margin:0;position:relative;width:2rem}.flatpickr-day.inRange,.flatpickr-day.nextMonthDay.inRange,.flatpickr-day.nextMonthDay.today.inRange,.flatpickr-day.nextMonthDay:focus,.flatpickr-day.nextMonthDay:hover,.flatpickr-day.prevMonthDay.inRange,.flatpickr-day.prevMonthDay.today.inRange,.flatpickr-day.prevMonthDay:focus,.flatpickr-day.prevMonthDay:hover,.flatpickr-day.today.inRange,.flatpickr-day:focus,.flatpickr-day:hover{background:var(--color-primary-100);border-color:var(--color-primary-100);cursor:pointer;outline:0}.flatpickr-day.today{color:var(--color-primary);font-weight:600}.flatpickr-day.today:focus,.flatpickr-day.today:hover{background:var(--color-primary);border-color:var(--color-primary);color:var(--color-light)}.flatpickr-day.endRange,.flatpickr-day.endRange.inRange,.flatpickr-day.endRange.nextMonthDay,.flatpickr-day.endRange.prevMonthDay,.flatpickr-day.endRange:focus,.flatpickr-day.endRange:hover,.flatpickr-day.selected,.flatpickr-day.selected.inRange,.flatpickr-day.selected.nextMonthDay,.flatpickr-day.selected.prevMonthDay,.flatpickr-day.selected:focus,.flatpickr-day.selected:hover,.flatpickr-day.startRange,.flatpickr-day.startRange.inRange,.flatpickr-day.startRange.nextMonthDay,.flatpickr-day.startRange.prevMonthDay,.flatpickr-day.startRange:focus,.flatpickr-day.startRange:hover{background:var(--color-primary);border-color:var(--color-primary);box-shadow:none;color:var(--color-light)}.flatpickr-day.endRange.startRange,.flatpickr-day.selected.startRange,.flatpickr-day.startRange.startRange{border-radius:50px 0 0 50px}.flatpickr-day.endRange.endRange,.flatpickr-day.selected.endRange,.flatpickr-day.startRange.endRange{border-radius:0 50px 50px 0}.flatpickr-day.endRange.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.selected.startRange+.endRange:not(:nth-child(7n+1)),.flatpickr-day.startRange.startRange+.endRange:not(:nth-child(7n+1)){box-shadow:-10px 0 0 var(--color-primary)}.flatpickr-day.endRange.startRange.endRange,.flatpickr-day.selected.startRange.endRange,.flatpickr-day.startRange.startRange.endRange{border-radius:50px}.flatpickr-day.inRange{border-radius:0;box-shadow:-5px 0 0 var(--color-primary-100),5px 0 0 var(--color-primary-100);color:var(--color-primary-700)}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover,.flatpickr-day.nextMonthDay,.flatpickr-day.notAllowed,.flatpickr-day.notAllowed.nextMonthDay,.flatpickr-day.notAllowed.prevMonthDay,.flatpickr-day.prevMonthDay{background:transparent;border-color:transparent;color:var(--color-dark);cursor:default}.flatpickr-day.flatpickr-disabled,.flatpickr-day.flatpickr-disabled:hover{color:rgba(57,57,57,.1);cursor:not-allowed}.flatpickr-day.week.selected{border-radius:0;box-shadow:-5px 0 0 #569ff7,5px 0 0 #569ff7}.flatpickr-day.hidden{visibility:hidden}.flatpickr-day.flatpickr-month{height:3.5rem;width:5rem}.flatpickr-day.flatpickr-year{height:3rem;margin-top:0!important;width:100%}.rangeMode .flatpickr-day{margin-top:1px}.flatpickr-weekwrapper{float:left}.flatpickr-weekwrapper .flatpickr-weeks{box-shadow:1px 0 0 #e6e6e6;padding:0 12px}.flatpickr-weekwrapper .flatpickr-weekday{float:none;line-height:28px;width:100%}.flatpickr-weekwrapper span.flatpickr-day,.flatpickr-weekwrapper span.flatpickr-day:hover{background:transparent;border:none;color:rgba(57,57,57,.3);cursor:default;display:block;max-width:none;width:100%}.flatpickr-innerContainer{display:flex;font-size:.75rem;height:17rem;line-height:1rem;overflow:hidden;padding:.5rem .75rem}.flatpickr-rContainer{display:inline-block;padding:0}.flatpickr-time{align-items:center;display:flex;padding:.75rem}.flatpickr-time .numInputWrapper{border:none;display:flex;padding:0}.flatpickr-time .numInputWrapper span.arrowUp:after{border-bottom-color:#393939}.flatpickr-time .numInputWrapper span.arrowDown:after{border-top-color:#393939}.flatpickr-time.hasSeconds .numInputWrapper{width:26%}.flatpickr-time.time24hr .numInputWrapper{width:50%}.flatpickr-time input{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.flatpickr-time input~.error{color:var(--color-negative)}.flatpickr-time input:hover{border-color:var(--color-dark-400)}.flatpickr-time input:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.flatpickr-time input:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.flatpickr-time input::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.flatpickr-time input::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.flatpickr-time input.field-valid{border-color:var(--color-success)}.flatpickr-time input.field-valid~.success{display:block}.flatpickr-time input.field-error{border-color:var(--color-negative)}.flatpickr-time input.field-error~.error{display:block}input.flatpickr-time input:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.flatpickr-time input:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.flatpickr-time input:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.flatpickr-time input:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.flatpickr-time input{height:auto}select.flatpickr-time input{padding-right:2rem}.djn-table>.djn-tbody td .flatpickr-time input:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.flatpickr-time .flatpickr-am-pm,.flatpickr-time .flatpickr-time-separator{align-items:center;display:flex;float:left;font-weight:700;height:inherit;justify-content:center;line-height:inherit;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:1rem}.flatpickr-time .flatpickr-am-pm{cursor:pointer;font-weight:400;outline:0;text-align:center;width:18%}.flatpickr-input[readonly]{cursor:pointer}@keyframes fpFadeInDown{0%{opacity:0;transform:translate3d(0,-20px,0)}to{opacity:1;transform:translateZ(0)}}.flatpickr-shortcuts{margin-bottom:1rem;padding-top:.25rem}.flatpickr-shortcuts>label{padding:0}.flatpickr-footer{padding-bottom:.25rem;text-align:left}.flatpickr-custom-events-overlay{bottom:0;cursor:pointer;left:0;position:absolute;right:0;top:0}.flatpickr-custom-views-wrapper{position:relative;z-index:10}.flatpickr-custom-months-view,.flatpickr-custom-years-view{background-color:var(--color-light);left:0;position:absolute;right:0;width:100%}.flatpickr-back{color:var(--color-primary);cursor:pointer;display:inline-block;font-size:.875rem;line-height:1.25rem;padding:.5rem .75rem;position:absolute;right:0;top:100%}.js-timepicker{max-width:4rem}.noUi-target,.noUi-target *{-webkit-touch-callout:none;-webkit-tap-highlight-color:rgba(0,0,0,0);box-sizing:border-box;touch-action:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}.noUi-target{position:relative}.noUi-base,.noUi-connects{height:100%;position:relative;width:100%;z-index:1}.noUi-connects{overflow:hidden;z-index:0}.noUi-connect,.noUi-origin{height:100%;position:absolute;right:0;top:0;-ms-transform-origin:0 0;-webkit-transform-origin:0 0;transform-origin:0 0;-webkit-transform-style:preserve-3d;transform-style:flat;width:100%;will-change:transform;z-index:1}.noUi-txt-dir-rtl.noUi-horizontal .noUi-origin{left:0;right:auto}.noUi-vertical .noUi-origin{top:-100%;width:0}.noUi-horizontal .noUi-origin{height:0}.noUi-handle{-webkit-backface-visibility:hidden;backface-visibility:hidden;position:absolute}.noUi-touch-area{--tw-translate-x:-50%;--tw-translate-y:-50%;height:1.25rem;left:50%;position:absolute;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));width:1.25rem}.noUi-state-tap .noUi-connect,.noUi-state-tap .noUi-origin{transition:transform .3s}.noUi-state-drag *{cursor:inherit!important}.noUi-horizontal{height:.25rem}.noUi-horizontal .noUi-handle{height:1rem;right:-7px;top:-7px;width:1rem}.noUi-vertical{width:18px}.noUi-vertical .noUi-handle{bottom:-17px;height:34px;right:-6px;width:28px}.noUi-txt-dir-rtl.noUi-horizontal .noUi-handle{left:-17px;right:auto}.noUi-target{background-color:var(--color-dark-200);border-radius:2px}.noUi-connects{border-radius:3px}.noUi-connect{background:#3fb8af}.noUi-draggable{cursor:ew-resize}.noUi-vertical .noUi-draggable{cursor:ns-resize}.noUi-handle{--tw-shadow:0 2px 4px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 2px 4px 0 var(--tw-shadow-color);background-color:var(--color-primary);border:2px solid var(--color-light);border-radius:9999px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);cursor:pointer}.noUi-active{background-color:var(--color-primary-400)}.noUi-vertical .noUi-handle:after,.noUi-vertical .noUi-handle:before{height:1px;left:6px;top:14px;width:14px}.noUi-vertical .noUi-handle:after{top:17px}[disabled] .noUi-connect{background:#b8b8b8}[disabled] .noUi-handle,[disabled].noUi-handle,[disabled].noUi-target{cursor:not-allowed}.noUi-pips,.noUi-pips *{box-sizing:border-box}.noUi-pips{color:#999;position:absolute}.noUi-value{position:absolute;text-align:center;white-space:nowrap}.noUi-value-sub{color:#ccc;font-size:10px}.noUi-marker{background:#ccc;position:absolute}.noUi-marker-large,.noUi-marker-sub{background:#aaa}.noUi-pips-horizontal{height:80px;left:0;padding:10px 0;top:100%;width:100%}.noUi-value-horizontal{transform:translate(-50%,50%)}.noUi-rtl .noUi-value-horizontal{transform:translate(50%,50%)}.noUi-marker-horizontal.noUi-marker{height:5px;margin-left:-1px;width:2px}.noUi-marker-horizontal.noUi-marker-sub{height:10px}.noUi-marker-horizontal.noUi-marker-large{height:15px}.noUi-pips-vertical{height:100%;left:100%;padding:0 10px;top:0}.noUi-value-vertical{padding-left:25px;transform:translateY(-50%)}.noUi-rtl .noUi-value-vertical{transform:translateY(50%)}.noUi-marker-vertical.noUi-marker{height:2px;margin-top:-1px;width:5px}.noUi-marker-vertical.noUi-marker-sub{width:10px}.noUi-marker-vertical.noUi-marker-large{width:15px}.noUi-tooltip{background:#fff;border:1px solid #d9d9d9;border-radius:3px;color:#000;display:block;padding:5px;position:absolute;text-align:center;white-space:nowrap}.noUi-horizontal .noUi-tooltip{bottom:120%;left:50%;transform:translate(-50%)}.noUi-vertical .noUi-tooltip{right:120%;top:50%;transform:translateY(-50%)}.noUi-horizontal .noUi-origin>.noUi-tooltip{bottom:10px;left:auto;transform:translate(50%)}.noUi-vertical .noUi-origin>.noUi-tooltip{right:28px;top:auto;transform:translateY(-18px)}.tabular::-webkit-scrollbar{height:9px;width:9px}.tabular::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.tabular::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.tabular:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.tabular{overflow-x:auto}.djn-table{border-collapse:separate;border-spacing:0;height:100%;min-width:100%;white-space:nowrap}.djn-table>.djn-thead th{background-color:var(--color-dark-50);border-bottom-width:1px;border-color:var(--color-dark-200);border-top-width:1px;color:var(--color-dark-600);font-size:.875rem;font-weight:400;height:3rem;line-height:1.25rem;padding:.5rem;text-align:left;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.djn-table>.djn-thead th.original{min-width:2.5rem;width:2.5rem}.djn-table>.djn-thead th.original:not(.is-sortable){display:none}.flatpickr-day.djn-table>.djn-thead th.original:not(.is-sortable){visibility:hidden}.djn-table>.djn-thead th.original:not(.is-sortable)+td{border-left:0}.djn-table>.djn-thead td{font-size:.875rem;font-weight:400;line-height:1.25rem}.djn-table>.djn-tbody td{border-bottom-width:1px;border-color:var(--color-dark-200);min-height:3.5rem;position:relative}.djn-table>.djn-tbody td label:first-child:not(.input-file-edit-btn){display:none}.flatpickr-day.djn-table>.djn-tbody td label:first-child:not(.input-file-edit-btn){visibility:hidden}.djn-table>.djn-tbody td:not(:first-child){border-left-width:1px}.djn-table>.djn-tbody td.original{min-width:2.5rem;width:2.5rem}.djn-table>.djn-tbody td.original:not(.is-sortable){display:none}.flatpickr-day.djn-table>.djn-tbody td.original:not(.is-sortable){visibility:hidden}.djn-table>.djn-tbody td.original:not(.is-sortable)+td{border-left:0}.djn-table>.djn-tbody td.original>p{display:none}.flatpickr-day.djn-table>.djn-tbody td.original>p{visibility:hidden}.djn-table>.djn-tbody td select,.djn-table>.djn-tbody td>input[type=text]{height:100%;min-width:10rem}.djn-table>.djn-tbody td>.autocomplete-data-wrapper+p{display:none}.flatpickr-day.djn-table>.djn-tbody td>.autocomplete-data-wrapper+p{visibility:hidden}.djn-table>.djn-tbody td.field-image{max-width:23.125rem}.djn-table>.djn-tbody td .btn:not(.input-file-edit-btn),.djn-table>.djn-tbody td .input:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.djn-table>.djn-tbody td .toggle~label{margin-left:.5rem}.djn-table>.djn-tbody td .input-file-wrapper>.input-file{border-width:0}.djn-table>.djn-tbody:last-child>tr:last-child>td:first-child{border-bottom-left-radius:6px}.djn-table>.djn-tbody:last-child>tr:last-child>td:last-child{border-bottom-right-radius:6px}.djn-table>.djn-tbody.ui-sortable-placeholder td{background-color:var(--color-primary-50);height:3.5rem}.djn-table>.djn-tbody.has-errors td{vertical-align:top}.djn-table>:nth-last-child(2) td:first-child,.djn-table>:nth-last-child(2) th:first-child{border-bottom-left-radius:6px}.djn-table>:nth-last-child(2) td:last-child,.djn-table>:nth-last-child(2) th:last-child{border-bottom-right-radius:6px}.inline-group .empty-form{display:none!important}.djn-item{position:relative}.djn-drag-handler{--tw-translate-y:-50%;cursor:move;display:flex;left:.5rem;margin-right:.5rem;position:absolute;top:50%;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.stacked-row .form-row{display:flex;flex-direction:column;margin-bottom:1.5rem}.stacked-row .form-row>div>.help,.stacked-row .form-row>div>label:first-child{display:none}.stacked-row .form-row>.errorlist{order:1}.checkbox-row>label{display:none}fieldset.module>h2{align-items:center;color:var(--color-dark-900);display:flex;font-size:1.125rem;font-weight:600;line-height:1.25rem;margin-bottom:1.5rem}fieldset.module>h2.stacked-inline-heading{font-size:1.5rem;line-height:2rem}@media (max-width:767px){fieldset.module>h2.stacked-inline-heading{padding-left:1.5rem;padding-right:1.5rem}}.djn-group .djn-group.djn-group-nested{border:0;margin:0}.djn-group .djn-group>fieldset>.djn-add-item,.djn-group .djn-group>fieldset>.stacked-inline-heading{padding-left:1.5rem;padding-right:1.5rem}.djn-td input[type=checkbox].toggle+label+label{font-size:0}:root{--modal-dialog-margin:0.5rem;--modal-dialog-margin-y-sm-up:1.75rem}.query-builder input,.query-builder select:not(.select2-hidden-accessible){--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder input~.error,.query-builder select:not(.select2-hidden-accessible)~.error{color:var(--color-negative)}.query-builder input:hover,.query-builder select:not(.select2-hidden-accessible):hover{border-color:var(--color-dark-400)}.query-builder input:not(:disabled):focus,.query-builder select:not(.select2-hidden-accessible):not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder input:disabled,.query-builder select:not(.select2-hidden-accessible):disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder input::-moz-placeholder,.query-builder select:not(.select2-hidden-accessible)::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder input::placeholder,.query-builder select:not(.select2-hidden-accessible)::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder input.field-valid,.query-builder select:not(.select2-hidden-accessible).field-valid{border-color:var(--color-success)}.query-builder input.field-valid~.success,.query-builder select:not(.select2-hidden-accessible).field-valid~.success{display:block}.query-builder input.field-error,.query-builder select:not(.select2-hidden-accessible).field-error{border-color:var(--color-negative)}.query-builder input.field-error~.error,.query-builder select:not(.select2-hidden-accessible).field-error~.error{display:block}input .query-builder input:-moz-read-only,input.query-builder select:not(.select2-hidden-accessible):-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input .query-builder input:read-only,input.query-builder select:not(.select2-hidden-accessible):read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input .query-builder input:not(:disabled):not(:-moz-read-only):focus,input.query-builder select:not(.select2-hidden-accessible):not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input .query-builder input:not(:disabled):not(:read-only):focus,input.query-builder select:not(.select2-hidden-accessible):not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea .query-builder input,textarea.query-builder select:not(.select2-hidden-accessible){height:auto}select .query-builder input,select.query-builder select:not(.select2-hidden-accessible){padding-right:2rem}.query-builder input,.query-builder select:not(.select2-hidden-accessible){width:100%!important}.djn-table>.djn-tbody td .query-builder input:not(.choices__input),.djn-table>.djn-tbody td .query-builder select:not(.select2-hidden-accessible):not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .select2{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative!important;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in!important;width:100%!important}.query-builder .select2~.error{color:var(--color-negative)}.query-builder .select2:hover{border-color:var(--color-dark-400)}.query-builder .select2:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .select2:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .select2::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .select2::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .select2.field-valid{border-color:var(--color-success)}.query-builder .select2.field-valid~.success{display:block!important}.query-builder .select2.field-error{border-color:var(--color-negative)}.query-builder .select2.field-error~.error{display:block!important}input.query-builder .select2:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.query-builder .select2:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.query-builder .select2:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .select2:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .select2{height:auto}select.query-builder .select2{padding-right:2rem}.query-builder .rules-group-container{background-color:var(--color-transparent)!important;border-color:var(--color-dark-200)!important;border-radius:6px!important;margin:0!important;padding:0!important}.query-builder .rules-group-container:after,.query-builder .rules-group-container:before{display:none}.flatpickr-day .query-builder .rules-group-container:after,.flatpickr-day.query-builder .rules-group-container:before{visibility:hidden}.query-builder .rules-group-container .rules-group-header{align-items:center;background-color:var(--color-dark-100);display:flex;flex-wrap:wrap;gap:1rem;margin-bottom:0;padding:1rem}.query-builder .rules-group-container .rules-group-header .drag-handle{order:1}.query-builder .rules-group-container .rules-group-header button[data-not]{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-transparent)!important;border-style:none!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;display:flex;font-weight:600;gap:.375rem;height:1.5rem;margin-right:1rem!important;padding:0!important;position:relative;text-transform:capitalize}@media (min-width:768px){.query-builder .rules-group-container .rules-group-header button[data-not]{font-size:1rem!important;line-height:1.25rem!important}}.query-builder .rules-group-container .rules-group-header button[data-not]:before{background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:9999px;border-width:1px;content:"";display:block;flex-shrink:0;height:1.5rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;position:relative;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:2.75rem}.query-builder .rules-group-container .rules-group-header button[data-not]:after{background-color:var(--color-dark-200);border-radius:9999px;content:"";display:block;flex-shrink:0;height:1.25rem;left:.125rem;position:absolute;top:.125rem;transition:left .15s ease-in-out,background-color .15s ease-in-out;width:1.25rem}.query-builder .rules-group-container .rules-group-header button[data-not]:not(.active):hover:before{border-color:var(--color-dark-400)}.query-builder .rules-group-container .rules-group-header button[data-not].active:before{background-color:var(--color-primary);border-color:var(--color-primary)}.query-builder .rules-group-container .rules-group-header button[data-not].active:after{background-color:var(--color-light);background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='m13.805 5.138-6.667 6.667a.667.667 0 0 1-.942 0L2.862 8.47l.943-.942 2.862 2.862 6.195-6.196.943.943Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;left:calc(2.75rem - 22px)}.query-builder .rules-group-container .rules-group-header .group-conditions{align-items:center;display:flex;margin-right:auto;order:2}.query-builder .rules-group-container .rules-group-header .group-actions{align-items:center;display:flex;flex-wrap:wrap;order:3;row-gap:.5rem}.query-builder .rules-group-container .rules-group-header .btn{height:2rem}.query-builder .rules-group-container .rules-list{display:flex;flex-direction:column;gap:1rem;margin:1rem;padding-left:0!important}.query-builder .rules-group-container .group-conditions label.btn{--tw-shadow:0 0 #0000!important;--tw-shadow-colored:0 0 #0000!important;align-items:center;background-color:var(--color-light)!important;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;color:var(--color-dark)!important;display:flex;justify-content:center;padding:.25rem .5rem!important}.query-builder .rules-group-container .group-conditions label.btn.active{background-color:var(--color-primary-600)!important;color:var(--color-light)!important}.query-builder .rule-container{display:grid;gap:.5rem;grid-template-columns:repeat(18,1fr);grid-template-rows:repeat(2,1fr);margin:0!important;padding-bottom:.5rem!important;padding-top:.5rem!important}@media (min-width:768px){.query-builder .rule-container{padding-bottom:1rem!important;padding-top:1rem!important}}.query-builder .rule-container{background-color:var(--color-dark-100)!important;border-color:var(--color-dark-200)!important;border-radius:6px!important}.query-builder .rule-container:after,.query-builder .rule-container:before{display:none}.flatpickr-day .query-builder .rule-container:after,.flatpickr-day.query-builder .rule-container:before{visibility:hidden}.query-builder .rule-container .drag-handle{display:flex;grid-column-end:2;grid-column-start:1;grid-row-end:3;grid-row-start:1;justify-content:center;margin:auto 0;width:100%}.query-builder .rule-container .drag-handle:before{width:1.25rem}.query-builder .rule-container .rule-filter-container{grid-column-end:18;grid-column-start:2;grid-row-end:2;grid-row-start:1}.query-builder .rule-container .rule-operator-container{grid-column-end:10;grid-column-start:2;grid-row-end:2;grid-row-start:2;margin-right:0!important;width:100%}.query-builder .rule-container .rule-operator-container:empty{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder .rule-container .rule-operator-container:empty~.error{color:var(--color-negative)}.query-builder .rule-container .rule-operator-container:empty:hover{border-color:var(--color-dark-400)}.query-builder .rule-container .rule-operator-container:empty:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .rule-container .rule-operator-container:empty:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .rule-container .rule-operator-container:empty::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-operator-container:empty::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-operator-container:empty.field-valid{border-color:var(--color-success)}.query-builder .rule-container .rule-operator-container:empty.field-valid~.success{display:block}.query-builder .rule-container .rule-operator-container:empty.field-error{border-color:var(--color-negative)}.query-builder .rule-container .rule-operator-container:empty.field-error~.error{display:block}input.query-builder .rule-container .rule-operator-container:empty:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-operator-container:empty:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-operator-container:empty:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .rule-container .rule-operator-container:empty:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .rule-container .rule-operator-container:empty{height:auto}select.query-builder .rule-container .rule-operator-container:empty{padding-right:2rem}.query-builder .rule-container .rule-operator-container:empty{border-style:none;cursor:not-allowed}.djn-table>.djn-tbody td .query-builder .rule-container .rule-operator-container:empty:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rule-container .rule-value-container{grid-column-end:18;grid-column-start:10;grid-row-end:3;grid-row-start:2;margin-right:0!important;width:100%}.query-builder .rule-container .rule-value-container:empty{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in;width:100%}.query-builder .rule-container .rule-value-container:empty~.error{color:var(--color-negative)}.query-builder .rule-container .rule-value-container:empty:hover{border-color:var(--color-dark-400)}.query-builder .rule-container .rule-value-container:empty:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.query-builder .rule-container .rule-value-container:empty:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.query-builder .rule-container .rule-value-container:empty::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-value-container:empty::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.query-builder .rule-container .rule-value-container:empty.field-valid{border-color:var(--color-success)}.query-builder .rule-container .rule-value-container:empty.field-valid~.success{display:block}.query-builder .rule-container .rule-value-container:empty.field-error{border-color:var(--color-negative)}.query-builder .rule-container .rule-value-container:empty.field-error~.error{display:block}input.query-builder .rule-container .rule-value-container:empty:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-value-container:empty:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default}input.query-builder .rule-container .rule-value-container:empty:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.query-builder .rule-container .rule-value-container:empty:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.query-builder .rule-container .rule-value-container:empty{height:auto}select.query-builder .rule-container .rule-value-container:empty{padding-right:2rem}.query-builder .rule-container .rule-value-container:empty{cursor:not-allowed}.djn-table>.djn-tbody td .query-builder .rule-container .rule-value-container:empty:not(.choices__input){--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;border-radius:0;border-width:0;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)}.query-builder .rule-container .rule-value-container input[type=text]{padding-left:.625rem;padding-right:.625rem}.query-builder .rule-container .rule-header{display:grid;grid-column-end:19;grid-column-start:18;grid-row-end:3;grid-row-start:1;height:100%;margin:auto 0;width:100%}.query-builder .rule-container .rule-header .btn-group{align-items:center;display:flex;justify-content:center}.query-builder .rule-container .rule-header .btn-group .btn{margin-right:0}.query-builder .drag-handle{flex-shrink:0;height:1.25rem;width:1.25rem}@media (max-width:767px){.query-builder .drag-handle{display:none!important}}.query-builder .drag-handle i{display:none}.flatpickr-day.query-builder .drag-handle i{visibility:hidden}.query-builder .drag-handle:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M6.25 5.833a1.667 1.667 0 1 0 0-3.333 1.667 1.667 0 0 0 0 3.333ZM7.916 10a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm0 5.833a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm5.834-10a1.667 1.667 0 1 0 0-3.333 1.667 1.667 0 0 0 0 3.333ZM15.416 10a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Zm0 5.833a1.667 1.667 0 1 1-3.333 0 1.667 1.667 0 0 1 3.333 0Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .rule-header{order:2}.query-builder .btn[data-delete]{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-transparent)!important;border-style:none;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-transparent)!important;flex-shrink:0;height:1.25rem;margin:0!important;padding:0!important;width:1.25rem}.query-builder .btn[data-delete] i{display:none}.flatpickr-day.query-builder .btn[data-delete] i{visibility:hidden}.query-builder .btn[data-delete]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='20' height='20' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='M8.037.833a.833.833 0 0 0-.73.433L6.173 3.333H1.667V5h1.25v13.333c0 .46.373.834.833.834h12.5c.46 0 .834-.373.834-.834V5h1.25V3.333H13.832l-1.107-2.06a.833.833 0 0 0-.734-.44H8.037Zm3.903 2.5-.447-.833H8.53l-.457.833h3.866ZM6.667 5H4.584v12.5h10.833V5h-8.75Zm.833 8.75V8.333h1.667v5.417H7.5Zm3.334-5.417v5.417H12.5V8.333h-1.666Z' fill='%239CA3AF'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:block;height:100%;width:100%}.query-builder .btn[data-delete]:hover{background-color:var(--color-transparent)!important;border-color:var(--color-transparent)!important}.query-builder .rule-filter-container,.query-builder .rule-operator-container{width:100%}@media (min-width:768px){.query-builder .rule-operator-container{width:50%}}.query-builder .rules-list:empty{display:none!important}.query-builder .rule-value-container{border-style:none!important;display:flex;padding-left:0!important}.query-builder .rule-value-container .select2{border-radius:6px;max-width:100%;min-width:0;overflow:hidden;padding:0!important}.query-builder .rule-value-container .select2:hover{border-color:var(--color-dark-400)!important}.query-builder .rule-value-container .select2 .select2-selection{border-style:none!important;height:100%}.query-builder .rule-value-container .select2 .select2-selection>span{align-items:center;display:flex;height:100%;text-overflow:ellipsis}.query-builder .rule-value-container .select2 .select2-selection .select2-selection__arrow{background-color:var(--color-light);right:0!important;top:0!important}.query-builder button[data-add]{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1)!important;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color)!important;align-items:center;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow)!important;display:flex;font-size:.875rem!important;font-weight:600;gap:.25rem;line-height:1.25rem!important;padding-left:.75rem!important;padding-right:.75rem!important}.query-builder button[data-add]:before{background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' fill='none'%3E%3Cpath fill-rule='evenodd' clip-rule='evenodd' d='m7.346 8.667-.005 3.999 1.333.002.005-4.001h3.987V7.333H8.681l.005-3.999-1.333-.001-.005 4H3.333v1.334h4.013Z' fill='%23111827'/%3E%3C/svg%3E");background-position:50%;background-repeat:no-repeat;background-size:contain;content:"";display:inline-block;flex-shrink:0;height:1rem;width:1rem}@media (min-width:768px){.select2-search{padding:.5rem!important}}.select2-search__field{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.1);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);background-color:var(--color-light);border-color:var(--color-dark-300);border-radius:6px;border-width:1px;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-900);font-size:.875rem;height:2.5rem;line-height:1.25rem;outline-color:var(--color-transparent);outline-style:solid;outline-width:1px;padding:.625rem;position:relative!important;transition:color .1s ease-in,background-color .1s ease-in,border-color .1s ease-in,box-shadow .1s ease-in,outline-color .1s ease-in!important;width:100%!important}.select2-search__field~.error{color:var(--color-negative)}.select2-search__field:hover{border-color:var(--color-dark-400)}.select2-search__field:not(:disabled):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}.select2-search__field:disabled{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600)}.select2-search__field::-moz-placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.select2-search__field::placeholder{color:var(--color-dark);padding-left:.25rem;padding-right:.25rem}.select2-search__field.field-valid{border-color:var(--color-success)}.select2-search__field.field-valid~.success{display:block!important}.select2-search__field.field-error{border-color:var(--color-negative)}.select2-search__field.field-error~.error{display:block!important}input.select2-search__field:-moz-read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.select2-search__field:read-only{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;background-color:var(--color-dark-50);border-color:var(--color-dark-200);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000 0),var(--tw-ring-shadow,0 0 #0000 0),var(--tw-shadow);color:var(--color-dark-600);cursor:default!important}input.select2-search__field:not(:disabled):not(:-moz-read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}input.select2-search__field:not(:disabled):not(:read-only):focus{border-color:var(--color-primary);border-width:1px;outline-color:var(--color-primary)}textarea.select2-search__field{height:auto}select.select2-search__field{padding-right:2rem}.select2-search__field{padding-left:.5rem!important;padding-right:.5rem!important}.select2-dropdown{border-color:var(--color-dark-300)!important;border-radius:6px!important;overflow:hidden}.select2-results__option{font-size:.875rem!important;line-height:1.25rem!important}@media (min-width:768px){.select2-results__option{padding:.625rem!important}}.select2-results__option{transition:background-color .05s ease-in-out,color .05s ease-in-out}.select2-results__option--highlighted{background-color:var(--color-primary)!important;color:var(--color-light)!important}.choices{display:flex;flex-direction:column;position:relative}.choices:not(.search-on):not(.search-off){display:none}.flatpickr-day.choices:not(.search-on):not(.search-off){visibility:hidden}.choices.search-on{padding-top:2.5rem}.choices.search-off .choices__inner>label,.choices.search-off .choices__input{display:none}.flatpickr-day .choices.search-off .choices__inner>label,.flatpickr-day.choices.search-off .choices__input{visibility:hidden}.choices.search-off .choices__list.choices__list--dropdown{margin-top:0}.choices__inner{order:1}.choices__input{background-color:transparent;left:0;padding-right:0;position:absolute;top:0;width:100%!important}.choices__input+label,.choices__list.choices__list--single+label{align-items:center;display:flex;height:2.5rem;justify-content:center;position:absolute;right:0;top:0;width:2.5rem;z-index:-1}.choices__input+label>svg,.choices__list.choices__list--single+label>svg{height:1.25rem;width:1.25rem}.choice__item{position:relative}.choices__list[role=listbox]::-webkit-scrollbar{height:9px;width:9px}.choices__list[role=listbox]::-webkit-scrollbar-track{background-color:var(--color-dark-50);border:none}.choices__list[role=listbox]::-webkit-scrollbar-thumb{background-clip:content-box;background-color:var(--color-dark-300);border:2px solid transparent;border-radius:6px;left:2px;right:2px}.choices__list[role=listbox]:hover::-webkit-scrollbar-thumb{background-color:var(--color-dark-400)}.choices__list[role=listbox]{max-height:13.5rem;overflow:auto}.choices__list.choices__list--dropdown{margin:.5rem -.75rem .25rem}.choices__list.choices__list--dropdown .choices__item{color:var(--color-dark-900);padding:.5rem .75rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.choices__list.choices__list--dropdown .choices__item:not(.has-no-choices):not(.has-no-results){cursor:pointer}.choices__list.choices__list--dropdown .choices__item:not(.has-no-choices):not(.has-no-results):hover{background-color:var(--color-dark-100)}.choices__list.choices__list--dropdown .choices__item.has-no-choices{padding-bottom:0;padding-top:.25rem}.choices__list.choices__list--single{display:none}.choices__list.choices__list--multiple{display:flex;flex-wrap:wrap;gap:.25rem;margin-left:-.75rem;margin-right:-.75rem;padding-bottom:0;padding-left:.75rem;padding-right:.75rem}.choices__list.choices__list--multiple:not(:empty){border-color:var(--color-dark-200);border-top-width:1px;padding-top:.75rem}.choices__list.choices__list--multiple .choices__item{align-items:center;background-color:var(--color-dark-100);border-color:var(--color-dark-200);border-radius:6px;border-width:1px;color:var(--color-dark-900);display:flex;font-size:.75rem;font-weight:500;line-height:1rem;padding:.25rem .5rem}.choices__list.choices__list--multiple .choices__item svg{color:var(--color-dark);display:flex;height:1rem;margin-left:.25rem;pointer-events:none;width:1rem}.js-ready .sidebar,.js-ready [class*=":sidebar"]{transition-duration:.3s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}.first-letter\:uppercase:first-letter{text-transform:uppercase}.empty\:hidden:empty{display:none}.hover\:rotate-90:hover{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:bg-dark-100:hover{background-color:var(--color-dark-100)}.hover\:text-dark-900:hover{color:var(--color-dark-900)}.hover\:text-notice:hover{color:var(--color-notice)}.hover\:text-dark-400:hover{color:var(--color-dark-400)}.peer:checked~.peer-checked\:border-dark-300{border-color:var(--color-dark-300)}.peer:checked~.peer-checked\:bg-dark-50{background-color:var(--color-dark-50)}@media (min-width:576px){.sm\:-mx-16{margin-left:-1rem;margin-right:-1rem}.sm\:mb-24{margin-bottom:1.5rem}.sm\:min-w-84{min-width:5.25rem}.sm\:flex-1{flex:1 1 0%}.sm\:grid-cols-2{grid-template-columns:repeat(2,minmax(0,1fr))}.sm\:gap-24{gap:1.5rem}.sm\:p-24{padding:1.5rem}}@media (min-width:768px){.md\:left-40{left:2.5rem}.md\:top-40{top:2.5rem}.md\:mr-8{margin-right:.5rem}.md\:block{display:block}.md\:hidden{display:none}.md\:w-1\/4{width:25%}.md\:max-w-640{max-width:40rem}.md\:grid-cols-3{grid-template-columns:repeat(3,minmax(0,1fr))}.md\:flex-wrap{flex-wrap:wrap}.md\:gap-16{gap:1rem}.md\:gap-x-8{-moz-column-gap:.5rem;column-gap:.5rem}.md\:p-16{padding:1rem}.md\:px-24{padding-left:1.5rem;padding-right:1.5rem}.md\:pb-32{padding-bottom:2rem}.md\:pt-24{padding-top:1.5rem}.md\:text-30{font-size:1.875rem;line-height:2.75rem}}@media (min-width:992px){.lg\:hidden{display:none}.lg\:w-370{width:23.125rem}.lg\:flex-shrink-0{flex-shrink:0}.lg\:gap-24{gap:1.5rem}}@media (min-width:1200px){.xl\:fixed{position:fixed}.xl\:left-260{left:16.25rem}.xl\:\!block{display:block!important}.xl\:hidden{display:none}.xl\:pl-260{padding-left:16.25rem}}@media (max-width:1199px){.max-lg\:sidebar{--tw-translate-x:-100%;height:100%;left:0;overflow:hidden;position:fixed;top:0;z-index:51}.max-lg\:sidebar,.max-lg\:sidebar.active{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.max-lg\:sidebar.active{--tw-translate-x:0}.max-lg\:sidebar.active+.bg-filter{opacity:1;transition:opacity .3s ease-in-out,z-index 0s linear 0s;z-index:50}.max-lg\:py-16{padding-bottom:1rem;padding-top:1rem}}@media (max-width:991px){.max-md\:flex-wrap{flex-wrap:wrap}}@media (max-width:767px){.max-sm\:-order-1{order:-1}.max-sm\:mt-8{margin-top:.5rem}.max-sm\:hidden{display:none}.max-sm\:flex-shrink-0{flex-shrink:0}.max-sm\:flex-wrap{flex-wrap:wrap}.max-sm\:overflow-x-auto{overflow-x:auto}.max-sm\:px-16{padding-left:1rem;padding-right:1rem}.max-sm\:px-24{padding-left:1.5rem;padding-right:1.5rem}}@media (max-width:575px){.max-xs\:hidden{display:none}.max-xs\:w-full{width:100%}.max-xs\:flex-wrap{flex-wrap:wrap}.max-xs\:px-20{padding-left:1.25rem;padding-right:1.25rem}.max-xs\:py-16{padding-bottom:1rem;padding-top:1rem}.max-xs\:text-12{font-size:.75rem;line-height:1.25rem}}
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/table.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/table.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/dist/translations.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/dist/translations.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/favicon.ico`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/favicon/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/fonts/Inter-Ext.woff2`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/fonts/Inter.woff2`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ag.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ai.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/al.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/al.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/au.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/au.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ba.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bi.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/br.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/br.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bs.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/bz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/caf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cas.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ceu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cna.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/coc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/csa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cv.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/cy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dj.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/dz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/en.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/en.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/er.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/er.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/et.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/et.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/eu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fj.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/fm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gb.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gq.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/gy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/hr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ht.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/il.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/il.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/im.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/im.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ir.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/je.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/je.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jo.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/jp.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ke.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/km.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/km.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kp.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ky.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/kz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/lr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ma.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/me.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/me.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mo.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ms.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mx.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/my.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/my.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/mz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/na.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/na.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/np.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/np.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/nz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pf.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ph.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/pt.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/rs.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sa.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sb.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sd.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sh.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sk.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/st.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/st.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/sz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tc.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tl.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tm.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tn.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/to.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/to.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tr.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tt.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/tz.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ug.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/us.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/us.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/uy.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vg.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/vu.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/ww.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/za.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/za.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/flags/zw.png`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/login.jpg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/login.jpg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/login.webp` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/login.webp`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/logo.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/logo.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/images/sk.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/images/sk.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/codemirror.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/django.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/codemirror/overlay.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/lazysizes.bgset.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/lazysizes.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/ls.unveilhooks.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/prices.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/prices.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/remove-me.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/remove-me.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/js/tabulator.min.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Accept-email.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Ad-product.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Add-picture.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/All-application.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Alphabetical-sorting.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-menu.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Application.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-left.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Arrow-circle-right.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/At-sign.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Attention.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Back-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bank-card-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Bookmark.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Box.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Camera.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-correct.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one-filled.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Check-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Close-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cut.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Cylinder.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Delete-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Download-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Drag.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Edit.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Export.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Figma-component.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Filter.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Find.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-ahead.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Go-on.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Headset-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Help.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Home.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Id-card-h.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Info.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Lightning.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Like.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Link-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/List-checkbox.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic-wand.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Magic.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-download.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Mail-open.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-emoji.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Message-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-three.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/More.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Paperclip.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Parallel-gateway.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/People-top-card.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Percentage.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Picture-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin Filled.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-close.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Preview-open.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Pushpin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Refresh-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Save.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Send-email.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Setting-two.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shop.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-bag.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping-cart-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Shopping.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Sort.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Star.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Success.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Table-report.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Tag-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translate.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Translation.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Triangle-round-rectangle.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Truck.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Undo.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Upload-one.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/User-business.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/View-grid-list.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Write.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/sprites/sb_admin/Zoom-in.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_base.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_base.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_choices.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_colors.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_components.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_components.css`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                 > a > svg {
                     @apply text-primary;
                 }
             }
         }
 
         &.active {
-            @apply text-primary font-semibold bg-light;
+            @apply text-primary-600 font-semibold bg-primary-100;
 
             svg {
                 @apply text-primary;
             }
         }
     }
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_datepicker.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_inlines.css`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,17 @@
     white-space: nowrap;
     min-width: 100%;
     @apply h-full;
     > .djn-thead {
         th {
             @apply p-8 h-48;
             @apply transition-colors;
-            @apply bg-dark-100 text-dark-600;
+            @apply bg-dark-50 text-dark-600;
             @apply text-14 font-normal text-left;
-            /*
-            &:first-child {
-                @apply border-l border-dark-200;
-            }
-            &:last-child {
-                @apply border-r border-dark-200;
-            }
-             */
+            @apply border-y border-dark-200;
             &.original {
                 @apply w-40 min-w-40;
                 &:not(.is-sortable) {
                     @apply hidden;
                     + td {
                         border-left: 0;
                     }
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_nouislider.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_tabulator.css`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 .tabulator .tabulator-header {
     position: relative;
     box-sizing: border-box;
     width: 100%;
     white-space: nowrap;
     overflow: hidden;
     user-select: none;
-    @apply border-b border-dark-200 bg-dark-100 text-dark-600;
+    @apply border-b border-dark-200 bg-dark-50 text-dark-600;
 }
 
 .tabulator .tabulator-header.tabulator-header-hidden {
     display: none;
 }
 
 .tabulator .tabulator-header .tabulator-header-contents {
@@ -47,23 +47,28 @@
     box-sizing: border-box;
     flex-direction: column;
     justify-content: flex-start;
     text-align: left;
     vertical-align: bottom;
     overflow: hidden;
     @apply transition-colors;
-    @apply bg-dark-100 text-dark-600;
+    @apply bg-dark-50 text-dark-600;
 }
 
 .tabulator .tabulator-header .tabulator-col .tabulator-col-content {
     box-sizing: border-box;
     position: relative;
     @apply p-8 min-h-48 flex items-center;
 }
 
+.tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title-holder {
+    display: flex;
+    align-items: center;
+}
+
 .tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title-holder.tabulator-col-sorter-element {
     position: relative;
 }
 
 .tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-title {
     box-sizing: border-box;
     width: 100%;
@@ -80,18 +85,14 @@
     white-space: normal;
     text-overflow: initial;
 }
 
 .tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter {
     display: flex;
     align-items: center;
-    position: absolute;
-    top: 0;
-    bottom: 0;
-    @apply right-2;
 }
 
 .tabulator .tabulator-header .tabulator-col .tabulator-col-content .tabulator-col-sorter .tabulator-arrow {
     border: none !important;
     opacity: 0;
     @apply transition-opacity;
     &:before {
@@ -123,15 +124,15 @@
     }
     .tabulator-col-content .tabulator-col-sorter .tabulator-arrow {
         opacity: 1;
     }
 }
 
 .tabulator .tabulator-header .tabulator-col.tabulator-sortable .tabulator-col-title {
-    @apply pr-20;
+    @apply pr-10;
 }
 
 .tabulator .tabulator-header .tabulator-col.tabulator-sortable[aria-sort="ascending"] .tabulator-col-content .tabulator-col-sorter .tabulator-arrow {
     &:before {
         border-bottom: 4px solid theme('colors.dark.800');
     }
 }
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/_utilities.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_button.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_dropdown.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_input.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_modal.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_nav-tabs.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_query-builder.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_toggle.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/css/components/_tooltip.css`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/chart.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/chart.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/choices.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/choices.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/datepicker.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/main.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -40,14 +40,17 @@
             return null
         })
 
         this.initDropdowns()
         document.addEventListener('formset:added', (e) => {
             this.initDropdowns(e.target)
             this.initFileInputs(e.target)
+            if (e.target !== e.target.parentNode.firstChild) {
+                e.target.parentNode.insertBefore(e.target, e.target.parentNode.firstChild)
+            }
         })
         document.addEventListener('openUrl', (e) => {
             window.open(e.detail.url, e.detail?.target || '_blank')
         })
 
         new Sidebar()
         new Datepicker()
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/multiselect.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/range.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/range.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/sidebar.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/sorting.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/column_display_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/data_edit_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/detail_view_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/filter_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/movable_columns_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/selection_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/table_params_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/table_modules/views_module.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/translations.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/translations.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/static/sb_admin/src/js/utils.js` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/static/sb_admin/src/js/utils.js`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/change_form.html`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 {% block js_init %}
     {{ block.super }}
     <script type="text/javascript" src="{% url 'admin:jsi18n' %}"></script>
     {{ media }}
 {% endblock %}
 
+{% block view_class %}change-form{% endblock %}
+
 {% block js %}
     {{ block.super }}
     <script type="text/javascript"
             id="django-admin-form-add-constants"
             src="{% static 'admin/js/change_form.js' %}"
         {% if adminform and add %}
             data-model-name="{{ opts.model_name }}"
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends "sb_admin/sb_admin_base.html" %} {% load i18n admin_urls static
 admin_modify sb_admin_tags %} {% block js_init %} {{ block.super }}
-{{ media }} {% endblock %} {% block js %} {{ block.super }}
+{{ media }} {% endblock %} {% block view_class %}change-form{% endblock %} {%
+block js %} {{ block.super }}
 % if adminform and add %} data-model-name="{{ opts.model_name }}" {% endif %}>
 {# JavaScript for prepopulated fields #} {% prepopulated_fields_js %} {%
 endblock %} {% block content %} {% block form_modal %} {% include 'sb_admin/
 partials/modal/modal.html' %} {% endblock %} {% get_tabular_context adminform
 inline_admin_formsets tabs_context as tabular_context %} {% block header %}
 {% if not is_popup and has_view_permission %} {% url opts|admin_urlname:
 'changelist' as changelist_url %} {% endif %}
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/change_password.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/list.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/list.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 {% extends list_base_template|default:"sb_admin/sb_admin_base.html" %}
 {% load sb_admin_tags i18n static %}
 
+{% block view_class %}change-list{% endblock %}
+
 {% block content %}
     {% block form_modal %}
         {% include 'sb_admin/partials/modal/modal.html' %}
     {% endblock %}
     {% block page_header %}
         <div class="py-16 md:pb-32 flex items-center max-xs:px-20">
             <h1 class="text-24 md:text-30 text-dark-900 font-bold font-heading line-clamp-1 first-letter:uppercase">{{ list_title }}</h1>
@@ -109,15 +111,15 @@
                                 class="btn btn-empty btn-small">{% trans 'Select all' %}
                         </button>
                         <button type="button"
                                 onclick="window.SBAdminTable['{{ view_id }}'].moduleInstances.selectionModule.selectNoData()"
                                 class="btn btn-empty btn-small">{% trans 'Select none' %}
                         </button>
                         {% for list_selection_action in content_context.list_selection_actions %}
-                            <button {% if list_action.open_in_modal %}{% include 'sb_admin/actions/partials/open_modal_attrs.html' with action=list_action %} hx-vals="js:{params: window.SBAdminTable['{{ view_id }}'].getAllUrlParams()}" {% else %}onclick="window.location.href='{{ list_selection_action.url }}' + window.SBAdminTable['{{ view_id }}'].getUrlParamsString()"{% endif %}
+                            <button {% if list_selection_action.open_in_modal %}{% include 'sb_admin/actions/partials/open_modal_attrs.html' with action=list_selection_action %} hx-vals="js:{params: window.SBAdminTable['{{ view_id }}'].getAllUrlParams()}" {% else %}onclick="window.location.href='{{ list_selection_action.url }}' + window.SBAdminTable['{{ view_id }}'].getUrlParamsString()"{% endif %}
                                     class="btn btn-small {{ list_selection_action.css_class|default_if_none:'' }}">{{ list_selection_action.title }}
                             </button>
                         {% endfor %}
                     </div>
                 </div>
             </div>
         {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% extends list_base_template|default:"sb_admin/sb_admin_base.html" %} {% load
-sb_admin_tags i18n static %} {% block content %} {% block form_modal %} {%
-include 'sb_admin/partials/modal/modal.html' %} {% endblock %} {% block
-page_header %}
+sb_admin_tags i18n static %} {% block view_class %}change-list{% endblock %} {%
+block content %} {% block form_modal %} {% include 'sb_admin/partials/modal/
+modal.html' %} {% endblock %} {% block page_header %}
 ************ {{{{ lliisstt__ttiittllee }}}} ************
     *     o {% block dropdown_actions %} {% for list_action in
             content_context.list_actions %}
           o % if list_action.open_in_modal %}{% include 'sb_admin/actions/
             partials/open_modal_attrs.html' with action=list_action %} hx-
             vals="js:{params: window.SBAdminTable['{{ view_id
             }}'].getAllUrlParams()}" {% else %}onclick="window.location.href='{
@@ -37,18 +37,18 @@
 {% endblock %}
 {% include 'sb_admin/components/filters.html' with
 filters=content_context.filters %}
 {% endwith %} {% endblock %}
 ??
 {% trans 'Select all' %} {% trans 'Select none' %} {% for list_selection_action
 in content_context.list_selection_actions %}
-% if list_action.open_in_modal %}{% include 'sb_admin/actions/partials/
-open_modal_attrs.html' with action=list_action %} hx-vals="js:{params:
-window.SBAdminTable['{{ view_id }}'].getAllUrlParams()}" {% else
-%}onclick="window.location.href='{{ list_selection_action.url }}' +
+% if list_selection_action.open_in_modal %}{% include 'sb_admin/actions/
+partials/open_modal_attrs.html' with action=list_selection_action %} hx-
+vals="js:{params: window.SBAdminTable['{{ view_id }}'].getAllUrlParams()}" {%
+else %}onclick="window.location.href='{{ list_selection_action.url }}' +
 window.SBAdminTable['{{ view_id }}'].getUrlParamsString()"{% endif %}
 class="btn btn-small {{ list_selection_action.css_class|default_if_none:'' }}">
 {{ list_selection_action.title }} {% endfor %}
 {% endblock %} {% block tabulator_body %}
 {% endblock %} {% block tabulator_custom_footer %}
 {% trans 'For page' %}
 {% endblock %}
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/object_history.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/partials/translations_status_row.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations-detail.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations-language-choice.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/actions/translations.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/actions/translations.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/login.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/login.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/login_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/authentification/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/buttons.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/buttons.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/columns.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/columns.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/filters.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/filters.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/components/inputs.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/components/inputs.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/config/view.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/config/view.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_aggregate_sub_widget.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/chart_widget.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/dashboard/widget_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/autocomplete_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/boolean_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/date_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/multiple_choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/number_range_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/partials/clear.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/radio_choice_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/filter_widgets/string_field.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/fonts.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/fonts.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/components.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/components.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/inline_fieldset.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/includes/notifications.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/stacked_inline.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline.html`

 * *Files 3% similar despite different names*

```diff
@@ -132,14 +132,17 @@
                                                             {% if field.field.is_hidden %} {{ field.field }} {% endif %}
                                                         {% endfor %}
                                                     {% endfor %}
                                                 {% endfor %}
                                             {% endspaceless %}
                                         </td>
 
+                                        {% block table_inline_after_sortable %}
+                                        {% endblock %}
+
                                         {% for fieldset in inline_admin_form %}
                                             {% for line in fieldset %}
                                                 {% for field in line %}
                                                     {% if not field.field.is_hidden %}
                                                         <td class="djn-td field-{{ field.field.name }}">
                                                             {% if field.is_readonly %}
                                                                 <div class="px-10 py-8">{{ field.contents }}</div>
@@ -150,33 +153,17 @@
                                                                 {% endif %}
                                                             {% endif %}
                                                         </td>
                                                     {% endif %}
                                                 {% endfor %}
                                             {% endfor %}
                                         {% endfor %}
-                                        {% if inline_admin_formset.formset.can_delete %}
-                                            {% if inline_admin_form.original %}
-                                                <td>
-                                                    <div class="relative min-h-40 flex items-center delete djn-delete-handler {{ inline_admin_formset.handler_classes|join:" " }}">
-                                                        {% render_field inline_admin_form.deletion_field.field class="checkbox checkbox-delete" %}
-                                                        <label for="{{ inline_admin_form.deletion_field.field.auto_id }}">
-                                                            <svg class="w-20 h-20"><use xlink:href="#Delete"></use></svg>
-                                                        </label>
-                                                    </div>
-                                                </td>
-                                            {% else %}
-                                                <td class="delete">
-                                                    <a
-                                                    class="flex-center h-40 inline-deletelink djn-remove-handler {{ inline_admin_formset.handler_classes|join:" " }}"
-                                                    href="javascript:void(0)"><svg class="w-20 h-20 text-dark-300 hover:text-dark-400"><use xlink:href="#Delete"></use></svg></a>
-                                                </td>
-                                            {% endif %}
-                                        {% endif %}
-
+                                        {% block table_inline_delete_button %}
+                                            {% include "sb_admin/includes/table_inline_delete_button.html" %}
+                                        {% endblock %}
                                     </tr>
 
                                     {% if inline_admin_form.form.inlines %}
                                         <tr class="djn-tr">
                                             <td class="djn-td" colspan="{{ inline_admin_form|cell_count }}">
                                                 {% for nested in inline_admin_form.form.inlines %}
                                                     {% include nested.opts.template with inline_admin_formset=nested %}
```

#### html2text {}

```diff
@@ -13,38 +13,38 @@
  {% endfor %} {% if inline_admin_formset.has_add_permission %}
 }}"> {% trans 'Add' %}
 {% endif %}
 {{ inline_admin_formset.formset.management_form }} {% if
 inline_admin_formset.formset.non_form_errors %}
 {{ inline_admin_formset.formset.non_form_errors }}
 {% endif %}
-                                                   {{{{ ffiieelldd..llaabbeell||ccaappffiirrsstt
-                                                   }}}}{{%% iiff ffiieelldd..rreeqquuiirreedd
-                                                   %%}}**{{%% eennddiiff %%}} {{%% iiff
+                                                   {{{{ ffiieelldd..llaabbeell||ccaappffiirrsstt }}}}
+                                                   {{%% iiff ffiieelldd..rreeqquuiirreedd %%}}**{{%%
+                                                   eennddiiff %%}} {{%% iiff
                                                    ffiieelldd..hheellpp__tteexxtt %%}}? 
                                                    {{%% eennddiiff %%}}
     * {{ inline_admin_form.form.non_field_errors
       }}
 {% if
 inline_admin_formset.opts.sortable_field_name %}
 {% endif %} {% if inline_admin_form.original or
 inline_admin_form.show_url %}
 {% if inline_admin_form.original %} {
 { inline_admin_form.original }} {% if
 inline_admin_form.model_admin.show_change_link and
-inline_admin_form.model_admin.has_registered_model {% if field.is_readonly
-%} _{_%_ _i_f                                           %}
+inline_admin_form.model_admin.has_registered_model
+%} _{_%_ _i_f                                           {% if field.is_readonly %}
 _i_n_l_i_n_e___a_d_m_i_n___f_o_r_m_s_e_t_._h_a_s___c_h_a_n_g_e___p_e_r_m_i_s_s_i_o_n_ _%_}_ _{_%   {{ field.contents }}
-_t_r_a_n_s_ _"_C_h_a_n_g_e_"_ _%_}_{_%_ _e_l_s_e_ _%_}_ _{_%_ _t_r_a_n_s_ _"_V_i_e_w_"_ _%_}_{_%   {% else %} {             }}"> {% render_field                   }}"
-_e_n_d_i_f_ _%_}{% endif %} {% endif %} {% if              { field.field }} {% if   inline_admin_form.deletion_field.field href="javascript:
-inline_admin_form.show_url %} _{_%_ _t_r_a_n_s_ _"_V_i_e_w_ _o_n    field.field.errors %} {  class="checkbox checkbox-delete" %}    void(0)">
-_s_i_t_e_"_ _%_}{% endif %}                                {
-{% endif %} {% if                                  field.field.errors.as_ul
-inline_admin_form.needs_explicit_pk_field %} {     }} {% endif %} {% endif
-{ inline_admin_form.pk_field.field }}{% endif %}   %}
+_t_r_a_n_s_ _"_C_h_a_n_g_e_"_ _%_}_{_%_ _e_l_s_e_ _%_}_ _{_%_ _t_r_a_n_s_ _"_V_i_e_w_"_ _%_}_{_%   {% else %} {{ field.field
+_e_n_d_i_f_ _%_}{% endif %} {% endif %} {% if              }} {% if field.field.errors
+inline_admin_form.show_url %} _{_%_ _t_r_a_n_s_ _"_V_i_e_w_ _o_n    %} {
+_s_i_t_e_"_ _%_}{% endif %}                                { field.field.errors.as_ul
+{% endif %} {% if                                  }} {% endif %} {% endif %}
+inline_admin_form.needs_explicit_pk_field %} {
+{ inline_admin_form.pk_field.field }}{% endif %}
 {% if inline_admin_form.fk_field %} {
 { inline_admin_form.fk_field.field }}{% endif %}
 {% spaceless %} {% for fieldset in
 inline_admin_form %} {% for line in fieldset %} {%
 for field in line %} {% if field.field.is_hidden
 %} {{ field.field }} {% endif %} {% endfor %} {%
 endfor %} {% endfor %} {% endspaceless %}
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/inlines/table_inline_paginated.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/cms/page_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/filer_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/folder_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/filer/image_change_form.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/integrations/sorting/change_list.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/navigation.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/navigation.html`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         </div>
         <img src="{{ LAZY_LOAD_DEFAULT_IMAGE }}" data-src="{% static 'sb_admin/images/logo.svg' %}" class="lazyload h-32 w-auto"
                  alt="SBAdmin" width="106" height="16">
         <div class="w-32 h-32 rounded-full leading-none flex-center flex-shrink-0 bg-dark-300 ml-auto">
             {{ username_data.initials }}
         </div>
     </header>
-    <nav class="w-260 xl:fixed top-0 bottom-0 left-0 max-lg:sidebar border-r border-dark-200 overflow-hidden flex flex-col relative bg-dark-100 z-1"
+    <nav class="w-260 xl:fixed top-0 bottom-0 left-0 max-lg:sidebar border-r border-dark-200 overflow-hidden flex flex-col relative bg-dark-50 z-1"
          id="main-navigation">
         <header class="px-24 py-32 hidden xl:!block">
             <img src="{{ LAZY_LOAD_DEFAULT_IMAGE }}" data-src="{% static 'sb_admin/images/logo.svg' %}" class="lazyload h-32 w-auto"
                  alt="SBAdmin" width="133" height="20">
         </header>
         <header class="px-16 py-8 flex items-center xl:hidden border-b border-dark-200 bg-light min-h-56">
             <div class="js-sidebar-toggle w-24 h-24 flex-center ml-auto" data-sidebar-target="main-navigation">
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/messages/alert_base.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/partials/modal/modal.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sb_admin_base_no_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sb_admin_js_trans.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/sprites/sb_admin.svg`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/submit_line.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/tailwind_whitelist.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/array.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/array.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/autocomplete.html`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
     <div class="relative">
         {% include 'sb_admin/widgets/includes/field_label.html' %}
         <div id="{{ widget.attrs.id }}-wrapper">
             <button
                     data-bs-toggle="dropdown"
                     aria-expanded="false"
                     data-bs-offset="[0, 8]"
-                    class="btn px-10 font-normal w-full"
+                    class="autocomplete-button btn px-10 font-normal w-full"
             >
-                <span id="{{ widget.attrs.id }}-value">{{ widget.form_field.empty_label }}</span>
-                <svg class="ml-8">
-                    <use xlink:href="#Down"></use>
-                </svg>
+                {% block autocomplete_button_text %}
+                    <span id="{{ widget.attrs.id }}-value">{{ widget.form_field.empty_label }}</span>
+                    <svg class="ml-8">
+                        <use xlink:href="#Down"></use>
+                    </svg>
+                {% endblock %}
             </button>
             <div class="dropdown-menu max-h-none w-248">
                 <div class="px-12 pt-8">
                     {% include 'sb_admin/widgets/input.html' %}
                     <select {% if filter_widget.multiselect %}multiple{% endif %} class="js-autocomplete"
                             data-autocomplete-data-id="{{ autocomplete_data_id }}">
                     </select>
@@ -29,15 +31,15 @@
                                 <use xlink:href="#Add-one"></use>
                             </svg>
                             <span>{% trans 'Add' %} '<span class="js-add-item-label"></span>'</span>
                         </button>
                     </div>
                 {% endif %}
                 {% if widget.form_field.required %}
-                        <div class="pb-8"></div>
+                    <div class="pb-8"></div>
                 {% else %}
                     <div class="relative px-12 py-8 flex">
                         <button type="button"
                                 class="text-primary js-clear-autocomplete">
                             {% trans 'Clear' %}
                         </button>
                     </div>
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/checkbox_select.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/ckeditor.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templates/sb_admin/widgets/password.html` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templates/sb_admin/widgets/password.html`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templatetags/base.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templatetags/base.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/templatetags/sb_admin_tags.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/templatetags/sb_admin_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from django_smartbase_admin.templatetags.base import InclusionSBAdminNode
 
 register = template.Library()
 
 
 class SBAdminJSONEncoder(DjangoJSONEncoder):
     def default(self, o):
+        if callable(o):
+            return o.__name__
         to_json_method = getattr(o, "to_json", None)
         if to_json_method:
             return to_json_method()
         return super().default(o)
 
 
 @register.filter
```

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/utils.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/utils.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/dashboard_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/dashboard_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/global_filter_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/global_filter_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/src/django_smartbase_admin/views/translations_view.py` & `django_smartbase_admin-0.2.9/src/django_smartbase_admin/views/translations_view.py`

 * *Files identical despite different names*

### Comparing `django_smartbase_admin-0.2.7/PKG-INFO` & `django_smartbase_admin-0.2.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: django-smartbase-admin
-Version: 0.2.7
+Version: 0.2.9
 Summary: 
 Author: SmartBase
 Author-email: info@smartbase.sk
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=4.1,<6.0)
 Requires-Dist: django-admin-inline-paginator (>=0.4.0,<0.5.0)
 Requires-Dist: django-ckeditor (>=6.7.1,<7.0.0)
 Requires-Dist: django-filer (>=3.1.1,<4.0.0)
+Requires-Dist: django-htmx (>=1.17.3,<2.0.0)
 Requires-Dist: django-nested-admin (>=4.0.2,<5.0.0)
 Requires-Dist: django-widget-tweaks (>=1.5.0,<2.0.0)
 Requires-Dist: easy-thumbnails[svg] (>=2.8.5,<3.0.0)
 Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # django-smartbase-admin
```

