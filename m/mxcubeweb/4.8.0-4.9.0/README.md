# Comparing `tmp/mxcubeweb-4.8.0.tar.gz` & `tmp/mxcubeweb-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcubeweb-4.8.0.tar", max compression
+gzip compressed data, was "mxcubeweb-4.9.0.tar", max compression
```

## Comparing `mxcubeweb-4.8.0.tar` & `mxcubeweb-4.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     7652 2023-11-29 09:08:03.189871 mxcubeweb-4.8.0/LICENSE
--rw-r--r--   0        0        0     9865 2023-11-29 09:08:03.189871 mxcubeweb-4.8.0/README.md
--rw-r--r--   0        0        0     4162 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/__init__.py
--rw-r--r--   0        0        0     1183 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/__version__.py
--rw-r--r--   0        0        0    19650 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/app.py
--rw-r--r--   0        0        0     1401 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/config.py
--rw-r--r--   0        0        0        0 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/__init__.py
--rw-r--r--   0        0        0        0 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/__init__.py
--rw-r--r--   0        0        0     2416 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/actuator_adapter.py
--rw-r--r--   0        0        0    13711 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/adapter_base.py
--rw-r--r--   0        0        0     1971 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/beam_adapter.py
--rw-r--r--   0        0        0     1646 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/beamline_action_adapter.py
--rw-r--r--   0        0        0     3451 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/beamline_adapter.py
--rw-r--r--   0        0        0     1595 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/data_publisher_adapter.py
--rw-r--r--   0        0        0      503 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/detector_adapter.py
--rw-r--r--   0        0        0     1288 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/diffractometer_adapter.py
--rw-r--r--   0        0        0      595 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/energy_adapter.py
--rw-r--r--   0        0        0     1388 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/flux_adapter.py
--rw-r--r--   0        0        0     1968 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/machine_info_adapter.py
--rw-r--r--   0        0        0     2224 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/motor_adapter.py
--rw-r--r--   0        0        0     1767 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/nstate_adapter.py
--rw-r--r--   0        0        0     2939 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/adapter/wavelength_adapter.py
--rw-r--r--   0        0        0    12203 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/beamline.py
--rw-r--r--   0        0        0     1434 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/chat.py
--rw-r--r--   0        0        0      632 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/component_base.py
--rw-r--r--   0        0        0    16437 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/lims.py
--rw-r--r--   0        0        0    91921 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/queue.py
--rw-r--r--   0        0        0    19688 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/samplechanger.py
--rw-r--r--   0        0        0    22046 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/sampleview.py
--rw-r--r--   0        0        0     2094 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/user/database.py
--rw-r--r--   0        0        0      420 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/user/dummyusermanager.py
--rw-r--r--   0        0        0    15234 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/user/usermanager.py
--rw-r--r--   0        0        0     2067 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/components/workflow.py
--rw-r--r--   0        0        0     2529 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/models/adaptermodels.py
--rw-r--r--   0        0        0     4112 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/models/configmodels.py
--rw-r--r--   0        0        0      997 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/models/generic.py
--rw-r--r--   0        0        0     3409 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/models/usermodels.py
--rw-r--r--   0        0        0     2436 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/util/adapterutils.py
--rw-r--r--   0        0        0     1725 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/util/convertutils.py
--rw-r--r--   0        0        0      523 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/util/fsutils.py
--rw-r--r--   0        0        0     4675 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/core/util/networkutils.py
--rw-r--r--   0        0        0     1188 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/logging_handler.py
--rw-r--r--   0        0        0        0 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/__init__.py
--rw-r--r--   0        0        0     8545 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/beamline.py
--rw-r--r--   0        0        0      897 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/detector.py
--rw-r--r--   0        0        0     4102 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/diffractometer.py
--rw-r--r--   0        0        0     5313 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/lims.py
--rw-r--r--   0        0        0     1225 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/log.py
--rw-r--r--   0        0        0     3442 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/login.py
--rw-r--r--   0        0        0     2818 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/main.py
--rw-r--r--   0        0        0     4295 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/mockups.py
--rw-r--r--   0        0        0    11440 2023-11-29 09:08:03.193871 mxcubeweb-4.8.0/mxcubeweb/routes/queue.py
--rw-r--r--   0        0        0     6611 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/routes/ra.py
--rw-r--r--   0        0        0    13826 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/routes/samplecentring.py
--rw-r--r--   0        0        0     5088 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/routes/samplechanger.py
--rw-r--r--   0        0        0    21073 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/routes/signals.py
--rw-r--r--   0        0        0     1138 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/routes/workflow.py
--rw-r--r--   0        0        0     7663 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/server.py
--rw-r--r--   0        0        0     1442 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/state_storage.py
--rw-r--r--   0        0        0      771 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/templates/characterisation-results.js
--rw-r--r--   0        0        0     3610 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/templates/data-collection-results.html
--rw-r--r--   0        0        0   329138 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/templates/precompiled.templates.min.js
--rw-r--r--   0        0        0      721 2023-11-29 09:08:03.197871 mxcubeweb-4.8.0/mxcubeweb/templates/workflow-results.js
--rw-r--r--   0        0        0     1864 2023-11-29 09:08:13.297876 mxcubeweb-4.8.0/pyproject.toml
--rw-r--r--   0        0        0    11792 1970-01-01 00:00:00.000000 mxcubeweb-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/LICENSE
+-rw-r--r--   0        0        0     9865 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/README.md
+-rw-r--r--   0        0        0     4162 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/__init__.py
+-rw-r--r--   0        0        0     1183 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/__version__.py
+-rw-r--r--   0        0        0    19650 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/app.py
+-rw-r--r--   0        0        0     1401 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/config.py
+-rw-r--r--   0        0        0        0 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2416 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/actuator_adapter.py
+-rw-r--r--   0        0        0    13711 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/adapter_base.py
+-rw-r--r--   0        0        0     1971 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/beam_adapter.py
+-rw-r--r--   0        0        0     1646 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/beamline_action_adapter.py
+-rw-r--r--   0        0        0     3451 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/beamline_adapter.py
+-rw-r--r--   0        0        0     1595 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/data_publisher_adapter.py
+-rw-r--r--   0        0        0      503 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/detector_adapter.py
+-rw-r--r--   0        0        0     1288 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/diffractometer_adapter.py
+-rw-r--r--   0        0        0      595 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/energy_adapter.py
+-rw-r--r--   0        0        0     1388 2023-11-30 11:09:28.320936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/flux_adapter.py
+-rw-r--r--   0        0        0     1968 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/machine_info_adapter.py
+-rw-r--r--   0        0        0     2224 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/motor_adapter.py
+-rw-r--r--   0        0        0     1767 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/nstate_adapter.py
+-rw-r--r--   0        0        0     2939 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/adapter/wavelength_adapter.py
+-rw-r--r--   0        0        0    12203 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/beamline.py
+-rw-r--r--   0        0        0     1434 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/chat.py
+-rw-r--r--   0        0        0      632 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/component_base.py
+-rw-r--r--   0        0        0    16437 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/lims.py
+-rw-r--r--   0        0        0    91921 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/queue.py
+-rw-r--r--   0        0        0    19688 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/samplechanger.py
+-rw-r--r--   0        0        0    22046 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/sampleview.py
+-rw-r--r--   0        0        0     2094 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/user/database.py
+-rw-r--r--   0        0        0      420 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/user/dummyusermanager.py
+-rw-r--r--   0        0        0    15234 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/user/usermanager.py
+-rw-r--r--   0        0        0     2067 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/components/workflow.py
+-rw-r--r--   0        0        0     2529 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/models/adaptermodels.py
+-rw-r--r--   0        0        0     4112 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/models/configmodels.py
+-rw-r--r--   0        0        0      997 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/models/generic.py
+-rw-r--r--   0        0        0     3409 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/models/usermodels.py
+-rw-r--r--   0        0        0     2436 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/util/adapterutils.py
+-rw-r--r--   0        0        0     1725 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/util/convertutils.py
+-rw-r--r--   0        0        0      523 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/util/fsutils.py
+-rw-r--r--   0        0        0     4675 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/core/util/networkutils.py
+-rw-r--r--   0        0        0     1188 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/logging_handler.py
+-rw-r--r--   0        0        0        0 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/__init__.py
+-rw-r--r--   0        0        0     8545 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/beamline.py
+-rw-r--r--   0        0        0      897 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/detector.py
+-rw-r--r--   0        0        0     4102 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/diffractometer.py
+-rw-r--r--   0        0        0     5313 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/lims.py
+-rw-r--r--   0        0        0     1225 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/log.py
+-rw-r--r--   0        0        0     3442 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/login.py
+-rw-r--r--   0        0        0     2818 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/main.py
+-rw-r--r--   0        0        0     4295 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/mockups.py
+-rw-r--r--   0        0        0    11440 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/queue.py
+-rw-r--r--   0        0        0     6611 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/ra.py
+-rw-r--r--   0        0        0    13826 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/samplecentring.py
+-rw-r--r--   0        0        0     5088 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/samplechanger.py
+-rw-r--r--   0        0        0    21073 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/signals.py
+-rw-r--r--   0        0        0     1138 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/routes/workflow.py
+-rw-r--r--   0        0        0     7663 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/server.py
+-rw-r--r--   0        0        0     1442 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/state_storage.py
+-rw-r--r--   0        0        0      771 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/templates/characterisation-results.js
+-rw-r--r--   0        0        0     3610 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/templates/data-collection-results.html
+-rw-r--r--   0        0        0   329138 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/templates/precompiled.templates.min.js
+-rw-r--r--   0        0        0      721 2023-11-30 11:09:28.324936 mxcubeweb-4.9.0/mxcubeweb/templates/workflow-results.js
+-rw-r--r--   0        0        0     1864 2023-11-30 11:09:47.577102 mxcubeweb-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11792 1970-01-01 00:00:00.000000 mxcubeweb-4.9.0/PKG-INFO
```

### Comparing `mxcubeweb-4.8.0/LICENSE` & `mxcubeweb-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/README.md` & `mxcubeweb-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/__init__.py` & `mxcubeweb-4.9.0/mxcubeweb/__init__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/__version__.py` & `mxcubeweb-4.9.0/mxcubeweb/__version__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/app.py` & `mxcubeweb-4.9.0/mxcubeweb/app.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/config.py` & `mxcubeweb-4.9.0/mxcubeweb/config.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/actuator_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/actuator_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/adapter_base.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/beam_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/beam_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/beamline_action_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/beamline_action_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/beamline_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/beamline_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/data_publisher_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/data_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/diffractometer_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/diffractometer_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/energy_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/energy_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/flux_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/flux_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/machine_info_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/machine_info_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/motor_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/motor_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/nstate_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/nstate_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/adapter/wavelength_adapter.py` & `mxcubeweb-4.9.0/mxcubeweb/core/adapter/wavelength_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/beamline.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/chat.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/chat.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/component_base.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/component_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/lims.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/queue.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/samplechanger.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/sampleview.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/sampleview.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/user/database.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/user/database.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/user/usermanager.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/user/usermanager.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/components/workflow.py` & `mxcubeweb-4.9.0/mxcubeweb/core/components/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/models/adaptermodels.py` & `mxcubeweb-4.9.0/mxcubeweb/core/models/adaptermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/models/configmodels.py` & `mxcubeweb-4.9.0/mxcubeweb/core/models/configmodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/models/generic.py` & `mxcubeweb-4.9.0/mxcubeweb/core/models/generic.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/models/usermodels.py` & `mxcubeweb-4.9.0/mxcubeweb/core/models/usermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/util/adapterutils.py` & `mxcubeweb-4.9.0/mxcubeweb/core/util/adapterutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/util/convertutils.py` & `mxcubeweb-4.9.0/mxcubeweb/core/util/convertutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/util/fsutils.py` & `mxcubeweb-4.9.0/mxcubeweb/core/util/fsutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/core/util/networkutils.py` & `mxcubeweb-4.9.0/mxcubeweb/core/util/networkutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/logging_handler.py` & `mxcubeweb-4.9.0/mxcubeweb/logging_handler.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/beamline.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/detector.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/detector.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/diffractometer.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/diffractometer.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/lims.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/log.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/log.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/login.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/login.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/main.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/main.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/mockups.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/mockups.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/queue.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/ra.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/ra.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/samplecentring.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/samplecentring.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/samplechanger.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/signals.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/signals.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/routes/workflow.py` & `mxcubeweb-4.9.0/mxcubeweb/routes/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/server.py` & `mxcubeweb-4.9.0/mxcubeweb/server.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/state_storage.py` & `mxcubeweb-4.9.0/mxcubeweb/state_storage.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/templates/characterisation-results.js` & `mxcubeweb-4.9.0/mxcubeweb/templates/characterisation-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/templates/data-collection-results.html` & `mxcubeweb-4.9.0/mxcubeweb/templates/data-collection-results.html`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/templates/precompiled.templates.min.js` & `mxcubeweb-4.9.0/mxcubeweb/templates/precompiled.templates.min.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/mxcubeweb/templates/workflow-results.js` & `mxcubeweb-4.9.0/mxcubeweb/templates/workflow-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-4.8.0/pyproject.toml` & `mxcubeweb-4.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcubeweb"
-version = "4.8.0"
+version = "4.9.0"
 license = "LGPL-3.0-or-later"
 description = "MXCuBE Web user interface"
 authors = ["The MXCuBE collaboration <mxcube@esrf.fr>"]
 maintainers = [
     "MXCuBE collaboration <mxcube@esrf.fr>",
 ]
 readme = "README.md"
```

### Comparing `mxcubeweb-4.8.0/PKG-INFO` & `mxcubeweb-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcubeweb
-Version: 4.8.0
+Version: 4.9.0
 Summary: MXCuBE Web user interface
 Home-page: http://github.com/mxcube/mxcubeweb
 License: LGPL-3.0-or-later
 Keywords: mxcube,mxcube3,mxcubeweb
 Author: The MXCuBE collaboration
 Author-email: mxcube@esrf.fr
 Maintainer: MXCuBE collaboration
```

