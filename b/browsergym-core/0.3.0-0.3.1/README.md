# Comparing `tmp/browsergym_core-0.3.0.tar.gz` & `tmp/browsergym_core-0.3.1.tar.gz`

## Comparing `browsergym_core-0.3.0.tar` & `browsergym_core-0.3.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/requirements.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/__init__.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/constants.py
--rw-r--r--   0        0        0    21281 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/env.py
--rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/observation.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/registration.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/spaces.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/__init__.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/base.py
--rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/functions.py
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/highlevel.py
--rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/parsers.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/python.py
--rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/action/utils.py
--rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/chat_files/assistant.png
--rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/chat_files/chatbox.html
--rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/chat_files/chatbox_modern.html
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/chat_files/img/send.svg
--rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/javascript/frame_mark_elements.js
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/core/javascript/frame_unmark_elements.js
--rw-r--r--   0        0        0    18836 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/src/browsergym/utils/obs.py
--rw-r--r--   0        0        0    39837 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/test_actions_highlevel.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/test_actions_python.py
--rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/test_gym_envs.py
--rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/test_observation.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/utils.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/example.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/hover.html
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/long_page.html
--rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/screenshot.png
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/test_page.html
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/test_page_2.html
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/textbox.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/basic_iframe.html
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/inner-iframe.html
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/outer-iframe.html
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/button_input.html
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/checkbox_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/color_picker_input.html
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/date_input.html
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/date_min_max_input.html
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/date_time_local_input.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/email_input.html
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/file_input.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/hidden_field_input.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/image_input.html
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/img_submit.gif
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/number_input.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/number_step_input.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/password_input.html
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/radio_input.html
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/range_input.html
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/reset_input.html
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/search_input.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/submit_input.html
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/submit_nn_input.html
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/telephone_input.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/text_input.html
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/time_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/url_input.html
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/tests/data/input_type/week_input.html
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/.gitignore
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/requirements.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/__init__.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/constants.py
+-rw-r--r--   0        0        0    21281 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/env.py
+-rw-r--r--   0        0        0    20773 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/observation.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/registration.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/spaces.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/base.py
+-rw-r--r--   0        0        0    17851 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/functions.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/highlevel.py
+-rw-r--r--   0        0        0     3596 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/parsers.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/python.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/action/utils.py
+-rw-r--r--   0        0        0   133496 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/chat_files/assistant.png
+-rw-r--r--   0        0        0     6687 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/chat_files/chatbox.html
+-rw-r--r--   0        0        0    10919 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/chat_files/chatbox_modern.html
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/chat_files/img/send.svg
+-rw-r--r--   0        0        0    11891 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/javascript/frame_mark_elements.js
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/core/javascript/frame_unmark_elements.js
+-rw-r--r--   0        0        0    18836 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/src/browsergym/utils/obs.py
+-rw-r--r--   0        0        0    39837 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/test_actions_highlevel.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/test_actions_python.py
+-rw-r--r--   0        0        0     8715 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/test_gym_envs.py
+-rw-r--r--   0        0        0    23345 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/test_observation.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/utils.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/example.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/hover.html
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/long_page.html
+-rw-r--r--   0        0        0    26054 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/screenshot.png
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/test_page.html
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/test_page_2.html
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/textbox.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_dom_site/basic_shadow_dom.html
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_dom_site/simple_shadow_dom.html
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/basic_iframe.html
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/basic_iframe_2.html
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/inner-iframe.html
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/outer-iframe.html
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/button_input.html
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/checkbox_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/color_picker_input.html
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/date_input.html
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/date_min_max_input.html
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/date_time_local_input.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/email_input.html
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/file_input.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/hidden_field_input.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/image_input.html
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/img_submit.gif
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/number_input.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/number_step_input.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/password_input.html
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/radio_input.html
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/range_input.html
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/reset_input.html
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/search_input.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/submit_input.html
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/submit_nn_input.html
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/telephone_input.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/text_input.html
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/time_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/url_input.html
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/tests/data/input_type/week_input.html
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/.gitignore
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 browsergym_core-0.3.1/PKG-INFO
```

### Comparing `browsergym_core-0.3.0/src/browsergym/core/__init__.py` & `browsergym_core-0.3.1/src/browsergym/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 import playwright.sync_api
 
 # we use a global playwright instance
 _PLAYWRIGHT = None
```

### Comparing `browsergym_core-0.3.0/src/browsergym/core/chat.py` & `browsergym_core-0.3.1/src/browsergym/core/chat.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/env.py` & `browsergym_core-0.3.1/src/browsergym/core/env.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/observation.py` & `browsergym_core-0.3.1/src/browsergym/core/observation.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/registration.py` & `browsergym_core-0.3.1/src/browsergym/core/registration.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/spaces.py` & `browsergym_core-0.3.1/src/browsergym/core/spaces.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/task.py` & `browsergym_core-0.3.1/src/browsergym/core/task.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/base.py` & `browsergym_core-0.3.1/src/browsergym/core/action/base.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/functions.py` & `browsergym_core-0.3.1/src/browsergym/core/action/functions.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/highlevel.py` & `browsergym_core-0.3.1/src/browsergym/core/action/highlevel.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/parsers.py` & `browsergym_core-0.3.1/src/browsergym/core/action/parsers.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/python.py` & `browsergym_core-0.3.1/src/browsergym/core/action/python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/action/utils.py` & `browsergym_core-0.3.1/src/browsergym/core/action/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/chat_files/assistant.png` & `browsergym_core-0.3.1/src/browsergym/core/chat_files/assistant.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/chat_files/chatbox.html` & `browsergym_core-0.3.1/src/browsergym/core/chat_files/chatbox.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/chat_files/chatbox_modern.html` & `browsergym_core-0.3.1/src/browsergym/core/chat_files/chatbox_modern.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/chat_files/img/send.svg` & `browsergym_core-0.3.1/src/browsergym/core/chat_files/img/send.svg`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/javascript/frame_mark_elements.js` & `browsergym_core-0.3.1/src/browsergym/core/javascript/frame_mark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/core/javascript/frame_unmark_elements.js` & `browsergym_core-0.3.1/src/browsergym/core/javascript/frame_unmark_elements.js`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/src/browsergym/utils/obs.py` & `browsergym_core-0.3.1/src/browsergym/utils/obs.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/test_actions_highlevel.py` & `browsergym_core-0.3.1/tests/test_actions_highlevel.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/test_actions_python.py` & `browsergym_core-0.3.1/tests/test_actions_python.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/test_gym_envs.py` & `browsergym_core-0.3.1/tests/test_gym_envs.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/test_observation.py` & `browsergym_core-0.3.1/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/utils.py` & `browsergym_core-0.3.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/example.html` & `browsergym_core-0.3.1/tests/data/example.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/long_page.html` & `browsergym_core-0.3.1/tests/data/long_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/screenshot.png` & `browsergym_core-0.3.1/tests/data/screenshot.png`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/test_page.html` & `browsergym_core-0.3.1/tests/data/test_page.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/test_page_2.html` & `browsergym_core-0.3.1/tests/data/test_page_2.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_iframe_site/basic_iframe.html` & `browsergym_core-0.3.1/tests/data/basic_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_iframe_site/inner-iframe.html` & `browsergym_core-0.3.1/tests/data/basic_iframe_site/inner-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_iframe_site/outer-iframe.html` & `browsergym_core-0.3.1/tests/data/basic_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_shadow_dom_site/basic_shadow_dom.html` & `browsergym_core-0.3.1/tests/data/basic_shadow_dom_site/basic_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_shadow_dom_site/simple_shadow_dom.html` & `browsergym_core-0.3.1/tests/data/basic_shadow_dom_site/simple_shadow_dom.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/basic_iframe.html` & `browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/basic_iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/basic_shadow_iframe_site/outer-iframe.html` & `browsergym_core-0.3.1/tests/data/basic_shadow_iframe_site/outer-iframe.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/checkbox_input.html` & `browsergym_core-0.3.1/tests/data/input_type/checkbox_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/color_picker_input.html` & `browsergym_core-0.3.1/tests/data/input_type/color_picker_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/date_min_max_input.html` & `browsergym_core-0.3.1/tests/data/input_type/date_min_max_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/date_time_local_input.html` & `browsergym_core-0.3.1/tests/data/input_type/date_time_local_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/image_input.html` & `browsergym_core-0.3.1/tests/data/input_type/image_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/img_submit.gif` & `browsergym_core-0.3.1/tests/data/input_type/img_submit.gif`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/password_input.html` & `browsergym_core-0.3.1/tests/data/input_type/password_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/reset_input.html` & `browsergym_core-0.3.1/tests/data/input_type/reset_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/submit_input.html` & `browsergym_core-0.3.1/tests/data/input_type/submit_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/telephone_input.html` & `browsergym_core-0.3.1/tests/data/input_type/telephone_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/text_input.html` & `browsergym_core-0.3.1/tests/data/input_type/text_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/tests/data/input_type/time_input.html` & `browsergym_core-0.3.1/tests/data/input_type/time_input.html`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/pyproject.toml` & `browsergym_core-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `browsergym_core-0.3.0/PKG-INFO` & `browsergym_core-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: browsergym-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: BrowserGym: a gym environment for web task automation in the Chromium browser
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Léo Boisvert, Massimo Caccia, Alex Drouin, Maxime Gasse, Alex Lacoste, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

