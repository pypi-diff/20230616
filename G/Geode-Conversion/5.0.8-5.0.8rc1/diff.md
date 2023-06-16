# Comparing `tmp/Geode_Conversion-5.0.8-cp39-cp39-win_amd64.whl.zip` & `tmp/Geode_Conversion-5.0.8rc1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 1213857 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-16 04:09 geode_conversion/__init__.py
--rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-16 04:09 geode_conversion/model.py
--rw-rw-rw-  2.0 fat  2416128 b- defN 23-Jun-16 04:09 geode_conversion/bin/Geode-Conversion_model.dll
--rw-rw-rw-  2.0 fat   150528 b- defN 23-Jun-16 04:09 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2001 b- defN 23-Jun-16 04:09 Geode_Conversion-5.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-16 04:09 Geode_Conversion-5.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-16 04:09 Geode_Conversion-5.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      731 b- defN 23-Jun-16 04:09 Geode_Conversion-5.0.8.dist-info/RECORD
-8 files, 2569854 bytes uncompressed, 1212569 bytes compressed:  52.8%
+Zip file size: 1213885 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-13 15:29 geode_conversion/__init__.py
+-rw-rw-rw-  2.0 fat      178 b- defN 23-Jun-13 15:29 geode_conversion/model.py
+-rw-rw-rw-  2.0 fat  2416128 b- defN 23-Jun-13 15:29 geode_conversion/bin/Geode-Conversion_model.dll
+-rw-rw-rw-  2.0 fat   150528 b- defN 23-Jun-13 15:29 geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     2007 b- defN 23-Jun-13 15:30 Geode_Conversion-5.0.8rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Jun-13 15:30 Geode_Conversion-5.0.8rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jun-13 15:30 Geode_Conversion-5.0.8rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      743 b- defN 23-Jun-13 15:30 Geode_Conversion-5.0.8rc1.dist-info/RECORD
+8 files, 2569872 bytes uncompressed, 1212573 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: geode_conversion/bin/Geode-Conversion_model.dll
 Comment: 
 
 Filename: geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd
 Comment: 
 
-Filename: Geode_Conversion-5.0.8.dist-info/METADATA
+Filename: Geode_Conversion-5.0.8rc1.dist-info/METADATA
 Comment: 
 
-Filename: Geode_Conversion-5.0.8.dist-info/WHEEL
+Filename: Geode_Conversion-5.0.8rc1.dist-info/WHEEL
 Comment: 
 
-Filename: Geode_Conversion-5.0.8.dist-info/top_level.txt
+Filename: Geode_Conversion-5.0.8rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: Geode_Conversion-5.0.8.dist-info/RECORD
+Filename: Geode_Conversion-5.0.8rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## geode_conversion/bin/Geode-Conversion_model.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001801a1b68
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jun 16 04:09:47 2023
+Time/Date		Tue Jun 13 15:29:53 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000001a6400
 SizeOfInitializedData	00000000000a7600
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000001a1b68
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00255000
 SizeOfHeaders		00000400
-CheckSum		00252e47
+CheckSum		00257947
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -709451,16 +709451,16 @@
    180210a78:	(bad)
    180210a7d:	insb   (%dx),%es:(%rdi)
    180210a7e:	insb   (%dx),%es:(%rdi)
    180210a7f:	outsl  %ds:(%rsi),(%dx)
    180210a80:	movsxd 0x74(%rcx),%esp
    180210a83:	imul   $0x0,0x6e(%rdi),%ebp
    180210a8a:	add    %al,(%rax)
-   180210a8c:	mov    %eax,%esp
-   180210a8e:	mov    0x0(%rax,%rax,1),%esp
+   180210a8c:	jno    0x180210a19
+   180210a8e:	mov    %ah,0x0(%rax,%rax,1)
    180210a92:	add    %al,(%rax)
    180210a94:	or     $0x60000000,%eax
    180210a99:	add    (%rax),%eax
    180210a9b:	add    %bh,(%rax)
    180210a9d:	ss and %eax,(%rax)
    180210aa0:	cmp    %bl,(%rsi)
    180210aa2:	and    %eax,(%rax)
@@ -776517,23 +776517,18 @@
    180239777:	imul   $0x24406873,0x65(%rbp,%rcx,2),%esp
    18023977f:	xor    %dh,(%rdx)
    180239781:	rex
    180239782:	outsl  %gs:(%esi),(%dx)
    180239785:	fs gs rex
    180239788:	rex
    180239789:	rex (bad)
-   18023978b:	xor    %dil,0x34(%r8)
-   18023978f:	cmp    %dh,(%rbx)
-   180239791:	(bad)
-   180239793:	xor    (%rax),%esi
-   180239795:	xor    $0x40,%al
-   180239797:	rex add %al,(%rax)
-   18023979a:	add    %al,(%rax)
-   18023979c:	add    %al,(%rax)
-   18023979e:	add    %al,(%rax)
+   18023978b:	xor    %dil,0x35(%r8)
+   18023978f:	xor    %si,%gs:(%rdi)
+   180239793:	ss xor %al,%fs:0x40(%rax)
+	...
    1802397a0:	test   $0x9,%al
    1802397a2:	and    %eax,0x1(%rax)
 	...
    1802397b0:	cs (bad)
    1802397b2:	push   %r14
    1802397b4:	rex.WB insl (%dx),%es:(%rdi)
    1802397b6:	jo     0x180239824
@@ -776572,20 +776567,18 @@
    18023980c:	gs jae 0x180239877
    18023980f:	rex and $0x30,%al
    180239812:	xor    %eax,0x67(%rax)
    180239815:	outsl  %gs:(%rsi),(%dx)
    180239817:	fs gs rex
    18023981a:	rex
    18023981b:	rex (bad)
-   18023981d:	xor    %dil,0x34(%r8)
-   180239821:	cmp    %dh,(%rbx)
-   180239823:	(bad)
-   180239825:	xor    (%rax),%esi
-   180239827:	xor    $0x40,%al
-   180239829:	rex add %al,(%rax)
+   18023981d:	xor    %dil,0x35(%r8)
+   180239821:	xor    %si,%gs:(%rdi)
+   180239825:	ss xor %al,%fs:0x40(%rax)
+   18023982a:	add    %al,(%rax)
    18023982c:	add    %al,(%rax)
    18023982e:	add    %al,(%rax)
    180239830:	test   $0x9,%al
    180239832:	and    %eax,0x1(%rax)
 	...
    180239840:	cs (bad)
    180239842:	push   %r14
@@ -776626,20 +776619,18 @@
    18023989c:	gs jae 0x180239907
    18023989f:	rex and $0x30,%al
    1802398a2:	xor    0x67(%rax),%al
    1802398a5:	outsl  %gs:(%rsi),(%dx)
    1802398a7:	fs gs rex
    1802398aa:	rex
    1802398ab:	rex (bad)
-   1802398ad:	xor    %dil,0x34(%r8)
-   1802398b1:	cmp    %dh,(%rbx)
-   1802398b3:	(bad)
-   1802398b5:	xor    (%rax),%esi
-   1802398b7:	xor    $0x40,%al
-   1802398b9:	rex add %al,(%rax)
+   1802398ad:	xor    %dil,0x35(%r8)
+   1802398b1:	xor    %si,%gs:(%rdi)
+   1802398b5:	ss xor %al,%fs:0x40(%rax)
+   1802398ba:	add    %al,(%rax)
    1802398bc:	add    %al,(%rax)
    1802398be:	add    %al,(%rax)
    1802398c0:	test   $0x9,%al
    1802398c2:	and    %eax,0x1(%rax)
 	...
    1802398d0:	cs (bad)
    1802398d2:	push   %r14
```

## Comparing `Geode_Conversion-5.0.8.dist-info/METADATA` & `Geode_Conversion-5.0.8rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Geode-Conversion
-Version: 5.0.8
+Version: 5.0.8rc1
 Summary: Conversion module for Geode-solutions OpenGeode modules
 Home-page: https://github.com/Geode-solutions/Geode-Conversion
 Author: Geode-solutions
 Author-email: contact@geode-solutions.com
 License: Proprietary
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: opengeode-core (==14.*,>=14.3.2)
+Requires-Dist: opengeode-core (==14.*,>=14.3.2rc2)
 
 <h1 align="center">Geode-Conversion<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">Conversion OpenGeode module</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/Geode-Conversion_private/workflows/CD/badge.svg" alt="Deploy Status">
```

### html2text {}

```diff
@@ -1,11 +1,12 @@
-Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.8 Summary: Conversion
-module for Geode-solutions OpenGeode modules Home-page: https://github.com/
-Geode-solutions/Geode-Conversion Author: Geode-solutions Author-email:
-contact@geode-solutions.com License: Proprietary Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: opengeode-core (==14.*,>=14.3.2)
+Metadata-Version: 2.1 Name: Geode-Conversion Version: 5.0.8rc1 Summary:
+Conversion module for Geode-solutions OpenGeode modules Home-page: https://
+github.com/Geode-solutions/Geode-Conversion Author: Geode-solutions Author-
+email: contact@geode-solutions.com License: Proprietary Platform: UNKNOWN
+Description-Content-Type: text/markdown Requires-Dist: opengeode-core
+(==14.*,>=14.3.2rc2)
                ****** Geode-Conversionby Geode-solutions ******
                      **** Conversion OpenGeode module ****
           [Build Status] [Deploy Status] [Coverage Status] [Version]
              [Windows support] [Ubuntu support] [Red Hat support]
   [Language] [License] [Semantic-release] [Slack_invite] Copyright (c) 2019 -
                             2023, Geode-solutions
```

## Comparing `Geode_Conversion-5.0.8.dist-info/RECORD` & `Geode_Conversion-5.0.8rc1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 geode_conversion/__init__.py,sha256=Ia-ZwhIAokDIC6uBDumiY-s6IwjLi8gNTQti1qPYKh4,171
 geode_conversion/model.py,sha256=w4pnyFhioSDpM5WfYbW6h0wyzZSYYvZewwttq1oMEy4,178
-geode_conversion/bin/Geode-Conversion_model.dll,sha256=tmHbfbTsZOdNj8nHKWRi40hh8K5QbdzIp1cF2aTRR4o,2416128
-geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=Iqd1veFBryOX4CWtzMcg0nzKLMAAoGlTzoR2ia0XHi8,150528
-Geode_Conversion-5.0.8.dist-info/METADATA,sha256=K90lzIJvIqlcCGS3dNudRgsYmURtEmGNrLHY_qpX27g,2001
-Geode_Conversion-5.0.8.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
-Geode_Conversion-5.0.8.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
-Geode_Conversion-5.0.8.dist-info/RECORD,,
+geode_conversion/bin/Geode-Conversion_model.dll,sha256=8FHTAN1yeGOxRBjwt6qf8hFCSA8QXXRhTbf4jiBM42Y,2416128
+geode_conversion/bin/geode_conversion_py_model.cp39-win_amd64.pyd,sha256=4937HPntahmDQYNZu8uIbe0L-RkQ3fmB6SJpbB5UPDU,150528
+Geode_Conversion-5.0.8rc1.dist-info/METADATA,sha256=P2zcK4f-ishGW4vcTOZPssc0MW-K0NTiAwZzSPiihA8,2007
+Geode_Conversion-5.0.8rc1.dist-info/WHEEL,sha256=eep6QWEFiQfg2wcclssb_WY-D33AnLYLnEKGA9Rn-VU,100
+Geode_Conversion-5.0.8rc1.dist-info/top_level.txt,sha256=PnM_M6Sy8psC1M_rMpCs6FAGjv7uyDWsRvR46jFUpXU,17
+Geode_Conversion-5.0.8rc1.dist-info/RECORD,,
```

