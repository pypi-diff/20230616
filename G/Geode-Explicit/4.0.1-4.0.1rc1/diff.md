# Comparing `tmp/Geode_Explicit-4.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Explicit-4.0.1rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 2230750 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      194 b- defN 23-Jun-16 04:18 geode_explicit/__init__.py
--rw-rw-rw-  2.0 fat      271 b- defN 23-Jun-16 04:18 geode_explicit/brep.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-16 04:18 geode_explicit/section.py
--rw-rw-rw-  2.0 fat  2244096 b- defN 23-Jun-16 04:19 geode_explicit/bin/Geode-Explicit_brep.dll
--rw-rw-rw-  2.0 fat    19968 b- defN 23-Jun-16 04:19 geode_explicit/bin/Geode-Explicit_common.dll
--rw-rw-rw-  2.0 fat  2065920 b- defN 23-Jun-16 04:19 geode_explicit/bin/Geode-Explicit_section.dll
--rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-16 04:19 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   141824 b- defN 23-Jun-16 04:19 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2380 b- defN 23-Jun-16 04:19 Geode_Explicit-4.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-16 04:19 Geode_Explicit-4.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-16 04:19 Geode_Explicit-4.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1118 b- defN 23-Jun-16 04:19 Geode_Explicit-4.0.1.dist-info/RECORD
-12 files, 4629735 bytes uncompressed, 2228850 bytes compressed:  51.9%
+Zip file size: 2230794 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      194 b- defN 23-Jun-14 13:50 geode_explicit/__init__.py
+-rw-rw-rw-  2.0 fat      271 b- defN 23-Jun-14 13:50 geode_explicit/brep.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-Jun-14 13:50 geode_explicit/section.py
+-rw-rw-rw-  2.0 fat  2244096 b- defN 23-Jun-14 13:50 geode_explicit/bin/Geode-Explicit_brep.dll
+-rw-rw-rw-  2.0 fat    19968 b- defN 23-Jun-14 13:50 geode_explicit/bin/Geode-Explicit_common.dll
+-rw-rw-rw-  2.0 fat  2065920 b- defN 23-Jun-14 13:50 geode_explicit/bin/Geode-Explicit_section.dll
+-rw-rw-rw-  2.0 fat   153600 b- defN 23-Jun-14 13:50 geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   141824 b- defN 23-Jun-14 13:50 geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2395 b- defN 23-Jun-14 13:50 Geode_Explicit-4.0.1rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-14 13:50 Geode_Explicit-4.0.1rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-14 13:50 Geode_Explicit-4.0.1rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1130 b- defN 23-Jun-14 13:50 Geode_Explicit-4.0.1rc1.dist-info/RECORD
+12 files, 4629762 bytes uncompressed, 2228870 bytes compressed:  51.9%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd
 Comment: 
 
 Filename: geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Explicit-4.0.1.dist-info/METADATA
+Filename: Geode_Explicit-4.0.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Explicit-4.0.1.dist-info/WHEEL
+Filename: Geode_Explicit-4.0.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Explicit-4.0.1.dist-info/top_level.txt
+Filename: Geode_Explicit-4.0.1rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Explicit-4.0.1.dist-info/RECORD
+Filename: Geode_Explicit-4.0.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_explicit/bin/Geode-Explicit_brep.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801867dc
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun 16 04:19:01 2023
+Time/Date		Wed Jun 14 13:50:30 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000189200
 SizeOfInitializedData	000000000009a800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001867dc
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		0022b000
 SizeOfHeaders		00000400
-CheckSum		0022db44
+CheckSum		0022a122
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -666684,18 +666684,18 @@
    1801f2978:	(bad)
    1801f297d:	insb   (%dx),%es:(%rdi)
    1801f297e:	insb   (%dx),%es:(%rdi)
    1801f297f:	outsl  %ds:(%rsi),(%dx)
    1801f2980:	movsxd 0x74(%rcx),%esp
    1801f2983:	imul   $0x0,0x6e(%rdi),%ebp
    1801f298a:	add    %al,(%rax)
-   1801f298c:	mov    $0xe2,%ch
-   1801f298e:	mov    0x0(%rax,%rax,1),%esp
-   1801f2992:	add    %al,(%rax)
-   1801f2994:	or     $0x60000000,%eax
+   1801f298c:	cmpsb  %es:(%rdi),%ds:(%rsi)
+   1801f298d:	vpcmpgtb (%rax),%xmm14,%xmm0
+   1801f2991:	add    %al,(%rax)
+   1801f2993:	add    %cl,0x60000000(%rip)        # 0x1e01f2999
    1801f2999:	add    (%rax),%eax
    1801f299b:	add    %ah,(%rax)
    1801f299d:	rex.WB (bad)
    1801f299f:	add    %ah,(%rax)
    1801f29a1:	(bad)
    1801f29a2:	(bad)
 	...
```

## geode_explicit/bin/Geode-Explicit_common.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800020b0
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun 16 04:18:25 2023
+Time/Date		Wed Jun 14 13:50:12 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000002000
 SizeOfInitializedData	0000000000002a00
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000020b0
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00009000
 SizeOfHeaders		00000400
-CheckSum		00012e1c
+CheckSum		0000f41e
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -3586,17 +3586,17 @@
    1800033da:	(bad)
    1800033db:	(bad)
    1800033dc:	(bad)
    1800033dd:	(bad)
    1800033de:	(bad)
    1800033df:	incl   (%rax)
    1800033e1:	add    %al,(%rax)
-   1800033e3:	add    %dl,0x648be2(%rcx)
-   1800033e9:	add    %al,(%rax)
-   1800033eb:	add    %cl,0x7c000000(%rip)        # 0x1fc0033f1
+   1800033e3:	add    %dl,0x6489(%rbp,%rax,8)
+   1800033ea:	add    %al,(%rax)
+   1800033ec:	or     $0x7c000000,%eax
    1800033f1:	add    (%rax),%al
    1800033f3:	add    %cl,%ah
    1800033f5:	cmp    %al,(%rax)
    1800033f7:	add    %cl,%ah
    1800033f9:	sub    $0x0,%al
    1800033fb:	add    %al,(%rax)
    1800033fd:	add    %al,(%rax)
```

## geode_explicit/bin/Geode-Explicit_section.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180165310
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun 16 04:18:42 2023
+Time/Date		Wed Jun 14 13:50:16 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		0000000000166e00
 SizeOfInitializedData	0000000000091400
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000165310
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		001ff000
 SizeOfHeaders		00000400
-CheckSum		001fcb82
+CheckSum		001f916a
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -622492,27 +622492,26 @@
    1801ceef8:	(bad)
    1801ceefd:	insb   (%dx),%es:(%rdi)
    1801ceefe:	insb   (%dx),%es:(%rdi)
    1801ceeff:	outsl  %ds:(%rsi),(%dx)
    1801cef00:	movsxd 0x74(%rcx),%esp
    1801cef03:	imul   $0x0,0x6e(%rdi),%ebp
    1801cef0a:	add    %al,(%rax)
-   1801cef0c:	movabs %al,0xd00000000648be2
-   1801cef15:	add    %al,(%rax)
-   1801cef17:	add    %ah,0x3(%rax)
-   1801cef1a:	add    %al,(%rax)
-   1801cef1c:	mov    $0xa,%ah
-   1801cef1e:	sbb    $0x1cfcb400,%eax
-	...
-   1801cef2f:	add    %bh,(%rax)
-   1801cef31:	add    %eax,(%rax)
-	...
-   1801cef87:	add    %cl,(%rax)
-   1801cef89:	pop    %rbp
-   1801cef8a:	(bad)
+   1801cef0c:	cwtl
+   1801cef0d:	vpcmpgtb (%rax),%xmm14,%xmm0
+   1801cef11:	add    %al,(%rax)
+   1801cef13:	add    %cl,0x60000000(%rip)        # 0x1e01cef19
+   1801cef19:	add    (%rax),%eax
+   1801cef1b:	add    %dh,-0x34bffe3(%rdx,%rcx,1)
+   1801cef22:	sbb    $0x0,%al
+	...
+   1801cef30:	cmp    %al,(%rcx)
+	...
+   1801cef86:	add    %al,(%rax)
+   1801cef88:	or     %bl,0x1e(%rbp)
    1801cef8b:	addb   $0x0,(%rcx)
 	...
    1801cef9e:	add    %al,(%rax)
    1801cefa0:	clc
    1801cefa1:	mov    (%rsi),%dl
    1801cefa3:	addb   $0x0,(%rcx)
    1801cefa6:	add    %al,(%rax)
```

## Comparing `Geode_Explicit-4.0.1.dist-info/METADATA` & `Geode_Explicit-4.0.1rc1.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: Geode-Explicit
-Version: 4.0.1
+Version: 4.0.1rc1
 Summary: Geode-solutions OpenGeode module for building explicit models
 Home-page: https://github.com/Geode-solutions/Geode-Explicit
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: geode-background (==7.*,>=7.2.1)
-Requires-Dist: geode-common (==26.*,>=26.1.0)
-Requires-Dist: geode-conversion (==5.*,>=5.0.8)
-Requires-Dist: opengeode-core (==14.*,>=14.3.2)
-Requires-Dist: opengeode-geosciences (==7.*,>=7.0.12)
-Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.5)
+Requires-Dist: geode-common (==26.*,>=26.0.4)
+Requires-Dist: geode-conversion (==5.*,>=5.0.8rc1)
+Requires-Dist: opengeode-core (==14.*,>=14.3.2rc3)
+Requires-Dist: opengeode-geosciences (==7.*,>=7.0.12rc1)
+Requires-Dist: opengeode-geosciencesio (==4.*,>=4.1.5rc1)
 Requires-Dist: opengeode-inspector (==3.*,>=3.0.6)
 Requires-Dist: opengeode-io (==6.*,>=6.0.7)
 
 <h1 align="center">Geode-Explicit<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Geode-solutions OpenGeode module for building explicit models</h3>
 
 <p align="center">
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.1 Summary: Geode-
+Metadata-Version: 2.1 Name: Geode-Explicit Version: 4.0.1rc1 Summary: Geode-
 solutions OpenGeode module for building explicit models Home-page: https://
 github.com/Geode-solutions/Geode-Explicit Author: Geode-solutions Author-email:
 contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: geode-background (==7.*,>=7.2.1)
-Requires-Dist: geode-common (==26.*,>=26.1.0) Requires-Dist: geode-conversion
-(==5.*,>=5.0.8) Requires-Dist: opengeode-core (==14.*,>=14.3.2) Requires-Dist:
-opengeode-geosciences (==7.*,>=7.0.12) Requires-Dist: opengeode-geosciencesio
-(==4.*,>=4.1.5) Requires-Dist: opengeode-inspector (==3.*,>=3.0.6) Requires-
-Dist: opengeode-io (==6.*,>=6.0.7)
+Requires-Dist: geode-common (==26.*,>=26.0.4) Requires-Dist: geode-conversion
+(==5.*,>=5.0.8rc1) Requires-Dist: opengeode-core (==14.*,>=14.3.2rc3) Requires-
+Dist: opengeode-geosciences (==7.*,>=7.0.12rc1) Requires-Dist: opengeode-
+geosciencesio (==4.*,>=4.1.5rc1) Requires-Dist: opengeode-inspector
+(==3.*,>=3.0.6) Requires-Dist: opengeode-io (==6.*,>=6.0.7)
                 ****** Geode-Explicitby Geode-solutions ******
     **** Geode-solutions OpenGeode module for building explicit models ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Explicit-4.0.1.dist-info/RECORD` & `Geode_Explicit-4.0.1rc1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 geode_explicit/__init__.py,sha256=-1Ma-Q_qKho5-HJywdEjGH_v91Dp0h8zchFCzKp7ADk,194
 geode_explicit/brep.py,sha256=5gXUGyujJVK7W7i2Zoqb5_9Mb5jPPZLiYZX9piVVUGY,271
 geode_explicit/section.py,sha256=diHY0-G0OXfICdOX3HSTnwrdrW3WOsct7GAT4rECQb4,249
-geode_explicit/bin/Geode-Explicit_brep.dll,sha256=2WVClpdccqX74bD88nKMLaoRBJh2muvIODUzYCgxNRs,2244096
-geode_explicit/bin/Geode-Explicit_common.dll,sha256=nUJLo-9guFFduSyBpknptghcJh2N9mcamaQFMrr6jdc,19968
-geode_explicit/bin/Geode-Explicit_section.dll,sha256=foGBUiXBzOrP5bU1TwHD3BBaAmlpzyOwYuRUEBS5ofI,2065920
-geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=n_hEVSS46ll0dk1GF5_0mzYWDVeKtZIPrrtgizwZuc0,153600
-geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=Z_govyl_x9XZ5XAVCAbTGarqMPRBeGWdWSxcRMabyVc,141824
-Geode_Explicit-4.0.1.dist-info/METADATA,sha256=Xg0GJ9DV_GulSZdQNPNVDOwYkrJGBTEsvKs_jlLIz7o,2380
-Geode_Explicit-4.0.1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Explicit-4.0.1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
-Geode_Explicit-4.0.1.dist-info/RECORD,,
+geode_explicit/bin/Geode-Explicit_brep.dll,sha256=7lHLhx0t1ygrh4SZDcdltnK0ZR9LJiIjrzejXjaHKbI,2244096
+geode_explicit/bin/Geode-Explicit_common.dll,sha256=bNho9R2-iN82DDdvg-XYpTRhgyyZmF6M8rfd6-e66Ug,19968
+geode_explicit/bin/Geode-Explicit_section.dll,sha256=EY3BTNvyziwVff_xMdv72yaaPuN0nT1zWzYSeEbQs4Q,2065920
+geode_explicit/bin/geode_explicit_py_brep.cp39-win_amd64.pyd,sha256=L5qdDkIi8FsALuDhsjopawJEFi1H9QfY_DzJdrZgi94,153600
+geode_explicit/bin/geode_explicit_py_section.cp39-win_amd64.pyd,sha256=YQx0tKZyXxGWppkqWGtUJ-mFkMnxigoYz9X8BqT3Z8c,141824
+Geode_Explicit-4.0.1rc1.dist-info/METADATA,sha256=uC8TuJUZScQb3A7F4jkfZoeTjDGapMp30hiL2hyI8nk,2395
+Geode_Explicit-4.0.1rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Explicit-4.0.1rc1.dist-info/top_level.txt,sha256=SLuJS840PQSB1EAIYibu72OEG1sORAkOdcw3z29RuQQ,15
+Geode_Explicit-4.0.1rc1.dist-info/RECORD,,
```

