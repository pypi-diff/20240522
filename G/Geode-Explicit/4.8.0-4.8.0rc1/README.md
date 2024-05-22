# Comparing `tmp/Geode_Explicit-4.8.0-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.8.0rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 3139230 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 24-May-22 00:27 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 24-May-22 00:27 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 24-May-22 00:27 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  4021248 b- defN 24-May-22 00:28 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    33792 b- defN 24-May-22 00:28 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  3715072 b- defN 24-May-22 00:28 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   147456 b- defN 24-May-22 00:28 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   135680 b- defN 24-May-22 00:28 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2205 b- defN 24-May-22 00:28 Geode_Explicit-4.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-22 00:28 Geode_Explicit-4.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-May-22 00:28 Geode_Explicit-4.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 24-May-22 00:28 Geode_Explicit-4.8.0.dist-info/RECORD
-12 files, 8057400 bytes uncompressed, 3137330 bytes compressed:  61.1%
+Zip file size: 3139253 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 24-May-21 18:41 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 24-May-21 18:41 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 24-May-21 18:41 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  4021248 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    33792 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  3715072 b- defN 24-May-21 18:42 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   147456 b- defN 24-May-21 18:42 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   135680 b- defN 24-May-21 18:42 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2212 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 24-May-21 18:42 Geode_Explicit-4.8.0rc1.dist-info/RECORD
+12 files, 8057419 bytes uncompressed, 3137329 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.8.0.dist-info/METADATA
+Filename: Geode_Explicit-4.8.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.8.0.dist-info/WHEEL
+Filename: Geode_Explicit-4.8.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.8.0.dist-info/top_level.txt
+Filename: Geode_Explicit-4.8.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.8.0.dist-info/RECORD
+Filename: Geode_Explicit-4.8.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802e2024
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 22 00:27:55 2024
+Time/Date		Tue May 21 18:42:13 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002e6200
 SizeOfInitializedData	00000000000f1e00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002e2024
@@ -359150,15 +359150,15 @@
    1801327dd:	test   %rax,%rax
    1801327e0:	je     0x180132808
    1801327e2:	movq   $0x1,(%rax)
    1801327e9:	mov    %r15b,0x8(%rax)
    1801327ed:	xor    %eax,%eax
    1801327ef:	mov    %rax,0x10(%rbx)
    1801327f3:	mov    %r15,0x10(%rbx)
-   1801327f7:	lea    0x252452(%rip),%rax        # 0x180384c50
+   1801327f7:	lea    0x252432(%rip),%rax        # 0x180384c30
    1801327fe:	mov    %rax,0x18(%rbx)
    180132802:	mov    %rsi,0x40(%rbx)
    180132806:	jmp    0x18013280b
    180132808:	mov    %r15,%rbx
    18013280b:	mov    %rbx,-0x60(%rbp)
    18013280f:	mov    %r15,-0x30(%rbp)
    180132813:	mov    (%rbx),%rax
@@ -359209,15 +359209,15 @@
    1801328c0:	test   %rax,%rax
    1801328c3:	je     0x1801328eb
    1801328c5:	movq   $0x1,(%rax)
    1801328cc:	movb   $0x0,0x8(%rax)
    1801328d0:	xor    %eax,%eax
    1801328d2:	mov    %rax,0x10(%rbx)
    1801328d6:	mov    %r15,0x10(%rbx)
-   1801328da:	lea    0x25234f(%rip),%rax        # 0x180384c30
+   1801328da:	lea    0x2522ef(%rip),%rax        # 0x180384bd0
    1801328e1:	mov    %rax,0x18(%rbx)
    1801328e5:	mov    %rsi,0x40(%rbx)
    1801328e9:	jmp    0x1801328ee
    1801328eb:	mov    %r15,%rbx
    1801328ee:	mov    %rbx,-0x50(%rbp)
    1801328f2:	mov    %r15,-0x28(%rbp)
    1801328f6:	mov    (%rbx),%rax
@@ -404837,15 +404837,15 @@
    18015adf9:	test   %rax,%rax
    18015adfc:	je     0x18015ae39
    18015adfe:	movq   $0x1,(%rax)
    18015ae05:	mov    %r15b,0x8(%rax)
    18015ae09:	xor    %eax,%eax
    18015ae0b:	mov    %rax,0x10(%rsi)
    18015ae0f:	mov    %r15,0x10(%rsi)
-   18015ae13:	lea    0x229db6(%rip),%rax        # 0x180384bd0
+   18015ae13:	lea    0x229e36(%rip),%rax        # 0x180384c50
    18015ae1a:	mov    %rax,0x18(%rsi)
    18015ae1e:	movups (%rbx),%xmm0
    18015ae21:	movups %xmm0,0x40(%rsi)
    18015ae25:	mov    0x80(%rsp),%rcx
    18015ae2d:	mov    (%rcx),%rax
    18015ae30:	mov    %rax,0x50(%rsi)
    18015ae34:	mov    %r15,(%rcx)
@@ -1080893,20 +1080893,20 @@
    180384bba:	cmp    %al,0x1(%rax)
    180384bc0:	rex.RB js 0x180384c33
    180384bc3:	insb   (%dx),%es:(%rdi)
    180384bc4:	imul   $0x74,0x69(%rbx),%esp
    180384bcb:	add    %bh,%bh
    180384bcd:	(bad)
    180384bce:	(bad)
-   180384bcf:	inc    %eax
-   180384bd1:	adc    (%rsi),%edx
-   180384bd3:	addb   $0x0,(%rcx)
-   180384bd6:	add    %al,(%rax)
-   180384bd8:	movabs 0x3000000001801614,%al
-   180384be1:	adc    $0x16,%al
+   180384bcf:	push   -0x1f(%rax)
+   180384bd2:	adc    $0x180,%eax
+   180384bd7:	add    %ah,-0x1c(%rax)
+   180384bda:	adc    $0x180,%eax
+   180384bdf:	add    %ah,(%rax)
+   180384be1:	loop   0x180384bf8
    180384be3:	addb   $0x0,(%rcx)
    180384be6:	add    %al,(%rax)
    180384be8:	shl    $1,%cl
    180384bea:	adc    $0x180,%eax
    180384bef:	add    %dh,-0x1f(%rax)
    180384bf2:	adc    $0x180,%eax
    180384bf7:	add    %ah,-0x1e(%rax)
@@ -1080925,28 +1080925,28 @@
    180384c21:	loop   0x180384c38
    180384c23:	addb   $0x0,(%rcx)
    180384c26:	add    %al,(%rax)
    180384c28:	shl    $1,%cl
    180384c2a:	adc    $0x180,%eax
    180384c2f:	add    %dh,-0x1f(%rax)
    180384c32:	adc    $0x180,%eax
-   180384c37:	add    %ah,-0x1c(%rax)
-   180384c3a:	adc    $0x180,%eax
+   180384c37:	add    %dh,0x18015e4(%rax)
+   180384c3d:	add    %al,(%rax)
    180384c3f:	add    %ah,(%rax)
    180384c41:	loop   0x180384c58
    180384c43:	addb   $0x0,(%rcx)
    180384c46:	add    %al,(%rax)
    180384c48:	shl    $1,%cl
    180384c4a:	adc    $0x180,%eax
-   180384c4f:	add    %dh,-0x1f(%rax)
-   180384c52:	adc    $0x180,%eax
-   180384c57:	add    %dh,0x18015e4(%rax)
-   180384c5d:	add    %al,(%rax)
-   180384c5f:	add    %ah,(%rax)
-   180384c61:	loop   0x180384c78
+   180384c4f:	add    %al,%al
+   180384c51:	adc    (%rsi),%edx
+   180384c53:	addb   $0x0,(%rcx)
+   180384c56:	add    %al,(%rax)
+   180384c58:	movabs 0x3000000001801614,%al
+   180384c61:	adc    $0x16,%al
    180384c63:	addb   $0x0,(%rcx)
    180384c66:	add    %al,(%rax)
    180384c68:	shl    $1,%cl
    180384c6a:	adc    $0x180,%eax
    180384c6f:	add    %bh,0x4c(%rcx)
    180384c72:	cmp    %al,0x1(%rax)
 	...
@@ -1081569,19 +1081569,17 @@
    18038532a:	(bad)
    18038532b:	(bad)
    18038532c:	(bad)
    18038532d:	(bad)
    18038532e:	(bad)
    18038532f:	incl   (%rax)
    180385331:	add    %al,(%rax)
-   180385333:	add    %cl,(%rbx)
-   180385335:	cmp    $0x4d,%al
-   180385337:	data16 add %al,(%rax)
-   18038533a:	add    %al,(%rax)
-   18038533c:	or     $0x88000000,%eax
+   180385333:	add    %al,0x664ceb(%rip)        # 0x1809ea024
+   180385339:	add    %al,(%rax)
+   18038533b:	add    %cl,-0x78000000(%rip)        # 0x108385341
    180385341:	add    (%rax),%eax
    180385343:	add    %cl,0x38(%rsi,%rdi,2)
    180385347:	add    %cl,0x38(%rsp,%riz,2)
    18038534b:	add    %al,(%rax)
    18038534d:	add    %al,(%rax)
    18038534f:	add    %bh,(%rax)
    180385351:	add    %eax,(%rax)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180003fd8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 22 00:27:31 2024
+Time/Date		Tue May 21 18:41:52 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000004000
 SizeOfInitializedData	0000000000004600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000003fd8
@@ -6574,17 +6574,18 @@
    180005522:	(bad)
    180005523:	(bad)
    180005524:	(bad)
    180005525:	ljmp   (bad)
    180005526:	out    %eax,(%dx)
    180005527:	jg     0x180005529
    180005529:	add    %al,(%rax)
-   18000552b:	add    %dh,%bl
-   18000552d:	cmp    0x66(%rbp),%ecx
-   180005530:	add    %al,(%rax)
+   18000552b:	add    %dh,%al
+   18000552d:	(bad)
+   18000552e:	rex.WR
+   18000552f:	data16 add %al,(%rax)
    180005532:	add    %al,(%rax)
    180005534:	or     $0xa4000000,%eax
    180005539:	add    (%rax),%al
    18000553b:	add    %dl,0x0(%rbx,%rbx,2)
    18000553f:	add    %dl,0x0(%rdi,%rcx,2)
 	...
    18000554f:	add    %bh,(%rax)
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001802a9da8
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed May 22 00:27:36 2024
+Time/Date		Tue May 21 18:41:57 2024
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000002aba00
 SizeOfInitializedData	00000000000e1a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000002a9da8
@@ -1002208,17 +1002208,18 @@
    18034900a:	(bad)
    18034900b:	(bad)
    18034900c:	(bad)
    18034900d:	(bad)
    18034900e:	(bad)
    18034900f:	incl   (%rax)
    180349011:	add    %al,(%rax)
-   180349013:	add    %bh,%al
-   180349015:	cmp    0x66(%rbp),%ecx
-   180349018:	add    %al,(%rax)
+   180349013:	add    %dh,%ch
+   180349015:	(bad)
+   180349016:	rex.WR
+   180349017:	data16 add %al,(%rax)
    18034901a:	add    %al,(%rax)
    18034901c:	or     $0x88000000,%eax
    180349021:	add    (%rax),%eax
    180349023:	add    %cl,-0x54(%rax)
    180349026:	xor    $0x0,%al
    180349028:	rex.W (bad)
    18034902a:	xor    $0x0,%al
```

## Comparing `Geode_Explicit-4.8.0.dist-info/METADATA` & `Geode_Explicit-4.8.0rc1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.8.0
+Version: 4.8.0rc1
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background ==7.*,>=7.9.8
+Requires-Dist: geode-background ==7.*,>=7.10.0rc1
 Requires-Dist: geode-common ==31.*,>=31.1.0
 Requires-Dist: geode-conversion ==5.*,>=5.2.9
 Requires-Dist: opengeode-core ==14.*,>=14.20.0
 Requires-Dist: opengeode-inspector ==5.*,>=5.1.4
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
```

### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.8.0 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.8.0rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.9.8
+Content-Type: text/markdown Requires-Dist: geode-background ==7.*,>=7.10.0rc1
 Requires-Dist: geode-common ==31.*,>=31.1.0 Requires-Dist: geode-conversion
 ==5.*,>=5.2.9 Requires-Dist: opengeode-core ==14.*,>=14.20.0 Requires-Dist:
 opengeode-inspector ==5.*,>=5.1.4
                 ************ GGeeooddee--EExxpplliicciittbbyy GGeeooddee--ssoolluuttiioonnss ************
     ******** GGeeooddee--ssoolluuttiioonnss OOppeennGGeeooddee mmoodduullee ffoorr bbuuiillddiinngg eexxpplliicciitt mmooddeellss ********
             [Build Status][Deploy Status][Coverage Status][Version]
               [Windows support][Ubuntu support][Red Hat support]
```

## Comparing `Geode_Explicit-4.8.0.dist-info/RECORD` & `Geode_Explicit-4.8.0rc1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=3IEZJDMtMfFSTtDJOl8tpLIg5P9Iytnx2bE1I6Gg8qo,194
 geode_explicit/brep.py,sha256=i4sDZvKY0NnpwATBxQHOq2egAGLbxDH5u4iZqCHMOlk,271
 geode_explicit/section.py,sha256=k_Q35aAqi_ZAP004Xc86lQf4FSYA2u0kU6y1_iR9Ahk,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=0x4ehFZvtG7c87usG3LljZRQCvuiK4kc42Zqme2pftY,4021248
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=qN_hykbT79icFj0gla1NtDl5v78_a-xCCtMpdj278-4,33792
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=GgQhn0uCFDSjA4273vEE1lj7DMqxW7O4RAHQ4PzajXk,3715072
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=ShYp5vwQ-fS-cZ2L7oZB3ihlkLp7XtzYjNEfvmy7XMY,147456
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=V9WhrH0nouI3JYWHjjun9Q0Ov8PxgylfmXw9vEi1uNU,135680
-Geode_Explicit-4.8.0.dist-info/METADATA,sha256=XnSW1fvwHIBa7l94aPR7a9JZpBtLTIIW0NDhZ-vlHSY,2205
-Geode_Explicit-4.8.0.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-Geode_Explicit-4.8.0.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.8.0.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=bLx4Q0rkjOE__X5IgHlQU2LoAXPLtGhAAo70L225eNo,4021248
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=G7E6Cf7ImDf-VxhGxBBRpG9LiqEV88Vr41xwdEPf4dM,33792
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=S8xclsfFmxXN3uu50wWJ9sfcl_dF56KhAqiqfnXfU_w,3715072
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=JrLaFChWK8AbnEfQ1hHi_Y7LxwR70vzyjFSBWONzP4c,147456
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=si6Bgvpf9Y7tzPG7eGzgza_OPPqNQT-XTsDkTHkCzLY,135680
+Geode_Explicit-4.8.0rc1.dist-info/METADATA,sha256=C3sEXm4LwaAzkzjKuofXHAom6JP0RHHIXDmUdCY7pRs,2212
+Geode_Explicit-4.8.0rc1.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
+Geode_Explicit-4.8.0rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.8.0rc1.dist-info/RECORD,,
```

