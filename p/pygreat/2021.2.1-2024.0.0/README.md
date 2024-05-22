# Comparing `tmp/pygreat-2021.2.1-py2.py3-none-any.whl.zip` & `tmp/pygreat-2024.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 26677 bytes, number of entries: 13
--rw-------  2.0 unx       38 b- defN 19-Apr-12 11:03 pygreat/__init__.py
--rw-r--r--  2.0 unx    14236 b- defN 20-Jul-15 02:33 pygreat/board.py
--rw-r--r--  2.0 unx    49299 b- defN 20-Jul-15 02:33 pygreat/comms.py
--rw-------  2.0 unx     4112 b- defN 19-Apr-12 11:03 pygreat/errors.py
--rw-------  2.0 unx        0 b- defN 19-Apr-12 11:03 pygreat/classes/__init__.py
--rw-r--r--  2.0 unx     4412 b- defN 20-Jul-15 02:33 pygreat/classes/core.py
--rw-------  2.0 unx        0 b- defN 19-Apr-12 11:03 pygreat/comms_backends/__init__.py
--rw-r--r--  2.0 unx    17128 b- defN 21-Jan-06 14:35 pygreat/comms_backends/usb.py
--rw-r--r--  2.0 unx      960 b- defN 21-Feb-23 15:56 pygreat-2021.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Feb-23 15:56 pygreat-2021.2.1.dist-info/WHEEL
--rw-------  2.0 unx       20 b- defN 21-Feb-23 15:56 pygreat-2021.2.1.dist-info/entry_points.txt
--rw-------  2.0 unx        8 b- defN 21-Feb-23 15:56 pygreat-2021.2.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1039 b- defN 21-Feb-23 15:56 pygreat-2021.2.1.dist-info/RECORD
-13 files, 91362 bytes uncompressed, 24939 bytes compressed:  72.7%
+Zip file size: 32545 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       38 b- defN 24-May-22 12:20 pygreat/__init__.py
+-rw-r--r--  2.0 unx    14236 b- defN 24-May-22 12:20 pygreat/board.py
+-rw-r--r--  2.0 unx    50234 b- defN 24-May-22 12:20 pygreat/comms.py
+-rw-r--r--  2.0 unx     4112 b- defN 24-May-22 12:20 pygreat/errors.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 12:20 pygreat/classes/__init__.py
+-rw-r--r--  2.0 unx     4412 b- defN 24-May-22 12:20 pygreat/classes/core.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 12:20 pygreat/comms_backends/__init__.py
+-rw-r--r--  2.0 unx    17254 b- defN 24-May-22 12:20 pygreat/comms_backends/usb.py
+-rw-r--r--  2.0 unx    19372 b- defN 24-May-22 12:20 pygreat/comms_backends/usb1.py
+-rw-r--r--  2.0 unx      992 b- defN 24-May-22 12:22 pygreat-2024.0.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 12:22 pygreat-2024.0.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-22 12:22 pygreat-2024.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1028 b- defN 24-May-22 12:22 pygreat-2024.0.0.dist-info/RECORD
+13 files, 111778 bytes uncompressed, 30833 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pygreat/comms_backends/__init__.py
 Comment: 
 
 Filename: pygreat/comms_backends/usb.py
 Comment: 
 
-Filename: pygreat-2021.2.1.dist-info/METADATA
+Filename: pygreat/comms_backends/usb1.py
 Comment: 
 
-Filename: pygreat-2021.2.1.dist-info/WHEEL
+Filename: pygreat-2024.0.0.dist-info/METADATA
 Comment: 
 
-Filename: pygreat-2021.2.1.dist-info/entry_points.txt
+Filename: pygreat-2024.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: pygreat-2021.2.1.dist-info/top_level.txt
+Filename: pygreat-2024.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pygreat-2021.2.1.dist-info/RECORD
+Filename: pygreat-2024.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygreat/comms.py

```diff
@@ -73,25 +73,35 @@
         'p': 'string',
         'P': 'int',
     }
 
 
     @classmethod
     def from_device_uri(cls, **device_uri):
-        """ Creates a CommsBackend object apporpriate for the given device_uri.  """
+        """ Creates a CommsBackend object appropriate for the given device_uri.  """
 
-        #FIXME: implment this properly
-
-        from .comms_backends.usb import USBCommsBackend
+        #FIXME: implement this properly
 
         # TODO: handle providing board "URIs", like "usb://1234abcd/?param=value",
         # and automatic resolution to a backend?
         # TODO: support more than USB
 
+        # Use the usb1 backend if this is a Cynthion.
+        # TODO use cynthion vendor/product id and interface protocol field
+        # TODO we should probably rather run through the backends and return
+        #      the backend that can successfully match the device_identifiers
+        if 'idVendor' in device_uri and 'idProduct' in device_uri:
+            idVendor = device_uri['idVendor']
+            idProduct = device_uri['idProduct']
+            if idVendor == 0x1d50 and idProduct == 0x615b:
+                from .comms_backends.usb1 import USB1CommsBackend
+                return USB1CommsBackend(**device_uri)
+
         # XXX: for now, just create a USB backend, as that's all we support
+        from .comms_backends.usb import USBCommsBackend
         return USBCommsBackend(**device_uri)
 
 
     def __init__(self, **device_arguments):
         """ Sets up a new communication channel for a libgreat device.
 
         Args:
@@ -575,14 +585,22 @@
 
         # Return the composed byte-string.
         return result
 
     @classmethod
     @memoize_with_lru_cache(maxsize=128)
     def unpack(cls, format_string, raw_bytes):
+        try:
+            return cls._unpack(cls, format_string, raw_bytes)
+        except Exception as e:
+            import logging
+            logging.error(f"Failed to unpack struct from raw bytes: {len(raw_bytes)} bytes => {raw_bytes}")
+            raise e
+
+    def _unpack(cls, format_string, raw_bytes):
         """ Extended version of struct.unpack() for libgreat communciations.
 
         Accepts mostly the same arguments as struct.pack, with the following
         additional supported format strings:
 
             S -- c-style, UTF-8, null-terminated string
             X -- as-is; returns a byte-string. If specified with a
```

## pygreat/comms_backends/usb.py

```diff
@@ -141,14 +141,17 @@
                 usb.util.claim_interface(self.device, 0)
                 return
             except usb.core.USBError as e:
 
                 # If we have EBUSY (linux) or EACCES (macos), or None (windows), try again.
                 if e.errno in (errno.EBUSY, errno.EACCES, None):
                     pass
+                # If we have None (windows), just return
+                elif e.errno in (None, ):
+                    return
                 else:
                     raise
 
             if time.time() > timeout:
                 raise IOError("timed out trying to claim access to a libgreat device!")
```

## Comparing `pygreat-2021.2.1.dist-info/METADATA` & `pygreat-2024.0.0.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: pygreat
-Version: 2021.2.1
+Version: 2024.0.0
 Summary: Python library for talking with libGreat devices
-Home-page: https://greatscottgadgets.com/greatfet/
-Author: Katherine J. Temkin
-Author-email: ktemkin@greatscottgadgets.com
+Author-email: Great Scott Gadgets <dev@greatscottgadgets.com>
 License: BSD
-Platform: any
+Project-URL: Source, https://greatscottgadgets.com/greatfet
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Environment :: Console
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Security
+Description-Content-Type: text/markdown
 Requires-Dist: pyusb
 Requires-Dist: future
 Requires-Dist: backports.functools-lru-cache
 
 # libgreat host-side libraries
 
 This folder contains an experimental host-side python utility. It should work with
 both python2 and python3.
-
-
```

## Comparing `pygreat-2021.2.1.dist-info/RECORD` & `pygreat-2024.0.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pygreat/__init__.py,sha256=aqqK-zU-EX1ZsImxW8d9hBUWGz2fKoCXPU48ydupXoo,38
 pygreat/board.py,sha256=YIr1AV8zorLcOmRO1Ief_r3A_AfZoWTu-YOajQNQEOU,14236
-pygreat/comms.py,sha256=SYGKM0RNGJKDlJ9tCZa_2tglb9R7lhtX2geas4RX8uA,49299
+pygreat/comms.py,sha256=yoLfMRy16IUFP8TPQv8kmUNC4hmJh4rX_gFkQPgaISo,50234
 pygreat/errors.py,sha256=XGuK8h803QSTaBd7dXzq3hqwwmzeOEaKREHnk2wCuuk,4112
 pygreat/classes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pygreat/classes/core.py,sha256=edu4vxnbouA1b-Ui2qNYZgwADMm_VD1HviUw0Ku8xm8,4412
 pygreat/comms_backends/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pygreat/comms_backends/usb.py,sha256=PZkmbEKkcADXn1V0as1Vzu2l3OVfjBV5Aes7YYfx93o,17128
-pygreat-2021.2.1.dist-info/METADATA,sha256=tM_FeInAKkVHemu3Ik3GzK9v6rDLjuFlRGNqe_zxd_8,960
-pygreat-2021.2.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-pygreat-2021.2.1.dist-info/entry_points.txt,sha256=eqGnTHtEVMYwfXVk1Z9MhC8O2N8wuqAbr0lisLmrkxs,20
-pygreat-2021.2.1.dist-info/top_level.txt,sha256=JdFOHYUylXUhkO8kL2b-UW2VTFV-HLtvqV0ULiHMpsg,8
-pygreat-2021.2.1.dist-info/RECORD,,
+pygreat/comms_backends/usb.py,sha256=_iTJM67g2b_ipt-rwXCoPs0FGgNdLiPpNMZfE-7hEKo,17254
+pygreat/comms_backends/usb1.py,sha256=hbEEKxL97GYG4dVwk_hvNPcXyA6Movdygoy1eGq4YZ4,19372
+pygreat-2024.0.0.dist-info/METADATA,sha256=VKZzOLpCJIK0mKI26p3PfdyNei1eZxDa9rKJrImsEK4,992
+pygreat-2024.0.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pygreat-2024.0.0.dist-info/top_level.txt,sha256=JdFOHYUylXUhkO8kL2b-UW2VTFV-HLtvqV0ULiHMpsg,8
+pygreat-2024.0.0.dist-info/RECORD,,
```

