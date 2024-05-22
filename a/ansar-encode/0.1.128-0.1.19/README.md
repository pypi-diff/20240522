# Comparing `tmp/ansar_encode-0.1.128.tar.gz` & `tmp/ansar-encode-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_encode-0.1.128.tar", last modified: Wed May 22 01:08:13 2024, max compression
+gzip compressed data, was "ansar-encode-0.1.19.tar", last modified: Mon Oct  3 01:32:06 2022, max compression
```

## Comparing `ansar_encode-0.1.128.tar` & `ansar-encode-0.1.19.tar`

### file list

```diff
@@ -1,36 +1,32 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.547423 ansar_encode-0.1.128/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-18 03:22:14.000000 ansar_encode-0.1.128/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1567 2024-05-22 01:08:13.547423 ansar_encode-0.1.128/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      830 2023-04-19 07:09:52.000000 ansar_encode-0.1.128/README.md
--rw-rw-r--   0 scott     (1000) scott     (1000)      766 2023-12-12 15:27:28.000000 ansar_encode-0.1.128/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-22 01:08:13.547423 ansar_encode-0.1.128/setup.cfg
--rw-rw-r--   0 scott     (1000) scott     (1000)     2014 2023-12-25 14:22:44.000000 ansar_encode-0.1.128/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.539423 ansar_encode-0.1.128/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.539423 ansar_encode-0.1.128/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.539423 ansar_encode-0.1.128/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)     3673 2023-12-30 22:35:56.000000 ansar_encode-0.1.128/src/ansar/command/ansar_command.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.547423 ansar_encode-0.1.128/src/ansar/encode/
--rw-rw-r--   0 scott     (1000) scott     (1000)     6172 2024-05-22 01:08:10.000000 ansar_encode-0.1.128/src/ansar/encode/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     7542 2024-01-26 02:33:43.000000 ansar_encode-0.1.128/src/ansar/encode/args.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    37644 2024-03-22 18:42:35.000000 ansar_encode-0.1.128/src/ansar/encode/codec.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    16906 2024-05-09 12:34:53.000000 ansar_encode-0.1.128/src/ansar/encode/command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14953 2024-03-22 18:42:40.000000 ansar_encode-0.1.128/src/ansar/encode/convert.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10140 2024-03-22 18:42:44.000000 ansar_encode-0.1.128/src/ansar/encode/file.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    19686 2023-06-18 03:20:48.000000 ansar_encode-0.1.128/src/ansar/encode/folder.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3584 2023-07-13 03:32:34.000000 ansar_encode-0.1.128/src/ansar/encode/json.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34014 2024-03-22 18:42:49.000000 ansar_encode-0.1.128/src/ansar/encode/message.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10084 2023-07-13 03:32:38.000000 ansar_encode-0.1.128/src/ansar/encode/portable.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    11231 2024-02-13 14:54:40.000000 ansar_encode-0.1.128/src/ansar/encode/primitive.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9388 2023-12-30 22:33:57.000000 ansar_encode-0.1.128/src/ansar/encode/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3260 2023-12-18 13:32:24.000000 ansar_encode-0.1.128/src/ansar/encode/release.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5801 2024-03-22 18:42:55.000000 ansar_encode-0.1.128/src/ansar/encode/runtime.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     5873 2024-03-26 19:19:48.000000 ansar_encode-0.1.128/src/ansar/encode/support.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1787 2023-07-13 03:32:48.000000 ansar_encode-0.1.128/src/ansar/encode/version.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10434 2023-07-13 03:32:51.000000 ansar_encode-0.1.128/src/ansar/encode/xml.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-22 01:08:13.547423 ansar_encode-0.1.128/src/ansar_encode.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1567 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)      784 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       59 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       41 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-22 01:08:13.000000 ansar_encode-0.1.128/src/ansar_encode.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.459076 ansar-encode-0.1.19/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1106 2022-04-13 01:31:47.000000 ansar-encode-0.1.19/LICENSE
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2022-10-03 01:32:06.459076 ansar-encode-0.1.19/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      830 2022-10-02 23:59:34.000000 ansar-encode-0.1.19/README.md
+-rw-rw-r--   0 scott     (1000) scott     (1000)      309 2022-10-03 00:32:14.000000 ansar-encode-0.1.19/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2022-10-03 01:32:06.459076 ansar-encode-0.1.19/setup.cfg
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2148 2022-10-03 01:10:22.000000 ansar-encode-0.1.19/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.455076 ansar-encode-0.1.19/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.455076 ansar-encode-0.1.19/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.455076 ansar-encode-0.1.19/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10805 2022-08-28 22:05:19.000000 ansar-encode-0.1.19/src/ansar/command/show_release.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.459076 ansar-encode-0.1.19/src/ansar/encode/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     4952 2022-10-03 01:31:48.000000 ansar-encode-0.1.19/src/ansar/encode/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    37212 2022-09-25 21:38:09.000000 ansar-encode-0.1.19/src/ansar/encode/codec.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15863 2022-09-25 21:52:41.000000 ansar-encode-0.1.19/src/ansar/encode/convert.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11215 2022-09-07 08:49:07.000000 ansar-encode-0.1.19/src/ansar/encode/file.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    17474 2022-09-07 08:49:12.000000 ansar-encode-0.1.19/src/ansar/encode/folder.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2780 2022-08-03 00:55:21.000000 ansar-encode-0.1.19/src/ansar/encode/framework.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3719 2022-04-13 01:31:47.000000 ansar-encode-0.1.19/src/ansar/encode/json.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    30299 2022-10-02 01:29:00.000000 ansar-encode-0.1.19/src/ansar/encode/message.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10957 2022-09-21 20:36:53.000000 ansar-encode-0.1.19/src/ansar/encode/portable.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3334 2022-09-05 20:25:39.000000 ansar-encode-0.1.19/src/ansar/encode/release.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6031 2022-07-31 21:53:47.000000 ansar-encode-0.1.19/src/ansar/encode/runtime.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1644 2022-09-08 06:48:17.000000 ansar-encode-0.1.19/src/ansar/encode/version.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    11517 2022-08-03 00:49:03.000000 ansar-encode-0.1.19/src/ansar/encode/xml.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2022-10-03 01:32:06.459076 ansar-encode-0.1.19/src/ansar_encode.egg-info/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1482 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)      672 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       68 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       41 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2022-10-03 01:32:06.000000 ansar-encode-0.1.19/src/ansar_encode.egg-info/top_level.txt
```

### Comparing `ansar_encode-0.1.128/LICENSE` & `ansar-encode-0.1.19/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-Author: Scott Woods <scott.18.ansar@gmail.com.com>
+Author: Scott Woods <scott.suzuki@gmail.com>
 MIT License
 
-Copyright (c) 2017-2023 Scott Woods
+Copyright (c) 2017-2021
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ansar_encode-0.1.128/PKG-INFO` & `ansar-encode-0.1.19/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.128
+Version: 0.1.19
 Summary: Persistence of complex application data
 Author: Scott Woods
-Author-email: Scott Woods <scott.18.ansar@gmail.com>
-Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1/index.html
+Author-email: Scott Woods <scott.suzuki@gmail.com>
+Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defusedxml>=0.7.1
-Requires-Dist: python-dateutil>=2.8.1
 
 # ansar-encode
 
 The **ansar-encode** library provides for the convenient storage and recovery of
 application data using system files. Files are created using standard encodings - the
 default is JSON - and are human readable. Complex application data can be stored
 including containers, instances of classes and object graphs.
```

### Comparing `ansar_encode-0.1.128/README.md` & `ansar-encode-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `ansar_encode-0.1.128/src/ansar/encode/__init__.py` & `ansar-encode-0.1.19/src/ansar/encode/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2021
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -19,18 +19,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Persistence of complex application data.
 
-Repo: git@github.com:mr-ansar/ansar-encode.git
+Repo: git@ansar.gitlab.com:scott-ansar/ansar-encode.git
 Branch: main
-Commit: fa877641a1d03728d13c0c32d0ce61c9149f04a5
-Version: 0.1.127 (2024-05-22@13:08:10+NZST)
+Commit: d54e25fa53ee233533da84c8b72225ffa8d859a7
+Version: 0.1.18 (2022-10-03@14:31:48+NZDT)
 """
 
 from .portable import Boolean
 from .portable import Byte, Character, Rune
 from .portable import Integer2, Integer4, Integer8
 from .portable import Unsigned2, Unsigned4, Unsigned8
 from .portable import Float4, Float8
@@ -47,34 +47,35 @@
 from .portable import Word, Any
 from .portable import complete_list, complete_set
 from .portable import is_portable, is_container, is_structural, is_portable_class, is_container_class
 from .portable import NO_SUCH_ADDRESS
 from .portable import is_address, address_on_proxy
 from .portable import deque
 
-from .runtime import USER_LOG_FAULT, USER_LOG_WARNING, USER_LOG_CONSOLE, USER_LOG_OBJECT, USER_LOG_TRACE, USER_LOG_DEBUG, USER_LOG_NONE
-from .runtime import TAG_CREATED, TAG_DESTROYED, TAG_SENT, TAG_RECEIVED, TAG_STARTED, TAG_ENDED
-from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG, TAG_CHECK, TAG_SAMPLE
-from .runtime import tag_to_number
+from .runtime import USER_LOG_FAULT, USER_LOG_WARNING, USER_LOG_CONSOLE, USER_LOG_TRACE, USER_LOG_DEBUG, USER_LOG_NONE
+from .runtime import TAG_ANSAR
+from .runtime import TAG_CREATED, TAG_DESTROYED, TAG_SENT, TAG_RECEIVED, TAG_TRACKING
+from .runtime import TAG_FAULT, TAG_WARNING, TAG_CONSOLE, TAG_TRACE, TAG_DEBUG
+from .runtime import ANSAR_CREATED, ANSAR_DESTROYED, ANSAR_SENT, ANSAR_RECEIVED, ANSAR_TRACKING
+from .runtime import ANSAR_FAULT, ANSAR_WARNING, ANSAR_CONSOLE, ANSAR_TRACE, ANSAR_DEBUG
 from .runtime import Runtime
 from .runtime import CodingProblem, PlatformFailure
 
 from .message import MessageError, MessageRegistrationError
 from .message import Message, is_message, is_message_class
 from .message import Unknown, Incognito
 from .message import TypeTrack, correct_track
 from .message import default_clock, default_span
 from .message import default_world, default_delta, default_uuid
-from .message import default_array, default_vector, default_set, default_map, default_deque
-from .message import make, make_self, fake
+from .message import default_vector, default_set, default_map, default_deque
+from .message import make, make_member, make_self, make_value
 from .message import fix_expression, fix_schema, compile_schema, compile_history
 from .message import encode_type, decode_type
 from .message import Added, Moved, Deleted
-from .message import major_minor, bind_message, change_history, equal_to
-from .message import type_to_text
+from .message import major_minor, bind, change_history, equal_to
 from .message import INITIAL_VERSION, INITIAL_SUPPORT
 from .message import SCENARIO_INAPPROPRIATE, SCENARIO_UNSUPPORTED, SCENARIO_BEHIND, SCENARIO_AHEAD, SCENARIO_SAME
 from .message import version_scenario
 from .message import get_history, get_version, get_slice
 from .message import effective_type, type_version
 
 from .release import released_document
@@ -92,45 +93,16 @@
 from .codec import CodecError, CodecUsage, CodecFailed, EnumerationFailed
 from .codec import python_to_word, word_to_python
 from .codec import Codec
 
 from .json import word_to_json, json_to_word, CodecJson
 from .xml import word_to_xml, xml_to_word, CodecXml
 
-from .file import FileFailure, FileOpenFailure, FileNotFound, FileNoAccess, FileNotAFile, FileIOFailure, FileEncoding
+from .file import FileFailure, FileNotFound, FileNoAccess, FileNotAFile, FileIoFailed, FileEncoding
 from .file import File
 from .file import read_from_file, write_to_file
 
-from .folder import Folder, remove_contents, remove_folder, shape_of_folder
+from .folder import Folder
 
-from .version import migrate, cannot_upgrade
+from .framework import program_name, command_args
 
-from .support import Gas, breakpath, tof
-from .support import Incomplete
-from .support import jump_table
-from .support import show_fault, name_text
-from .support import Faulted, Rejected, Failed, FAULTED_SCHEMA
-
-from .primitive import CommandError
-from .primitive import value_type, word_argument, word_argument_2
-from .primitive import argv0, program_path, program_name, program_extent
-from .primitive import file_recover, file_store
-from .primitive import input_decode, output_encode
-from .primitive import output_line, output_human
-from .primitive import command_error
-
-from .procedure import VersioningSettings, CompareSettings, ReleaseSettings
-from .procedure import procedure_versioned, procedure_compare, procedure_release
-
-from .args import break_args, extract_args
-from .args import arg_values, environment_variables
-from .args import sub_args
-
-from .command import CommandSettings, command_settings
-from .command import command_variables, command_executable, command_args, command_unknown, command_words, command_custom_settings
-from .command import create_command, command_passing, sub_command_passing
-from .command import load_args, load_variables
-from .command import command_help
-
-# Provide default registration function at the
-# level of this library
-bind = bind_message
+from .version import migrate, cannot_upgrade
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/codec.py` & `ansar-encode-0.1.19/src/ansar/encode/codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2021
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -97,16 +97,20 @@
 
     def __init__(self, note):
         """Construct the exception.
 
         :param note: hint as to what happened
         :type name: str
         """
-        Exception.__init__(self, note)
-        self.note = note				# For quick access.
+        Exception.__init__(self)
+        self.note = note
+
+    def __str__(self):
+        """Auto-convert to text representation. Return string."""
+        return self.note
 
 class CodecUsage(CodecError):
     """Cannot proceed due to its supplied environment such as unusable parameters."""
 
     def __init__(self, note, *a):
         """Construct the exception.
 
@@ -337,38 +341,32 @@
     # Perhaps the JSON encoder passes this
     # through as a list anyway. No need for
     # transform?
     w = list(p)
     return w
 
 def p2w_address(c, p, t):
-	if c.space is not None:
-		i = len(c.space)
-		c.space.append(p)
-		return i
     # Check to see if an address is being
     # passed back over the connection it
     # arrived on. Prevents trombone behaviour.
     # Detection happens *here* at the remote
     # end of the trombone because this codec
     # knows it is sending an address back to
     # where it came from. Add the invalid point
     # id. See w2p_address.
-	if c.return_proxy is not None:
-		a = c.return_proxy
-		if p[-1] == a:
-			# Need to advise remote that address
-			# is returning to where it came from.
-			w = list(p[:-1])    # DROP THIS PROXY
-			#w = p[:-1]          # DROP THIS PROXY
-			w.append(0)         # SPECIAL MARK
-			return w
-	w = list(p)
-	#w = p
-	return w
+    if c.return_proxy is not None:
+        a = c.return_proxy
+        if p[-1] == a:
+            # Need to advise remote that address
+            # is returning to where it came from.
+            w = list(p[:-1])    # DROP THIS PROXY
+            w.append(0)         # SPECIAL MARK
+            return w
+    w = list(p)
+    return w
 
 def p2w_any(c, p, t):
     a = p.__class__
     if a == Incognito:          # Created during a previous decoding operation.
         t = p.type_name         # Global identifier
         w = p.decoded_word      # Generic body
         if p.saved_pointers:
@@ -425,16 +423,16 @@
     (bool, PointerTo): p2w_pointer,
     (int, PointerTo): p2w_pointer,
     (float, PointerTo): p2w_pointer,
     (bytearray, PointerTo): p2w_pointer,
     (bytes, PointerTo): p2w_pointer,
     (str, PointerTo): p2w_pointer,
     # ClockTime and TimeDelta. Float/ptr already in table.
-    # (float, PointerTo): p2w_pointer,
-    # (float, PointerTo): p2w_pointer,
+    #(float, PointerTo): p2w_pointer,
+    #(float, PointerTo): p2w_pointer,
     (datetime, PointerTo): p2w_pointer,
     (timedelta, PointerTo): p2w_pointer,
     (uuid.UUID, PointerTo): p2w_pointer,
     (list, PointerTo): p2w_pointer,
     (set, PointerTo): p2w_pointer,
     (dict, PointerTo): p2w_pointer,
     (deque, PointerTo): p2w_pointer,
@@ -482,20 +480,20 @@
     (NoneType, ClockTime): pass_thru,
     (NoneType, TimeSpan): pass_thru,
     (NoneType, WorldTime): pass_thru,
     (NoneType, TimeDelta): pass_thru,
     (NoneType, UUID): pass_thru,
     (NoneType, Enumeration): pass_thru,
     # DO NOT ALLOW
-    # (NoneType, UserDefined): pass_thru,
-    # (NoneType, ArrayOf): pass_thru,
-    # (NoneType, VectorOf): pass_thru,
-    # (NoneType, SetOf): pass_thru,
-    # (NoneType, MapOf): pass_thru,
-    # (NoneType, DequeOf): pass_thru,
+    #(NoneType, UserDefined): pass_thru,
+    #(NoneType, ArrayOf): pass_thru,
+    #(NoneType, VectorOf): pass_thru,
+    ##(NoneType, SetOf): pass_thru,
+    #(NoneType, MapOf): pass_thru,
+    #(NoneType, DequeOf): pass_thru,
     (NoneType, PointerTo): pass_thru,
     (NoneType, Type): pass_thru,
     (NoneType, TargetAddress): pass_thru,
     (NoneType, Address): pass_thru,
     (NoneType, Word): pass_thru,
     (NoneType, Any): pass_thru,
 }
@@ -739,39 +737,33 @@
             p.append(None)
             c.patch_work.append([d, patch])
     return p
 
 def w2p_target(c, w, t):
     if c.local_termination is None:
         p = tuple(w)
-        #p = w
     elif len(w) < 2:
         p = c.local_termination,
     else:
         p = tuple(w[:-1])
-        #p = w[:-1]
     return p
 
 def w2p_address(c, w, t):
-    if c.space is not None:
-        p = c.space[w]
-        return p
     if c.return_proxy is not None:
         # Clean out any trombone detected
         # in the remote. See p2w_address.
         a = w[-1]
         if a == 0:      # SPECIAL MARK
             # Address has returned home
             # No need to append a trip back
             # over this connection.
             w.pop()
         else:
             w.append(c.return_proxy)
     p = tuple(w)                 # Now convert.
-    #p = w                 # Now convert.
     return p
 
 def w2p_null_pointer(c, w, t):
     return [0, None]
 
 # Covert inbound 2-word tuple into the original
 # object
@@ -823,15 +815,14 @@
     (list, ArrayOf): w2p_array,
     (list, VectorOf): w2p_vector,
     (list, SetOf): w2p_set,
     (list, MapOf): w2p_map,
     (list, DequeOf): w2p_deque,
     (list, TargetAddress): w2p_target,
     (list, Address): w2p_address,
-    (int, Address): w2p_address,
     (str, PointerTo): w2p_pointer,
 
     # Two mechanisms for including messages
     # and the representation of message type.
     (dict, UserDefined): w2p_message,
     (list, Any): w2p_any,
     (str, Type): w2p_type,
@@ -869,20 +860,20 @@
     (NoneType, WorldTime): pass_thru,
     (NoneType, ClockTime): pass_thru,
     (NoneType, TimeSpan): pass_thru,
     (NoneType, UUID): pass_thru,
     (NoneType, Enumeration): pass_thru,
     # DO NOT allow the automatic acceptance
     # of None as a structured value.
-    # (NoneType, UserDefined): pass_thru,
-    # (NoneType, ArrayOf): pass_thru,
-    # (NoneType, VectorOf): pass_thru,
-    # (NoneType, SetOf): pass_thru,
-    # (NoneType, MapOf): pass_thru,
-    # (NoneType, DequeOf): pass_thru,
+    #(NoneType, UserDefined): pass_thru,
+    #(NoneType, ArrayOf): pass_thru,
+    #(NoneType, VectorOf): pass_thru,
+    #(NoneType, SetOf): pass_thru,
+    #(NoneType, MapOf): pass_thru,
+    #(NoneType, DequeOf): pass_thru,
     (NoneType, PointerTo): pass_thru,
     (NoneType, Type): pass_thru,
     (NoneType, TargetAddress): pass_thru,
     (NoneType, Address): pass_thru,
     (NoneType, Word): pass_thru,
     (NoneType, Any): pass_thru,
 }
@@ -957,32 +948,30 @@
         :type decorate_names: bool
         """
         self.extension = extension
         self.w2t = w2t
         self.t2w = t2w
 
         if return_proxy is None:
-            self.return_proxy = 0
-        elif not isinstance(return_proxy, (tuple, list)) or len(return_proxy) != 1:
+            self.return_proxy = 0,  # Tuple
+        elif not isinstance(return_proxy, tuple) or len(return_proxy) != 1:
             raise CodecUsage('unusable address passed as return proxy')
         else:
             self.return_proxy = return_proxy[0]
 
         if local_termination is None:
-            self.local_termination = 0
-        elif not isinstance(local_termination, (tuple, list)) or len(local_termination) != 1:
+            self.local_termination = 0,     # Tuple
+        elif not isinstance(local_termination, tuple) or len(local_termination) != 1:
             raise CodecUsage('unusable address passed as local termination')
         else:
             self.local_termination = local_termination[0]
 
         self.pretty_format = pretty_format
         self.decorate_names = decorate_names
 
-        self.space = None
-
         # Encode/decode collections
         self.walking_stack = []
         self.aliased_pointer = {}           # Encoding.
         self.portable_pointer = {}          # Both.
         self.pointer_reference = set()
         self.decoded_pointer = {}           # Decoding.
         self.patch_work = []
@@ -1019,27 +1008,26 @@
 
         # Provide full engine access.
         self.effective = effective      # Type of none
         self.version = version          # Selected or none
         self.latest = latest            # Latest version or none
         self.released = released        # Dict of sets of names or none
 
-    def encode(self, value, expression, version=None, space=None):
+    def encode(self, value, expression, version=None):
         """Encode an application value to its portable representation.
 
         :param value: a runtime application value
         :type value: a type consistent with the specified `expression`
         :param expression: a formal description of the `value`
         :type expression: :ref:`type expression<type-expressions>`
         :param version: an explicit version override
         :type version: string
         :return: a portable representation of the `value`
         :rtype: str
         """
-        self.space = space
         self.walking_stack = []         # Breadcrumbs for m.a[0].f.c[1] tracking.
         self.aliased_pointer = {}       # Pointers encountered in value.
         self.portable_pointer = {}      # Pointers accumulated from Incognitos.
         self.any_stack = [set()]
         self.pointer_alias = STARTING_ALIAS
 
         u4 = uuid.uuid4()
@@ -1080,25 +1068,23 @@
             # representation.
 
             s = self.w2t(self, shipment)
         except (TypeError, ValueError) as e:
             raise CodecFailed('serialization (%s)', str(e))
         return s
 
-    def decode(self, representation, expression, version=None, space=None):
+    def decode(self, representation, expression, version=None):
         """Decode a representation to its final application form.
 
         :param representation: the result of a previous encode operation
         :type representation: str
         :param expression: a formal description of portable
         :type expression: a :ref:`type expression<type-expressions>`
         :return: an application value
         """
-        self.space = space
-
         self.walking_stack = []         # Breadcrumbs for m.a[0].f.c[1] tracking.
         self.portable_pointer = {}      # Shipped pointer materials.
         self.decoded_pointer = {}       # Pointers transformed to final type.
         self.patch_work = []
 
         self.versioning(expression, version)    # Establish versioning context.
 
@@ -1129,16 +1115,14 @@
             # and save into convenient map. Does not transform
             # into final types.
             flat = shipment['pointer']
             portable = decode(flat, MapOf(Word(), Word()))
             self.portable_pointer.update(portable)  # Use EXISTING portable_pointer
         except KeyError:
             pass
-        except (AttributeError, TypeError, ValueError, IndexError):
-            raise CodecFailed('unexpected input (not the output of an encoding?)')
 
         try:
             w = shipment['value']
         except KeyError:
             raise CodecFailed('no "value" available')
 
         # Decode the word to its final application resting-place. This performs
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/folder.py` & `ansar-encode-0.1.19/src/ansar/encode/folder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2022 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -36,17 +36,14 @@
 
 # .. autoclass:: Folder
 #   :members:
 #   :no-undoc-members:
 
 __all__ = [
     'Folder',
-    'remove_folder',
-    'remove_contents',
-    'shape_of_folder',
 ]
 
 import os
 import errno
 import re as regex
 
 from .portable import *
@@ -57,84 +54,31 @@
 from .file import *
 
 CREATE_FOLDER = 'create folder'
 REMOVE_FOLDER = 'remove folder'
 REMOVE_FILE = 'remove file'
 #
 #
-def remove_contents(path):
-    """Delete everything under the given folder, down."""
-
-    what = 'remove contents from'
+def remove_folder(path):
     try:
         for f in os.listdir(path):
             p = os.path.join(path, f)
             if os.path.isdir(p):
                 remove_folder(p)
             elif os.path.isfile(p):
                 os.remove(p)
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            return
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(what, path, 'access or permissions')
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(what, path, 'name in path is not a folder')
-        elif e.errno == errno.EISDIR:
-            raise FileNotAFile(what, path, 'name refers to a folder')
-        raise FileFailure(what, path, e.strerror, e.errno)
-
-#
-#
-def remove_folder(path):
-    """Delete everything under the given folder, and then the folder."""
-
-    remove_contents(path)
-
-    what = 'remove folder'
-
-    try:
         os.rmdir(path)
     except OSError as e:
         if e.errno == errno.ENOENT:
-            return
+            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist', e.errno)
         elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(what, path, 'access or permissions')
+            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions', e.errno)
         elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(what, path, 'name in path is not a folder')
-        raise FileFailure(what, path, e.strerror, e.errno)
-
-#
-#
-def shape_of_folder(path):
-    """Walk the given folder, acumulating folders, files and bytes (3-tuple)."""
-    folders, files, bytes = 0, 0, 0
-    try:
-        p = path
-        for f in os.listdir(path):
-            p = os.path.join(path, f)
-            if os.path.isdir(p):
-                folders += 1
-                fo, fi, by = shape_of_folder(p)
-                folders += fo
-                files += fi
-                bytes += by
-            elif os.path.isfile(p):
-                s = os.stat(p)
-                files += 1
-                bytes += s.st_size
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            raise FileNotFound(REMOVE_FOLDER, p, 'name does not exist')
-        elif e.errno in (errno.EACCES, errno.EPERM):
-            raise FileNoAccess(REMOVE_FOLDER, p, 'access or permissions')
-        elif e.errno == errno.ENOTDIR:
-            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder')
-        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', e.errno)
-    return folders, files, bytes
+            raise FileNotAFile(REMOVE_FOLDER, p, 'name in path is not a folder', e.errno)
+        raise FileFailure(REMOVE_FOLDER, p, 'unexpected platform code', code=0)
 
 #
 #
 class Folder(object):
     """Create and manage a collection of application values, using a folder.
 
     :param path: the location in the filesystem
@@ -149,23 +93,21 @@
     :type pretty_format: bool
     :param decorate_names: auto-append an encoding-dependent extension to the file name, defaults to ``True``
     :type decorate_names: bool
     :param keys_names: a key-composer function and a name-composer function
     :type keys_names: 2-tuple of functions
     :param make_absolute: expand a relative path to be an absolute location, defaults to ``True``
     :type make_absolute: bool
-    :param auto_create: create folders as necessary, defaults to ``True``
-    :type auto_create: bool
     """
 
     def __init__(self, path=None,
             te=None, re=None, encoding=None,
             pretty_format=True, decorate_names=True,
             create_default=False, keys_names=None,
-            make_absolute=True, auto_create=True):
+            make_absolute=True):
         """Construct a Folder instance."""
         path = path or '.'
         if make_absolute:
             path = os.path.abspath(path)
         if te:
             te = fix_expression(te, dict())
         self.path = path
@@ -175,32 +117,28 @@
             self.re = regex.compile(re)
         self.te = te
         self.encoding = encoding or CodecJson
         self.pretty_format = pretty_format
         self.decorate_names = decorate_names
         self.create_default = create_default
         self.keys_names = keys_names
-        self.auto_create = auto_create
 
-        if not auto_create:
-            return
         try:
             os.makedirs(self.path)
         except OSError as e:
             if e.errno == errno.EEXIST:
                 return
             elif e.errno in (errno.EACCES, errno.EPERM):
-                raise FileNoAccess(CREATE_FOLDER, self.path, 'access or permissions')
+                raise FileNoAccess(CREATE_FOLDER, self.path, 'access or permissions', code=e.errno)
             elif e.errno == errno.ENOTDIR:
-                raise FileNotAFile(CREATE_FOLDER, self.path, 'name in path is not a folder')
-            raise FileFailure(CREATE_FOLDER, self.path, 'unexpected platform code', e.errno)
+                raise FileNotAFile(CREATE_FOLDER, self.path, 'name in path is not a folder', code=e.errno)
+            raise FileFailure(CREATE_FOLDER, self.path, 'unexpected platform code', code=e.errno)
 
     def folder(self, name, te=None, re=None, encoding=None,
-            pretty_format=None, decorate_names=None, create_default=None,
-            auto_create=None, keys_names=None):
+            pretty_format=None, decorate_names=None, create_default=None, keys_names=None):
         """Create a new :py:class:`~ansar.folder.Folder` object representing a sub-folder at the current location.
 
         :param path: the name to be added to the saved ``path``
         :type path: str
         :param te: formal description of the content
         :type te: :ref:`type expression<type-expressions>`
         :param re: formal description of expected file names
@@ -211,37 +149,34 @@
         :type pretty_format: bool
         :param decorate_names: auto-append an encoding-dependent extension to the file name, defaults to ``True``
         :type decorate_names: bool
         :param keys_names: a key-composer function and a name-composer function
         :type keys_names: 2-tuple of functions
         :param make_absolute: expand a relative path to be an absolute location, defaults to ``True``
         :type make_absolute: bool
-        :param auto_create: create folders as necessary, defaults to ``None``
-        :type auto_create: bool
         :return: a new location in the filesystem
         :rtype: :py:class:`~ansar.folder.Folder`
         """
         if te:
             te = fix_expression(te, dict())
         te = te or self.te
         if re is None:
             self.re = None
         else:
             self.re = regex.compile(re)
         encoding = encoding or self.encoding
         if pretty_format is None: pretty_format = self.pretty_format
         if decorate_names is None: decorate_names = self.decorate_names
         if create_default is None: create_default = self.create_default
-        if auto_create is None: auto_create = self.auto_create
         keys_names = keys_names or self.keys_names
 
         path = os.path.join(self.path, name)
         return Folder(path, re=re, te=te, encoding=encoding,
             pretty_format=pretty_format, decorate_names=decorate_names, create_default=create_default,
-            keys_names=keys_names, make_absolute=False, auto_create=auto_create)
+            keys_names=keys_names, make_absolute=False)
 
     def file(self, name, te, encoding=None,
             pretty_format=None, decorate_names=None, create_default=None):
         """Create a new :py:class:`~ansar.file.File` object representing a file at the current location.
 
         :param name: the name to be added to the saved ``path``
         :type name: str
@@ -285,15 +220,15 @@
                 continue
             if decorate_names:
                 b, e = os.path.splitext(f)
                 if e != extension:
                     continue
                 f = b
             if re:
-                m = re.fullmatch(f)
+                m = re.match(f)
                 if not m:
                     continue
             yield f
 
     def each(self):
         """Process the files in the folder.
 
@@ -376,58 +311,58 @@
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be added
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('add to', self.path, 'key/name functions not set', None)
+            raise FileFailure('add to', self.path, 'key/name functions not set', code=0)
 
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         io = self.file(name, self.te)
         if key in values:
-            raise FileFailure('add', io.name, 'entry already present', None)
+            raise FileFailure('add', io.name, 'entry already present', code=0)
         io.store(item)
         values[key] = item
 
     def update(self, values, item):
         """Update a value, both in a ``dict`` of values and as a file in the folder.
 
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be updated
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('update', self.path, 'key/name functions not set', None)
+            raise FileFailure('update', self.path, 'key/name functions not set', code=0)
 
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         io = self.file(name, self.te)
         if key not in values:
-            raise FileFailure('update', io.name, 'not an existing entry', None)
+            raise FileFailure('update', io.name, 'not an existing entry', code=0)
 
         io.store(item)
         values[key] = item
 
     def remove(self, values, item):
         """Remove a value, both from a ``dict`` of values and as a file in the folder.
 
         :param values: a collection of application values
         :type values: dict
         :param item: the value to be removed
         :type item: refer to ``Folder.te``
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('remove from', self.path, 'key/name functions not set', None)
+            raise FileFailure('remove from', self.path, 'key/name functions not set', code=0)
         key = keys_names[0](item)
         name = keys_names[1](item)
 
         self.erase(name)
         del values[key]
 
     def clear(self, values):
@@ -452,39 +387,36 @@
         path = os.path.join(self.path, name)
         name = path
         if self.decorate_names:
             name = '%s.%s' % (path, self.encoding.EXTENSION)
         if os.path.isfile(name):
             try:
                 os.remove(name)
-            except OSError as e:
+            except IOError as e:
                 if e.errno == errno.ENOENT:
-                    raise FileNotFound(REMOVE_FILE, name, 'name does not exist')
+                    raise FileNotFound(REMOVE_FILE, name, 'name does not exist', e.errno)
                 elif e.errno in (errno.EACCES, errno.EPERM):
-                    raise FileNoAccess(REMOVE_FILE, name, 'access or permissions')
+                    raise FileNoAccess(REMOVE_FILE, name, 'access or permissions', e.errno)
                 elif e.errno == errno.ENOTDIR:
-                    raise FileNotAFile(REMOVE_FILE, name, 'name in path is not a folder')
-                raise FileFailure(REMOVE_FILE, name, 'unexpected platform code', e.errno)
+                    raise FileNotAFile(REMOVE_FILE, name, 'name in path is not a folder', e.errno)
+                raise FileFailure(REMOVE_FILE, name, 'unexpected platform code', code=0)
             return True
         elif os.path.isdir(path):
             remove_folder(path)
             return True
         return False
 
-    def exists(self, name=None):
+    def exists(self, name):
         """Detect the named file, within the folder.
 
         :param name: a name of a file
         :type name: str
         :return: does the file exist
         :rtype: bool
         """
-        if name is None:
-            return os.path.isdir(self.path)
-
         path = os.path.join(self.path, name)
         name = path
         if self.decorate_names:
             name = '%s.%s' % (path, self.encoding.EXTENSION)
         if os.path.isfile(name):
             return True
         elif os.path.isdir(path):
@@ -497,22 +429,22 @@
         :param item: an application value
         :type name: see ``Folder.te``
         :return: the key
         :rtype: folder dependent
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('compose key', self.path, 'key/name functions not set', None)
+            raise FileFailure('compose key', self.path, 'key/name functions not set', code=0)
         return keys_names[0](item)
 
     def name(self, item):
         """Generate the stable filename for a given application value.
 
         :param item: an application value
         :type name: see ``Folder.te``
         :return: the filename
         :rtype: str
         """
         keys_names = self.keys_names
         if keys_names is None:
-            raise FileFailure('compose name', self.path, 'key/name functions not set', None)
+            raise FileFailure('compose name', self.path, 'key/name functions not set', code=0)
         return keys_names[1](item)
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/json.py` & `ansar-encode-0.1.19/src/ansar/encode/json.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2021
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -50,66 +50,66 @@
 from .convert import *
 from .runtime import *
 from .message import *
 from .codec import *
 
 
 __all__ = [
-	'word_to_json',
-	'json_to_word',
-	'CodecJson'
+    'word_to_json',
+    'json_to_word',
+    'CodecJson'
 ]
 
 # Standard JSON library version of generation and
 # parsing of standard-conforming text.
 def word_to_json(c, w):
-	"""Generate the JSON representation of a generic word.
+    """Generate the JSON representation of a generic word.
 
-	If the codec `pretty_format` property is true, this
-	function will produce a more human-readable rendering
-	of JSON.
-
-	:param c: an active codec
-	:type c: a Codec-based object
-	:param w: a generic word
-	:rtype: the JSON text.
-	"""
-	if c.pretty_format:
-		j = json.dumps(w, sort_keys=True, indent=4, separators=(',', ': '))
-	else:
-		j = json.dumps(w, separators=(',', ':'))
-	return j
+    If the codec `pretty_format` property is true, this
+    function will produce a more human-readable rendering
+    of JSON.
+
+    :param c: an active codec
+    :type c: a Codec-based object
+    :param w: a generic word
+    :rtype: the JSON text.
+    """
+    if c.pretty_format:
+        j = json.dumps(w, sort_keys=True, indent=4, separators=(',', ': '))
+    else:
+        j = json.dumps(w, separators=(',', ':'))
+    return j
 
 # Decoding - from parsing of JSON to transformation
 # into app data items.
 
 def json_to_word(c, j):
-	"""Produce a generic word from the parsing of a text JSON representation.
+    """Produce a generic word from the parsing of a text JSON representation.
 
-	:param c: an active codec
-	:type c: a Codec-based instance
-	:param j: the JSON text
-	:type j: string
-	:rtype: a generic word.
-	"""
-	j = json.loads(j)
-	return j
+    :param c: an active codec
+    :type c: a Codec-based instance
+    :param j: the JSON text
+    :type j: string
+    :rtype: a generic word.
+    """
+    j = json.loads(j)
+    return j
 
 #
 #
 class CodecJson(Codec):
-	"""Encoding and decoding of JSON representations.
+    """Encoding and decoding of JSON representations.
 
-	This class is the default value for the ``encoding`` parameter, related
-	to the various store and recover operations of the library. Refer to the
-	:ref:`base codec class<codec-base>` for the significant methods.
-	"""
-
-	EXTENSION = 'json'
-
-	def __init__(self, return_proxy=None, local_termination=None, pretty_format=False, decorate_names=True):
-		"""Construct a JSON codec."""
-		Codec.__init__(self,
-			CodecJson.EXTENSION,
-			word_to_json,
-			json_to_word,
-			return_proxy, local_termination, pretty_format, decorate_names)
+    This class is the default value for the ``encoding`` parameter, related
+    to the various store and recover operations of the library. Refer to the
+    :ref:`base codec class<codec-base>` for the significant methods.
+    """
+
+    EXTENSION = 'json'
+
+    def __init__(self, return_proxy=None, local_termination=None, pretty_format=False, decorate_names=True):
+        """Construct a JSON codec."""
+        Codec.__init__(self,
+            CodecJson.EXTENSION,
+            word_to_json,
+            json_to_word,
+            return_proxy, local_termination, pretty_format, decorate_names)
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/message.py` & `ansar-encode-0.1.19/src/ansar/encode/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2021
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -33,26 +33,27 @@
 .. autoclass:: Incognito
 
 .. autofunction:: default_clock
 .. autofunction:: default_span
 .. autofunction:: default_world
 .. autofunction:: default_delta
 .. autofunction:: default_uuid
-.. autofunction:: default_array
 .. autofunction:: default_vector
 .. autofunction:: default_set
 .. autofunction:: default_map
 .. autofunction:: default_deque
 
 .. autofunction:: make
+.. autofunction:: make_member
 .. autofunction:: make_self
+.. autofunction:: make_value
 
 .. autofunction:: decode_type
 .. autofunction:: encode_type
-.. autofunction:: bind_message
+.. autofunction:: bind
 """
 
 __docformat__ = 'restructuredtext'
 
 import sys
 import uuid
 from datetime import MINYEAR, datetime, timedelta, timezone
@@ -83,16 +84,17 @@
     'default_vector',
     'default_set',
     'default_map',
     'default_deque',
 
     # Require parameters.
     'make',
+    'make_member',
     'make_self',
-    'fake',
+    'make_value',
 
     'is_message',
     'is_message_class',
 
     'fix_expression',
     'fix_schema',
     'compile_schema',
@@ -102,20 +104,18 @@
     'decode_type',
 
     'Added',
     'Moved',
     'Deleted',
 
     'major_minor',
-    'bind_message',
+    'bind',
     'change_history',
     'equal_to',
 
-    'type_to_text',
-
     'INITIAL_VERSION',
     'INITIAL_SUPPORT',
     'SCENARIO_INAPPROPRIATE',
     'SCENARIO_UNSUPPORTED',
     'SCENARIO_BEHIND',
     'SCENARIO_AHEAD',
     'SCENARIO_SAME',
@@ -207,16 +207,15 @@
 
 def is_message_class(c):
     """Has *c* been registered with the library; return a bool."""
     try:
         p = c.__class__     # Parent class.
     except AttributeError:
         return hasattr(c, '__art__')
-    a = getattr(c, '__art__', None)
-    b = a is not None and a.name == c.__name__
+    b = not hasattr(p, '__art__') and hasattr(c, '__art__')
     return b
 
 # Holds nested names that would be helpful in the event
 # of an error.
 class TypeTrack(Exception):
     """Construct a readable name for a message.member.member, during exceptions."""
 
@@ -339,22 +338,14 @@
     """Initialize a UUID variable.
 
     :return: a global, constant UUID value
     :rtype: uuid.UUID
     """
     return DEFAULT_UUID
 
-def default_array(value, size):
-    """Initialize a vector variable.
-
-    :return: a fresh, empty vector
-    :rtype: list
-    """
-    return [value] * size   # New object.
-
 def default_vector():
     """Initialize a vector variable.
 
     :return: a fresh, empty vector
     :rtype: list
     """
     return list()   # New object.
@@ -391,34 +382,40 @@
     :param te: see :ref:`type expression<type-expressions>`
     :return: an item of application data
     """
     f = fix_expression(e, dict())
     v = from_type(f)
     return v
 
+def make_member(a, k, schema):
+    """Initialize the named member of an object to a useful default, if the default is None."""
+    v = getattr(a, k)
+    if v is None:
+        t = schema[k]
+        v = from_type(t)
+        setattr(a, k, v)
+
 def make_self(a, schema):
     """Initialize all the members of an object that are not present or set to None, to a useful default."""
     for k, t in schema.items():
         v = getattr(a, k)
         if v is None:
             v = from_type(t)
             setattr(a, k, v)
 
-#
-#
-def fake(e):
-    """Fake an instance of any variable starting from a type expression.
-
-    :param e: see :ref:`type expression<type-expressions>`
-    :return: an item of application data
-    """
-    v = fake_type(e)
+def make_value(a, k):
+    """Form a proper value for the named member of the object."""
+    rt = a.__art__
+    # Forces and AttributeError on the caller for
+    # improper use.
+    schema = rt.value
+    t = schema[k]
+    v = from_type(t)
     return v
 
-
 # Allow the use of basic python types
 # in type expressions.
 equivalent = {
     bool: Boolean(),
     int: Integer8(),
     float: Float8(),
     datetime: WorldTime(),
@@ -746,112 +743,14 @@
     if isinstance(t, UserDefined):
         return t.element()
 
     raise MessageRegistrationError(None, 'internal failure to create from memory')
 
 #
 #
-def character_bytes(): return b'c'
-def rune_str(): return 'C'
-def block_bytearray(): return bytearray([0x0c, 0x0a, 0x0f, 0x0e])
-def string_bytes(): return b'CAFE'
-def unicode_str(): return 'CAFE'
-
-def fake_clock(): return datetime(1963, 3, 26).timestamp()
-def fake_span(): return 0.5
-def fake_world(): return datetime(1963, 3, 26)
-def fake_delta(): return timedelta(seconds=0.5)
-def fake_uuid(): return uuid.uuid4()
-def fake_type_(): return Unknown
-def fake_target(): return [0x0c, 0x0a, 0x0f, 0x0e]
-def fake_address(): return [0x0c, 0x0a, 0x0f, 0x0e]
-def fake_any(): return Unknown()
-
-fake_class = {
-    Boolean: bool,
-    Byte: int,
-    Character: character_bytes,
-    Rune: rune_str,
-    Integer2: int,
-    Integer4: int,
-    Integer8: int,
-    Unsigned2: int,
-    Unsigned4: int,
-    Unsigned8: int,
-    Float4: float,
-    Float8: float,
-    Block: block_bytearray,
-    String: string_bytes,
-    Unicode: unicode_str,
-    Enumeration: lambda: "MOTORCYCLE",
-    ClockTime: fake_clock,
-    TimeSpan: fake_span,
-    WorldTime: fake_world,
-    TimeDelta: fake_delta,
-    UUID: fake_uuid,
-    Type: fake_type_,
-    TargetAddress: fake_target,
-    Address: fake_address,
-    Any: fake_any,
-}
-
-def fake_type(t):
-    """Synthesizes an example of the Python equivalent, or None."""
-    if not is_portable(t):
-        raise MessageRegistrationError(None, 'non-memory type presented for construction - %r' % (t,))
-
-    try:
-        c = fake_class[t.__class__]
-        return c()
-    except KeyError:
-        pass
-    except AttributeError:
-        raise MessageRegistrationError(None, 'internal failure to create from class')
-
-    # Following types are more involved - cant be
-    # ctor'd solely from the class.
-    if isinstance(t, VectorOf):
-        e = fake_type(t.element)
-        d = [e]
-        return d
-    elif isinstance(t, ArrayOf):
-        d = [None] * t.size
-        for i in range(t.size):
-            d[i] = fake_type(t.element)
-        return d
-    elif isinstance(t, DequeOf):
-        e = fake_type(t.element)
-        d = deque()
-        d.append(e)
-        return d
-    elif isinstance(t, SetOf):
-        e = fake_type(t.element)
-        d = set()
-        d.add(e)
-        return d
-    elif isinstance(t, MapOf):
-        k = fake_type(t.key)
-        v = fake_type(t.value)
-        d = {}
-        d[k] = v
-        return d
-    elif isinstance(t, UserDefined):
-        element = t.element
-        schema = element.__art__.value
-        d = element()
-        for k, v in schema.items():
-            setattr(d, k, fake_type(v))
-        return d
-    elif isinstance(t, PointerTo):
-        return fake_type(t.element)
-
-    raise MessageRegistrationError(None, 'internal failure to create from memory')
-
-#
-#
 def decode_type(s):
     """Convert the dotted string *s* to a class, or None."""
     try:
         i = s.rindex('.')
     except ValueError:
         return None
     module = s[:i]
@@ -881,15 +780,15 @@
         """Add *name* to the set of expected members."""
         self.name = name
 
 class Moved(object):
     """Perfom a rename within the history of a class."""
 
     def __init__(self, previous, latest):
-        """Remove *previous* and replace with *latest* in the set of expected members."""
+        """Remove *previous* and replace with "latest" in the set of expected members."""
         self.previous = previous
         self.latest = latest
 
 class Deleted(object):
     """Perfom a deletion within the history of a class."""
 
     def __init__(self, name):
@@ -1037,15 +936,15 @@
     noop = b == INITIAL_VERSION and e == INITIAL_VERSION
     if noop:
         return None
     return e
 
 #
 #
-def bind_message(message, object_schema=None, version_history=None,
+def bind(message, object_schema=None, version_history=None,
         message_trail=True, execution_trace=True,
         copy_before_sending=True, not_portable=False):
     """Set the type information and runtime controls for the given message type.
 
     :param message: a message class.
     :type message: class
     :param object_schema: application-supplied type information.
@@ -1095,23 +994,23 @@
     rt.version_history = history
     if history and rt.value:
         rt.version_slice = compile_history(history, rt.value, rt.name)
     else:
         rt.version_slice = None
     return previous
 
-bind_message(Unknown)
+bind(Unknown)
 
 # This should not need be needed as they are never on-the-wire.
 # But registration needed for dispatching within encode/decode
 # process.
-bind_message(Incognito, object_schema={
-    'type_name': Unicode,
+bind(Incognito, object_schema={
+    'type_name': String,
     'decoded_word': Word,
-    'saved_pointers': MapOf(Unicode, Word),
+    'saved_pointers': MapOf(String, Word),
 })
 
 def equal_to(a, b, t=None):
     """Compare the two operands as instances of portable memory."""
     if t is None:
         if not is_message(b):
             return a == b
@@ -1160,39 +1059,7 @@
         return False
     elif isinstance(t, Any):
         if equal_to(a, b):
             return True
         return False
     else:
         return a == b
-
-#
-#
-NON_CONTAINER = {t: '%s()' % (t.__name__,) for t in complete_list if not is_container_class(t)}
-
-def type_to_text(t, bread={}):
-    """."""
-    try:
-        s = NON_CONTAINER[type(t)]
-        return s
-    except KeyError:
-        pass
-
-    if isinstance(t, UserDefined):
-        return 'UserDefined({element})'.format(element=t.element.__art__.path)
-    elif isinstance(t, (VectorOf, ArrayOf, DequeOf, SetOf)):
-        container = t.__class__.__name__
-        element = type_to_text(t.element, bread)
-        return '{container}({element})'.format(container=container, element=element)
-    elif isinstance(t, MapOf):
-        key = type_to_text(t.key, bread)
-        value = type_to_text(t.value, bread)
-        return 'MapOf({key},{value})'.format(key=key, value=value)
-    elif isinstance(t, PointerTo):
-        k = id(t)
-        try:
-            e = bread[k]
-        except KeyError:
-            e = type_to_text(t.element, bread)
-            bread[k] = e
-        return 'PointerTo({element})'.format(element=e)
-    return None
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/portable.py` & `ansar-encode-0.1.19/src/ansar/encode/portable.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2021
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -86,363 +86,363 @@
 import sys
 import time
 import calendar
 import re
 import uuid
 
 __all__ = [
-	'Portable',
-	'Container',
+    'Portable',
+    'Container',
 
-	'Boolean',		  # The basic types. Integrals.
-	'Byte',
-	'Character',
-	'Rune',
-	'Integer2',
-	'Integer4',
-	'Integer8',
-	'Unsigned2',
-	'Unsigned4',
-	'Unsigned8',
-
-	'Float4',		   # Floating point.
-	'Float8',
-
-	'Block',			# Sequence of basic units
-	'String',
-	'Unicode',
-
-	'Enumeration',
-
-	'ClockTime',		# Time.
-	'TimeSpan',
-	'WorldTime',
-	'TimeDelta',
-
-	'UUID',			 # UUID - RFC 4122
-
-	'ArrayOf',		  # Containers.
-	'VectorOf',
-	'SetOf',
-	'MapOf',
-	'DequeOf',
-
-	'UserDefined',	  # User-defined type.
-	'Type',			 # Type of a message.
-	'PointerTo',		# Reference to one of the above.
-
-	'TargetAddress',	# Destination.
-	'Address',		  # An address, such as the sender.
-
-	'Word',			 # Instance of generic form, e.g. results of python_to_word
-	'Any',			  # Any message - on-the-wire, a tuple of Type and Word.
-
-	'complete_list',
-	'complete_set',
-
-	'is_portable',
-	'is_container',
-	'is_structural',
-	'is_portable_class',
-	'is_container_class',
+    'Boolean',          # The basic types. Integrals.
+    'Byte',
+    'Character',
+    'Rune',
+    'Integer2',
+    'Integer4',
+    'Integer8',
+    'Unsigned2',
+    'Unsigned4',
+    'Unsigned8',
+
+    'Float4',           # Floating point.
+    'Float8',
+
+    'Block',            # Sequence of basic units
+    'String',
+    'Unicode',
+
+    'Enumeration',
+
+    'ClockTime',        # Time.
+    'TimeSpan',
+    'WorldTime',
+    'TimeDelta',
+
+    'UUID',             # UUID - RFC 4122
+
+    'ArrayOf',          # Containers.
+    'VectorOf',
+    'SetOf',
+    'MapOf',
+    'DequeOf',
+
+    'UserDefined',      # User-defined type.
+    'Type',             # Type of a message.
+    'PointerTo',        # Reference to one of the above.
+
+    'TargetAddress',    # Destination.
+    'Address',          # An address, such as the sender.
+
+    'Word',             # Instance of generic form, e.g. results of python_to_word
+    'Any',              # Any message - on-the-wire, a tuple of Type and Word.
+
+    'complete_list',
+    'complete_set',
+
+    'is_portable',
+    'is_container',
+    'is_structural',
+    'is_portable_class',
+    'is_container_class',
 
-	'NO_SUCH_ADDRESS',  # A properly formed "null" address.
+    'NO_SUCH_ADDRESS',  # A properly formed "null" address.
 
-	'is_address',	   # Can be used to direct movement.
-	'address_on_proxy',
+    'is_address',       # Can be used to direct movement.
+    'address_on_proxy',
 
-	'deque',			# Auto-inject into namespace.
+    'deque',            # Auto-inject into namespace.
 ]
 
 # Each class is used to describe a unit
 # of memory.
 class Portable(object):
-	"""Base for all portables."""
+    """Base for all portables."""
 
 class Container(Portable):
-	"""The subset of portables that contain zero or more portables."""
+    """The subset of portables that contain zero or more portables."""
 
 class Boolean(Portable):
-	"""True or false."""
+    """True or false."""
 
 class Byte(Portable):
-	"""The smallest unit of data - 8 bit, unsigned integer."""
+    """The smallest unit of data - 8 bit, unsigned integer."""
 
 class Character(Portable):
-	"""A byte that more often contains a printable ASCII character, than not."""
+    """A byte that more often contains a printable ASCII character, than not."""
 
 class Rune(Portable):
-	"""A Unicode codepoint."""
+    """A Unicode codepoint."""
 
 
 class Integer2(Portable):
-	"""A 2-byte, signed integer."""
+    """A 2-byte, signed integer."""
 
 class Integer4(Portable):
-	"""A 4-byte, signed integer."""
+    """A 4-byte, signed integer."""
 
 class Integer8(Portable):
-	"""An 8-byte, signed integer."""
+    """An 8-byte, signed integer."""
 
 class Unsigned2(Portable):
-	"""A 2-byte, unsigned integer."""
+    """A 2-byte, unsigned integer."""
 
 class Unsigned4(Portable):
-	"""A 4-byte, unsigned integer."""
+    """A 4-byte, unsigned integer."""
 
 class Unsigned8(Portable):
-	"""An 8-byte, unsigned integer."""
+    """An 8-byte, unsigned integer."""
 
 class Float4(Portable):
-	"""A 4-byte, floating point number."""
+    """A 4-byte, floating point number."""
 
 class Float8(Portable):
-	"""An 8-byte, floating point number."""
+    """An 8-byte, floating point number."""
 
 
 class Block(Portable):
-	"""A sequence of Byte."""
+    """A sequence of Byte."""
 
 class String(Portable):
-	"""A sequence of Characters."""
+    """A sequence of Characters."""
 
 class Unicode(Portable):
-	"""A sequence of codepoints."""
+    """A sequence of codepoints."""
 
 class Enumeration(Portable):
-	"""Integers that have names.
+    """Integers that have names.
 
-	:param kv: map of strings and their integer value.
-	:type kv: dict
-	"""
-
-	def __init__(self, **kv):
-		"""Refer to class."""
-		self.kv = kv
-		for k, v in kv.items():
-			setattr(self, k, v)
-		self.vk = {v: k for k, v in kv.items()}
-
-	def to_name(self, v):
-		"""Accept an integer and return the related name (string).
-
-		:param v: previously registered number.
-		:type v: int
-		:returns: associated name.
-		:rtype: str
-		"""
-		return self.vk[v]
-
-	def to_number(self, k):
-		"""Accept a name and return the related number.
-
-		:param k: previously registered name.
-		:type k: str
-		:returns: associated number.
-		:rtype: int
-		"""
-		return self.kv[k]
+    :param kv: map of strings and their integer value.
+    :type kv: dict
+    """
+
+    def __init__(self, **kv):
+        """Refer to class."""
+        self.kv = kv
+        for k, v in kv.items():
+            setattr(self, k, v)
+        self.vk = {v: k for k, v in kv.items()}
+
+    def to_name(self, v):
+        """Accept an integer and return the related name (string).
+
+        :param v: previously registered number.
+        :type v: int
+        :returns: associated name.
+        :rtype: str
+        """
+        return self.vk[v]
+
+    def to_number(self, k):
+        """Accept a name and return the related number.
+
+        :param k: previously registered name.
+        :type k: str
+        :returns: associated number.
+        :rtype: int
+        """
+        return self.kv[k]
 
 class ClockTime(Portable):
-	"""The time on the wall clock as an epoch value; a float."""
+    """The time on the wall clock as an epoch value; a float."""
 
 class TimeSpan(Portable):
-	"""Difference between two ``ClockTime`` values; a float."""
+    """Difference between two ``ClockTime`` values; a float."""
 
 class WorldTime(Portable):
-	"""The time at the Greenwich meridian; a datetime object."""
+    """The time at the Greenwich meridian; a datetime object."""
 
 class TimeDelta(Portable):
-	"""Difference between two ``WorldTime`` values; a timedelta object."""
+    """Difference between two ``WorldTime`` values; a timedelta object."""
 
 class UUID(Portable):
-	"""An RFC 4122 UUID (random); a ``uuid.UUID`` object."""
+    """An RFC 4122 UUID (random); a ``uuid.UUID`` object."""
 
 class ArrayOf(Container):
-	"""A fixed-length sequence of elements.
+    """A fixed-length sequence of elements.
 
-	:param element: type of the content.
-	:type element: :ref:`type expression<type-expressions>`
-	:param size: fixed size.
-	:type size: int
-	"""
-
-	def __init__(self, element, size):
-		"""Refer to class."""
-		self.element = element
-		self.size = size
+    :param element: type of the content.
+    :type element: :ref:`type expression<type-expressions>`
+    :param size: fixed size.
+    :type size: int
+    """
+
+    def __init__(self, element, size):
+        """Refer to class."""
+        self.element = element
+        self.size = size
 
 class VectorOf(Container):
-	"""A variable-length sequence of elements.
+    """A variable-length sequence of elements.
 
-	:param element: type of the content.
-	:type element: :ref:`type expression<type-expressions>`
-	"""
-
-	def __init__(self, element):
-		"""Refer to class."""
-		self.element = element
+    :param element: type of the content.
+    :type element: :ref:`type expression<type-expressions>`
+    """
+
+    def __init__(self, element):
+        """Refer to class."""
+        self.element = element
 
 class SetOf(Container):
-	"""A collection of unique elements.
+    """A collection of unique elements.
 
-	:param element: type of the content, a hash-able value.
-	:type element: :ref:`type expression<type-expressions>`
-	"""
-
-	def __init__(self, element):
-		"""Refer to class."""
-		self.element = element
+    :param element: type of the content, a hash-able value.
+    :type element: :ref:`type expression<type-expressions>`
+    """
+
+    def __init__(self, element):
+        """Refer to class."""
+        self.element = element
 
 class MapOf(Container):
-	"""A map of unique, key-value pairs.
+    """A map of unique, key-value pairs.
 
-	:param key: type of the key, a hash-able value.
-	:type key: :ref:`type expression<type-expressions>`
-	:param value: type of the content.
-	:type value: :ref:`type expression<type-expressions>`
-	"""
-
-	def __init__(self, key, value):
-		"""Refer to class."""
-		self.key = key
-		self.value = value
+    :param key: type of the key, a hash-able value.
+    :type key: :ref:`type expression<type-expressions>`
+    :param value: type of the content.
+    :type value: :ref:`type expression<type-expressions>`
+    """
+
+    def __init__(self, key, value):
+        """Refer to class."""
+        self.key = key
+        self.value = value
 
 class DequeOf(Container):
-	"""A double-ended sequence of elements.
+    """A double-ended sequence of elements.
 
-	:param element: type of the content.
-	:type element: :ref:`type expression<type-expressions>`
-	"""
-
-	def __init__(self, element):
-		"""Refer to class."""
-		self.element = element
+    :param element: type of the content.
+    :type element: :ref:`type expression<type-expressions>`
+    """
+
+    def __init__(self, element):
+        """Refer to class."""
+        self.element = element
 
 class UserDefined(Container):
-	"""A structure of named elements.
+    """A structure of named elements.
 
-	:param element: registered class.
-	:type element: class
-	"""
-
-	def __init__(self, element):
-		"""Refer to class."""
-		self.element = element
+    :param element: registered class.
+    :type element: class
+    """
+
+    def __init__(self, element):
+        """Refer to class."""
+        self.element = element
 
 class PointerTo(Container):
-	"""An object that refers to another object.
+    """An object that refers to another object.
 
-	:param element: type of the object being pointed to.
-	:type element: :ref:`type expression<type-expressions>`
-	"""
-
-	def __init__(self, element):
-		"""Refer to class."""
-		self.element = element
+    :param element: type of the object being pointed to.
+    :type element: :ref:`type expression<type-expressions>`
+    """
+
+    def __init__(self, element):
+        """Refer to class."""
+        self.element = element
 
 class Type(Portable):
-	"""The unique, portable identity of a registered message."""
+    """The unique, portable identity of a registered message."""
 
 class Word(Portable):
-	"""A well-formed but untyped unit of data."""
+    """A well-formed but untyped unit of data."""
 
 class Any(Portable):
-	"""The combination of a Type and a Word."""
+    """The combination of a Type and a Word."""
 
-	def __init__(self, *possibles):
-		"""Accept these types in a version-managed scenario."""
-		self.possibles = possibles
+    def __init__(self, *possibles):
+        """Accept these types in a version-managed scenario."""
+        self.possibles = possibles
 
 class TargetAddress(Portable):
-	"""The address of a receiving object."""
+    """The address of a receiving object."""
 
 class Address(Portable):
-	"""The address of a sending object."""
+    """The address of a sending object."""
 
 # List of the library types.
 complete_list = [
-	Boolean,
-	Byte,
-	Character,
-	Rune,
-	Integer2,
-	Integer4,
-	Integer8,
-	Unsigned2,
-	Unsigned4,
-	Unsigned8,
-	Float4,
-	Float8,
-	String,
-	Unicode,
-	Block,
-	Enumeration,
-	ClockTime,
-	TimeSpan,
-	WorldTime,
-	TimeDelta,
-	UUID,
-	UserDefined,
-	ArrayOf,
-	VectorOf,
-	SetOf,
-	MapOf,
-	DequeOf,
-	PointerTo,
-	Type,
-	Word,
-	Any,
-	TargetAddress,
-	Address,
+    Boolean,
+    Byte,
+    Character,
+    Rune,
+    Integer2,
+    Integer4,
+    Integer8,
+    Unsigned2,
+    Unsigned4,
+    Unsigned8,
+    Float4,
+    Float8,
+    String,
+    Unicode,
+    Block,
+    Enumeration,
+    ClockTime,
+    TimeSpan,
+    WorldTime,
+    TimeDelta,
+    UUID,
+    UserDefined,
+    ArrayOf,
+    VectorOf,
+    SetOf,
+    MapOf,
+    DequeOf,
+    PointerTo,
+    Type,
+    Word,
+    Any,
+    TargetAddress,
+    Address,
 ]
 
 # Set of the library types.
 complete_set = set(complete_list)
 
 # Few handy type predicates.
 #
 
 def is_portable(a):
-	"""Is object *a* an instance of one of the portable types."""
-	return isinstance(a, Portable)
+    """Is object *a* an instance of one of the portable types."""
+    return isinstance(a, Portable)
 
 def is_container(a):
-	"""Is object *a* an instance of one of the portable container types."""
-	return isinstance(a, Container)
+    """Is object *a* an instance of one of the portable container types."""
+    return isinstance(a, Container)
 
 def is_structural(a):
-	"""Is object *a* an instance of one of the portable container types and not a pointer."""
-	b = isinstance(a, Container) and not isinstance(a, PointerTo)
-	return b
+    """Is object *a* an instance of one of the portable container types and not a pointer."""
+    b = isinstance(a, Container) and not isinstance(a, PointerTo)
+    return b
 
 def is_portable_class(c):
-	"""Is object *c* one of the portable types."""
-	try:
-		return issubclass(c, Portable)
-	except TypeError:
-		return False
+    """Is object *c* one of the portable types."""
+    try:
+        return issubclass(c, Portable)
+    except TypeError:
+        return False
 
 def is_container_class(c):
-	"""Is object *c* one of the portable container types."""
-	try:
-		return issubclass(c, Container)
-	except TypeError:
-		return False
+    """Is object *c* one of the portable container types."""
+    try:
+        return issubclass(c, Container)
+    except TypeError:
+        return False
 
 # This is the official null address and where required the
 # default value for an address.
-NO_SUCH_ADDRESS = (0,)
+NO_SUCH_ADDRESS = None
 
 def is_address(a):
-	"""Is object *a* is a valid point address."""
-	try:
-		return isinstance(a, tuple) and len(a) > 0
-	except (TypeError, ValueError):
-		return False
+    """Is object *a* is a valid point address."""
+    try:
+        return isinstance(a, tuple) and len(a) > 0
+    except (TypeError, ValueError):
+        return False
 
 def address_on_proxy(a, p):
-	"""Check that address *a* refers to an object behind the proxy address, p."""
-	if a[-1] == p[-1]:
-		if len(p) == 1 and len(a) > 1:
-			return True
-	return False
+    """Check that address *a* refers to an object behind the proxy address, p."""
+    if a[-1] == p[-1]:
+        if len(p) == 1 and len(a) > 1:
+            return True
+    return False
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/release.py` & `ansar-encode-0.1.19/src/ansar/encode/release.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2022 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,84 +25,80 @@
 
 Functions to support the full, formal management of object versioning.
 """
 
 __docformat__ = 'restructuredtext'
 
 __all__ = [
-	'reachable',
-	'released_document',
+    'reachable',
+    'released_document',
 ]
 
 import sys
 
 from .portable import *
 from .runtime import *
 from .message import *
 
 __all__ = [
-	'reachable',
-	'released_document',
+    'reachable',
+    'released_document',
 ]
 
 reachable = {}
 
 #
 #
 def released_document(doc):
-	"""Register an application object for saving to disk.
+    """Register an application object for saving to disk.
 
-	This function registers a document for the purposes of version
-	support. Registered information is used during encoding to select
-	the proper name slice.
-
-	Registered materials are also used during building and releasing
-	to enforce the broader application versioning strategy.
-
-	:param doc: the base document type
-	:type doc: a registered message type
-	:return: None
-	"""
-	if not hasattr(doc, '__art__'):
-		t = doc.__name__
-		s = f'cannot include "{t}" for version management - not registered'
-		raise CodingProblem(s)
-	e = UserDefined(doc)
-
-	# Compile the set of all messages reachable from the
-	# specified type.
-	r = set(t for t in reachable_type(e, set()))
-
-	# Compile a type-version dictionary for the set of
-	# reachable classes.
-	d = {}
-	for t in r:
-		v = get_version(t)
-		if v is None:
-			n1 = e.element.__name__
-			n2 = t.__name__
-			s = 'cannot include "%s" for version management - "%s" is unversioned' % (n1, n2)
-			raise CodingProblem(s)
-		d[t] = v
+    This function registers a document for the purposes of version
+    support. Registered information is used during encoding to select
+    the proper name slice.
+
+    Registered materials are also used during building and releasing
+    to enforce the broader application versioning strategy.
+
+    :param doc: the base document type
+    :type doc: a registered message type
+    :return: None
+    """
+    e = UserDefined(doc)
+
+    # Compile the set of all messages reachable from the
+    # specified type.
+    r = set(t for t in reachable_type(e, set()))
+
+    # Compile a type-version dictionary for the set of
+    # reachable classes.
+    d = {}
+    for t in r:
+        v = get_version(t)
+        if v is None:
+            n1 = e.element.__name__
+            n2 = t.__name__
+            s = 'cannot register "%s" for version management - "%s" is unversioned.' % (n1, n2)
+            raise CodingProblem(s)
+        d[t] = v
 
-	reachable[e.element] = d
+    reachable[e.element] = d
 
 
 def reachable_type(t, bread):
-	"""Determine the main type, e.g. portable, UDT or content of a container."""
-	if isinstance(t, UserDefined):
-		e = t.element
-		for _, v in e.__art__.value.items():
-			yield from reachable_type(v, bread)
-		yield e
-	elif isinstance(t, (VectorOf, ArrayOf, DequeOf, SetOf)):
-		yield from reachable_type(t.element, bread)
-	elif isinstance(t, MapOf):
-		yield from reachable_type(t.value, bread)
-	elif isinstance(t, PointerTo):
-		k = id(t)
-		if k not in bread:
-			bread.add(k)
-			yield from reachable_type(t.element, bread)
-	elif isinstance(t, Any):
-		for p in t.possibles:
-			yield from reachable_type(p, bread)
+    """Determine the main type, e.g. portable, UDT or content of a container."""
+    if isinstance(t, UserDefined):
+        e = t.element
+        for _, v in e.__art__.value.items():
+            yield from reachable_type(v, bread)
+        yield e
+    elif isinstance(t, (VectorOf, ArrayOf, DequeOf, SetOf)):
+        yield from reachable_type(t.element, bread)
+    elif isinstance(t, MapOf):
+        yield from reachable_type(t.value, bread)
+    elif isinstance(t, PointerTo):
+        k = id(t)
+        if k not in bread:
+            bread.add(k)
+            yield from reachable_type(t.element, bread)
+    elif isinstance(t, Any):
+        for p in t.possibles:
+            yield from reachable_type(p, bread)
```

### Comparing `ansar_encode-0.1.128/src/ansar/encode/version.py` & `ansar-encode-0.1.19/src/ansar/encode/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Author: Scott Woods <scott.18.ansar@gmail.com.com>
+# Author: Scott Woods <scott.suzuki@gmail.com>
 # MIT License
 #
-# Copyright (c) 2017-2023 Scott Woods
+# Copyright (c) 2017-2022 Scott Woods
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -25,22 +25,20 @@
 
 Functions to assist with the coding of application version support.
 """
 
 __docformat__ = 'restructuredtext'
 
 __all__ = [
-	'migrate',
-	'cannot_upgrade',
+    'migrate',
+    'cannot_upgrade',
 ]
 
 def migrate(f, upgrade, *args, **kwargs):
-	"""Recover the specified file and store (i.e. migrate) as necessary."""
-	r, v = f.recover()
-	a = upgrade(r, v, *args, **kwargs)
-	if id(a) != id(r):
-		f.store(a)
-	return a
+    r, v = f.recover()
+    a = upgrade(r, v, *args, **kwargs)
+    if id(a) != id(r):
+        f.store(a)
+    return a
 
 def cannot_upgrade(r, v):
-	"""Raise a ValueError with relevant information about the failed upgrade of an object."""
-	raise ValueError('cannot upgrade "%s" (version "%s")' % (r.__class__.__name__, v))
+    raise ValueError('cannot upgrade "%s" (version "%s")' % (r.__class__.__name__, v))
```

### Comparing `ansar_encode-0.1.128/src/ansar_encode.egg-info/PKG-INFO` & `ansar-encode-0.1.19/src/ansar_encode.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: ansar-encode
-Version: 0.1.128
+Version: 0.1.19
 Summary: Persistence of complex application data
 Author: Scott Woods
-Author-email: Scott Woods <scott.18.ansar@gmail.com>
-Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.1/index.html
+Author-email: Scott Woods <scott.suzuki@gmail.com>
+Project-URL: Documentation, http://ansar-encode-manual.s3-website-ap-southeast-2.amazonaws.com/0.1.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: defusedxml>=0.7.1
-Requires-Dist: python-dateutil>=2.8.1
 
 # ansar-encode
 
 The **ansar-encode** library provides for the convenient storage and recovery of
 application data using system files. Files are created using standard encodings - the
 default is JSON - and are human readable. Complex application data can be stored
 including containers, instances of classes and object graphs.
```

### Comparing `ansar_encode-0.1.128/src/ansar_encode.egg-info/SOURCES.txt` & `ansar-encode-0.1.19/src/ansar_encode.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-src/ansar/command/ansar_command.py
+src/ansar/command/show_release.py
 src/ansar/encode/__init__.py
-src/ansar/encode/args.py
 src/ansar/encode/codec.py
-src/ansar/encode/command.py
 src/ansar/encode/convert.py
 src/ansar/encode/file.py
 src/ansar/encode/folder.py
+src/ansar/encode/framework.py
 src/ansar/encode/json.py
 src/ansar/encode/message.py
 src/ansar/encode/portable.py
-src/ansar/encode/primitive.py
-src/ansar/encode/procedure.py
 src/ansar/encode/release.py
 src/ansar/encode/runtime.py
-src/ansar/encode/support.py
 src/ansar/encode/version.py
 src/ansar/encode/xml.py
 src/ansar_encode.egg-info/PKG-INFO
 src/ansar_encode.egg-info/SOURCES.txt
 src/ansar_encode.egg-info/dependency_links.txt
 src/ansar_encode.egg-info/entry_points.txt
 src/ansar_encode.egg-info/requires.txt
```

