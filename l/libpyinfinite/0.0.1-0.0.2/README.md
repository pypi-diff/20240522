# Comparing `tmp/libpyinfinite-0.0.1.tar.gz` & `tmp/libpyinfinite-0.0.2.tar.gz`

## Comparing `libpyinfinite-0.0.1.tar` & `libpyinfinite-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/module.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/moduleBlockHeader.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/moduleFile.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/moduleHeader.py
--rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/module/oodle/oodleDecompressor.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/reader/__init__.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/reader/common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/__init__.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tag.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagDataBlock.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagDataReference.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagDependency.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagHeader.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagReference.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagStruct.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/tagTypes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/__init__.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetHeader.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetInstance.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetTag.py
--rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/LICENSE
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/README.md
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    42975 2020-02-02 00:00:00.000000 libpyinfinite-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/__init__.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/module.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/moduleBlockHeader.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/moduleFile.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/moduleHeader.py
+-rw-r--r--   0        0        0     3834 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/module/oodle/oodleDecompressor.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/reader/__init__.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/reader/common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/__init__.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tag.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagDataBlock.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagDataReference.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagDependency.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagHeader.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagReference.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagStruct.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/tagTypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/definitions/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/definitions/cmsw.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/definitions/rucs.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/definitions/rucy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/structs/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/structs/anyTag.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/structs/infiniteStructs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetHeader.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetInstance.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetTag.py
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/README.md
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    43543 2020-02-02 00:00:00.000000 libpyinfinite-0.0.2/PKG-INFO
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/module/module.py` & `libpyinfinite-0.0.2/libpyinfinite/module/module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from io import BytesIO
 from typing import List
 
-from .. reader import common
+from ..reader.common import read_integer, skip_empty_bytes
 
 from .moduleBlockHeader import HiModuleBlockEntry
 from .moduleFile import HiModuleFileEntry
 from .moduleHeader import HiModuleHeader
 from .oodle.oodleDecompressor import OodleDecompressor
 
 __all__ = ["HiModule"]
@@ -40,25 +40,25 @@
             file_entry = HiModuleFileEntry()
             file_entry.read(f)
             self.Files.append(file_entry)
 
         f.seek(f.tell() + 8)  # 8 Byte padding, for some reason.
 
         for _ in range(self.Header.resourceCount):
-            resource = common.read_integer(f, True, 4)
+            resource = read_integer(f, True, 4)
             self.Resources.append(resource)
 
         self.BlockListOffset = f.tell()
 
         for _ in range(self.Header.blockCount):
             block_entry = HiModuleBlockEntry()
             block_entry.read(f)
             self.Blocks.append(block_entry)
 
-        common.skip_empty_bytes(f)  # Align itself to ??????1000, done via skipping 0x00.
+        skip_empty_bytes(f)  # Align itself to ??????1000, done via skipping 0x00.
         self.FileDataOffset = f.tell()
 
     def read_tag(self, f: BytesIO, index: int, decompressor: OodleDecompressor) -> BytesIO:
         """
         Reads specified tag index from a module file.
 
         For tags with blocks:
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/module/moduleBlockHeader.py` & `libpyinfinite-0.0.2/libpyinfinite/module/moduleBlockHeader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer
 
 __all__ = ["HiModuleBlockEntry"]
 
 
 class HiModuleBlockEntry:
     """
     Module Block (20 Bytes).
@@ -20,12 +20,12 @@
         self.decomp_size: int = -1
         self.b_compressed: int = False
 
     def read(self, f: BytesIO) -> None:
         """
         Read module block variables.
         """
-        self.comp_offset = common.read_integer(f, True, 4)
-        self.comp_size = common.read_integer(f, True, 4)
-        self.decomp_offset = common.read_integer(f, True, 4)
-        self.decomp_size = common.read_integer(f, True, 4)
-        self.b_compressed = common.read_integer(f, False, 4)
+        self.comp_offset = read_integer(f, True, 4)
+        self.comp_size = read_integer(f, True, 4)
+        self.decomp_offset = read_integer(f, True, 4)
+        self.decomp_size = read_integer(f, True, 4)
+        self.b_compressed = read_integer(f, False, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/module/moduleFile.py` & `libpyinfinite-0.0.2/libpyinfinite/module/moduleFile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import struct
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer, read_string
 from enum import IntFlag
 
 __all__ = ["HiModuleFileEntry"]
 
 
 class HiModuleDataOffsetType(IntFlag):
     """
@@ -48,28 +47,28 @@
         self.assetChecksum: int = -1
         self.assetId: str = ""
 
     def read(self, f: BytesIO) -> None:
         """
         Read module file entry variables.
         """
-        self.resourceCount = common.read_integer(f, True, 4)
-        self.parentIndex = common.read_integer(f, True, 4)
-        self.unk = common.read_integer(f, True, 2)
-        self.blockCount = common.read_integer(f, True, 2)
-        self.blockIndex = common.read_integer(f, True, 4)
-        self.resourceIndex = common.read_integer(f, True, 4)
-        self.classId = common.reverse_string(struct.unpack("4s", f.read(4))[0])
-        self.dataOffset = common.read_integer(f, True, 6) & 0xFFFFFFFFFFFF
-        self.dataOffsetFlags = HiModuleDataOffsetType(common.read_integer(f, True, 2))
-        self.totalCompressedSize = common.read_integer(f, False, 4)
-        self.totalUncompressedSize = common.read_integer(f, False, 4)
-        self.globalTagId = hex(common.read_integer(f, False, 4))
-        self.uncompressedHeaderSize = common.read_integer(f, False, 4)
-        self.uncompressedTagDataSize = common.read_integer(f, False, 4)
-        self.uncompressedResourceDataSize = common.read_integer(f, False, 4)
-        self.uncompressedActualResourceSize = common.read_integer(f, False, 4)
-        self.resourceBlockCount = common.read_integer(f, True, 4)
-        self.nameOffset = common.read_integer(f, True, 4)
-        self.parentResource = common.read_integer(f, True, 4)
-        self.assetChecksum = common.read_integer(f, True, 8)
-        self.assetId = hex(common.read_integer(f, False, 8))
+        self.resourceCount = read_integer(f, True, 4)
+        self.parentIndex = read_integer(f, True, 4)
+        self.unk = read_integer(f, True, 2)
+        self.blockCount = read_integer(f, True, 2)
+        self.blockIndex = read_integer(f, True, 4)
+        self.resourceIndex = read_integer(f, True, 4)
+        self.classId = read_string(f, 4)
+        self.dataOffset = read_integer(f, True, 6) & 0xFFFFFFFFFFFF
+        self.dataOffsetFlags = HiModuleDataOffsetType(read_integer(f, True, 2))
+        self.totalCompressedSize = read_integer(f, False, 4)
+        self.totalUncompressedSize = read_integer(f, False, 4)
+        self.globalTagId = hex(read_integer(f, False, 4))
+        self.uncompressedHeaderSize = read_integer(f, False, 4)
+        self.uncompressedTagDataSize = read_integer(f, False, 4)
+        self.uncompressedResourceDataSize = read_integer(f, False, 4)
+        self.uncompressedActualResourceSize = read_integer(f, False, 4)
+        self.resourceBlockCount = read_integer(f, True, 4)
+        self.nameOffset = read_integer(f, True, 4)
+        self.parentResource = read_integer(f, True, 4)
+        self.assetChecksum = read_integer(f, True, 8)
+        self.assetId = hex(read_integer(f, False, 8))
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/module/moduleHeader.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tagHeader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,59 @@
-import struct
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer, read_string
 
-__all__ = ["HiModuleHeader"]
+__all__ = ["HiTagHeader"]
 
 
-class HiModuleHeader:
-    """
-    Module Header (72 Bytes).
-    """
-
+class HiTagHeader:
     def __init__(self) -> None:
         """
-        Initialize module header variables.
+        Initialize tag header variables.
         """
         self.magic: str = ""
         self.version: int = -1
-        self.moduleId: int = -1
-        self.fileCount: int = -1
-        self.manifest0Count: int = -1
-        self.manifest1Count: int = -1
-        self.manifest2Count: int = -1
-        self.resourceIndex: int = -1
-        self.stringsSize: int = -1
-        self.resourceCount: int = -1
-        self.blockCount: int = -1
-        self.BuildVersion: int = -1
-        self.hd1Delta: int = -1
+        self.tagHash: int = -1
+        self.assetChecksum: int = -1
+        self.dependencyCount: int = -1
+        self.datablockCount: int = -1
+        self.tagStructCount: int = -1
+        self.dataReferenceCount: int = -1
+        self.tagReferenceCount: int = -1
+        self.stringTableSize: int = -1
+        self.zonesetDataSize: int = -1
+        self.unknownDescInfoType: int = -1
+        self.headerSize: int = -1
         self.dataSize: int = -1
+        self.resourceDataSize: int = -1
+        self.ActualResourceSize: int = -1
+        self.headerAlignment: int = -1
+        self.tagDataAlignment: int = -1
+        self.resourceDataAlignment: int = -1
+        self.ActualResourceAlignment: int = -1
+        self.unknownProperty: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
-        Read module header variables.
+        Read tag header variables.
         """
-        self.magic = struct.unpack("4s", f.read(4))[0]
-        self.version = common.read_integer(f, True, 4)
-        self.moduleId = common.read_integer(f, True, 8)
-        self.fileCount = common.read_integer(f, True, 4)
-        self.manifest0Count = common.read_integer(f, True, 4)
-        self.manifest1Count = common.read_integer(f, True, 4)
-        self.manifest2Count = common.read_integer(f, True, 4)
-        self.resourceIndex = common.read_integer(f, True, 4)
-        self.stringsSize = common.read_integer(f, False, 4)
-        self.resourceCount = common.read_integer(f, False, 4)
-        self.blockCount = common.read_integer(f, False, 4)
-        self.BuildVersion = common.read_integer(f, False, 8)
-        self.hd1Delta = common.read_integer(f, False, 8)
-        self.dataSize = common.read_integer(f, True, 8)
+        self.magic = read_string(f, 4)
+        self.version = read_integer(f, True, 4)
+        self.tagHash = read_integer(f, True, 8)
+        self.assetChecksum = read_integer(f, True, 8)
+        self.dependencyCount = read_integer(f, True, 4)
+        self.datablockCount = read_integer(f, True, 4)
+        self.tagStructCount = read_integer(f, True, 4)
+        self.dataReferenceCount = read_integer(f, True, 4)
+        self.tagReferenceCount = read_integer(f, True, 4)
+        self.stringTableSize = read_integer(f, True, 4)
+        self.zonesetDataSize = read_integer(f, True, 4)
+        self.unknownDescInfoType = read_integer(f, True, 4)
+        self.headerSize = read_integer(f, True, 4)
+        self.dataSize = read_integer(f, True, 4)
+        self.resourceDataSize = read_integer(f, True, 4)
+        self.ActualResourceSize = read_integer(f, True, 4)
+        self.headerAlignment = read_integer(f, True, 1)
+        self.tagDataAlignment = read_integer(f, True, 1)
+        self.resourceDataAlignment = read_integer(f, True, 1)
+        self.ActualResourceAlignment = read_integer(f, True, 1)
+        self.unknownProperty = read_integer(f, True, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/module/oodle/oodleDecompressor.py` & `libpyinfinite-0.0.2/libpyinfinite/module/oodle/oodleDecompressor.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tag.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tag.py`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tagDataBlock.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tagDataBlock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer
 
 from .tagTypes import HiTagSectionType
 
 __all__ = ["HiTagDataBlock"]
 
 
 class HiTagDataBlock:
@@ -21,11 +21,11 @@
         self.section: HiTagSectionType = HiTagSectionType(0)
         self.offset: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
         Reads data block variables.
         """
-        self.entrySize = common.read_integer(f, True, 4)
-        self.pad = common.read_integer(f, True, 2)
-        self.section = HiTagSectionType(common.read_integer(f, True, 2))
-        self.offset = common.read_integer(f, True, 8)
+        self.entrySize = read_integer(f, True, 4)
+        self.pad = read_integer(f, True, 2)
+        self.section = HiTagSectionType(read_integer(f, True, 2))
+        self.offset = read_integer(f, True, 8)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tagDataReference.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tagDataReference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer
 
 __all__ = ["HiTagDataReference"]
 
 
 class HiTagDataReference:
     """
     Tag Data Reference (20 Bytes)
@@ -20,12 +20,12 @@
         self.fieldBlock: int = -1
         self.fieldOffset: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
         Read Tag Data variables.
         """
-        self.parentStructIndex = common.read_integer(f, True, 4)
-        self.unknown = common.read_integer(f, True, 4)
-        self.targetIndex = common.read_integer(f, True, 4)
-        self.fieldBlock = common.read_integer(f, True, 4)
-        self.fieldOffset = common.read_integer(f, False, 4)
+        self.parentStructIndex = read_integer(f, True, 4)
+        self.unknown = read_integer(f, True, 4)
+        self.targetIndex = read_integer(f, True, 4)
+        self.fieldBlock = read_integer(f, True, 4)
+        self.fieldOffset = read_integer(f, False, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tagDependency.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tagReference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import struct
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer
 
-__all__ = ["HiTagDependency"]
+__all__ = ["HiTagReference"]
 
 
-class HiTagDependency:
+class HiTagReference:
+    """
+    Tag Reference (16 Bytes)
+    """
+
     def __init__(self) -> None:
         """
-        Initialize tag dependency variables.
+        Initializes tag reference variables.
         """
-        self.tagGroup: str = ""
+        self.fieldBlock: int = -1
+        self.fieldOffset: int = -1
         self.nameOffset: int = -1
-        self.assetId: int = -1
-        self.globalId: int = -1
-        self.parent: int = -1
+        self.dependencyIndex: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
-        Read tag dependency variables.
+        Reads tag reference variables.
         """
-        self.tagGroup = common.reverse_string(struct.unpack("4s", f.read(4))[0])
-        self.nameOffset = common.read_integer(f, True, 4)
-        self.assetId = common.read_integer(f, True, 8)
-        self.globalId = common.read_integer(f, True, 4)
-        self.parent = common.read_integer(f, True, 4)
+        self.fieldBlock = read_integer(f, True, 4)
+        self.fieldOffset = read_integer(f, False, 4)
+        self.nameOffset = read_integer(f, False, 4)
+        self.dependencyIndex = read_integer(f, True, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tagReference.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/tagStruct.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from io import BytesIO
 
-from .. reader import common
+from ..reader.common import read_integer
 
-__all__ = ["HiTagReference"]
+from .tagTypes import HiTagStructType
 
+__all__ = ["HiTagStruct"]
 
-class HiTagReference:
+
+class HiTagStruct:
     """
-    Tag Reference (16 Bytes)
+    Tag Struct (32 Bytes)
     """
 
     def __init__(self) -> None:
         """
-        Initializes tag reference variables.
+        Initializes tag struct variables.
         """
+        self.guid: int = -1
+        self.type: HiTagStructType = HiTagStructType(0)
+        self.unknown: int = -1
+        self.targetIndex: int = -1
         self.fieldBlock: int = -1
         self.fieldOffset: int = -1
-        self.nameOffset: int = -1
-        self.dependencyIndex: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
-        Reads tag reference variables.
+        Reads tag struct variables.
         """
-        self.fieldBlock = common.read_integer(f, True, 4)
-        self.fieldOffset = common.read_integer(f, False, 4)
-        self.nameOffset = common.read_integer(f, False, 4)
-        self.dependencyIndex = common.read_integer(f, True, 4)
+        self.guid = read_integer(f, True, 16)
+        self.type = HiTagStructType(read_integer(f, True, 2))
+        self.unknown = read_integer(f, True, 2)
+        self.targetIndex = read_integer(f, True, 4)
+        self.fieldBlock = read_integer(f, True, 4)
+        self.fieldOffset = read_integer(f, False, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/tagStruct.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/structs/anyTag.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 from io import BytesIO
+from ...reader.common import read_integer
 
-from .. reader import common
+__all__ = ["AnyTag"]
 
-from .tagTypes import HiTagStructType
 
-__all__ = ["HiTagStruct"]
+class InternalStruct:
+    def __init__(self) -> None:
+        self.globalTagId: str = ""
+        self.localTagHandle: int = -1
+
+    def read(self, f: BytesIO) -> None:
+        self.globalTagId = hex(read_integer(f, False, 4))
+        self.localTagHandle = read_integer(f, False, 4)
 
 
-class HiTagStruct:
+class AnyTag:
     """
-    Tag Struct (32 Bytes)
+    AnyTag is located at the top struct of every tag.
+    It initializes tag pointers and also provides the global tag ID
+    which is registered on the "hydrated" tag list in memory.
     """
 
     def __init__(self) -> None:
-        """
-        Initializes tag struct variables.
-        """
-        self.guid: int = -1
-        self.type: HiTagStructType = HiTagStructType(0)
-        self.unknown: int = -1
-        self.targetIndex: int = -1
-        self.fieldBlock: int = -1
-        self.fieldOffset: int = -1
+        self.vtableSpace: int = -1
+        self.internalStruct: InternalStruct = InternalStruct()
 
     def read(self, f: BytesIO) -> None:
-        """
-        Reads tag struct variables.
-        """
-        self.guid = common.read_integer(f, True, 16)
-        self.type = HiTagStructType(common.read_integer(f, True, 2))
-        self.unknown = common.read_integer(f, True, 2)
-        self.targetIndex = common.read_integer(f, True, 4)
-        self.fieldBlock = common.read_integer(f, True, 4)
-        self.fieldOffset = common.read_integer(f, False, 4)
+        self.vtableSpace = read_integer(f, False, 8)
+        self.internalStruct.read(f)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetHeader.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetHeader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 
-from ... reader import common
+from ...reader.common import read_integer
 
 __all__ = ["HiTagZonesetHeader"]
 
 
 class HiTagZonesetHeader:
     """
     Zoneset Header (16 Bytes)
@@ -19,11 +19,11 @@
         self.footerCount: int = -1
         self.parents: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
         Reads Zoneset Header.
         """
-        self.version = common.read_integer(f, True, 4)
-        self.zonesetCount = common.read_integer(f, True, 4)
-        self.footerCount = common.read_integer(f, True, 4)
-        self.parents = common.read_integer(f, True, 4)
+        self.version = read_integer(f, True, 4)
+        self.zonesetCount = read_integer(f, True, 4)
+        self.footerCount = read_integer(f, True, 4)
+        self.parents = read_integer(f, True, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetInstance.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetInstance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .zonesetInstanceHeader import HiTagZonesetInstanceHeader
 from .zonesetTag import HiTagZonesetTag
 from typing import List
 from io import BytesIO
-from ... reader import common
+from ...reader.common import read_integer
 
 __all__ = ["HiTagZoneInstance"]
 
 
 class HiTagZoneInstance:
     """
     Main zoneset instance block.
@@ -36,9 +36,9 @@
 
         for _ in range(self.Header.footerCount):
             footer_tag_entry = HiTagZonesetTag()
             footer_tag_entry.read(f)
             self.ZoneSetFooterTags.append(footer_tag_entry)
 
         for _ in range(self.Header.parentCount):
-            parent_entry = common.read_integer(f, True, 4)
+            parent_entry = read_integer(f, True, 4)
             self.ZoneSetParents.append(parent_entry)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetInstanceHeader.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BytesIO
 
-from ... reader import common
+from ...reader.common import read_integer
 
 __all__ = ["HiTagZonesetInstanceHeader"]
 
 
 class HiTagZonesetInstanceHeader:
     """
     Zoneset Instance Header (16 Bytes)
@@ -19,11 +19,11 @@
         self.parentCount: int = -1
         self.footerCount: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
         Reads zoneset instance header variables.
         """
-        self.stringId = common.read_integer(f, True, 4)
-        self.tagCount = common.read_integer(f, True, 4)
-        self.parentCount = common.read_integer(f, True, 4)
-        self.footerCount = common.read_integer(f, True, 4)
+        self.stringId = read_integer(f, True, 4)
+        self.tagCount = read_integer(f, True, 4)
+        self.parentCount = read_integer(f, True, 4)
+        self.footerCount = read_integer(f, True, 4)
```

### Comparing `libpyinfinite-0.0.1/libpyinfinite/tag/zonesets/zonesetTag.py` & `libpyinfinite-0.0.2/libpyinfinite/tag/zonesets/zonesetTag.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from io import BytesIO
 
-from ... reader import common
+from ...reader.common import read_integer
 
 __all__ = ["HiTagZonesetTag"]
 
 
 class HiTagZonesetTag:
     """
     Zoneset Tag (8 Bytes)
     """
 
     def __init__(self) -> None:
         """
         Initialize zoneset tag variables.
         """
-        self.globalId: int = -1
+        self.globalId: str = ""
         self.stringId: int = -1
 
     def read(self, f: BytesIO) -> None:
         """
         Reads zoneset tag variables.
         """
-        self.globalId = common.read_integer(f, False, 4)
-        self.stringId = common.read_integer(f, True, 4)
+        self.globalId = hex(read_integer(f, False, 4))
+        self.stringId = read_integer(f, True, 4)
```

### Comparing `libpyinfinite-0.0.1/.gitignore` & `libpyinfinite-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.0.1/LICENSE` & `libpyinfinite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libpyinfinite-0.0.1/pyproject.toml` & `libpyinfinite-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "libpyinfinite"
-version = "0.0.1"
-description = "Python library for dealing with binary files from Halo Infinite"
+version = "0.0.2"
+description = "Python library for parsing binary files from Halo Infinite."
 license = {file = "LICENSE"}
 authors = [{ name = "Surasia"}]
 requires-python = ">= 3.11.0"
 readme = "README.md"
 keywords = ["Halo", "Halo Infinite", "Module", "Tags", "Module"]
 classifiers = [
     "Typing :: Typed",
@@ -16,14 +16,15 @@
     "Intended Audience :: Developers",
     "Development Status :: 3 - Alpha"
 ]
 
 [project.urls]
 Repository = "https://github.com/Surasia/libpyinfinite"
 Issues = "https://github.com/Surasia/libpyinfinite/issues"
+Changelog = "https://github.com/Surasia/libpyinfinite/main/CHANGELOG.md"
 
 
 
 [tool.rye]
 dev-dependencies = [
     "pyright",
     "mypy",
@@ -38,15 +39,14 @@
 format = { chain = ["format:ruff","fix:ruff",]}
 "format:ruff" = "ruff format"
 "lint" = { chain = ["check:ruff","typecheck",]}
 "check:ruff" = "ruff ."
 "fix:ruff" = "ruff --fix ."
 typecheck = { chain = ["typecheck:pyright","typecheck:mypy"]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes openai --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
```

### Comparing `libpyinfinite-0.0.1/PKG-INFO` & `libpyinfinite-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: libpyinfinite
-Version: 0.0.1
-Summary: Python library for dealing with binary files from Halo Infinite
+Version: 0.0.2
+Summary: Python library for parsing binary files from Halo Infinite.
 Project-URL: Repository, https://github.com/Surasia/libpyinfinite
 Project-URL: Issues, https://github.com/Surasia/libpyinfinite/issues
+Project-URL: Changelog, https://github.com/Surasia/libpyinfinite/main/CHANGELOG.md
 Author: Surasia
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -687,66 +688,91 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 
-# libpyinfinite 
-[![latest](https://img.shields.io/pypi/v/libpyinfinite.svg)](https://pypi.python.org/pypi/libpinfinite/)
+# libpyinfinite
 
-LibPyInfinite is a typed python library for parsing Halo Infinite binary files. It implements a module and tag reader that can be used indepently, including all types required.
+[![latest](https://img.shields.io/pypi/v/libpyinfinite.svg)](https://pypi.python.org/pypi/libpyinfinite/)
+
+LibPyInfinite is a typed python library for parsing Halo Infinite binary files. It implements a module and tag reader that can be used indepently or in conjunction.
 
 ## Installation
+
 Libpyinfinite is available on pypi.
 
 `pip install libpyinfinite`
 
 ## Example Usage
 
 #### Reading a module instance:
+
 ```python
 from libpyinfinite.module.module import HiModule
 
-def readModule():
+def read_module():
     with open(modulepath, "rb") as file:
-        moduleInstance = HiModule()
-        moduleInstance.read(file)
+        module_instance = HiModule()
+        module_instance.read(file)
 ```
 
 #### Creating a Oodle Decompressor:
-Oodle is a decompression library used to pack module files, requiring DLL calls to oo2core_8_win64.dll. This requirement limits libpyinfinite's tag reader to 64-Bit Windows only, though a Linux implementation via linoodle is planned. 
+
+Oodle is a decompression library used to pack module files, requiring DLL calls to oo2core_8_win64.dll. This is achieved by either directly specifying the DLL or in Linux systems, using [linoodle](https://github.com/McSimp/linoodle/releases/tag/1.0.0).
+
 ```python
 from libpyinfinite.module.oodle.oodleDecompressor import OodleDecompressor
 
-decompressor = OodleDecompressor("./oo2core_8_win64.dll")
+decompressor = OodleDecompressor("./oo2core_8_win64.dll") # Windows 64-Bit
+decompressor = OodleDecompressor("./linoodle.so") # Linux/Linux-like. (Requires DLL to be in the same directory.)
 ```
 
 #### Reading the third tag from a module instance:
+
 ```python
 from libpyinfinite.tag.tag import HiTag
 
+# File handle of module, index of tag, decompressor
 tagData = moduleInstance.read_tag(file, 3, decompressor)
 tagInstance = HiTag()
 tagInstance.read(tagData)
 ```
 
 #### Accessing values from a tag:
+
 ```python
 print(tagInstance.Header.magic)
 
 >>> "ucsh"
 
 for ref in tagInstance.Dependencies:
     print(f"Tag Reference: {ref.globalId}")
 
->>> "Tag Reference: FFFFFFF"
->>> "Tag Reference: 0A00000"
+>>> "Tag Reference: 0xFFFFFFF"
+>>> "Tag Reference: 0x0A00000"
+```
+
+#### Using defined tag structures
+```python
+# Reading "RUCY" tag
+from libpyinfinite.tag.definitions.rucy import RuntimeCoatingStyleTag
+
+rucy = RuntimeCoatingStyleTag()
+rucy.read(tagData)
+
+# What's the emissive intensity of this tag?
+print(rucy.info.emissiveIntensity)
+
+>>> 0.00
+
 ```
 
 ## Credits
+
 - MontagueM for OodleDecompressor
 - Gamergotten for TagFramework
 - Coreforge for libinfinite
 - Z-15 for HITE
 - Urium86 for pyhirtlib and LibHIRT
-- Shockfire for Ausardocs
+- Shockfire for Ausardocs
```

