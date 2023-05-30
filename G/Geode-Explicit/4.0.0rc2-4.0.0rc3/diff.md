# Comparing `tmp/Geode_Explicit-4.0.0rc2-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.0.0rc3-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2246042 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-May-27 13:41 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-May-27 13:41 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-May-27 13:41 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2249216 b- defN 23-May-27 13:41 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    47616 b- defN 23-May-27 13:41 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2069504 b- defN 23-May-27 13:41 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-May-27 13:41 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-May-27 13:41 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2382 b- defN 23-May-27 13:41 Geode_Explicit-4.0.0rc2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-27 13:41 Geode_Explicit-4.0.0rc2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-27 13:41 Geode_Explicit-4.0.0rc2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1130 b- defN 23-May-27 13:41 Geode_Explicit-4.0.0rc2.dist-info/RECORD
-12 files, 4666101 bytes uncompressed, 2244118 bytes compressed:  51.9%
+Zip file size: 2246049 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-May-30 15:10 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-May-30 15:10 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-May-30 15:10 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  2249216 b- defN 23-May-30 15:11 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    47616 b- defN 23-May-30 15:11 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  2069504 b- defN 23-May-30 15:11 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-May-30 15:11 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-May-30 15:11 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2399 b- defN 23-May-30 15:11 Geode_Explicit-4.0.0rc3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-May-30 15:11 Geode_Explicit-4.0.0rc3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-30 15:11 Geode_Explicit-4.0.0rc3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 23-May-30 15:11 Geode_Explicit-4.0.0rc3.dist-info/RECORD
+12 files, 4666118 bytes uncompressed, 2244125 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc2.dist-info/METADATA
+Filename: Geode_Explicit-4.0.0rc3.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc2.dist-info/WHEEL
+Filename: Geode_Explicit-4.0.0rc3.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc2.dist-info/top_level.txt
+Filename: Geode_Explicit-4.0.0rc3.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.0.0rc2.dist-info/RECORD
+Filename: Geode_Explicit-4.0.0rc3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018018795c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat May 27 13:41:44 2023
+Time/Date		Tue May 30 15:11:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		000000000018a400
 SizeOfInitializedData	000000000009aa00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000018795c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0022c000
 SizeOfHeaders		00000400
-CheckSum		0022a65c
+CheckSum		0022b94c
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -667638,16 +667638,16 @@
    1801f3938:	(bad)
    1801f393d:	insb   (%dx),%es:(%rdi)
    1801f393e:	insb   (%dx),%es:(%rdi)
    1801f393f:	outsl  %ds:(%rsi),(%dx)
    1801f3940:	movsxd 0x74(%rcx),%esp
    1801f3943:	imul   $0x0,0x6e(%rdi),%ebp
    1801f394a:	add    %al,(%rax)
-   1801f394c:	cwtl
-   1801f394d:	or     %dh,0x64(%rdx)
+   1801f394c:	or     $0x12,%al
+   1801f394e:	jbe    0x1801f39b4
    1801f3950:	add    %al,(%rax)
    1801f3952:	add    %al,(%rax)
    1801f3954:	or     $0x60000000,%eax
    1801f3959:	add    (%rax),%eax
    1801f395b:	add    %ah,(%rax)
    1801f395d:	pop    %rcx
    1801f395e:	(bad)
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180006a6c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat May 27 13:41:25 2023
+Time/Date		Tue May 30 15:10:53 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000006a00
 SizeOfInitializedData	0000000000004c00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000006a6c
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00010000
 SizeOfHeaders		00000400
-CheckSum		0000c163
+CheckSum		0000d45b
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -10112,16 +10112,16 @@
    1800086a0:	movsxd 0x74(%rcx),%esp
    1800086a3:	imul   $0xc1800000,0x6e(%rdi),%ebp
    1800086aa:	add    %al,0x1(%rax)
    1800086b0:	and    %al,%dl
    1800086b2:	add    %al,0x1(%rax)
    1800086b8:	add    %al,(%rax)
    1800086ba:	add    %al,(%rax)
-   1800086bc:	test   %ecx,(%rax)
-   1800086be:	jb     0x180008724
+   1800086bc:	std
+   1800086bd:	adc    %esi,0x64(%rsi)
    1800086c0:	add    %al,(%rax)
    1800086c2:	add    %al,(%rax)
    1800086c4:	or     $0xec000000,%eax
    1800086c9:	add    (%rax),%al
    1800086cb:	add    %bl,-0x74(%rax)
    1800086ce:	add    %al,(%rax)
    1800086d0:	pop    %rax
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180165ef0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Sat May 27 13:41:28 2023
+Time/Date		Tue May 30 15:10:54 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000167a00
 SizeOfInitializedData	0000000000091600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000165ef0
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00200000
 SizeOfHeaders		00000400
-CheckSum		0020721d
+CheckSum		00208511
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -622498,16 +622498,16 @@
    1801cfeb8:	(bad)
    1801cfebd:	insb   (%dx),%es:(%rdi)
    1801cfebe:	insb   (%dx),%es:(%rdi)
    1801cfebf:	outsl  %ds:(%rsi),(%dx)
    1801cfec0:	movsxd 0x74(%rcx),%esp
    1801cfec3:	imul   $0x0,0x6e(%rdi),%ebp
    1801cfeca:	add    %al,(%rax)
-   1801cfecc:	mov    %cl,(%rax)
-   1801cfece:	jb     0x1801cff34
+   1801cfecc:	(bad)
+   1801cfecd:	adc    %esi,0x64(%rsi)
    1801cfed0:	add    %al,(%rax)
    1801cfed2:	add    %al,(%rax)
    1801cfed4:	or     $0x60000000,%eax
    1801cfed9:	add    (%rax),%eax
    1801cfedb:	add    %ch,0x8ac001d(%rdx,%rbx,1)
    1801cfee2:	sbb    $0x0,%eax
 	...
```

## Comparing `Geode_Explicit-4.0.0rc2.dist-info/METADATA` & `Geode_Explicit-4.0.0rc3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.0.0rc2
+Version: 4.0.0rc3
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: geode-background (==7.*,>=7.1.5)
-Requires-Dist: geode-common (==25.*,>=25.0.9)
-Requires-Dist: geode-conversion (==5.*,>=5.0.5)
-Requires-Dist: opengeode-core (==14.*,>=14.1.9)
+Requires-Dist: geode-background (==7.*,>=7.1.6rc2)
+Requires-Dist: geode-common (==25.*,>=25.0.10rc4)
+Requires-Dist: geode-conversion (==5.*,>=5.0.6rc1)
+Requires-Dist: opengeode-core (==14.*,>=14.1.10rc5)
 Requires-Dist: opengeode-geosciences (==7.*,>=7.0.8)
 Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3)
-Requires-Dist: opengeode-inspector (==3.*,>=3.0.5)
+Requires-Dist: opengeode-inspector (==3.*,>=3.0.6rc1)
 Requires-Dist: opengeode-io (==6.*,>=6.0.6)
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Explicit_private/workflows/CI/badge.svg" alt="Build Status">
```

### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.0rc2 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.0rc3 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.1.5)
-Requires-Dist: geode-common (==25.*,>=25.0.9) Requires-Dist: geode-conversion
-(==5.*,>=5.0.5) Requires-Dist: opengeode-core (==14.*,>=14.1.9) Requires-Dist:
-opengeode-geosciences (==7.*,>=7.0.8) Requires-Dist: opengeode-geosciencesio
-(==4.*,>=4.1.3) Requires-Dist: opengeode-inspector (==3.*,>=3.0.5) Requires-
-Dist: opengeode-io (==6.*,>=6.0.6)
+Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.1.6rc2)
+Requires-Dist: geode-common (==25.*,>=25.0.10rc4) Requires-Dist: geode-
+conversion (==5.*,>=5.0.6rc1) Requires-Dist: opengeode-core
+(==14.*,>=14.1.10rc5) Requires-Dist: opengeode-geosciences (==7.*,>=7.0.8)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.3) Requires-Dist:
+opengeode-inspector (==3.*,>=3.0.6rc1) Requires-Dist: opengeode-io
+(==6.*,>=6.0.6)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

