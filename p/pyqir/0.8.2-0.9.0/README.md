# Comparing `tmp/pyqir-0.8.2-cp37-abi3-win_amd64.whl.zip` & `tmp/pyqir-0.9.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 1433216 bytes, number of entries: 13
--rw-r--r--  4.6 unx     4331 b- defN 23-May-02 16:21 pyqir-0.8.2.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-May-02 16:21 pyqir-0.8.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     1090 b- defN 23-May-02 16:21 pyqir-0.8.2.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx   354241 b- defN 23-May-02 16:21 pyqir-0.8.2.dist-info/license_files/NOTICE-WHEEL.txt
--rw-r--r--  4.6 unx        0 b- defN 23-May-02 16:21 pyqir/py.typed
--rw-r--r--  4.6 unx      543 b- defN 23-May-02 16:21 pyqir/qis.py
--rw-r--r--  4.6 unx      327 b- defN 23-May-02 16:21 pyqir/rt.py
--rw-r--r--  4.6 unx     4852 b- defN 23-May-02 16:21 pyqir/_basicqis.py
--rw-r--r--  4.6 unx    33968 b- defN 23-May-02 16:21 pyqir/_native.pyi
--rw-r--r--  4.6 unx     3855 b- defN 23-May-02 16:21 pyqir/_simple.py
--rw-r--r--  4.6 unx     2275 b- defN 23-May-02 16:21 pyqir/__init__.py
--rwxr-xr-x  4.6 unx  3680256 b- defN 23-May-02 16:21 pyqir/_native.pyd
--rw-r--r--  4.6 unx      988 b- defN 23-May-02 16:21 pyqir-0.8.2.dist-info/RECORD
-13 files, 4086821 bytes uncompressed, 1431602 bytes compressed:  65.0%
+Zip file size: 1437750 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     4330 b- defN 23-Aug-29 16:58 pyqir-0.9.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Aug-29 16:58 pyqir-0.9.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1090 b- defN 23-Aug-29 16:58 pyqir-0.9.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx   354241 b- defN 23-Aug-29 16:58 pyqir-0.9.0.dist-info/license_files/NOTICE-WHEEL.txt
+-rw-r--r--  4.6 unx        0 b- defN 23-Aug-29 16:58 pyqir/py.typed
+-rw-r--r--  4.6 unx      543 b- defN 23-Aug-29 16:58 pyqir/qis.py
+-rw-r--r--  4.6 unx      327 b- defN 23-Aug-29 16:58 pyqir/rt.py
+-rw-r--r--  4.6 unx     4852 b- defN 23-Aug-29 16:58 pyqir/_basicqis.py
+-rw-r--r--  4.6 unx     1678 b- defN 23-Aug-29 16:58 pyqir/_entry_point.py
+-rw-r--r--  4.6 unx    34783 b- defN 23-Aug-29 16:58 pyqir/_native.pyi
+-rw-r--r--  4.6 unx     3855 b- defN 23-Aug-29 16:58 pyqir/_simple.py
+-rw-r--r--  4.6 unx     2357 b- defN 23-Aug-29 16:58 pyqir/__init__.py
+-rwxr-xr-x  4.6 unx  3693056 b- defN 23-Aug-29 16:58 pyqir/_native.pyd
+-rw-r--r--  4.6 unx     1066 b- defN 23-Aug-29 16:58 pyqir-0.9.0.dist-info/RECORD
+14 files, 4102272 bytes uncompressed, 1436018 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -1,40 +1,43 @@
-Filename: pyqir-0.8.2.dist-info/METADATA
+Filename: pyqir-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pyqir-0.8.2.dist-info/WHEEL
+Filename: pyqir-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyqir-0.8.2.dist-info/license_files/LICENSE
+Filename: pyqir-0.9.0.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: pyqir-0.8.2.dist-info/license_files/NOTICE-WHEEL.txt
+Filename: pyqir-0.9.0.dist-info/license_files/NOTICE-WHEEL.txt
 Comment: 
 
 Filename: pyqir/py.typed
 Comment: 
 
 Filename: pyqir/qis.py
 Comment: 
 
 Filename: pyqir/rt.py
 Comment: 
 
 Filename: pyqir/_basicqis.py
 Comment: 
 
+Filename: pyqir/_entry_point.py
+Comment: 
+
 Filename: pyqir/_native.pyi
 Comment: 
 
 Filename: pyqir/_simple.py
 Comment: 
 
 Filename: pyqir/__init__.py
 Comment: 
 
 Filename: pyqir/_native.pyd
 Comment: 
 
-Filename: pyqir-0.8.2.dist-info/RECORD
+Filename: pyqir-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyqir/_native.pyi

```diff
@@ -296,14 +296,26 @@
     def value(self) -> float:
         """The value."""
         ...
 
 class FloatPredicate(Enum):
     """A floating-point comparison predicate."""
 
+    def __richcmp__(self, other: Value, op: int) -> bool:
+        """
+        Compares this value to another value.
+        Only == and != are supported.
+
+        :param other: The other value.
+        :param op: The comparison operator.
+        :returns: The result of the comparison.
+        """
+        ...
+    def __hash__(self) -> int: ...
+
     FALSE: FloatPredicate
     OEQ: FloatPredicate
     OGT: FloatPredicate
     OGE: FloatPredicate
     OLT: FloatPredicate
     OLE: FloatPredicate
     ONE: FloatPredicate
@@ -410,14 +422,26 @@
     def value(self) -> int:
         """The value."""
         ...
 
 class IntPredicate(Enum):
     """An integer comparison predicate."""
 
+    def __richcmp__(self, other: Value, op: int) -> bool:
+        """
+        Compares this value to another value.
+        Only == and != are supported.
+
+        :param other: The other value.
+        :param op: The comparison operator.
+        :returns: The result of the comparison.
+        """
+        ...
+    def __hash__(self) -> int: ...
+
     EQ: IntPredicate
     NE: IntPredicate
     UGT: IntPredicate
     UGE: IntPredicate
     ULT: IntPredicate
     ULE: IntPredicate
     SGT: IntPredicate
@@ -440,14 +464,26 @@
     def width(self) -> int:
         """The number of bits in the integer."""
         ...
 
 class Linkage(Enum):
     """The linkage kind for a global value in a module."""
 
+    def __richcmp__(self, other: Value, op: int) -> bool:
+        """
+        Compares this value to another value.
+        Only == and != are supported.
+
+        :param other: The other value.
+        :param op: The comparison operator.
+        :returns: The result of the comparison.
+        """
+        ...
+    def __hash__(self) -> int: ...
+
     APPENDING: Linkage
     AVAILABLE_EXTERNALLY: Linkage
     COMMON: Linkage
     EXTERNAL: Linkage
     EXTERNAL_WEAK: Linkage
     INTERNAL: Linkage
     LINK_ONCE_ANY: Linkage
@@ -549,14 +585,26 @@
     APPEND: ModuleFlagBehavior
     APPEND_UNIQUE: ModuleFlagBehavior
     MAX: ModuleFlagBehavior
 
 class Opcode(Enum):
     """An instruction opcode."""
 
+    def __richcmp__(self, other: Value, op: int) -> bool:
+        """
+        Compares this value to another value.
+        Only == and != are supported.
+
+        :param other: The other value.
+        :param op: The comparison operator.
+        :returns: The result of the comparison.
+        """
+        ...
+    def __hash__(self) -> int: ...
+
     ADD: Opcode
     ADDR_SPACE_CAST: Opcode
     ALLOCA: Opcode
     AND: Opcode
     ASHR: Opcode
     ATOMIC_CMP_XCHG: Opcode
     ATOMIC_RMW: Opcode
@@ -764,35 +812,14 @@
 
     :param ty: The type of the value.
     :param value: The value of the constant.
     :returns: The constant value.
     """
     ...
 
-def entry_point(
-    module: Module,
-    name: str,
-    required_num_qubits: int,
-    required_num_results: int,
-    qir_profiles: Optional[str] = "custom",
-    output_labeling_schema: Optional[str] = "",
-) -> Function:
-    """
-    Creates an entry point.
-
-    :param Module module: The parent module.
-    :param str name: The entry point name.
-    :param int required_num_qubits: The number of qubits required by the entry point.
-    :param int required_num_results: The number of results required by the entry point.
-    :param Optional[str] qir_profiles: Value identifying the profile the entry point has been compiled for. Use base_profile when QIR is compliant.
-    :param Optional[str] output_labeling_schema: An arbitrary string value that identifies the schema used by a compiler frontend that produced the IR to label the recorded output
-    :returns: An entry point.
-    """
-    ...
-
 def qir_major_version(module: Module) -> Optional[int]:
     """The QIR major version this module is built for. None if unspecified."""
     ...
 
 def qir_minor_version(module: Module) -> Optional[int]:
     """The QIR minor version this module is built for. None if unspecified."""
     ...
@@ -1190,7 +1217,19 @@
 
     :param builder: The underlying builder used to build QIS instructions.
     :param cond: The result condition to branch on.
     :param one: A callable that inserts instructions for the branch where the result is one.
     :param zero: A callable that inserts instructions for the branch where the result is zero.
     """
     ...
+
+def add_string_attribute(
+    function: Function, kind: str, value: Optional[str] = None
+) -> bool:
+    """
+    Adds a string attribute to the given function.
+
+    :param function: The function.
+    :param key: The attribute key.
+    :param value: The attribute value.
+    """
+    ...
```

## pyqir/__init__.py

```diff
@@ -30,18 +30,18 @@
     Opcode,
     Phi,
     PointerType,
     StructType,
     Switch,
     Type,
     Value,
+    add_string_attribute,
     const,
     dynamic_qubit_management,
     dynamic_result_management,
-    entry_point,
     extract_byte_string,
     global_byte_string,
     is_entry_point,
     is_interop_friendly,
     is_qubit_type,
     is_result_type,
     qubit,
@@ -53,14 +53,15 @@
     required_num_qubits,
     required_num_results,
     result,
     result_id,
     result_type,
 )
 from pyqir._simple import SimpleModule
+from pyqir._entry_point import entry_point
 from pyqir._basicqis import BasicQisBuilder
 
 __all__ = [
     "ArrayType",
     "Attribute",
     "AttributeList",
     "AttributeSet",
@@ -90,14 +91,15 @@
     "Phi",
     "PointerType",
     "SimpleModule",
     "StructType",
     "Switch",
     "Type",
     "Value",
+    "add_string_attribute",
     "const",
     "dynamic_qubit_management",
     "dynamic_result_management",
     "entry_point",
     "extract_byte_string",
     "global_byte_string",
     "is_entry_point",
```

## Comparing `pyqir-0.8.2.dist-info/METADATA` & `pyqir-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pyqir
-Version: 0.8.2
+Version: 0.9.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
-Requires-Dist: pytest ~= 7.2.0; extra == 'test'
+Requires-Dist: pytest ~=7.2.0 ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 License-File: NOTICE-WHEEL.txt
 Summary: PyQIR parses, generates and evaluates the Quantum Intermediate Representation.
 Home-Page: https://github.com/qir-alliance/pyqir
 Author: Microsoft
 License: MIT
-Requires-Python: >= 3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/qir-alliance/pyqir
 
 # PyQIR
 
 The `pyqir` package provides the ability to generate
 [QIR](https://github.com/qir-alliance/qir-spec) as well as an easy way to
```

## Comparing `pyqir-0.8.2.dist-info/license_files/LICENSE` & `pyqir-0.9.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `pyqir-0.8.2.dist-info/license_files/NOTICE-WHEEL.txt` & `pyqir-0.9.0.dist-info/license_files/NOTICE-WHEEL.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19788,15 +19788,15 @@
 0004d4b0: 7468 6520 4c69 6365 6e73 6520 666f 7220  the License for 
 0004d4c0: 7468 6520 7370 6563 6966 6963 206c 616e  the specific lan
 0004d4d0: 6775 6167 6520 676f 7665 726e 696e 6720  guage governing 
 0004d4e0: 7065 726d 6973 7369 6f6e 7320 616e 640d  permissions and.
 0004d4f0: 0a6c 696d 6974 6174 696f 6e73 2075 6e64  .limitations und
 0004d500: 6572 2074 6865 204c 6963 656e 7365 2e0d  er the License..
 0004d510: 0a0d 0a0d 0a0d 0a71 6972 6c69 6220 302e  .......qirlib 0.
-0004d520: 382e 3220 2d20 5350 4458 3a20 4d49 5420  8.2 - SPDX: MIT 
+0004d520: 392e 3020 2d20 5350 4458 3a20 4d49 5420  9.0 - SPDX: MIT 
 0004d530: 2d20 4d49 5420 4c69 6365 6e73 650d 0a68  - MIT License..h
 0004d540: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0004d550: 6d2f 7169 722d 616c 6c69 616e 6365 2f70  m/qir-alliance/p
 0004d560: 7971 6972 0d0a 0d0a 2f2a 0d0a 436f 7079  yqir..../*..Copy
 0004d570: 7269 6768 7420 2863 2920 3230 3135 2050  right (c) 2015 P
 0004d580: 6574 6572 204d 6172 6865 696e 650d 0a0d  eter Marheine...
 0004d590: 0a50 6572 6d69 7373 696f 6e20 6973 2068  .Permission is h
@@ -20821,15 +20821,15 @@
 00051540: 494e 4720 4652 4f4d 2c0d 0a4f 5554 204f  ING FROM,..OUT O
 00051550: 4620 4f52 2049 4e20 434f 4e4e 4543 5449  F OR IN CONNECTI
 00051560: 4f4e 2057 4954 4820 5448 4520 534f 4654  ON WITH THE SOFT
 00051570: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
 00051580: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
 00051590: 5320 494e 2054 4845 0d0a 534f 4654 5741  S IN THE..SOFTWA
 000515a0: 5245 2e0d 0a0d 0a0d 0a0d 0a70 7971 6972  RE.........pyqir
-000515b0: 2030 2e38 2e32 202d 2053 5044 583a 204d   0.8.2 - SPDX: M
+000515b0: 2030 2e39 2e30 202d 2053 5044 583a 204d   0.9.0 - SPDX: M
 000515c0: 4954 202d 204d 4954 204c 6963 656e 7365  IT - MIT License
 000515d0: 0d0a 6874 7470 733a 2f2f 6769 7468 7562  ..https://github
 000515e0: 2e63 6f6d 2f71 6972 2d61 6c6c 6961 6e63  .com/qir-allianc
 000515f0: 652f 7079 7169 720d 0a0d 0a4d 4954 204c  e/pyqir....MIT L
 00051600: 6963 656e 7365 0d0a 0d0a 436f 7079 7269  icense....Copyri
 00051610: 6768 7420 2863 2920 3230 3231 2051 4952  ght (c) 2021 QIR
 00051620: 2041 6c6c 6961 6e63 650d 0a0d 0a50 6572   Alliance....Per
```

