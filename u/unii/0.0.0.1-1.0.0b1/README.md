# Comparing `tmp/unii-0.0.0.1.tar.gz` & `tmp/unii-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unii-0.0.0.1.tar", last modified: Thu Apr 25 12:10:17 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `unii-0.0.0.1.tar` & `unii-1.0.0b1.tar`

### file list

```diff
@@ -1,35 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:10:17.119844 unii-0.0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 12:10:07.000000 unii-0.0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 12:10:07.000000 unii-0.0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 12:10:17.119844 unii-0.0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-25 12:10:07.000000 unii-0.0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-25 12:10:07.000000 unii-0.0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 12:10:17.119844 unii-0.0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:10:17.115844 unii-0.0.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_auto_reconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_command_data_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_connect_encrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_connect_unencrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_device_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_equipment_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_message_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_message_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-25 12:10:07.000000 unii-0.0.0.1/test/test_unii_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:10:17.119844 unii-0.0.0.1/unii/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/sia_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/unii.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/unii_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/unii_command_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/unii_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12141 2024-04-25 12:10:07.000000 unii-0.0.0.1/unii/unii_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 12:10:17.119844 unii-0.0.0.1/unii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-25 12:10:17.000000 unii-0.0.0.1/unii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-25 12:10:17.000000 unii-0.0.0.1/unii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 12:10:17.000000 unii-0.0.0.1/unii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-25 12:10:17.000000 unii-0.0.0.1/unii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 12:10:17.000000 unii-0.0.0.1/unii.egg-info/top_level.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 unii-1.0.0b1/MANIFEST.in
+-rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 unii-1.0.0b1/logo.png
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 unii-1.0.0b1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/settings.json
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_auto_reconnect.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_command_data_helpers.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_connect_encrypted.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_connect_unencrypted.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_device_status.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_equipment_information.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_inputs.py
+-rw-r--r--   0        0        0    13286 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message_checksum.py
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_message_encryption.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_outputs.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 unii-1.0.0b1/tests/test_unii_sections.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/__init__.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/__main__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/py.typed
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/sia_code.py
+-rw-r--r--   0        0        0    18630 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_command.py
+-rw-r--r--   0        0        0    25805 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_command_data.py
+-rw-r--r--   0        0        0    10633 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_connection.py
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 unii-1.0.0b1/unii/unii_message.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 unii-1.0.0b1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 unii-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 unii-1.0.0b1/README.md
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 unii-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 unii-1.0.0b1/PKG-INFO
```

### Comparing `unii-0.0.0.1/LICENSE` & `unii-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/pyproject.toml` & `unii-1.0.0b1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,61 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling>=1.24", "hatch-vcs"]
+build-backend = "hatchling.build"
+
+[tool.hatch.build.hooks.vcs]
+version-file = "unii/_version.py"
+
+[tool.hatch.version]
+source = "vcs"
 
 [project]
 name = "unii"
-version = "0.0.0.1"
+dynamic = ["version"]
 license = {text = "Apache-2.0"}
 authors = [
-    { name="Rogier van Staveren" }
+    { name="Rogier van Staveren", email="rogier@batoid.com" }
 ]
 description = "Library to interface with Alphatronics UNii security systems."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
-    "Operating System :: OS Independent",
+    "Operating System :: POSIX",
+    "Operating System :: MacOS :: MacOS X",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Development Status :: 4 - Beta",
+    "Topic :: Security"
 ]
 dependencies = [
-	"pycryptodome>=3.6.6"
+	"pycryptodome>=3.6.6",
+	"semver>=3.0.2"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/unii-security/py-unii"
-"Bug Tracker" = "https://github.com/unii-security/py-unii/issues"
-
-[tool.black]
-target-version = ["py39", "py310"]
-exclude = 'generated'
+Homepage = "https://unii-security.com/"
+Repository = "https://github.com/unii-security/py-unii"
+Issues = "https://github.com/unii-security/py-unii/issues"
 
 [tool.isort]
 # https://github.com/PyCQA/isort/wiki/isort-Settings
 profile = "black"
+skip = "unii/_version.py"
+
+[tool.black]
+exclude = 'unii/_version.py'
+
+[tool.pylint]
+ignore = "_version.py"
+recursive = "y"
+
+[tool.mypy]
+python_version = "3.11"
+mypy_path = "unii"
+
+[[tool.mypy.overrides]]
+module = ["*._version"]
+ignore_missing_imports = true
```

### Comparing `unii-0.0.0.1/test/test_unii_auto_reconnect.py` & `unii-1.0.0b1/tests/test_unii_auto_reconnect.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_command_data_helpers.py` & `unii-1.0.0b1/tests/test_unii_command_data_helpers.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_connect_encrypted.py` & `unii-1.0.0b1/tests/test_unii_connect_encrypted.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_connect_unencrypted.py` & `unii-1.0.0b1/tests/test_unii_connect_unencrypted.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_device_status.py` & `unii-1.0.0b1/tests/test_unii_device_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             self._unii = UNiiLocal(host, port, shared_key)
 
     @async_test
     async def test_device_status(self):
         """
         Test connecting to Alphatronics UNii.
         """
+        await asyncio.sleep(1)
         try:
             result = await self._unii.connect()
             self.assertTrue(result, "Failed to connect to UNii")
             self.assertIsNotNone(self._unii.device_status, "Device Status not set")
             _LOGGER.debug(self._unii.device_status)
             self.assertEqual(len(self._unii.device_status.io_devices), 15)
             self.assertEqual(len(self._unii.device_status.keyboard_devices), 16)
```

### Comparing `unii-0.0.0.1/test/test_unii_equipment_information.py` & `unii-1.0.0b1/tests/test_unii_equipment_information.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             self._unii = UNiiLocal(host, port, shared_key)
 
     @async_test
     async def test_equipment_information(self):
         """
         Test connecting to Alphatronics UNii.
         """
+        await asyncio.sleep(1)
         try:
             result = await self._unii.connect()
             self.assertTrue(result, "Failed to connect to UNii")
             self.assertIsNotNone(self._unii.equipment_information)
             _LOGGER.debug(self._unii.equipment_information)
             self.assertEqual(
                 self._unii.equipment_information.device_name,
```

### Comparing `unii-0.0.0.1/test/test_unii_inputs.py` & `unii-1.0.0b1/tests/test_unii_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             self._unii = UNiiLocal(host, port, shared_key)
 
     @async_test
     async def test_inputs(self):
         """
         Test connecting to Alphatronics UNii.
         """
+        await asyncio.sleep(1)
         try:
             result = await self._unii.connect()
             self.assertTrue(result, "Failed to connect to UNii")
             self.assertIsNotNone(self._unii.inputs, "Input Status not set")
             for _, unii_input in self._unii.inputs.items():
                 if unii_input.status != UNiiInputState.DISABLED:
                     _LOGGER.info(unii_input)
```

### Comparing `unii-0.0.0.1/test/test_unii_message.py` & `unii-1.0.0b1/tests/test_unii_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         _LOGGER.debug(message)
         self.assertEqual(message.session_id, 0xED6C)
         self.assertEqual(message.tx_sequence, 0x37C13CFB)
         self.assertEqual(message.rx_sequence, 0x0000A9C9)
         self.assertEqual(message.command, UNiiCommand.EVENT_OCCURRED)
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data.event_description, "Sabotage schakelaar alarm")
-        self.assertEqual(message.data.device_id, 5016)
+        self.assertEqual(message.data.device_number, 5016)
         self.assertEqual(message.data.device_name, "UNii keypad 1")
         self.assertEqual(message.data.sia_code, SIACode.TAMPER)
 
     def test_encrypted_event_occurred_4(self):
         # pylint: disable=line-too-long
         message = UNiiResponseMessage(
             bytes.fromhex(
@@ -136,15 +136,15 @@
         _LOGGER.debug(message)
         self.assertEqual(message.session_id, 0xBDC5)
         self.assertEqual(message.tx_sequence, 0x7B6ED1F9)
         self.assertEqual(message.rx_sequence, 0x00003874)
         self.assertEqual(message.command, UNiiCommand.EVENT_OCCURRED)
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data.event_description, "Sabotage schakelaar herstel")
-        self.assertEqual(message.data.device_id, 5016)
+        self.assertEqual(message.data.device_number, 5016)
         self.assertEqual(message.data.device_name, "UNii keypad 1")
         self.assertEqual(message.data.sia_code, SIACode.TAMPER_RESTORAL)
 
     def test_encrypted_event_occurred_5(self):
         # pylint: disable=line-too-long
         message = UNiiResponseMessage(
             bytes.fromhex(
@@ -155,15 +155,15 @@
         _LOGGER.debug(message)
         self.assertEqual(message.session_id, 0xED6C)
         self.assertEqual(message.tx_sequence, 0x37C13CFB)
         self.assertEqual(message.rx_sequence, 0x0000A9CA)
         self.assertEqual(message.command, UNiiCommand.EVENT_OCCURRED)
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data.event_description, "Communicatie fout")
-        self.assertEqual(message.data.device_id, 5016)
+        self.assertEqual(message.data.device_number, 5016)
         self.assertEqual(message.data.device_name, "UNii keypad 1")
         self.assertEqual(message.data.sia_code, SIACode.TAMPER)
 
     def test_encrypted_event_occurred_6(self):
         # pylint: disable=line-too-long
         message = UNiiResponseMessage(
             bytes.fromhex(
@@ -174,15 +174,15 @@
         _LOGGER.debug(message)
         self.assertEqual(message.session_id, 0xBDC5)
         self.assertEqual(message.tx_sequence, 0x7B6ED1F9)
         self.assertEqual(message.rx_sequence, 0x00003873)
         self.assertEqual(message.command, UNiiCommand.EVENT_OCCURRED)
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data.event_description, "Communicatie herstel")
-        self.assertEqual(message.data.device_id, 5016)
+        self.assertEqual(message.data.device_number, 5016)
         self.assertEqual(message.data.device_name, "UNii keypad 1")
         self.assertEqual(message.data.sia_code, SIACode.TAMPER_RESTORAL)
 
     def test_encrypted_event_occurred_7(self):
         # pylint: disable=line-too-long
         message = UNiiResponseMessage(
             bytes.fromhex(
@@ -193,15 +193,15 @@
         _LOGGER.debug(message)
         self.assertEqual(message.session_id, 0xBDC5)
         self.assertEqual(message.tx_sequence, 0x7B6ED1F9)
         self.assertEqual(message.rx_sequence, 0x0000386B)
         self.assertEqual(message.command, UNiiCommand.EVENT_OCCURRED)
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data.event_description, "Config gewijzigd op afstand")
-        self.assertEqual(message.data.device_id, 5000)
+        self.assertEqual(message.data.device_number, 5000)
         self.assertEqual(message.data.device_name, "UNii centrale")
         self.assertEqual(message.data.sia_code, SIACode.REMOTE_PROGRAM_SUCCESS)
 
     def test_section_arrangement(self):
         # pylint: disable=line-too-long
         message = UNiiResponseMessage(
             bytes.fromhex(
@@ -216,11 +216,42 @@
         self.assertEqual(
             message.command, UNiiCommand.RESPONSE_REQUEST_SECTION_ARRANGEMENT
         )
         self.assertIsNotNone(message.data)
         self.assertEqual(message.data[1].active, True)
         self.assertEqual(message.data[1].name, "Sectie 1")
 
+    def test_response_request_input_arrangement(self):
+        """
+        Test special characters in input name.
+        """
+        # pylint: disable=line-too-long
+        message = UNiiResponseMessage(
+            bytes.fromhex(
+                "3fe151586c9f00007b21050202085a28f03ab0176ace4a6ad46d78ffdfbe3fbb787deb4900641c76fdac26b8dc05f8caadd668b29039a76e284e87d949ce0fa53e899b06ad0aaf66605129521d82c141c67091fb0f48c3cadebc960313ece81fef4772c810d42f7f6d092ffcf04f842ce01f7acb1f3fa529eafc1ec2e1f6502667ea35396df1bfdda867fabe17f6c46cc120e251112c50cbefb33ecd1aa64923116b4eedda480f2120ea8c65d98b68131694c1dffd0060b9ab7845036352a184ec617aa35036e3ef4d0fef1db6710e8322b00b1a90fc576b4c904ac1b9e4e5821df26ab6e6b5c879047a24eeaf12a77acedceaa7d27531572d4fa7d81363795610df521ec62082f78fb77f453978e08d4ee85a9d1528fd79960a600e869f2c041474fdb77ec05dbd207ad73782df904c6c52a03101dbf22117d283936f07dc806090c5e7a1b9e64850a663a5a0585a473ccda610bd09b3dcc5727de5c708cc8166a0b39c89dd578ed88a3393c516bf9ff12c7c8fedab05ce47584dee193e15cb7bac2b31ed7e9c2b9e24cb11c3613b82a191ebf8666c15fd9e947612cc7e09e1abedeaa7fa8b7e56412798c97c3266b2cdebf9808fe65fe58abeca61479cf6bc62ac76e54dee5a9773d128798960352b5cc5fd7dbed0502a852f7576dc6172dcb54a2cb40a65b28c79fbb5c81a255c32f5305e3934b9925a99a584b087bd0c3d60e51eee79541695"
+            ),
+            bytes.fromhex("30313233343536373839616263646566"),
+        )
+        _LOGGER.debug(message)
+        self.assertEqual(message.session_id, 0x3FE1)
+        self.assertEqual(message.tx_sequence, 0x51586C9F)
+        self.assertEqual(message.rx_sequence, 0x00007B21)
+        self.assertEqual(
+            message.command, UNiiCommand.RESPONSE_REQUEST_INPUT_ARRANGEMENT
+        )
+        self.assertIsNotNone(message.data)
+        self.assertEqual(message.data[1].name, "Ingang 1 é ë ê 1ï  B")
+
+    def test_response_request_output_arrangement(self):
+        # pylint: disable=line-too-long
+        message = UNiiResponseMessage(
+            bytes.fromhex(
+                "03a7155e79ad000093570502017d63849572e1395027d3310f4f6bdecb825097a6c2a28a03aad4a22985b0672d96513e390ab0c510e4875d00c875079f2a9d45cd6183f6ec632a57639336f7bfcb84074321c3cdff270347516063d03c6d4e8ae2e548e31d5726cc44d3361dea3075ec2ce2b826a8083778e1b95d244e7861b6f0abcbc24cdef47dc1f65a0f426fbf287090280eaf91ad21c54ebac2442b2827c805a37b3e4acd90431e4ab159be08ae713b873fe7c0c83b5c795f08543ee7d9439e3b7bebe9e66f0b3fea9aa9e0ac023e1da64c1a95a71ac93e82a4a78dc7b29f5325a3ccfc2f5420167ac4c4c0c344da7d05a202f921fb9491e155a822f891acb046eabb323459393e1e2b1746ca4bf1d9f93097d1560dd50eed4870d135f5e695e83b850a1e0cfe9685e90ace419a656668e07405a7e28d190014ade143328f8ad956f76a10bda1e078ec171f591bb102174f8945b62e0ba8beef85a8207bb5b1f9b6e486f5c1ecbbdf5686b34041b97e7a1a9afcab54cec4b9c9b6"
+            ),
+            bytes.fromhex("31323334353637383930616263646566"),
+        )
+        _LOGGER.debug(message)
+
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `unii-0.0.0.1/test/test_unii_message_checksum.py` & `unii-1.0.0b1/tests/test_unii_message_checksum.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_message_encryption.py` & `unii-1.0.0b1/tests/test_unii_message_encryption.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/test/test_unii_sections.py` & `unii-1.0.0b1/tests/test_unii_sections.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,14 @@
         await asyncio.sleep(1)
         try:
             result = await self._unii.connect()
             self.assertTrue(result, "Failed to connect to UNii")
             self.assertIsNotNone(self._unii.sections, "Sections not set")
             await self._unii.arm_section(1, self.user_code)
             result = await self._unii.disarm_section(1, self.user_code)
-            self.assertTrue(result)
             self.assertTrue(result, "Failed to disarm section")
         finally:
             await asyncio.sleep(1)
             await self._unii.disconnect()
 
 
 if __name__ == "__main__":
```

### Comparing `unii-0.0.0.1/unii/__main__.py` & `unii-1.0.0b1/unii/__main__.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/unii/sia_code.py` & `unii-1.0.0b1/unii/sia_code.py`

 * *Files identical despite different names*

### Comparing `unii-0.0.0.1/unii/unii.py` & `unii-1.0.0b1/unii/unii.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,68 +3,94 @@
 """
 
 import asyncio
 import logging
 import time
 from abc import ABC
 from datetime import datetime, timedelta
+from enum import IntFlag, auto
 from threading import Lock
-from typing import Final
+from typing import Any, Final
 
 from .unii_command import UNiiCommand
 from .unii_command_data import (
     UNiiArmDisarmSection,
     UNiiArmSectionStatus,
     UNiiArmState,
     UNiiData,
     UNiiDeviceStatus,
     UNiiDisarmSectionStatus,
     UNiiDisarmState,
     UNiiEquipmentInformation,
+    UNiiInput,
     UNiiInputArrangement,
     UNiiInputState,
     UNiiInputStatus,
+    UNiiInputStatusRecord,
+    UNiiOutput,
     UNiiRawData,
+    UNiiSection,
+    UNiiSectionArmedState,
     UNiiSectionArrangement,
     UNiiSectionStatus,
 )
 from .unii_connection import (
     DEFAULT_PORT,
     UNiiConnection,
     UNiiConnectionError,
     UNiiTCPConnection,
 )
+from .unii_message import UNiiResponseMessage
 
 logger = logging.getLogger(__name__)
 
 _POLL_ALIVE_INTERVAL: Final = timedelta(seconds=30)
 
 
+class UNiiFeature(IntFlag):
+    """Features implemented by the UNii library."""
+
+    ARM_SECTION: Final = auto()
+    BYPASS_ZONE: Final = auto()
+    SET_OUTPUT: Final = auto()
+
+
 class UNii(ABC):
     """
     UNii base class for interfacing with Alphatronics UNii security systems.
     """
 
-    unique_id = None
-    model = "Unknown"
-    connected = False
-
-    equipment_information: UNiiEquipmentInformation = None
-    sections = {}
-    inputs = {}
-    device_status: UNiiDeviceStatus = None
+    unique_id: str | None = None
+    model: str = "Unknown"
+    connected: bool = False
+
+    equipment_information: UNiiEquipmentInformation | None = None
+    sections: dict[int, UNiiSection]
+    inputs: dict[int, UNiiInput]
+    outputs: dict[int, UNiiOutput]
+    device_status: UNiiDeviceStatus | None = None
 
-    connection: UNiiConnection = None
+    connection: UNiiConnection
 
-    _event_occurred_callbacks = []
+    features: list[UNiiFeature]
+
+    _event_occurred_callbacks: list[Any]
 
     def __init__(
         self,
     ):
-        pass
+        super().__init__()
+
+        self.sections = {}
+        self.inputs = {}
+        self.outputs = {}
+
+        self.features = []
+
+        self._event_occurred_callbacks = []
 
     async def connect(self) -> bool:
         """
         Connect to Alphatronics UNii
         """
         raise NotImplementedError
 
@@ -77,21 +103,22 @@
     def add_event_occurred_callback(self, callback):
         """
         Adds an Event Occurred Callback to the UNii.
         """
         self._event_occurred_callbacks.append(callback)
 
     def _forward_to_event_occurred_callbacks(
-        self, command: UNiiCommand, data: UNiiData
+        self, command: UNiiCommand, data: UNiiData | None
     ):
         for callback in self._event_occurred_callbacks:
             try:
                 callback(command, data)
+            # pylint: disable=broad-exception-caught
             except Exception as ex:
-                logger.error(ex)
+                logger.error("Exception in Event Occurred Callback: %s", ex)
 
     async def arm_section(self, number: int, code: str) -> bool:
         """Arm a section."""
         raise NotImplementedError
 
     async def disarm_section(self, number: int, code: str) -> bool:
         """Disarm a section."""
@@ -101,86 +128,122 @@
 class UNiiLocal(UNii):
     # pylint: disable=too-many-instance-attributes
     """
     UNii class for interfacing with Alphatronics UNii security systems on the local
     network.
     """
 
-    _received_message_queue = {}
-    _waiting_for_message = {}
+    _received_message_queue: dict[int, list[Any]]
+    _waiting_for_message: dict[int, UNiiCommand | None]
 
-    _poll_alive_task: asyncio.Task = None
-    _stay_connected: bool = False
+    _poll_alive_task: asyncio.Task | None = None
 
     def __init__(
-        self, host: str, port: int = DEFAULT_PORT, shared_key: (str, bytes) = None
+        self, host: str, port: int = DEFAULT_PORT, shared_key: bytes | None = None
     ):
+        super().__init__()
+
         # If the shared key is provided as hex string convert it to bytes.
         if shared_key is not None and isinstance(shared_key, str):
             shared_key = bytes.fromhex(shared_key)
         self.connection = UNiiTCPConnection(host, port, shared_key)
         self.unique_id = f"{host}:{port}"
+
+        self._received_message_queue = {}
+        self._waiting_for_message = {}
+
         self._received_message_queue_lock = Lock()
 
     async def _connect(self) -> bool:
         await self.connection.connect()
 
         self.connection.set_message_received_callback(self._message_received_callback)
         response, _ = await self._send_receive(
             UNiiCommand.CONNECTION_REQUEST,
             None,
             UNiiCommand.CONNECTION_REQUEST_RESPONSE,
             False,
         )
         if response == UNiiCommand.CONNECTION_REQUEST_RESPONSE:
-            await self._send_receive(
+            response, data = await self._send_receive(
                 UNiiCommand.REQUEST_EQUIPMENT_INFORMATION,
                 None,
                 UNiiCommand.RESPONSE_REQUEST_EQUIPMENT_INFORMATION,
                 False,
             )
+            if (
+                response is None
+                or data is None
+                or response != UNiiCommand.RESPONSE_REQUEST_EQUIPMENT_INFORMATION
+                or self.equipment_information is None
+            ):
+                await self._disconnect()
+                return False
 
             await self._send_receive(
                 UNiiCommand.REQUEST_SECTION_ARRANGEMENT,
                 None,
                 UNiiCommand.RESPONSE_REQUEST_SECTION_ARRANGEMENT,
                 False,
             )
 
-            for _, section in self.sections.items():
-                await self._send_receive(
-                    UNiiCommand.REQUEST_SECTION_STATUS,
-                    UNiiRawData(section.number.to_bytes(1)),
-                    UNiiCommand.RESPONSE_REQUEST_SECTION_STATUS,
-                    False,
-                )
+            await self._send_receive(
+                UNiiCommand.REQUEST_SECTION_STATUS,
+                UNiiRawData(
+                    bytes.fromhex(
+                        "0102030405060708090a0b0c0d0e0f101112131415161718191a1b1c1d1e1f20"
+                    )
+                ),
+                UNiiCommand.RESPONSE_REQUEST_SECTION_STATUS,
+                False,
+            )
 
-            for i in range(1, 15):
-                await self._send_receive(
+            block = 0
+            while True:
+                block += 1
+                _, data = await self._send_receive(
                     UNiiCommand.REQUEST_INPUT_ARRANGEMENT,
-                    UNiiRawData(i.to_bytes(2)),
+                    UNiiRawData(block.to_bytes(2)),
                     UNiiCommand.RESPONSE_REQUEST_INPUT_ARRANGEMENT,
                     False,
                 )
+                if data is None:
+                    break
 
             await self._send_receive(
                 UNiiCommand.REQUEST_INPUT_STATUS,
                 None,
                 UNiiCommand.INPUT_STATUS_CHANGED,
                 False,
             )
+
+            software_version = (
+                self.equipment_information.software_version.finalize_version()
+            )
+            if software_version.match(">=2.17.0"):
+                block = 0
+                while True:
+                    block += 1
+                    _, data = await self._send_receive(
+                        UNiiCommand.REQUEST_OUTPUT_ARRANGEMENT,
+                        UNiiRawData(block.to_bytes(2)),
+                        UNiiCommand.RESPONSE_REQUEST_OUTPUT_ARRANGEMENT,
+                        False,
+                    )
+                    if data is None:
+                        break
+
             await self._send_receive(
                 UNiiCommand.REQUEST_DEVICE_STATUS,
                 None,
                 UNiiCommand.DEVICE_STATUS_CHANGED,
                 False,
             )
 
             self.connected = True
-            self._stay_connected = True
 
             self._forward_to_event_occurred_callbacks(
                 UNiiCommand.CONNECTION_REQUEST_RESPONSE, None
             )
 
             return True
         return False
@@ -195,128 +258,169 @@
         except UNiiConnectionError as ex:
             logger.error(str(ex))
 
         return False
 
     async def _disconnect(self) -> bool:
         await self._send(UNiiCommand.NORMAL_DISCONNECT, None, False)
-        self.connected = False
-        # Re-using the Normal Disconnect command to let the Event Occurred Callbacks know the UNii
-        # is disconnected.
-        self._forward_to_event_occurred_callbacks(UNiiCommand.NORMAL_DISCONNECT, None)
-        return await self.connection.close()
+        if await self.connection.close():
+            self.connected = False
+            # Re-using the Normal Disconnect command to let the Event Occurred Callbacks know the
+            # UNii is disconnected.
+            self._forward_to_event_occurred_callbacks(
+                UNiiCommand.NORMAL_DISCONNECT, None
+            )
+            return True
+
+        return False
 
     async def disconnect(self) -> bool:
-        self._stay_connected = False
+        await self._cancel_poll_alive()
 
         if self.connection is not None and self.connection.is_open:
             try:
                 if not await self._disconnect():
                     return False
             except UNiiConnectionError as ex:
                 logger.error(str(ex))
                 return False
 
         if self._poll_alive_task is not None:
             await self._poll_alive_task
         return True
 
     async def _send(
-        self, command: UNiiCommand, data: UNiiData = None, reconnect: bool = True
-    ) -> int:
+        self, command: UNiiCommand, data: UNiiData | None = None, reconnect: bool = True
+    ) -> int | None:
         if self.connection is None and reconnect:
-            logger.info("Trying to reconnect")
+            logger.info("Trying to connect")
             await self._connect()
         elif not self.connection.is_open and reconnect:
-            logger.info("Connection lost, trying to reconnect")
-            await self._disconnect()
+            logger.info("Trying to reconnect")
             await self._connect()
         elif self.connection is None or not self.connection.is_open:
             # ToDo: Throw exception?
             return None
 
         # logger.debug("Sending command %s", command)
         return await self.connection.send(command, data)
 
     async def _send_receive(
         self,
         command: UNiiCommand,
-        data: UNiiData = None,
-        expected_response: UNiiCommand = None,
+        data: UNiiData | None = None,
+        expected_response: UNiiCommand | None = None,
         reconnect: bool = True,
-    ) -> [UNiiCommand, UNiiData]:
+    ) -> list[Any]:
         tx_sequence = await self._send(command, data, reconnect)
         if tx_sequence is not None:
             return await self._get_received_message(tx_sequence, expected_response)
         return [None, None]
 
+    def _handle_equipment_information(self, data: UNiiEquipmentInformation):
+        if (
+            self.equipment_information is not None
+            and self.equipment_information != data
+        ):
+            self._forward_to_event_occurred_callbacks(
+                UNiiCommand.RELOAD_CONFIGURATION, None
+            )
+
+        self.equipment_information = data
+
+        # Get capabilities based on firmware version number
+        # Library is currently read-only, so disabled for now
+        # software_version = (
+        #     self.equipment_information.software_version.finalize_version()
+        # )
+        # if software_version.match(">=2.17.0"):
+        #     self.features.append(UNiiFeature.ARM_SECTION)
+        #     self.features.append(UNiiFeature.BYPASS_ZONE)
+        #     self.features.append(UNiiFeature.SET_OUTPUT)
+
     def _handle_section_arrangement(self, data: UNiiSectionArrangement):
-        for section_number, section in data.items():
-            if section_number not in self.inputs:
-                self.sections[section_number] = section
-            else:
-                self.sections[section_number].update(section)
+        for _, section in data.items():
+            if section.number not in self.sections and section.active:
+                self.sections[section.number] = section
+            elif section.number in self.sections:
+                self.sections[section.number].update(section)
 
     def _handle_section_status(self, data: UNiiSectionStatus):
-        self.sections[data.number]["armed_state"] = data["armed_state"]
+        for _, section_status in data.items():
+            if section_status.number in self.sections:
+                self.sections[section_status.number].update(section_status)
+                self.sections[section_status.number]["active"] = (
+                    section_status.armed_state != UNiiSectionArmedState.NOT_PROGRAMMED
+                )
+            elif section_status.armed_state != UNiiSectionArmedState.NOT_PROGRAMMED:
+                # This should never happen
+                logger.warning(
+                    "Status for unknown section %i changed", section_status.number
+                )
+
+    def _handle_input_status_update(self, input_status: UNiiInputStatusRecord):
+        if input_status.number in self.inputs:
+            self.inputs[input_status.number].update(input_status)
+        elif input_status.status != UNiiInputState.DISABLED:
+            # This should never happen
+            logger.warning("Status for unknown input %i changed", input_status.number)
 
     def _handle_input_status_changed(self, data: UNiiInputStatus):
-        for input_number, input_status in data.items():
-            if input_number in self.inputs:
-                self.inputs[input_number].update(input_status)
-            elif input_status.status != UNiiInputState.DISABLED:
-                # This should never happen
-                logger.warning("Status for unknown input %i changed", input_number)
+        for _, input_status in data.items():
+            self._handle_input_status_update(input_status)
 
     def _handle_input_arrangement(self, data: UNiiInputArrangement):
-        for input_number, unii_input in data.items():
+        if data is None:
+            return
+        for _, unii_input in data.items():
             # Expand sections
             for index, section in enumerate(unii_input.sections):
                 unii_input["sections"][index] = self.sections[section]
 
-            if input_number not in self.inputs:
-                self.inputs[input_number] = unii_input
+            if unii_input.number not in self.inputs:
+                self.inputs[unii_input.number] = unii_input
             else:
                 # Retain the input status before updating the input with new data.
-                unii_input.status = self.inputs[input_number].status
-                self.inputs[input_number].update(unii_input)
+                unii_input.status = self.inputs[unii_input.number].status
+                self.inputs[unii_input.number].update(unii_input)
 
     async def _message_received_callback(
         self, tx_sequence: int, command: UNiiCommand, data: UNiiData
     ):
         match command:
             case UNiiCommand.EVENT_OCCURRED:
                 self._forward_to_event_occurred_callbacks(command, data)
                 if self.connected:
                     await self._send(UNiiCommand.RESPONSE_EVENT_OCCURRED, None, False)
             case UNiiCommand.INPUT_STATUS_CHANGED:
                 self._handle_input_status_changed(data)
-                # self.inputs = data
+            case UNiiCommand.INPUT_STATUS_UPDATE:
+                self._handle_input_status_update(data)
             case UNiiCommand.DEVICE_STATUS_CHANGED:
                 self.device_status = data
             case UNiiCommand.RESPONSE_REQUEST_SECTION_ARRANGEMENT:
                 self._handle_section_arrangement(data)
             case UNiiCommand.RESPONSE_REQUEST_SECTION_STATUS:
                 self._handle_section_status(data)
             case UNiiCommand.RESPONSE_REQUEST_INPUT_ARRANGEMENT:
                 self._handle_input_arrangement(data)
             case UNiiCommand.RESPONSE_REQUEST_EQUIPMENT_INFORMATION:
-                self.equipment_information = data
+                self._handle_equipment_information(data)
 
         if tx_sequence in self._waiting_for_message and self._waiting_for_message[
             tx_sequence
         ] in [None, command]:
             with self._received_message_queue_lock:
                 self._received_message_queue[tx_sequence] = [command, data]
 
         self._forward_to_event_occurred_callbacks(command, data)
 
     async def _get_received_message(
-        self, tx_sequence: int, expected_response: UNiiCommand = None
-    ) -> [UNiiCommand, UNiiData]:
+        self, tx_sequence: int, expected_response: UNiiCommand | None = None
+    ) -> list[Any]:
         timeout = time.time() + 5
         self._waiting_for_message[tx_sequence] = expected_response
         while self.connection.is_open and time.time() < timeout:
             with self._received_message_queue_lock:
                 if tx_sequence in self._received_message_queue:
                     return self._received_message_queue.pop(tx_sequence)
             # logger.debug("Waiting for message %i to be received", tx_sequence)
@@ -328,40 +432,68 @@
 
     async def _poll_alive(self) -> bool:
         try:
             response, _ = await self._send_receive(
                 UNiiCommand.POLL_ALIVE_REQUEST,
                 None,
                 UNiiCommand.POLL_ALIVE_RESPONSE,
-                False,
+                True,
             )
             # logger.debug("Response received: %s", response)
             if response == UNiiCommand.POLL_ALIVE_RESPONSE:
                 # logger.debug("Poll Alive success")
                 return True
         except UNiiConnectionError as ex:
             logger.error(str(ex))
 
-        logger.error("Poll Alive failed")
+        if self.connection.is_open:
+            logger.error("Poll Alive failed")
         return False
 
+    async def _cancel_poll_alive(self) -> bool:
+        if self._poll_alive_task is not None and not (
+            self._poll_alive_task.done() or self._poll_alive_task.cancelled()
+        ):
+            if not self._poll_alive_task.cancel():
+                logger.error("Failed to cancel poll alive task")
+                logger.debug("Poll alive task: %s", self._poll_alive_task)
+                return False
+            try:
+                await self._poll_alive_task
+            except asyncio.CancelledError:
+                logger.debug("Poll alive task was cancelled")
+
+        if self._poll_alive_task is not None:
+            if self._poll_alive_task.done() or self._poll_alive_task.cancelled():
+                self._poll_alive_task = None
+            else:
+                logger.error("Failed to cancel poll alive task")
+                logger.debug("Poll alive task: %s", self._poll_alive_task)
+                return False
+
+        return self._poll_alive_task is None
+
     async def _poll_alive_coroutine(self):
         """
         To keep the connection alive (and NAT entries active) a poll message has to be sent every
         30 seconds if no other messages where sent during the last 30 seconds.
         """
-        while self._stay_connected:
-            if (
-                datetime.now()
-                > self.connection.last_message_sent + _POLL_ALIVE_INTERVAL
-                and not await self._poll_alive()
-            ):
-                if self.connection.is_open:
-                    await self._disconnect()
-            await asyncio.sleep(1)
+        while True:
+            try:
+                if (
+                    datetime.now()
+                    > self.connection.last_message_sent + _POLL_ALIVE_INTERVAL
+                    and not await self._poll_alive()
+                ):
+                    if self.connection.is_open:
+                        await self._disconnect()
+                await asyncio.sleep(1)
+            except asyncio.CancelledError:
+                logger.debug("Poll alive coroutine was canceled")
+                break
         # logger.debug("Poll Alive coroutine stopped")
 
     async def arm_section(self, number: int, code: str) -> bool:
         """Arm a section."""
         response, data = await self._send_receive(
             UNiiCommand.REQUEST_ARM_SECTION,
             UNiiArmDisarmSection(code, number),
@@ -385,9 +517,12 @@
         )
         if response == UNiiCommand.RESPONSE_DISARM_SECTION and data.disarm_state in [
             UNiiDisarmState.SECTION_DISARMED,
             UNiiDisarmState.NO_CHANGE,
         ]:
             return True
 
-        logger.error("Disarming failed: %s", data.disarm_state)
+        if data is not None:
+            logger.error("Disarming failed: %s", data.disarm_state)
+        else:
+            logger.error("Disarming failed")
         return False
```

### Comparing `unii-0.0.0.1/unii/unii_command.py` & `unii-1.0.0b1/unii/unii_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 
 
 class UNiiCommand(IntEnum):
     """
     UNii Commands
     """
 
+    # Virtual commands used within the library
+    RELOAD_CONFIGURATION: Final = 0x010001
+
     # Connection setup
     CONNECTION_REQUEST: Final = 0x0001
     CONNECTION_REQUEST_RESPONSE: Final = 0x0002
     CONNECTION_REQUEST_DENIED: Final = 0x0003
     NORMAL_DISCONNECT: Final = 0x0014
 
     # Operational commands
@@ -46,27 +49,30 @@
     REQUEST_OUTPUT_STATUS: Final = 0x011E
     RESPONSE_REQUEST_OUTPUT_STATUS: Final = 0x011F
     # REQUEST TO SET OUTPUT(S) WITH USER CODE: Final = 0X0120
     # RESPONSE REQUEST TO SET OUTPUT(S) WITH USER CODE: Final = 0X0121
     REQUEST_TO_RESET_ALARM: Final = 0x0122
     RESPONSE_REQUEST_TO_RESET_ALARM: Final = 0x0123
     EXIT_ENTRY_TIMER: Final = 0x0124
+    INPUT_STATUS_UPDATE: Final = 0x0125
 
     # Configuration commands
     REQUEST_SECTION_ARRANGEMENT: Final = 0x0130
     RESPONSE_REQUEST_SECTION_ARRANGEMENT: Final = 0x0131
     REQUEST_GROUP_ARRANGEMENT: Final = 0x0132
     RESPONSE_REQUEST_GROUP_ARRANGEMENT: Final = 0x0133
     REQUEST_INPUT_ARRANGEMENT: Final = 0x0140
     RESPONSE_REQUEST_INPUT_ARRANGEMENT: Final = 0x0141
     REQUEST_EQUIPMENT_INFORMATION: Final = 0x0142
     RESPONSE_REQUEST_EQUIPMENT_INFORMATION: Final = 0x0143
     REQUEST_DATE_AND_TIME: Final = 0x0144
     RESPONSE_REQUEST_DATE_AND_TIME: Final = 0x0145
     WRITE_DATE_AND_TIME: Final = 0x0146
     RESPONSE_WRITE_DATE_AND_TIME: Final = 0x0147
+    REQUEST_OUTPUT_ARRANGEMENT: Final = 0x0148
+    RESPONSE_REQUEST_OUTPUT_ARRANGEMENT: Final = 0x0149
 
     def __str__(self) -> str:
         return self.name
 
     def __repr__(self) -> str:
         return self.name
```

### Comparing `unii-0.0.0.1/unii/unii_command_data.py` & `unii-1.0.0b1/unii/unii_command_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 """
 Data classes used by the UNii library.
 """
 
 import logging
 import string
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from datetime import datetime
 from enum import IntEnum, IntFlag, auto
 from typing import Final
 
+import semver
+
 from .sia_code import SIACode
 
 logger = logging.getLogger(__name__)
 
 # Helper functions
 
 
-def bit_position_to_numeric(data: bytes) -> [int]:
+def bit_position_to_numeric(data: bytes) -> list[int]:
     """
     Returns which bits in an array of bytes are set, LSB first.
 
     00001010 => [2, 4]
     """
     data = int.from_bytes(data)
     numerics = []
     for i in range(0, 31):
         bit_position: int = pow(2, i)
         if data & bit_position:
             numerics.append(i + 1)
     return numerics
 
 
-def bcd_encode(data: bytes) -> bytes:
+def bcd_encode(data: str) -> bytes:
     """ "
     Encodes numeric string values in BCD format padded with zeroes to the right.
 
     https://en.wikipedia.org/wiki/Binary-coded_decimal
 
     Example implementation from:
     """
@@ -44,42 +46,53 @@
     # Add trailing zeroes
     while len(data) < 16:
         data += "0"
     logger.debug("Data: %s", data)
 
     return bytes.fromhex(data)
 
-    # This does the same but less efficient. I leave it in place for now, as reference and also to
-    # be modified if above implementation happens to be not how it's supposed to work.
-    # data = data.encode()
-    #
-    # # Split data in chunks of 2 bytes
-    # chunks = [data[pos : pos + 2] for pos in range(0, len(data), 2)]
-    #
-    # bcd_bytes = bytearray()
-    # for digits in chunks:
-    #     bcd_byte = ((digits[0] & 0x0F) << 4) + (digits[1] & 0x0F)
-    #     bcd_bytes.append(bcd_byte)
-    #
-    # return bcd_bytes
+
+def decode_and_strip(data: bytes) -> str:
+    """Decode a byte array to UTF-8 and strip all leading and trailing whitespace and \x00."""
+    return data.decode("utf-8", "replace").strip(string.whitespace + "\x00")
+
+
+def translate_input_number(input_number: int) -> int:
+    """Translate input number according to Appendix 4 of the UNii API."""
+    if input_number <= 511:
+        return input_number + 1
+    if 512 <= input_number <= 543:
+        return input_number + 189
+    # if 544 <= input_number <= 575:
+    #     return -1
+    if 576 <= input_number <= 639:
+        return input_number + 25
+    if 640 <= input_number <= 688:
+        return input_number + 161
+    # if 689 <= input_number <= 705:
+    #     return -1
+    if 706 <= input_number <= 962:
+        return input_number + 295
+
+    return -1
 
 
 # Generic command data classes
 
 
-class UNiiData:
+class UNiiData(ABC):
     # pylint: disable=too-few-public-methods
     """
     UNii Base data class.
 
     All data classes which are used to send or receive data should inherit from this class.
     """
 
 
-class UNiiSendData:
+class UNiiSendData(ABC):
     # pylint: disable=too-few-public-methods
     """
     Method which should be implemented by data classes which are used to send data.
     """
 
     @abstractmethod
     def to_bytes(self):
@@ -104,105 +117,145 @@
     def to_bytes(self):
         return self.raw_data
 
     def __repr__(self) -> str:
         return "0x" + self.raw_data.hex()
 
 
-class UNiiResultCode(UNiiData):
+class UNiiResultCode(IntEnum):
     """
     UNii Result Code data class.
 
     This data class is used as an ACK or NACK response from both sides for the defined commands.
     """
 
     # pylint: disable=too-few-public-methods
 
     OK: Final = 0x0000
     ERROR: Final = 0x0001
 
+    def __init__(self, data: bytes):
+        if isinstance(data, bytes):
+            data = int.from_bytes(data)
+        super().__init__(data)
+
 
 # Equipment related
 class UNiiEquipmentInformation(UNiiData):
     # pylint: disable=too-few-public-methods
+    # pylint: disable=too-many-instance-attributes
     """
     UNii Equipment Information data class.
 
     This data class contains the response of the "Request Equipment Information" command.
     """
 
-    software_date = None
-    device_id = None
-
     def __init__(self, data: bytes):
         # pylint: disable=consider-using-min-builtin
         # pylint: disable=too-many-locals
         """ """
         # Version
         version = data[1]
         if version not in [2, 3]:
-            raise ValueError()
+            raise ValueError("Invalid message version")
 
         if version == 2:
-            self.software_version = data[2:7].decode("utf-8", "replace")
-            software_date = (
-                data[7:19].decode("utf-8", "replace").strip(string.whitespace + "\x00")
-            )
+            software_version = decode_and_strip(data[2:7])
+            # The software version can be truncated, to make it a valid SemVer add 0 if the
+            # software version ends with .
+            if software_version.endswith("."):
+                software_version += "0"
+
+            software_date = decode_and_strip(data[7:19])
             self.software_date = datetime.strptime(software_date, "%d-%m-%Y").date()
         elif version == 3:
-            self.software_version = data[2:19].decode("utf-8", "replace")
+            software_version = decode_and_strip(data[2:19])
+            self.software_date = None
+
+        try:
+            self.software_version = semver.Version.parse(software_version)
+        except ValueError as ex:
+            # Fall back to version 0.0.0 when SemVer can not be parsed.
+            self.software_version = semver.Version(0, 0, 0)
+            logger.warning(ex)
 
         device_name_length = data[19]
-        self.device_name = (
-            data[20 : 20 + device_name_length]
-            .decode("utf-8", "replace")
-            .strip(string.whitespace + "\x00")
-        )
+        self.device_name = decode_and_strip(data[20 : 20 + device_name_length])
         data = data[20 + device_name_length :]
 
         self.max_inputs = int.from_bytes(data[0:2])
         self.max_groups = data[2]
         self.max_sections = data[3]
         self.max_users = int.from_bytes(data[4:6])
 
         if version == 3:
             device_id_length = data[6]
-            self.device_id = int.from_bytes(data[7 : 7 + device_id_length])
+            self.device_id = decode_and_strip(data[7 : 7 + device_id_length])
+            self.serial_number = self.device_id[:9]
+            mac_address = self.device_id[-12:]
+            self.mac_address = ":".join(
+                mac_address.lower()[i : i + 2] for i in range(0, 12, 2)
+            )
+        else:
+            self.device_id = None
+            self.serial_number = None
+            self.mac_address = None
 
     def __str__(self) -> str:
         return str(
             {
                 "software_version": self.software_version,
                 "software_date": str(self.software_date),
                 "device_name": self.device_name,
+                "device_id": self.device_id,
+                "serial_number": self.serial_number,
+                "mac_address": self.mac_address,
             }
         )
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, UNiiEquipmentInformation):
+            # don't attempt to compare against unrelated types
+            return NotImplemented
+
+        return (
+            self.software_version == other.software_version
+            and self.software_date == other.software_date
+            and self.device_name == other.device_name
+            and self.max_inputs == other.max_inputs
+            and self.max_groups == other.max_groups
+            and self.max_sections == other.max_sections
+            and self.max_users == other.max_users
+            and self.device_id == other.device_id
+            and self.serial_number == other.serial_number
+            and self.mac_address == other.mac_address
+        )
+
 
 # Section related
 class UNiiSection(dict):
     """
     UNii Section.
     """
 
     # Get dictionarry keys as attributes.
     __getattr__ = dict.get
 
     def __init__(self, data: bytes):
         # Version
         version = data[0]
         if version not in [0, 1]:
-            raise ValueError()
+            raise ValueError("Invalid message version")
 
         self["active"] = data[1] == 1
         if version == 0:
-            name = data[2:19].decode("utf-8", "replace").strip()
+            name = decode_and_strip(data[2:19])
         elif version == 1:
             name_length = data[2]
-            name = data[3 : 3 + name_length].decode("utf-8", "replace")
+            name = decode_and_strip(data[3 : 3 + name_length])
         self["name"] = name
 
 
 class UNiiSectionArrangement(dict, UNiiData):
     """
     UNii Section Arrangement data class.
 
@@ -212,15 +265,15 @@
     def __init__(self, data: bytes):
         offset = 0
         index = 1
         while offset < len(data):
             # Version
             version = data[0 + offset]
             if version not in [0, 1]:
-                raise ValueError()
+                raise ValueError("Invalid message version")
 
             section_length = 19
             if version == 1:
                 section_length = data[offset + 2] + 3
             section = UNiiSection(data[offset : offset + section_length])
             section["number"] = index
             self[index] = section
@@ -238,39 +291,59 @@
     ARMED: Final = 1
     DISARMED: Final = 2
     ALARM: Final = 7
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
+
+class UNiiSectionStatusRecord(dict):
+    """
+    UNii Section Status record.
+    """
+
+    # Get dictionarry keys as attributes.
+    __getattr__ = dict.get
+
+    def __init__(self, data: bytes):
+        self["number"] = data[0]
+        self["armed_state"] = UNiiSectionArmedState(data[1])
+
 
 class UNiiSectionStatus(dict, UNiiData):
     """
     UNii Section Status data class.
 
     This data class contains the response of the "Request Section Status" command.
     """
 
     # Get dictionarry keys as attributes.
     __getattr__ = dict.get
 
     def __init__(self, data: bytes):
-        self["number"] = data[0]
-        self["armed_state"] = UNiiSectionArmedState(data[1])
+        # Split data in chunks of 2 bytes
+        chunks = [data[pos : pos + 2] for pos in range(0, len(data), 2)]
+        # Convert chunks to Section Status Records
+        for chunk in chunks:
+            section_status_record = UNiiSectionStatusRecord(chunk)
+            self[section_status_record.number] = section_status_record
 
 
 class UNiiArmDisarmSection(UNiiData, UNiiSendData):
     # pylint: disable=too-few-public-methods
     """
     This data class contains the request for "Request Arm Section" and "Request Disarm Section"
     """
 
-    def __init__(self, code, number):
+    def __init__(self, code: str, number: int):
         self.code = code
-        self.number: int = number
+        self.number = number
 
     def to_bytes(self):
         bytes_ = bytearray()
         bytes_.append(0x00)
         bytes_.extend(bcd_encode(self.code))
         bytes_.extend(self.number.to_bytes(1))
         bytes_.append(0x01)
@@ -290,14 +363,17 @@
     SECTION_NOT_READY_FOR_ARMING: Final = 4
     NOT_AUTHORIZED_TO_ARM: Final = 5
     SYSTEM_ERROR: Final = 6
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiReadyToArmSectionStatus(UNiiData):
     # pylint: disable=too-few-public-methods
     """
     UNii Ready To Arm Section State data class
     """
 
@@ -316,14 +392,17 @@
     SECTION_ARMED: Final = 1
     ARMING_FAILED_SECTION_NOT_READY: Final = 2
     ARMING_FAILED_NOT_AUTHORIZED: Final = 3
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiArmSectionStatus(UNiiData):
     # pylint: disable=too-few-public-methods
     """
     UNii Arm Section State data class
     """
 
@@ -345,14 +424,17 @@
     SECTION_DISARMED: Final = 1
     DISARMING_FAILED: Final = 2
     DISARMING_FAILED_NOT_AUTHORIZED: Final = 3
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiDisarmSectionStatus(UNiiData):
     # pylint: disable=too-few-public-methods
     """
     UNii Disarm Section State data class
     """
 
@@ -378,14 +460,17 @@
     WIRELESS: Final = auto()
     KNX: Final = auto()
     DOOR: Final = auto()
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiSensorType(IntEnum):
     """
     The different kind of sensor types.
     """
 
     NOT_ACTIVE: Final = 0
@@ -404,14 +489,17 @@
     EN54_FIRE_MCP: Final = 13
     EN54_FAULT: Final = 14
     GLASSBREAK: Final = 15
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiReaction(IntEnum):
     """
     The different kind of reactions.
     """
 
     DIRECT: Final = 0
@@ -420,14 +508,17 @@
     TWENT_FOUR_HOUR: Final = 3
     LAST_DOOR: Final = 4
     DELAYED_ALARM: Final = 5
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiInput(dict):
     """
     UNii Input.
     """
 
     # Get dictionarry keys as attributes.
@@ -451,16 +542,15 @@
         self["input_type"] = input_type
 
         self["sensor_type"] = UNiiSensorType(data[2])
         self["reaction"] = UNiiReaction(data[3])
         name_length = data[4]
         name = None
         if name_length > 0:
-            name = data[5 : 5 + name_length]
-            name = name.decode("utf-8", "replace")
+            name = decode_and_strip(data[5 : 5 + name_length])
         self["name"] = name
         self["sections"] = bit_position_to_numeric(data[5 + name_length :])
         self["status"] = UNiiInputState.DISABLED
 
 
 class UNiiInputArrangement(dict, UNiiData):
     # pylint: disable=too-few-public-methods
@@ -471,21 +561,21 @@
     """
 
     def __init__(self, data: bytes):
         """ """
         # Version
         version = data[1]
         if version != 2:
-            raise ValueError()
+            raise ValueError("Invalid message version")
 
         # Block Number
         block_number = int.from_bytes(data[2:4])
 
         if block_number == 0xFFFF:
-            raise ValueError()
+            raise ValueError("Invalid block number")
 
         self.block_number = block_number
 
         offset = 4
         while offset < len(data):
             name_length = data[4 + offset]
             input_information = data[offset : 9 + offset + name_length]
@@ -508,41 +598,27 @@
     TAMPER: Final = 0x2
     MASKING: Final = 0x4
     DISABLED: Final = 0xF
 
     def __repr__(self) -> str:
         return self.name
 
+    def __str__(self) -> str:
+        return self.name.lower()
+
 
 class UNiiInputStatusRecord(dict):
     """
     UNii Input Status record.
     """
 
     # Get dictionarry keys as attributes.
     __getattr__ = dict.get
 
-    def __init__(self, index: int, data: int):
-        input_number = index
-        if index <= 511:
-            input_number += 1
-        elif 512 <= index <= 543:
-            input_number += 189
-        elif 544 <= index <= 575:
-            input_number = -1
-        elif 576 <= index <= 639:
-            input_number += 25
-        elif 640 <= index <= 688:
-            input_number += 161
-        elif 689 <= index <= 705:
-            input_number = -1
-        elif 706 <= index <= 962:
-            input_number += 295
-
-        self["number"] = input_number
+    def __init__(self, data: int):
         self["status"] = UNiiInputState(data & 0x0F)
         self["bypassed"] = data & 0b00010000 == 0b00010000
         self["alarm_memorized"] = data & 0b00100000 == 0b00100000
         self["low_battery"] = data & 0b01000000 == 0b01000000
         self["supervision"] = data & 0b10000000 == 0b10000000
 
 
@@ -555,19 +631,112 @@
     def __init__(self, data: bytes):
         # Version
         version = data[1]
         if version != 2:
             raise ValueError()
 
         for index, input_status in enumerate(data[2:]):
-            input_status = UNiiInputStatusRecord(index, input_status)
+            input_status = UNiiInputStatusRecord(input_status)
+            input_status["number"] = translate_input_number(index)
+
             if input_status.number >= 0:
                 self[input_status.number] = input_status
 
 
+class UNiiInputStatusUpdate(UNiiInputStatusRecord, UNiiData):
+    # pylint: disable=too-few-public-methods
+    """
+    UNii Input Status Update data class.
+    """
+
+    # Get dictionarry keys as attributes.
+    __getattr__ = dict.get
+
+    def __init__(self, data: bytes):
+        # Version
+        version = data[1]
+        if version != 2:
+            raise ValueError()
+
+        super().__init__(data[4])
+        self["number"] = int.from_bytes(data[2:4])
+
+
+# Output related
+
+
+class UNiiOutputType(IntEnum):
+    """
+    The available output types.
+    """
+
+    NOT_ACTIVE: Final = 0
+    DIRECT: Final = 1
+    TIMED: Final = 2
+    FOLLOW_INPUT: Final = 3
+
+
+class UNiiOutput(dict):
+    """
+    UNii Output.
+    """
+
+    # Get dictionarry keys as attributes.
+    __getattr__ = dict.get
+
+    def __init__(self, data: bytes):
+        output_number = int.from_bytes(data[0:2])
+        self["number"] = output_number
+
+        self["type"] = UNiiOutputType(data[2])
+
+        name_length = data[3]
+        name = None
+        if name_length > 0:
+            name = decode_and_strip(data[4 : 4 + name_length])
+        self["name"] = name
+        self["sections"] = bit_position_to_numeric(data[5 + name_length :])
+
+
+class UNiiOutputArrangement(dict, UNiiData):
+    # pylint: disable=too-few-public-methods
+    """
+    UNii Output Arrangement data class.
+
+    This data class contains the response of the "Request Output Arrangement" command.
+    """
+
+    def __init__(self, data: bytes):
+        """ """
+        # Version
+        version = data[1]
+        if version != 1:
+            raise ValueError("Invalid message version")
+
+        # Block Number
+        block_number = int.from_bytes(data[2:4])
+
+        if block_number == 0xFFFF:
+            raise ValueError("Invalid block number")
+
+        self.block_number = block_number
+
+        offset = 4
+        while offset < len(data):
+            name_length = data[3 + offset]
+            output_information = data[offset : 8 + offset + name_length]
+            output_information = UNiiOutput(output_information)
+            self[output_information.number] = output_information
+
+            offset += 8 + name_length
+
+    def __str__(self) -> str:
+        return str({"block_number": self.block_number, "inputs": super().__str__()})
+
+
 # Device related
 
 
 class UNiiDeviceStatusRecord(IntFlag):
     """
     UNii Device Status Record
     """
@@ -597,29 +766,29 @@
     # pylint: disable=too-few-public-methods
     """
     UNii Device Status data class.
 
     This data class contains the response of the "Request Device Status" command.
     """
 
-    io_devices = []
-    keyboard_devices = []
-    wiegand_devices = []
-    uwi_devices = []
+    io_devices: list[UNiiDeviceStatusRecord]
+    keyboard_devices: list[UNiiDeviceStatusRecord]
+    wiegand_devices: list[UNiiDeviceStatusRecord]
+    uwi_devices: list[UNiiDeviceStatusRecord]
 
     def __init__(self, data: bytes):
         # Version
         version = data[1]
         if version != 2:
-            raise ValueError()
+            raise ValueError("Invalid message version")
 
         # Split data in chunks of 2 bytes
         chunks = [data[pos : pos + 2] for pos in range(2, len(data), 2)]
         # Convert chunks to list of Device Status Records
-        device_status_records = [
+        device_status_records: list[UNiiDeviceStatusRecord] = [
             UNiiDeviceStatusRecord.from_bytes(chunk) for chunk in chunks
         ]
 
         # Control Panel
         self.control_panel = device_status_records[0]
 
         # IO Devices
@@ -664,33 +833,33 @@
     """
     UNii Event Record data class.
     """
 
     # pylint: disable=too-few-public-methods
     # pylint: disable=too-many-instance-attributes
 
-    event_description: str = None
-    user_id: int = None
-    user_name: str = None
-    input_id: int = None
-    input_name: str = None
-    device_id: int = None
-    device_name: str = None
-    bus_id: int = None
-    sections: [] = None
-    sia_code: SIACode = None
+    event_description: str | None = None
+    user_number: int | None = None
+    user_name: str | None = None
+    input_number: int | None = None
+    input_name: str | None = None
+    device_number: int | None = None
+    device_name: str | None = None
+    bus_number: int | None = None
+    sections: list[int] | None = None
+    sia_code: SIACode | None = None
 
     def __init__(self, data: bytes):
         # pylint: disable=consider-using-min-builtin
         # pylint: disable=too-many-locals
         """ """
         # Version
         version = data[1]
         if version != 3:
-            raise ValueError()
+            raise ValueError("Invalid message version")
 
         # Event Number
         self.event_number = int.from_bytes(data[2:4])
 
         # Timestamp
         year = 1900 + data[4]
         month = data[5] + 1
@@ -701,76 +870,77 @@
         self.timestamp = datetime(year, month, day, hour, minute, second)
 
         data = data[10:]
 
         # Description
         event_description_length = data[0]
         if event_description_length > 0:
-            event_description = data[1 : 1 + event_description_length]
-            self.event_description = event_description.decode("utf-8", "replace")
+            self.event_description = decode_and_strip(
+                data[1 : 1 + event_description_length]
+            )
 
         data = data[1 + event_description_length :]
 
         # User
-        user_id = int.from_bytes(data[0:2])
-        if user_id > 0:
-            self.user_id = user_id
+        user_number = int.from_bytes(data[0:2])
+        if user_number > 0:
+            self.user_number = user_number
 
         user_name_length = data[2]
         if user_name_length > 0:
-            user_name = data[3 : 3 + user_name_length]
-            self.user_name = user_name.decode("utf-8", "replace")
+            self.user_name = decode_and_strip(data[3 : 3 + user_name_length])
 
         data = data[3 + user_name_length :]
 
         # Input
-        input_id = int.from_bytes(data[0:2])
-        if input_id > 0:
-            self.input_id = input_id
+        input_number = int.from_bytes(data[0:2])
+        if input_number > 0:
+            self.input_number = input_number
 
         input_name_length = data[2]
         if input_name_length > 0:
-            input_name = data[3 : 3 + input_name_length]
-            self.input_name = input_name.decode("utf-8", "replace")
+            self.input_name = decode_and_strip(data[3 : 3 + input_name_length])
 
         data = data[3 + input_name_length :]
 
         # Device
-        device_id = int.from_bytes(data[0:2])
-        if device_id > 0:
-            self.device_id = device_id
+        device_number = int.from_bytes(data[0:2])
+        if device_number > 0:
+            self.device_number = device_number
 
         device_name_length = data[2]
         if device_name_length > 0:
-            device_name = data[3 : 3 + device_name_length]
-            self.device_name = device_name.decode("utf-8", "replace")
+            self.device_name = decode_and_strip(data[3 : 3 + device_name_length])
 
         data = data[3 + device_name_length :]
 
         # Bus
-        self.bus_id = data[0]
+        self.bus_number = data[0]
 
         # Sections
         self.sections = bit_position_to_numeric(data[1:5])
 
         # SIA Code
-        sia_code = data[5:7].decode("utf-8", "replace").strip()
+        sia_code = decode_and_strip(data[5:7])
         if sia_code != "":
-            self.sia_code = SIACode(data[5:7].decode("utf-8", "replace"))
+            try:
+                self.sia_code = SIACode(sia_code)
+            except ValueError as ex:
+                logger.warning(ex)
 
     def __repr__(self) -> str:
         return str(
             {
                 "event_number": self.event_number,
                 "timestamp": str(self.timestamp),
                 "event_description": self.event_description,
-                "user_id": self.user_id,
+                "user_number": self.user_number,
                 "user_name": self.user_name,
-                "input_id": self.input_id,
+                "input_number": self.input_number,
                 "input_name": self.input_name,
-                "device_id": self.device_id,
+                "device_number": self.device_number,
                 "device_name": self.device_name,
-                "bus_id": self.bus_id,
+                "bus_number": self.bus_number,
                 "sections": self.sections,
                 "sia_code": self.sia_code,
             }
         )
```

### Comparing `unii-0.0.0.1/unii/unii_connection.py` & `unii-1.0.0b1/unii/unii_connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import asyncio
 import logging
 import random
 from abc import ABC, abstractmethod
 from asyncio.exceptions import CancelledError
 from asyncio.streams import StreamReader, StreamWriter
+from asyncio.tasks import Task
 from datetime import datetime
 from threading import Lock
 from typing import Final
 
 from .unii_command import UNiiCommand
 from .unii_command_data import UNiiData
 from .unii_message import UNiiMessageError, UNiiRequestMessage, UNiiResponseMessage
@@ -52,19 +53,18 @@
 class UNiiConnection(ABC):
     """
     Abstract connection class on which the different connection types are build.
     """
 
     _MAX_LENGTH_OF_ANSWER: Final = 1500
 
-    last_message_sent = 0
-    last_message_received = 0
+    last_message_sent: datetime = datetime.now()
+    last_message_received: datetime = datetime.now()
     _message_received_callback = None
-
-    is_open: bool = None
+    unique_id: str
 
     def set_message_received_callback(self, callback):
         """
         Sets the call back for handling Event Occurred messages.
         """
         self._message_received_callback = callback
 
@@ -78,63 +78,72 @@
     @abstractmethod
     async def close(self) -> bool:
         """
         Closes the connection to the Alphatronics UNii.
         """
         raise NotImplementedError
 
+    @property
+    def is_open(self) -> bool:
+        """
+        If the connection is open
+        """
+        raise NotImplementedError
+
     @abstractmethod
     async def send(
         self,
         command: UNiiCommand,
-        data: UNiiData = None,
-    ) -> bool:
+        data: UNiiData | None = None,
+    ) -> int | None:
         """
-        Write to Alphatronics UNii and returns the response.
+        Constructs a message based on given command and data, writes this to the UNii and
+        returns the TX Sequence ID or None if writing failed.
         """
         raise NotImplementedError
 
 
 class UNiiTCPConnection(UNiiConnection):
     # pylint: disable=too-many-instance-attributes
     """
     Connection to an Alphatronics UNii over TCP/IP.
     """
 
-    _reader: StreamReader = None
-    _writer: StreamWriter = None
-    _session_id = None
-    _tx_sequence = -1
-    _rx_sequence = 0
-
-    _close_connection = True
-    _receive_task = None
-
-    def __init__(self, host: str, port: int = DEFAULT_PORT, shared_key=None):
+    _reader: StreamReader | None = None
+    _writer: StreamWriter | None = None
+    _session_id: int | None = None
+    _tx_sequence: int = -1
+    _rx_sequence: int = 0
+
+    _receive_task: Task | None = None
+
+    def __init__(
+        self, host: str, port: int = DEFAULT_PORT, shared_key: bytes | None = None
+    ):
         assert host is not None
         assert port is not None
 
         self._host = host
         self._port = port
         self._shared_key = shared_key
         self._writer_lock = Lock()
+        self.unique_id = host
 
     def __str__(self) -> str:
         return f"{self._host}:{self._port}"
 
     async def connect(self):
         try:
             if not self.is_open:
                 logger.info("Connecting to %s", self)
                 self._reader, self._writer = await asyncio.wait_for(
                     asyncio.open_connection(self._host, self._port), timeout=10
                 )
                 logger.info("Connected to %s", self)
 
-                self._close_connection = False
                 # Fixed session ID only one session
                 self._session_id = 0xFFFF
                 # Start with a random TX Sequence
                 self._tx_sequence = random.randint(0, 65535)
 
                 # Start the read coroutine
                 self._receive_task = asyncio.create_task(self._receive_coroutine())
@@ -145,17 +154,17 @@
             ConnectionRefusedError,
             ConnectionResetError,
             CancelledError,
         ) as ex:
             raise UNiiConnectionError(ex) from ex
 
     async def _close(self) -> bool:
-        self._close_connection = True
+        await self._cancel_receive()
 
-        if self.is_open:
+        if self.is_open and self._writer is not None:
             try:
                 with self._writer_lock:
                     self._writer.close()
                     await self._writer.wait_closed()
             except ConnectionResetError as ex:
                 logger.error(ex)
         self._writer = None
@@ -181,27 +190,52 @@
     @property
     def is_open(self) -> bool:
         """
         If the connection is open
         """
         return self._writer is not None
 
+    async def _cancel_receive(self) -> bool:
+        if self._receive_task is not None and not (
+            self._receive_task.done() or self._receive_task.cancelled()
+        ):
+            if not self._receive_task.cancel():
+                logger.error("Failed to cancel receive task")
+                logger.debug("Receive task: %s", self._receive_task)
+                return False
+            try:
+                await self._receive_task
+            except asyncio.CancelledError:
+                logger.debug("Receive task was cancelled")
+
+        if self._receive_task is not None:
+            if self._receive_task.done() or self._receive_task.cancelled():
+                self._receive_task = None
+            else:
+                logger.error("Failed to cancel receive task")
+                logger.debug("Receive task: %s", self._receive_task)
+                return False
+
+        return self._receive_task is None
+
     async def _receive_coroutine(self):
-        while not self._close_connection and self._reader is not None:
+        while self._reader is not None:
             try:
                 response = await asyncio.wait_for(self._reader.read(14), timeout=0.1)
                 if len(response) < 13:
                     continue
 
                 # Length
                 packet_length = int.from_bytes(response[12:14])
 
                 # Read remaining part of the message
-                if len(response) < packet_length:
+                while len(response) < packet_length:
                     response += await self._reader.read(packet_length - len(response))
+                    if len(response) < packet_length:
+                        logger.debug("Response not yet fully received")
 
                 message = UNiiResponseMessage(response, self._shared_key)
                 if message.command not in [
                     # UNiiCommand.CONNECTION_REQUEST_RESPONSE,
                     UNiiCommand.POLL_ALIVE_RESPONSE,
                     UNiiCommand.INPUT_STATUS_CHANGED,
                     UNiiCommand.DEVICE_STATUS_CHANGED,
@@ -213,15 +247,15 @@
                 else:
                     logger.debug(
                         "Received: %i, %s", message.rx_sequence, message.command
                     )
                 self.last_message_received = datetime.now()
                 # logger.debug("Last message received: %s", self.last_message_sent)
                 if message.rx_sequence != self._tx_sequence:
-                    logger.error(
+                    logger.warning(
                         "Invalid sequence number. Expected %i, received %i.",
                         self._tx_sequence,
                         message.rx_sequence,
                     )
 
                 self._session_id = message.session_id
                 self._rx_sequence = message.tx_sequence
@@ -232,51 +266,51 @@
                     )
             except UNiiMessageError as ex:
                 logger.error(ex)
             except ConnectionResetError as ex:
                 logger.debug(ex)
                 await self._close()
                 break
+            except asyncio.CancelledError:
+                logger.debug("Receive coroutine was canceled")
+                break
             except TimeoutError:
                 pass
             except IndexError as ex:
                 logger.error(ex)
             await asyncio.sleep(0.1)
         # logger.debug("Receive coroutine stopped")
 
     async def send(
         self,
         command: UNiiCommand,
-        data: UNiiData = None,
-    ) -> int:
-        """
-        Constructs a message based on given command and data, writes this to the UNii and
-        returns the TX Sequence ID or None if writing failed.
-        """
+        data: UNiiData | None = None,
+    ) -> int | None:
         if self.is_open:
             message = UNiiRequestMessage()
             message.session_id = self._session_id
             self._tx_sequence += 1
             message.tx_sequence = self._tx_sequence
             message.rx_sequence = self._rx_sequence
             message.command = command
             message.data = data
             # logger.debug("Sending: %s", message)
             # logger.debug("Sending: 0x%s", message.to_bytes(self._shared_key).hex())
-            try:
-                with self._writer_lock:
-                    self._writer.write(message.to_bytes(self._shared_key))
-                    await self._writer.drain()
-                    self.last_message_sent = datetime.now()
-                    # logger.debug("Last message sent: %s", self.last_message_sent)
-
-                return message.tx_sequence
-            except ConnectionResetError as ex:
-                await self.close()
-                raise UNiiConnectionError(str(ex)) from ex
+            if self._writer is not None:
+                try:
+                    with self._writer_lock:
+                        self._writer.write(message.to_bytes(self._shared_key))
+                        await self._writer.drain()
+                        self.last_message_sent = datetime.now()
+                        # logger.debug("Last message sent: %s", self.last_message_sent)
+
+                    return message.tx_sequence
+                except ConnectionResetError as ex:
+                    await self.close()
+                    raise UNiiConnectionError(str(ex)) from ex
 
         return None
 
 
 # UDP connections are currently not implemented.
 # class UNiiUDPConnection(UNiiConnection):
 #     """
```

### Comparing `unii-0.0.0.1/unii/unii_message.py` & `unii-1.0.0b1/unii/unii_message.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     UNiiData,
     UNiiDeviceStatus,
     UNiiDisarmSectionStatus,
     UNiiEquipmentInformation,
     UNiiEventRecord,
     UNiiInputArrangement,
     UNiiInputStatus,
+    UNiiInputStatusUpdate,
+    UNiiOutputArrangement,
     UNiiRawData,
     UNiiReadyToArmSectionStatus,
     UNiiResultCode,
     UNiiSectionArrangement,
     UNiiSectionStatus,
 )
 
@@ -114,19 +116,19 @@
 
     _CRC16_INIT: Final = 0x0000
     _CRC16_POLYNOMIAL: Final = 0x1021
     _CRC16_REFIN: Final = False
     _CRC16_REFOUT: Final = False
     _CRC16_XOROUT: Final = 0x0000
 
-    session_id: int = None
-    tx_sequence: int = None
-    rx_sequence: int = None
-    command: UNiiCommand = None
-    data: UNiiData = None
+    session_id: int | None = None
+    tx_sequence: int | None = None
+    rx_sequence: int | None = None
+    command: UNiiCommand | None = None
+    data: UNiiData | None = None
 
     def _calculate_crc16(self, message: bytes) -> int:
         """
         Calculates the CRC-16 checksum over the given message
         """
         crc = self._CRC16_INIT
         for _, byte in enumerate(message):
@@ -138,15 +140,14 @@
                 else:
                     crc <<= 1
         crc &= 0xFFFF
         # logger.debug("CRC-16 for 0x%s: %s", message.hex(), hex(crc))
         return crc
 
     def __str__(self) -> str:
-        # return "0x" + self._raw_message.hex()
         return str(
             {
                 "session_id": self.session_id,
                 "tx_sequence": self.tx_sequence,
                 "rx_sequence": self.rx_sequence,
                 "command": self.command,
                 "data": self.data,
@@ -157,18 +158,18 @@
 class UNiiRequestMessage(_UNiiMessage):
     """
     UNii Message class for sending
 
     All numbers are exchanged in big endian order (Most significant byte first)
     """
 
-    _protocol_id: UNiiProtocolID = None
+    _protocol_id: UNiiProtocolID | None = None
 
     @property
-    def packet_type(self) -> UNiiPacketType:
+    def packet_type(self) -> UNiiPacketType | None:
         """
         Get packet type based on command
         """
         if self.command is None:
             return None
         if self.command < 0x0008:
             return UNiiPacketType.SESSION_SETUP
@@ -216,15 +217,15 @@
 
         # variable length The actual data
         if self.data is not None:
             payload += self.data.to_bytes()
 
         return payload
 
-    def to_bytes(self, shared_key: bytes = None) -> bytes:
+    def to_bytes(self, shared_key: bytes | None = None) -> bytes:
         """
         Converts the UNii Message to a sequence of bytes
         """
         if shared_key is None:
             self._protocol_id = UNiiProtocolID.NO_ENCRYPTION
         else:
             self._protocol_id = UNiiProtocolID.BASIC_ENCRYPTION
@@ -274,22 +275,19 @@
     # pylint: disable=too-few-public-methods
     # pylint: disable=too-many-instance-attributes
     # pylint: disable=too-many-locals
     """
     UNii Message class for receiving
     """
 
-    _raw_message: bytes = None
-
-    def __init__(self, message: bytes, shared_key: bytes = None):
+    def __init__(self, message: bytes, shared_key: bytes | None = None):
+        # pylint: disable=too-many-statements
         """ """
         assert message is not None
 
-        self._raw_message = message
-
         # First 14 bytes Header
         header = message[:14]
         payload = message[14:-2]
         checksum = message[-2:]
 
         # Length
         packet_length = int.from_bytes(header[12:14])
@@ -314,15 +312,15 @@
         # Protocol ID
         protocol_id = UNiiProtocolID(header[10])
         # Packet Type
         # packet_type = UNiiPacketType(header[11])
         # Length
         # message_length = int.from_bytes(header[11:13])
 
-        if protocol_id == UNiiProtocolID.BASIC_ENCRYPTION:
+        if protocol_id == UNiiProtocolID.BASIC_ENCRYPTION and shared_key is not None:
             # As Initialization Vector for the encryption the first 12 bytes of the header are used.
             initial_value = header[:12]
             # The block counter is reset to 0 for every new message.
             initial_value += b"\00\00\00\00"
 
             payload = self._decrypt(shared_key, initial_value, payload)
 
@@ -335,15 +333,15 @@
             logger.warning(ex)
             self.command = None
 
         # Data length
         data_length = int.from_bytes(payload[2:4])
 
         # Data
-        data = None
+        data: bytes | UNiiData | None = None
         if data_length > 0:
             data = payload[4 : 4 + data_length]
             # logger.debug("%s data: %i bytes, 0x%s", self.command, len(data), data.hex())
             try:
                 match self.command:
                     # Generic
                     case UNiiCommand.GENERAL_RESPONSE:
@@ -363,25 +361,50 @@
                     case UNiiCommand.RESPONSE_DISARM_SECTION:
                         data = UNiiDisarmSectionStatus(data)
                     # Input related
                     case UNiiCommand.RESPONSE_REQUEST_INPUT_ARRANGEMENT:
                         data = UNiiInputArrangement(data)
                     case UNiiCommand.INPUT_STATUS_CHANGED:
                         data = UNiiInputStatus(data)
+                    case UNiiCommand.INPUT_STATUS_UPDATE:
+                        data = UNiiInputStatusUpdate(data)
+                    # Output related
+                    case UNiiCommand.RESPONSE_REQUEST_OUTPUT_ARRANGEMENT:
+                        data = UNiiOutputArrangement(data)
                     # Device related
                     case UNiiCommand.DEVICE_STATUS_CHANGED:
                         data = UNiiDeviceStatus(data)
                     # Event related
                     case UNiiCommand.EVENT_OCCURRED:
                         data = UNiiEventRecord(data)
                     case _:
                         data = UNiiRawData(data)
-            except (ValueError, LookupError) as ex:
+            except ValueError as ex:
+                data = None
+                if (
+                    self.command
+                    in [
+                        UNiiCommand.RESPONSE_REQUEST_INPUT_ARRANGEMENT,
+                        UNiiCommand.RESPONSE_REQUEST_OUTPUT_ARRANGEMENT,
+                    ]
+                    and str(ex) == "Invalid block number"
+                ):
+                    pass
+                else:
+                    logger.error(ex)
+                    logger.debug("Payload: 0x%s", payload.hex())
+            except LookupError as ex:
+                logger.error(ex)
+                logger.debug("Payload: 0x%s", payload.hex())
+                data = None
+            # Catch all exceptions while in development, to be removed once stable.
+            # pylint: disable=broad-exception-caught
+            except Exception as ex:
                 logger.error(ex)
-                # Fall back to raw data
-                data = UNiiRawData(data)
+                logger.debug("Payload: 0x%s", payload.hex())
+                data = None
         self.data = data
 
     def _decrypt(self, shared_key: bytes, initial_value: bytes, payload: bytes):
         aes = AES.new(shared_key, AES.MODE_CTR, initial_value=initial_value, nonce=b"")
 
         return aes.decrypt(payload)
```

