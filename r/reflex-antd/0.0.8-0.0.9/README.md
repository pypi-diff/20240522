# Comparing `tmp/reflex_antd-0.0.8.tar.gz` & `tmp/reflex_antd-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex_antd-0.0.8.tar", last modified: Mon May 13 02:45:24 2024, max compression
+gzip compressed data, was "reflex_antd-0.0.9.tar", last modified: Wed May 22 08:48:14 2024, max compression
```

## Comparing `reflex_antd-0.0.8.tar` & `reflex_antd-0.0.9.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.815598 reflex_antd-0.0.8/
--rw-rw-rw-   0        0        0    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1095 2024-05-13 02:45:24.814599 reflex_antd-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      392 2024-05-13 02:39:21.000000 reflex_antd-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.589887 reflex_antd-0.0.8/custom_components/
-drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.610886 reflex_antd-0.0.8/custom_components/reflex_antd/
--rw-rw-rw-   0        0        0        0 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.811597 reflex_antd-0.0.8/custom_components/reflex_antd/antd/
--rw-rw-rw-   0        0        0        0 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/__init__.py
--rw-rw-rw-   0        0        0      679 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.py
--rw-rw-rw-   0        0        0     3027 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.pyi
--rw-rw-rw-   0        0        0      977 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.py
--rw-rw-rw-   0        0        0     5761 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.pyi
--rw-rw-rw-   0        0        0     1028 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.py
--rw-rw-rw-   0        0        0     3581 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.pyi
--rw-rw-rw-   0        0        0     1549 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.py
--rw-rw-rw-   0        0        0     4343 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.pyi
--rw-rw-rw-   0        0        0     1025 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.py
--rw-rw-rw-   0        0        0     5821 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.pyi
--rw-rw-rw-   0        0        0      825 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.py
--rw-rw-rw-   0        0        0     5982 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.pyi
--rw-rw-rw-   0        0        0     3683 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.py
--rw-rw-rw-   0        0        0     6431 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.pyi
--rw-rw-rw-   0        0        0      760 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.py
--rw-rw-rw-   0        0        0     5336 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.pyi
--rw-rw-rw-   0        0        0      922 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.py
--rw-rw-rw-   0        0        0     3570 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.pyi
--rw-rw-rw-   0        0        0     1318 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.py
--rw-rw-rw-   0        0        0     3531 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.pyi
--rw-rw-rw-   0        0        0     1366 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.py
--rw-rw-rw-   0        0        0     8569 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.pyi
--rw-rw-rw-   0        0        0      814 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.py
--rw-rw-rw-   0        0        0     3312 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.pyi
--rw-rw-rw-   0        0        0     2282 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.py
--rw-rw-rw-   0        0        0     6036 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.pyi
--rw-rw-rw-   0        0        0     1269 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.py
--rw-rw-rw-   0        0        0     5878 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.pyi
--rw-rw-rw-   0        0        0      935 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.py
--rw-rw-rw-   0        0        0     3541 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.pyi
--rw-rw-rw-   0        0        0     1439 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.py
--rw-rw-rw-   0        0        0     4525 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.pyi
--rw-rw-rw-   0        0        0     4993 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.py
--rw-rw-rw-   0        0        0    18220 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.pyi
--rw-rw-rw-   0        0        0      709 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.py
--rw-rw-rw-   0        0        0     3523 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.pyi
--rw-rw-rw-   0        0        0      488 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.py
--rw-rw-rw-   0        0        0     3108 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.pyi
--rw-rw-rw-   0        0        0     1398 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.py
--rw-rw-rw-   0        0        0     4423 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.pyi
--rw-rw-rw-   0        0        0     1518 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.py
--rw-rw-rw-   0        0        0     7141 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.pyi
--rw-rw-rw-   0        0        0      340 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.py
--rw-rw-rw-   0        0        0     2824 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.pyi
--rw-rw-rw-   0        0        0      476 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.py
--rw-rw-rw-   0        0        0     2957 2024-05-13 02:45:17.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.pyi
--rw-rw-rw-   0        0        0     1568 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.py
--rw-rw-rw-   0        0        0     9702 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.pyi
--rw-rw-rw-   0        0        0     5933 2024-05-13 02:02:38.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.py
--rw-rw-rw-   0        0        0    13522 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.pyi
--rw-rw-rw-   0        0        0      907 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.py
--rw-rw-rw-   0        0        0     5795 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.pyi
--rw-rw-rw-   0        0        0      472 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/helper.py
--rw-rw-rw-   0        0        0     2234 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.py
--rw-rw-rw-   0        0        0     4382 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.pyi
--rw-rw-rw-   0        0        0      973 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.py
--rw-rw-rw-   0        0        0     5740 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.pyi
--rw-rw-rw-   0        0        0     1934 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.py
--rw-rw-rw-   0        0        0    16264 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.pyi
--rw-rw-rw-   0        0        0     1565 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.py
--rw-rw-rw-   0        0        0     4754 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.pyi
--rw-rw-rw-   0        0        0     1783 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.py
--rw-rw-rw-   0        0        0    17500 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.pyi
--rw-rw-rw-   0        0        0     1114 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.py
--rw-rw-rw-   0        0        0     8452 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.pyi
--rw-rw-rw-   0        0        0     1383 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.py
--rw-rw-rw-   0        0        0     4506 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.pyi
--rw-rw-rw-   0        0        0     1981 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.py
--rw-rw-rw-   0        0        0     4629 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.pyi
--rw-rw-rw-   0        0        0     4765 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.py
--rw-rw-rw-   0        0        0     3207 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.pyi
--rw-rw-rw-   0        0        0     4427 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.py
--rw-rw-rw-   0        0        0     5273 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.pyi
--rw-rw-rw-   0        0        0     2011 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/notification.py
--rw-rw-rw-   0        0        0     1169 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.py
--rw-rw-rw-   0        0        0     3720 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.pyi
--rw-rw-rw-   0        0        0      972 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.py
--rw-rw-rw-   0        0        0     3683 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.pyi
--rw-rw-rw-   0        0        0      473 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.py
--rw-rw-rw-   0        0        0     4339 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.pyi
--rw-rw-rw-   0        0        0     1039 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.py
--rw-rw-rw-   0        0        0     4205 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.pyi
--rw-rw-rw-   0        0        0      941 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.py
--rw-rw-rw-   0        0        0     3561 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.pyi
--rw-rw-rw-   0        0        0     1221 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.py
--rw-rw-rw-   0        0        0     8537 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.pyi
--rw-rw-rw-   0        0        0      977 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.py
--rw-rw-rw-   0        0        0     3526 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.pyi
--rw-rw-rw-   0        0        0      545 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.py
--rw-rw-rw-   0        0        0     3296 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.pyi
--rw-rw-rw-   0        0        0      850 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.py
--rw-rw-rw-   0        0        0     3358 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.pyi
--rw-rw-rw-   0        0        0     2862 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.py
--rw-rw-rw-   0        0        0     6991 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.pyi
--rw-rw-rw-   0        0        0      575 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.py
--rw-rw-rw-   0        0        0     3087 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.pyi
--rw-rw-rw-   0        0        0     1272 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.py
--rw-rw-rw-   0        0        0     3979 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.pyi
--rw-rw-rw-   0        0        0      755 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.py
--rw-rw-rw-   0        0        0     5937 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.pyi
--rw-rw-rw-   0        0        0      588 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.py
--rw-rw-rw-   0        0        0     3232 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.pyi
--rw-rw-rw-   0        0        0     1213 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.py
--rw-rw-rw-   0        0        0     8925 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.pyi
--rw-rw-rw-   0        0        0     1036 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.py
--rw-rw-rw-   0        0        0     3902 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.pyi
--rw-rw-rw-   0        0        0     1042 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.py
--rw-rw-rw-   0        0        0     3580 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.pyi
--rw-rw-rw-   0        0        0     2690 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.py
--rw-rw-rw-   0        0        0     5708 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.pyi
--rw-rw-rw-   0        0        0     2108 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.py
--rw-rw-rw-   0        0        0     5255 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.pyi
--rw-rw-rw-   0        0        0     1063 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.py
--rw-rw-rw-   0        0        0     5614 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.pyi
--rw-rw-rw-   0        0        0      566 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.py
--rw-rw-rw-   0        0        0     3155 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.pyi
--rw-rw-rw-   0        0        0     1352 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.py
--rw-rw-rw-   0        0        0     4321 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.pyi
--rw-rw-rw-   0        0        0     1237 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.py
--rw-rw-rw-   0        0        0     4153 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.pyi
--rw-rw-rw-   0        0        0     1997 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.py
--rw-rw-rw-   0        0        0     3945 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.pyi
--rw-rw-rw-   0        0        0     2609 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.py
--rw-rw-rw-   0        0        0     6106 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.pyi
--rw-rw-rw-   0        0        0     2869 2024-05-11 09:33:48.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.py
--rw-rw-rw-   0        0        0     6439 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.pyi
--rw-rw-rw-   0        0        0     1763 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.py
--rw-rw-rw-   0        0        0    15141 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.pyi
--rw-rw-rw-   0        0        0     1584 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.py
--rw-rw-rw-   0        0        0     4426 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.pyi
--rw-rw-rw-   0        0        0      738 2024-05-11 09:33:51.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.py
--rw-rw-rw-   0        0        0     3323 2024-05-13 02:45:18.000000 reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.pyi
--rw-rw-rw-   0        0        0    26581 2024-05-13 02:00:08.000000 reflex_antd-0.0.8/custom_components/reflex_antd/base.py
--rw-rw-rw-   0        0        0    15233 2024-05-13 02:45:09.000000 reflex_antd-0.0.8/custom_components/reflex_antd/base.pyi
--rw-rw-rw-   0        0        0     1919 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/constant.py
--rw-rw-rw-   0        0        0      996 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/display.py
--rw-rw-rw-   0        0        0      899 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/entry.py
--rw-rw-rw-   0        0        0      515 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/feedback.py
--rw-rw-rw-   0        0        0      289 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/general.py
--rw-rw-rw-   0        0        0      163 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/helper.py
--rw-rw-rw-   0        0        0      243 2024-05-11 09:33:47.000000 reflex_antd-0.0.8/custom_components/reflex_antd/layout.py
--rw-rw-rw-   0        0        0      288 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/navigation.py
--rw-rw-rw-   0        0        0     1654 2024-05-11 09:33:52.000000 reflex_antd-0.0.8/custom_components/reflex_antd/util.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:45:24.812598 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/
--rw-rw-rw-   0        0        0     1095 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6944 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 02:45:24.000000 reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      822 2024-05-13 02:39:38.000000 reflex_antd-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 02:45:24.815598 reflex_antd-0.0.8/setup.cfg
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:48:14.671549 reflex_antd-0.0.9/
+-rwxrwxrwx   0 see       (1000) see       (1000)    11357 2024-03-25 11:08:46.000000 reflex_antd-0.0.9/LICENSE
+-rwxrwxrwx   0 see       (1000) see       (1000)     1049 2024-05-22 08:48:14.664549 reflex_antd-0.0.9/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)      392 2024-05-13 02:39:21.000000 reflex_antd-0.0.9/README.md
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:48:10.664260 reflex_antd-0.0.9/custom_components/
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:48:10.987889 reflex_antd-0.0.9/custom_components/reflex_antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/__init__.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:48:14.629994 reflex_antd-0.0.9/custom_components/reflex_antd/antd/
+-rwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/__init__.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      679 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/affix.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3027 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/affix.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/alert.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5761 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/alert.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1028 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/anchor.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3581 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/anchor.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1549 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/auto_complete.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4343 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/auto_complete.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1025 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/avatar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5821 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/avatar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      825 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/badge.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5982 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/badge.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     3683 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6431 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      760 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/breadcrumb.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5336 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/breadcrumb.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      922 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3570 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1318 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/calendar.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3531 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/calendar.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1366 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/card.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8569 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/card.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      814 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/carousel.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3312 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/carousel.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2282 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/cascader.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6036 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/cascader.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1269 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/checkbox.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5878 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/checkbox.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      935 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/collapse.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3541 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/collapse.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1439 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/color_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4525 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/color_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4993 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/date_picker.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    18220 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/date_picker.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      709 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/descriptions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3523 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/descriptions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      488 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/divider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3108 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/divider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1398 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/drawer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4423 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/drawer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1518 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/dropdown.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     7141 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/dropdown.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      340 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/empty.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2824 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/empty.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      476 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/flex.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2957 2024-05-13 02:45:17.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/flex.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1568 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/float_button.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     9702 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/float_button.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     5945 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/form.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    13522 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/form.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      907 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/grid.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5795 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/grid.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      472 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/helper.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2234 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/icon.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4382 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/icon.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      973 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/image.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5740 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/image.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1934 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/input.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    16264 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/input.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1565 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/input_number.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4754 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/input_number.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1783 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    17500 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/layout.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1114 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/list.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8452 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/list.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1383 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/mentions.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4506 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/mentions.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1981 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/menu.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4629 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/menu.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     6287 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/message.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3207 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/message.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     4427 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/modal.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5273 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/modal.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2011 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/notification.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     1169 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/pagination.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3720 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/pagination.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      972 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/popconfirm.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3683 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/popconfirm.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      484 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/popover.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4339 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/popover.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1039 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/progress.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4205 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/progress.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      941 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/qrcode.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3561 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/qrcode.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1221 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/radio.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8537 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/radio.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      977 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/rate.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3526 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/rate.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      545 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/result.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3296 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/result.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      850 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/segmented.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3358 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/segmented.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2862 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6991 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      575 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/skeleton.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3087 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/skeleton.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1272 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/slider.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3979 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/slider.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      755 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/space.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5937 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/space.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      588 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/spin.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3232 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/spin.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1213 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/statistic.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     8925 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/statistic.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1036 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/steps.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3902 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/steps.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1042 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/switch.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3580 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/switch.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2690 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/table.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5708 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/table.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2108 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tabs.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5255 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tabs.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1063 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tag.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     5614 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tag.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      566 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/timeline.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3155 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/timeline.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1352 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tooltip.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4321 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tooltip.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1237 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tour.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4153 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tour.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1997 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/transfer.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3945 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/transfer.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2609 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6106 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     2869 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree_select.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     6439 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree_select.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1763 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/typography.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    15141 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/typography.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1584 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/upload.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     4426 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/upload.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)      738 2024-05-22 08:43:35.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/watermark.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     3323 2024-05-13 02:45:18.000000 reflex_antd-0.0.9/custom_components/reflex_antd/antd/watermark.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)    31638 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/base.py
+-rwxrwxrwx   0 see       (1000) see       (1000)    15233 2024-05-13 02:45:09.000000 reflex_antd-0.0.9/custom_components/reflex_antd/base.pyi
+-rwxrwxrwx   0 see       (1000) see       (1000)     1919 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/constant.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      996 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/display.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      899 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/entry.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      525 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/feedback.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      289 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/general.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      210 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/helper.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      243 2024-05-22 08:43:32.000000 reflex_antd-0.0.9/custom_components/reflex_antd/layout.py
+-rwxrwxrwx   0 see       (1000) see       (1000)      288 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/navigation.py
+-rwxrwxrwx   0 see       (1000) see       (1000)     2403 2024-05-22 08:43:36.000000 reflex_antd-0.0.9/custom_components/reflex_antd/util.py
+drwxrwxrwx   0 see       (1000) see       (1000)        0 2024-05-22 08:48:14.655988 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/
+-rwxrwxrwx   0 see       (1000) see       (1000)     1049 2024-05-22 08:48:09.000000 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/PKG-INFO
+-rwxrwxrwx   0 see       (1000) see       (1000)     6944 2024-05-22 08:48:10.000000 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/SOURCES.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)        1 2024-05-22 08:48:09.000000 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/dependency_links.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       33 2024-05-22 08:48:09.000000 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/requires.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)       12 2024-05-22 08:48:09.000000 reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/top_level.txt
+-rwxrwxrwx   0 see       (1000) see       (1000)      823 2024-05-22 08:45:23.000000 reflex_antd-0.0.9/pyproject.toml
+-rwxrwxrwx   0 see       (1000) see       (1000)       38 2024-05-22 08:48:14.671549 reflex_antd-0.0.9/setup.cfg
```

### Comparing `reflex_antd-0.0.8/LICENSE` & `reflex_antd-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/PKG-INFO` & `reflex_antd-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: reflex-antd
-Version: 0.0.8
-Summary: Reflex custom component antd
-Author-email: seewind <seewindcn@gmail.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: source, https://github.com/seewindcn/reflex-antd
-Keywords: reflex,reflex-custom-components,ant-design,antd
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.2
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# reflex-antd
-
-A Reflex custom component wrap [ant.design](https://ant.design/).
-pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
-
-## Installation
-
-```bash
-pip install reflex-antd
-```
-
-## antd-demo
-
-[antd-demo](https://antd-demo.reflex.run)
-
-
-### screen
-- table
-![table](docs/img/table1.png)
-- menu
-![menu1](docs/img/menu1.png)
-- transfer
-![transfer1](docs/img/transfer1.png)
-- ...
-
-
-
+Metadata-Version: 2.1
+Name: reflex-antd
+Version: 0.0.9
+Summary: Reflex custom component antd
+Author-email: seewind <seewindcn@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: source, https://github.com/seewindcn/reflex-antd
+Keywords: reflex,reflex-custom-components,ant-design,antd
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: reflex>=0.4.2
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# reflex-antd
+
+A Reflex custom component wrap [ant.design](https://ant.design/).
+pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
+
+## Installation
+
+```bash
+pip install reflex-antd
+```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/affix.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/affix.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/affix.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/alert.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/alert.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/alert.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/anchor.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/anchor.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/anchor.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/auto_complete.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/auto_complete.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/auto_complete.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/avatar.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/avatar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/badge.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/badge.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/badge.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/base.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/base.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/breadcrumb.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/breadcrumb.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/button.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/calendar.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/calendar.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/calendar.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/card.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/card.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/card.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/carousel.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/carousel.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/carousel.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/cascader.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/cascader.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/cascader.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/checkbox.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/checkbox.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/collapse.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/collapse.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/collapse.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/color_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/color_picker.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/color_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/date_picker.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/date_picker.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/date_picker.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/descriptions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/descriptions.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/descriptions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/divider.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/divider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/drawer.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/drawer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/dropdown.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/dropdown.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/dropdown.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/empty.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/empty.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/flex.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/flex.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/float_button.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/float_button.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/float_button.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,16 +85,14 @@
     validate_debounce: Optional[Var[float]]
     validate_first: Optional[Var[Union[bool, str]]]
     validate_status: Optional[Var[str]]
     validate_trigger: Optional[Var[Union[str, List[str]]]]
     value_prop_name: Optional[Var[str]]
     wrapper_col: Optional[Var[Dict]]
 
-    rules: Optional[Var[List[Dict]]]
-
 
 class FormList(AntdComponent):
     tag = 'Form.List'
 
     # children: Optional[Var[JsValue]]
     initial_value: Optional[Var[List]]
     name: Optional[Var[Union[str, int, List[Union[str, int]]]]]
@@ -124,14 +122,15 @@
     if form_id is None:
         form_id = f'form_{uuid.uuid4().hex}'
     props.update(
         form=form_id,
         preserve=False,
     )
     f = form(*children, **props)
+    f._memoization_mode = memo_never_no_recursive
 
     modal_config = modal_config or {}
     modal_config.update(destroy_on_close=True)
     modal_config['on_ok'] = js_value(f"""() => {{
         return new Promise((resolve, reject) => {{
     {form_id}
       .validateFields({{
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/form.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/form.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/grid.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/grid.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/grid.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/icon.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/icon.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/icon.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/image.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/image.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/image.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/input.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/input.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/input_number.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/input_number.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/input_number.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/layout.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/layout.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/layout.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/list.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/list.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/list.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/mentions.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/mentions.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/mentions.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/menu.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/menu.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/menu.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/modal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,132 @@
-from typing import Optional, Union, Dict, Any, List, Set, Iterator
+from typing import Optional, Union, Dict, Any, List, Set
 import uuid
 
 from reflex import Component, Var
 from reflex.utils import imports
-from reflex.components.base.bare import Bare
-from reflex.vars import BaseVar
 
-from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, version
-from ..constant import MessageType
+from ..base import AntdComponent, ContainVar, JsValue, ReactNode, ExStateItem, FakeComponentMixin
+from ..constant import TypeType
+
 from . import helper
 
 
-class Message(JsValue):
-    is_global: bool = True
-    class_name: Optional[Var[str]]
-    content: Optional[Var[ReactNode]]
-    duration: Optional[Var[Union[int, float]]]
-    icon: Optional[Var[ReactNode]]
-    key: Optional[Var[Union[str, int]]]
-    style: Optional[Var[dict]]
-    type: Optional[MessageType] = 'info'
-    config: Optional[Var[dict]]
+class Modal(AntdComponent):
+    tag = 'Modal'
+
+    class_names: Optional[Var[ContainVar]]
+    styles: Optional[Var[ContainVar]]
+    cancel_button_props: Optional[Var[ContainVar]]
+    cancel_text: Optional[Var[ReactNode]]
+    centered: Optional[Var[bool]]
+    close_icon: Optional[Var[Union[ReactNode, bool]]]
+    confirm_loading: Optional[Var[bool]]
+    destroy_on_close: Optional[Var[bool]]
+    focus_trigger_after_close: Optional[Var[bool]]
+    footer: Optional[Var[ContainVar]]
+    force_render: Optional[Var[bool]]
+    get_container: Optional[Var[Union[bool, ContainVar]]]
+    keyboard: Optional[Var[bool]]
+    mask: Optional[Var[bool]]
+    mask_closable: Optional[Var[bool]]
+    modal_render: Optional[Var[ReactNode]]
+    ok_button_props: Optional[Var[ContainVar]]
+    ok_text: Optional[Var[ReactNode]]
+    ok_type: Optional[Var[TypeType]]
+    title: Optional[Var[ReactNode]]
+    open: Optional[Var[bool]]
+    width: Optional[Var[Union[str, int]]]
+    wrapClassName: Optional[Var[str]]
+    zIndex: Optional[Var[int]]
+
+    def _get_hooks(self) -> str | None:
+        _hooks = []
+        # if self.open is not None and 'on_open' in self.event_triggers:
+        #     _hooks.append(helper.hook_state(
+        #         state_field=self.open,
+        #         on_update=f'{str(self.event_triggers["on_open"])}()',
+        #     ))
+        return '\n'.join(_hooks) if _hooks else None
+
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = super().get_event_triggers()
+        _triggers.update({
+            "after_close": lambda: [],
+            "on_cancel": lambda e: [],
+            "on_ok": lambda e: [],
+            "after_open_change": lambda open: [open],
+        })
+        return _triggers
+
 
-    top: Optional[Var[int]]
-    rtl: Optional[Var[bool]]
-    prefix_cls: Optional[Var[str]]
-    max_count: Optional[Var[int]]
+class Confirm(FakeComponentMixin, JsValue):
+    config: Optional[Var[dict]]
 
     @property
     def config_item(self) -> Optional[ExStateItem]:
         if not hasattr(self, 'config') or self.config is None:
             return None
         try:
             return self._config_item
         except AttributeError:
-            self._config_item = ExStateItem(self.config, self)
+            if isinstance(self.config, Var):
+                self._config_item = ExStateItem(self.config, self)
+            else:
+                self._config_item = ContainVar.create(self.config).init(self, 'config')
             return self._config_item
 
     @property
     def uid(self) -> str:
         try:
             return self._uid
         except AttributeError:
             self._uid = uuid.uuid4().hex
             return self._uid
 
-    def get_open_message(self) -> str:
-        return f'openMessage_{self.uid}'
+    def get_name(self) -> str:
+        return f'confirm_{self.uid}'
 
     def get_imports(self) -> imports.ImportDict:
         _imports = {
-            "antd": [imports.ImportVar(tag='message')],
-            "react": [imports.ImportVar(tag="useEffect")],
+            "antd": [imports.ImportVar(tag='Modal')],
         }
-        return _imports
+        return imports.merge_imports(
+            _imports,
+            self.config_item.get_imports(),
+        )
 
     def get_hooks(self) -> Set[str] | Dict[str, None]:
-        if self.config_item is not None:
-            open_func = """const %(name)s = () => {
-                           %(mn)s.open(%(cfg)s);
-                       };""" % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                cfg=self.config_item.serialize(),
-            )
-        else:
-            key_s = f'{self.key},' if hasattr(self, 'key') else ''
-            duration_s = f'duration: {self.duration},' if hasattr(self, 'duration') else ''
-            top_s = f'top: {self.top},' if hasattr(self, 'top') else ''
-
-            open_func = """
-            const %(name)s = () => {
-                %(mn)s.open({
-                  %(key)s
-                  type: '%(type)s',
-                  content: '%(content)s',
-                  %(duration)s %(top)s
-                });
-            };
-            """ % dict(
-                name=self.get_open_message(),
-                mn='messageApi' if not self.is_global else 'message',
-                key=key_s, type=self.type, content=self.content,
-                duration=duration_s,
-                top=top_s,
-            )
-        others = []
-        if self.config_item:
-            state = self.config_item.serialize()
-            others.extend([
-                *self.config_item.get_hooks(),
-                helper.hook_state(
-                    state_field=state,
-                    on_update='%(name)s(%(state)s)' % dict(name=self.get_open_message(), state=state),
-                    on_null='messageApi.destroy()',
-                ),
-            ])
-
-        _hooks = []
-        if self.is_global:
-            _hooks.extend([
-                open_func
-            ])
-        else:
-            _hooks.extend([
-                """const [messageApi, contextHolder] = message.useMessage();""",
-                open_func,
-                *others,
-            ])
-        if version <= '000.004.006':
-            return set(_hooks)
-        return dict((h, None) for h in _hooks)
-
-    def serialize(self) -> str:
-        # if self.config_item is not None:
-        #     return '{contextHolder}'
-        return self.get_open_message()
-
-
-class MessageHolder(Bare):
-    """
-    Message.hook:
-        const [messageApi, contextHolder] = message.useMessage();
-
-    MessageHolder:
-        <>
-            {contextHolder}
-        </>
-     """
-    msg: Optional[Message]
-
-    @classmethod
-    def create(cls, msg: Message) -> Component:
-        cs = ['<>']
-        if not msg.is_global:
-            cs.append('{contextHolder}')
-        cs.append('</>')
-        return cls(
-            msg=msg,
-            contents='\n'.join(cs),
+        before_open = None
+        if isinstance(self.config_item, ContainVar):
+            before_open = self.config_item._var_fmt.get_ex_item('config.before_open')
+        call_before_open = f'({before_open.serialize()})();' \
+            if before_open is not None else ''
+        confirm_func = """const %(name)s = () => {
+                                %(call_before_open)s
+                               Modal.confirm(%(cfg)s);
+                               };""" % dict(
+            name=self.get_name(),
+            call_before_open=call_before_open,
+            cfg=self.config_item.serialize() if hasattr(self.config_item, 'serialize') else str(self.config_item),
         )
+        return {
+            **self.config_item.get_hooks(),
+            confirm_func: None,
+        }
 
-    def _get_vars(self, include_children: bool = False) -> Iterator[Var]:
-        yield self.contents
-        yield BaseVar(
-            _var_name='',
-            _var_is_local=True,
-            _var_data=self.msg.get_var_data(),
-        )
+    def get_event_triggers(self) -> Dict[str, Any]:
+        _triggers = {}
+        _triggers.update({
+            "config.after_close": lambda: [],
+            "config.on_cancel": lambda e: [],
+            "config.on_ok": lambda e: [],
+            "config.before_open": lambda e: [],
+            # not support: "config.after_open_change": lambda open: [open],
+        })
+        return _triggers
 
+    def serialize(self) -> str:
+        return self.get_name()
 
-message = Message
-message_holder = MessageHolder.create
 
-# def message_holder():
-#     return Var.create_safe('{contextHolder}')
+modal = Modal.create
+confirm = Confirm
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/message.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/message.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/modal.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/modal.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/notification.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/notification.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/pagination.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/pagination.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/pagination.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/popconfirm.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popconfirm.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/popconfirm.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/popover.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/popover.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/progress.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/progress.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/progress.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/qrcode.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/qrcode.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/qrcode.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/radio.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/radio.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/radio.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/rate.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/rate.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/rate.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/result.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/result.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/result.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/segmented.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/segmented.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/segmented.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/select.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/select.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/skeleton.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/skeleton.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/slider.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/slider.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/slider.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/space.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/space.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/space.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/spin.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/spin.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/spin.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/statistic.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/statistic.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/statistic.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/steps.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/steps.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/steps.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/switch.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/switch.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/switch.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/table.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/table.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/table.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tabs.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tabs.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tag.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tag.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tag.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/timeline.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/timeline.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/timeline.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tooltip.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tooltip.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tour.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tour.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tour.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/transfer.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/transfer.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/transfer.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree_select.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/tree_select.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/tree_select.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/typography.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/typography.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/typography.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/upload.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/upload.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/upload.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/watermark.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/antd/watermark.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/antd/watermark.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/base.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from hashlib import md5
 import uuid
 import dataclasses
 import inspect
 import re
 
 import reflex as rx
-from reflex import Component, Var, State, Base
+from reflex import Component, Var, State, Base, ImportVar
 from reflex.base import pydantic
 from reflex.components.component import BaseComponent, CustomComponent, StatefulComponent
 from reflex.components.base.bare import Bare
 from reflex.constants import Hooks, Reflex, MemoizationDisposition, MemoizationMode
 from reflex.utils import imports, format
 from reflex.vars import BaseVar, VarData
 from reflex.event import EventHandler, EventSpec, EventChain
@@ -46,14 +46,15 @@
             _com = _hd(*args, **kwargs)
             if forced:
                 _com._memoization_mode = memo_always
                 # _com._memoization_mode.recursive = False
             # _sc = StatefulComponent.create(_com)
             # return _sc if _sc is not None else _com
             return _com
+
         return _wrap
 
     if hd is None:
         return _my
     else:
         return _my(hd)
 
@@ -68,15 +69,15 @@
     else:
         return {} if isinstance(com, str) else com._get_all_imports()
 
 
 def get_component_hooks(com) -> Set[str] | Dict[str, None]:
     if version <= '000.004.006':
         return set() if isinstance(com, str) else com.get_hooks()
-    return set() if isinstance(com, str) \
+    return {} if isinstance(com, str) \
         else com._get_all_hooks_internal() | com._get_all_hooks()
 
 
 def get_component_custom_code(com: Component) -> Set[str]:
     if version <= '000.004.006':
         return com.get_custom_code() if isinstance(com, BaseComponent) else set()
     return com._get_all_custom_code() if isinstance(com, BaseComponent) else set()
@@ -163,14 +164,15 @@
         return f'<{self.item.tag}/>'
 
 
 class JsEvent:
     hd: EventHandler
     # event_trigger use for custom trigger, must work with fmt=True
     event_trigger: Callable
+    _item: "ExEventHandlerItem" = None
 
     def __init__(self, hd: Any, js: str = '', fmt: bool = False, event_trigger: Callable = None):
         assert isinstance(hd, EventHandler)
         self.hd = hd
         self.js = js
         self.fmt = fmt
         self.event_trigger = event_trigger
@@ -182,20 +184,27 @@
 
     def get_event_args(self) -> str:
         _args = inspect.getfullargspec(self.hd.fn)
         rs = []
         for idx, _arg in enumerate(_args.args):
             if idx == 0:  # ignore self
                 continue
-            rs.append(f'{_arg}:{self.args[idx-1]}')
+            rs.append(f'{_arg}:{self.args[idx - 1]}')
         return ','.join(rs)
 
     def get_ex_item(self, parent, key) -> ExItem:
-        item = ExEventHandlerItem(self, parent, key=key)
-        return item
+        if self._item is not None:
+            return self._item
+        self._item = ExEventHandlerItem(self, parent, key=key)
+        return self._item
+
+    def to_hook_code(self, name: str) -> str:
+        assert self._item is not None, 'JsEvent to_hook_code depend get_ex_item'
+        code = self._item.serialize()
+        return code.strip('()')
 
 
 js_event = JsEvent
 
 
 class ExEventHandlerItem(ExItem):
     item: JsEvent
@@ -210,27 +219,29 @@
             return self._hd_item
         except AttributeError:
             self._hd_item = ExLambdaHandlerItem(self.item.hd, self.parent, key=self.key)
             self._hd_item.event_trigger = self.item.event_trigger
             return self._hd_item
 
     def _get_fn_name(self) -> str:
-        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}_{id(self)}"
+        if 0:
+            return (f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}"
+                    f"_{id(self)}")
+        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item.hd)}'.encode('utf-8')).hexdigest()}"
 
     def serialize(self) -> str:
         hd_name = self.hd_item.serialize()
         trigger = self.hd_item._get_event_trigger()
         args = inspect.getfullargspec(trigger).args
 
         if not self.item.fmt:
-            return f"""({','.join(args)}) => {{
+            return f"""(({','.join(args)}) => {{
                 {self.item.js}
                 {hd_name}({','.join(args)})
-            }}
-            """
+            }})"""
         else:
             return self.item.js % dict(name=hd_name)
 
     def get_hooks(self) -> Set[str] | Dict[str, None]:
         return self.hd_item.get_hooks()
 
     def get_imports(self) -> imports.ImportDict:
@@ -242,15 +253,18 @@
     event_trigger: Callable = None
 
     @classmethod
     def isinstance(cls, item: Any) -> bool:
         return isinstance(item, Callable)
 
     def _get_fn_name(self) -> str:
-        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}_{id(self)}"
+        if 0:
+            return (f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}"
+                    f"_{id(self)}")
+        return f"{self.key.replace('.', '_')}_{md5(f'{str(self.item)}'.encode('utf-8')).hexdigest()}"
 
     def _get_event_trigger_key(self) -> str:
         return RE_KEY_IDX.sub('.*.', self.key)
 
     def _get_event_trigger(self) -> Callable:
         if self.event_trigger is not None:
             return self.event_trigger
@@ -376,23 +390,27 @@
             imports=self.get_imports(),
             hooks=self.get_hooks(),
         )
 
     def get_custom_components(self) -> set[CustomComponent]:
         return get_component_custom_code(self.value)
 
+    def to_hook_code(self, name: str) -> str:
+        code = self.serialize()
+        return code.strip('()')
+
 
 class JsFunctionValue(JsValue):
     _value: Union[str, Component]
 
     def _init(self, **kwargs) -> None:
         super()._init(**kwargs)
         self._args = inspect.getfullargspec(self.value)
         args = self._args.args
-        self._value = self.value(*args)
+        self._value = self.value(*[CasualVar.create_safe(arg) for arg in args])
 
     def serialize(self) -> str:
         is_component = False
         if isinstance(self._value, str):
             v = self._value
         elif isinstance(self._value, Component):
             is_component = True
@@ -408,14 +426,19 @@
 
     def get_hooks(self) -> Set[str] | Dict[str, None]:
         return get_component_hooks(self._value)
 
     def get_custom_components(self) -> set[CustomComponent]:
         return set() if not isinstance(self._value, CustomComponent) else {self._value}
 
+    def to_hook_code(self, name: str) -> str:
+        code = self.serialize().strip('()')
+        code = f"{name}{code.replace('=>', ' ', 1)}"
+        return code
+
 
 def js_value(value: Union[str, Callable, Component], **kwargs) -> JsValue:
     if isinstance(value, (str, Component)):
         return JsValue(value, **kwargs)
     if isinstance(value, Callable):
         return JsFunctionValue(value, **kwargs)
     raise NotImplemented("Not implemented: %s(%s)" % (type(value), value))
@@ -573,14 +596,65 @@
 @dataclasses.dataclass(
     eq=False,
     **{"slots": True} if sys.version_info >= (3, 10) else {},
 )
 class ExVar(BaseVar):
     _var_value: Any = dataclasses.field(default=Any)
 
+    @classmethod
+    def create(
+            cls, value: Any, _var_is_local: bool = True, _var_is_string: bool = False,
+            _var_data: VarData | None = None,
+    ) -> Var | None:
+        v = BaseVar.create(value, _var_is_local=_var_is_local, _var_is_string=_var_is_string, _var_data=_var_data)
+        return cls(
+            _var_name=v._var_name,
+            _var_type=v._var_type,
+            _var_is_local=v._var_is_local,
+            _var_is_string=v._var_is_string,
+            _var_data=v._var_data,
+        )
+
+    def _replace(self, merge_var_data=None, **kwargs: Any) -> Self:
+        return self.__class__(
+            _var_name=kwargs.pop("_var_name", self._var_name),
+            _var_type=kwargs.pop("_var_type", self._var_type),
+            _var_is_local=kwargs.pop("_var_is_local", self._var_is_local),
+            _var_is_string=kwargs.pop("_var_is_string", self._var_is_string),
+            _var_full_name_needs_state_prefix=kwargs.pop(
+                "_var_full_name_needs_state_prefix",
+                self._var_full_name_needs_state_prefix,
+            ),
+            _var_data=VarData.merge(
+                kwargs.get("_var_data", self._var_data), merge_var_data
+            ),
+        )
+
+
+class CasualVar(ExVar):
+    def __getattribute__(self, name: str) -> Any:
+        try:
+            return super().__getattribute__(name)
+        except (AttributeError, ):
+            if name.startswith("_"):
+                raise
+            return self.create_safe(
+                f'{self._var_name}.{name}'
+            )
+
+    def to_js(self) -> Self:
+        return self._replace(
+            _var_name=f'({self._var_name})'
+        )
+
+    def to_react(self) -> Self:
+        return self._replace(
+            _var_name=f'{{{self._var_name}}}'
+        )
+
 
 class NodeVar(ExVar):
     """
     support:
         . base types: int, float, bool, str
         . js, like: {show ? 11 : 0}
      """
@@ -592,15 +666,16 @@
     **{"slots": True} if sys.version_info >= (3, 10) else {},
 )
 class ContainVar(ExVar):
     _var_fmt: ExFormatter = dataclasses.field(default=None)
 
     @property
     def _var_full_name(self) -> str:
-        return self._var_name
+        """ ContainVar used at Component property """
+        return self._var_fmt.get_value()
 
     @classmethod
     def create(cls, _args_: Any = None, **kwargs) -> Self:
         value = _args_ if _args_ is not None else kwargs
         # v: BaseVar = super().create(_name, _var_is_local=_var_is_local, _var_is_string=_var_is_string)
         return cls(
             _var_name='',
@@ -610,15 +685,14 @@
             _var_data=None,
             _var_value=value,
         )
 
     def init(self, parent: Component, name: str) -> Self:
         fmt = ExFormatter(self._var_value, parent=parent, name=name)
         self._var_fmt = fmt
-        self._var_name = fmt.get_value()
         self._var_data = fmt.get_var_data()
         return self
 
     def get_custom_components(self) -> set[CustomComponent]:
         rs = set()
         for ex in self._var_fmt._coms.values():
             rs |= ex.get_custom_components()
@@ -632,14 +706,42 @@
 
     def get_hooks(self) -> Set[str] | Dict[str, None]:
         return self._var_data.hooks
 
     def get_imports(self) -> imports.ImportDict:
         return self._var_data.imports
 
+    def to_hook_code(self) -> Dict[str, None]:
+        """ ContainVar used at hook code
+        . only support list or dict
+        . list item only support: JsValue, JsFunctionValue
+        """
+        assert isinstance(self._var_value, (list, dict)), 'ContainVar.to_hook_code only supports list'
+        items = self._var_value if isinstance(self._var_value, list) else self._var_value.values()
+        for item in items:
+            assert isinstance(item, (JsValue, JsFunctionValue, JsEvent)), \
+                'ContainVar.to_hook_code list item only support: JsValue, JsFunctionValue'
+
+        def _iter_items():
+            if isinstance(self._var_value, list):
+                for idx, item in enumerate(self._var_value):
+                    yield f'{self._var_fmt.name}_{idx}', item
+            elif isinstance(self._var_value, dict):
+                for k, v in self._var_value.items():
+                    yield f'{self._var_fmt.name}_{k}', v
+
+        hooks: Dict[str, None] = {}
+        for name, ex in _iter_items():
+            if isinstance(ex, JsEvent):
+                ex.get_ex_item(self, name)
+            hook = ex.to_hook_code(name)
+            hooks[hook] = None
+
+        return hooks
+
 
 contain = ContainVar.create
 
 
 def container(data: Union[list, dict], name: str = '') -> rx.Component:
     """ wrap contain to Component, use for:
         .foreach:  rx.foreach(GlobalState.subnav_items, _sub_item)
@@ -665,16 +767,17 @@
             imports=self.get_imports(),
         )
         yield from [v]
 
 
 class AntdBaseComponent(Component):
     _custom_components: Set[CustomComponent] = pydantic.PrivateAttr(default_factory=set)
+    _ex_hooks: List[ContainVar] = pydantic.PrivateAttr(default_factory=list)
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, ex_hooks: List[ContainVar] = None, **kwargs):
         contains = {}
         exs = {}
         kw = {}
         for k, v in kwargs.items():
             if isinstance(v, ContainVar):
                 contains[k] = v
             elif isinstance(v, (JsValue, JsEvent)):
@@ -683,15 +786,15 @@
                 kw[k] = v
         # super().__init__(*args, **kw)
         try:
             super().__init__(*args, **kw)
         except Exception as err:
             print(f"class<{self}>, args={args}, kw={kw}, error: {err}")
             raise
-        self._init_contains(contains, exs)
+        self._init_contains(contains, exs, ex_hooks)
 
     def _get_all_custom_components(
             self, seen: set[str] | None = None
     ) -> Set[CustomComponent]:
         _coms = super()._get_all_custom_components(seen=seen)
         if hasattr(self, '_custom_components') and self._custom_components:
             _coms |= self._custom_components
@@ -707,14 +810,41 @@
         """Get the style for the component.
 
         Returns:
             The dictionary of the component style as value and the style notation as key.
         """
         return {"style": self.style}
 
+    def add_imports(self) -> dict[str, str | ImportVar | list[str | ImportVar]]:
+        _imports = {}
+        if self._ex_hooks:
+            for ex in self._ex_hooks:
+                _imports = imports.merge_imports(
+                    ex.get_imports(),
+                    _imports,
+                )
+        return _imports
+
+    def _get_all_hooks(self) -> dict[str, None]:
+        """ fix 0.5.1 bug #3365 """
+        rs = super()._get_all_hooks()
+        rs = dict((k, None) for k in rs.keys())
+        return rs
+
+    def add_hooks(self) -> list[str]:
+        hooks = []
+        if self._ex_hooks:
+            for ex in self._ex_hooks:
+                hooks.extend(ex.get_hooks().keys())
+                codes = ex.to_hook_code()
+                if codes:
+                    hooks.extend(codes)
+
+        return hooks
+
     def _get_events_hooks(self) -> set[str] | Dict[str, None]:
         _hooks = super()._get_events_hooks()
         js_events: List[BaseVar] = [
             v for k, v in self.event_triggers.items()
             if isinstance(v, BaseVar) and v._var_data is not None and v._var_data.hooks]
 
         if version <= '000.004.006':
@@ -767,15 +897,20 @@
 
     def _iter_contains(self) -> Iterable[Tuple[str, ContainVar]]:
         for k in self.get_fields().keys():
             v = getattr(self, k, None)
             if isinstance(v, ContainVar):
                 yield k, v
 
-    def _init_contains(self, contains: Dict[str, ContainVar], exs: Dict[str, Any]):
+    def _init_contains(self, contains: Dict[str, ContainVar], exs: Dict[str, Any], ex_hooks: List[ContainVar]) -> None:
+        self._ex_hooks = []
+        if ex_hooks:
+            for ex in ex_hooks:
+                self._ex_hooks.append(ex.init(self, ''))
+
         for k, v in contains.items():
             v.init(self, k)
             self._custom_components |= v.get_custom_components()
             setattr(self, k, v)
 
         event_keys = self.get_event_triggers().keys()
         for k, v in exs.items():
@@ -858,8 +993,7 @@
         pass
 
     # StatefulComponent._get_memoized_event_triggers = classmethod(_my_get_memoized_event_triggers)
 
 
 ReactNode = Union[str, Component]
 JsNode = Union[JsValue, JsEvent]
-
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/base.pyi` & `reflex_antd-0.0.9/custom_components/reflex_antd/base.pyi`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/constant.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/constant.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/display.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/display.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/entry.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/entry.py`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd/feedback.py` & `reflex_antd-0.0.9/custom_components/reflex_antd/feedback.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .antd.progress import progress  # noqa
 from .antd.result import result  # noqa
 from .antd.skeleton import skeleton  # noqa
 from .antd.spin import spin  # noqa
 from .antd.watermark import watermark  # noqa
 from .antd.alert import alert, alert_error_boundary  # noqa
 from .antd.drawer import drawer  # noqa
-from .antd.message import message, message_holder  # noqa
+from .antd.message import message, message_holder, messages  # noqa
 from .antd.notification import notification  # noqa
 from .antd.modal import modal, confirm  # noqa
 from .antd.popconfirm import popconfirm  # noqa
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/PKG-INFO` & `reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-Metadata-Version: 2.1
-Name: reflex-antd
-Version: 0.0.8
-Summary: Reflex custom component antd
-Author-email: seewind <seewindcn@gmail.com>
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: homepage, https://github.com/seewindcn/reflex-antd
-Project-URL: source, https://github.com/seewindcn/reflex-antd
-Keywords: reflex,reflex-custom-components,ant-design,antd
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: reflex>=0.4.2
-Provides-Extra: dev
-Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-
-# reflex-antd
-
-A Reflex custom component wrap [ant.design](https://ant.design/).
-pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
-
-## Installation
-
-```bash
-pip install reflex-antd
-```
-
-## antd-demo
-
-[antd-demo](https://antd-demo.reflex.run)
-
-
-### screen
-- table
-![table](docs/img/table1.png)
-- menu
-![menu1](docs/img/menu1.png)
-- transfer
-![transfer1](docs/img/transfer1.png)
-- ...
-
-
-
+Metadata-Version: 2.1
+Name: reflex-antd
+Version: 0.0.9
+Summary: Reflex custom component antd
+Author-email: seewind <seewindcn@gmail.com>
+License: Apache-2.0
+Project-URL: Homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: homepage, https://github.com/seewindcn/reflex-antd
+Project-URL: source, https://github.com/seewindcn/reflex-antd
+Keywords: reflex,reflex-custom-components,ant-design,antd
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: reflex>=0.4.2
+Provides-Extra: dev
+Requires-Dist: build; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+
+# reflex-antd
+
+A Reflex custom component wrap [ant.design](https://ant.design/).
+pypi: [reflex-antd](https://pypi.org/pypi/reflex-antd/)
+
+## Installation
+
+```bash
+pip install reflex-antd
+```
+
+## antd-demo
+
+[antd-demo](https://antd-demo.reflex.run)
+
+
+### screen
+- table
+![table](docs/img/table1.png)
+- menu
+![menu1](docs/img/menu1.png)
+- transfer
+![transfer1](docs/img/transfer1.png)
+- ...
+
+
+
```

### Comparing `reflex_antd-0.0.8/custom_components/reflex_antd.egg-info/SOURCES.txt` & `reflex_antd-0.0.9/custom_components/reflex_antd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reflex_antd-0.0.8/pyproject.toml` & `reflex_antd-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "reflex-antd"
-version = "0.0.8"
+version = "0.0.9"
 description = "Reflex custom component antd"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.8"
 authors = [{ name = "seewind", email = "seewindcn@gmail.com" }]
 keywords = [
     "reflex",
@@ -33,9 +33,10 @@
 source = "https://github.com/seewindcn/reflex-antd"
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 
 
+
 [tool.setuptools.packages.find]
 where = ["custom_components"]
```

