# Comparing `tmp/tabdoc-1.0.3-py3-none-any.whl.zip` & `tmp/tabdoc-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5306943 bytes, number of entries: 12
--rw-r--r--  2.0 unx      205 b- defN 23-May-03 15:37 tabdoc/__init__.py
+Zip file size: 5307024 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      205 b- defN 23-Jun-16 09:41 tabdoc/__init__.py
 -rw-r--r--  2.0 unx     7681 b- defN 23-Apr-27 17:15 tabdoc/tabexcel.py
 -rw-r--r--  2.0 unx    10330 b- defN 19-Oct-15 10:31 tabdoc/tabpdf.py
--rw-r--r--  2.0 unx    16014 b- defN 23-May-10 05:13 tabdoc/tabword.py
+-rw-r--r--  2.0 unx    16022 b- defN 23-Jun-16 09:38 tabdoc/tabword.py
 -rw-r--r--  2.0 unx 10063973 b- defN 19-Feb-13 10:22 tabdoc/templates/SimHei.ttf
 -rw-r--r--  2.0 unx      112 b- defN 19-Jul-25 12:59 tabdoc/templates/__init__.py
--rw-r--r--  2.0 unx    17822 b- defN 23-May-04 09:15 tabdoc/templates/template.docx
--rw-r--r--  2.0 unx     1066 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1272 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      938 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/RECORD
-12 files, 10119512 bytes uncompressed, 5305393 bytes compressed:  47.6%
+-rw-r--r--  2.0 unx    17531 b- defN 23-Jun-16 09:41 tabdoc/templates/template.docx
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jun-16 09:43 tabdoc-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1272 b- defN 23-Jun-16 09:43 tabdoc-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 09:43 tabdoc-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-16 09:43 tabdoc-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      938 b- defN 23-Jun-16 09:43 tabdoc-1.0.4.dist-info/RECORD
+12 files, 10119229 bytes uncompressed, 5305474 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tabdoc/templates/__init__.py
 Comment: 
 
 Filename: tabdoc/templates/template.docx
 Comment: 
 
-Filename: tabdoc-1.0.3.dist-info/LICENSE
+Filename: tabdoc-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: tabdoc-1.0.3.dist-info/METADATA
+Filename: tabdoc-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: tabdoc-1.0.3.dist-info/WHEEL
+Filename: tabdoc-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: tabdoc-1.0.3.dist-info/top_level.txt
+Filename: tabdoc-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: tabdoc-1.0.3.dist-info/RECORD
+Filename: tabdoc-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tabdoc/__init__.py

```diff
@@ -3,12 +3,12 @@
 
 """
 @author: guoyanfeng
 @software: PyCharm
 @time: 19-3-20 下午6:29
 """
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from .tabexcel import *
 from .tabpdf import *
 from .tabword import *
```

## tabdoc/tabword.py

```diff
@@ -401,15 +401,15 @@
         为Word文档中添加图片
         Args:
             image_path: 图片在本地的路径
             image_text: 针对图片的说明文字
         Returns:
 
         """
-        p = self.document.add_paragraph(style="p-first-line-not-indent-center")
+        p = self.document.add_paragraph(style="picture-p-first-line-not-indent-center")
         p.alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
         run = p.add_run()
         if image_path:
             run.add_picture(image_path, width=Inches(5.8))
         bold_run = p.add_run(f"\n{image_text}")
         bold_run.font.size = Pt(12)
         bold_run.font.bold = True
```

## tabdoc/templates/template.docx

 * *Format-specific differences are supported for Microsoft Word .docx files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Microsoft Word 2007+*

```diff
@@ -1,1114 +1,1096 @@
 00000000: 504b 0304 0a00 0000 0000 874e e240 0000  PK.........N.@..
 00000010: 0000 0000 0000 0000 0000 0900 0000 646f  ..............do
 00000020: 6350 726f 7073 2f50 4b03 0414 0000 0008  cProps/PK.......
-00000030: 0087 4ee2 404d d85f e75e 0100 0072 0200  ..N.@M._.^...r..
+00000030: 0087 4ee2 4058 555a 175f 0100 0073 0200  ..N.@XUZ._...s..
 00000040: 0010 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
-00000050: 702e 786d 6c9d 91cd 6e83 3010 84ef 95fa  p.xml...n.0.....
-00000060: 0e88 3b18 c86f 23c7 514a 9a53 d546 8234  ..;..o#.QJ.S.F.4
-00000070: c7c8 321b b00a b665 3b51 f2f6 35a1 22f4  ..2....e;Q..5.".
-00000080: dadb ceac 3cfe b483 57d7 a6f6 2ea0 0d97  ....<...W.......
-00000090: 62e9 c761 e47b 2098 2cb8 2897 fe3e df06  b..a.{ .,.(..>..
-000000a0: 73df 3396 8a82 d652 c0d2 bf81 f157 e4f9  s.3....R.....W..
-000000b0: 09ef b454 a02d 07e3 b908 6196 7e65 ad5a  ...T.-....a.~e.Z
-000000c0: 2064 5805 0d35 a15b 0bb7 3949 dd50 eba4   dX..5.[..9I.P..
-000000d0: 2e91 3c9d 3883 8d64 e706 8445 4914 4d11  ..<.8..d...EI.M.
-000000e0: 5c2d 8802 8a40 f581 7e97 b8b8 d8ff 8616  \-...@..~.......
-000000f0: 92b5 7ce6 2bbf 2907 4c70 0e8d aaa9 05f2  ..|.+.).Lp......
-00000100: d1e2 d461 216d 8351 efe2 1d2d c190 18a3  ...a!m.Q...-....
-00000110: 6ec0 07a9 0b43 228c ba01 a715 d594 5977  n....C".......Yw
-00000120: a7d6 1c28 fcce 857b e9cc 6e70 499a 969a  ...(...{..npI...
-00000130: aaea 6e0e 14ce a5a5 75ce 1b20 7132 769f  ..n.....u.. q2v.
-00000140: f712 678c d690 3a60 72a2 b501 8c1e 469b  ..g...:`r.....F.
-00000150: ff6d f62a 979b 16ff 77ff d71c d01d b8ad  .m.*....w.......
-00000160: 3245 5987 f4e0 1cf8 78ad 54cd 19b5 ae71  2EY.....x.T....q
-00000170: 72d8 65de e7bd 9563 1c87 aefe 703e 4b92  r.e....c....p>K.
-00000180: e336 7e1b 25b3 d734 48a6 2f69 301e 4d8a  .6~.%..4H./i0.M.
-00000190: 601d 4f92 209a a493 7134 8fa2 245d 6334  `.O. ...q4..$]c4
-000001a0: 0cc2 aed5 0cd8 5973 7b6b af31 94ee aa7d  ......Ys{k.1...}
-000001b0: b7e4 0750 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
-000001c0: 4013 fa0c 9254 0100 007e 0200 0011 0000  @....T...~......
-000001d0: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
-000001e0: 6d6c 7d92 514f 8330 1485 df4d fc0f a4ef  ml}.QO.0...M....
-000001f0: d016 8c71 0db0 44cd 9e5c 6222 46e3 5b6d  ...q..D..\b"F.[m
-00000200: ef18 0aa5 69bb 31fe bd85 319c d1f8 787b  ....i.1...1...x{
-00000210: cefd eeb9 6dd3 e5a1 a983 3d18 5bb5 2a43  ....m.....=.[.*C
-00000220: 3422 2800 255a 59a9 3243 cfc5 2abc 4181  4"(.%ZY.2C..*.A.
-00000230: 755c 495e b70a 32d4 8345 cbfc f222 159a  u\I^..2..E..."..
-00000240: 89d6 c0a3 6935 1857 810d 3c49 5926 7486  ....i5.W..<IY&t.
-00000250: b6ce 6986 b115 5b68 b88d bc43 7971 d39a  ..i...[h...Cyq..
-00000260: 863b 5f9a 126b 2e3e 7909 3826 e41a 37e0  .;_..k.>y.8&..7.
-00000270: b8e4 8ee3 0118 ea99 8826 a414 3352 ef4c  .........&..3R.L
-00000280: 3d02 a4c0 5043 03ca 594c 238a bfbd 0e4c  =...PC..YL#....L
-00000290: 63ff 6c18 9533 6753 b95e fb9d a6b8 e76c  c.l..3gS.^.....l
-000002a0: 298e e2ec 3ed8 6a36 765d 1775 c918 c3e7  )...>.j6v].u....
-000002b0: a7f8 75fd f034 ae1a 566a b82b 0128 4fa5  ..u..4..Vj.+.(O.
-000002c0: 18c7 3161 803b 9081 07b0 e3b8 93f2 92dc  ..1a.;..........
-000002d0: dd17 2b94 c784 2e42 1287 3429 c882 d184  ..+....B..4)....
-000002e0: 11f2 96e2 936b ea1f 8047 566b f2f7 8f83  .....k...GVk....
-000002f0: 2174 f0cc 47c3 7bd4 dcba b57f ba4d 05f2  !t..G.{......M..
-00000300: b6cf cb5d db73 b501 55a6 f8b7 3a07 6ca6  ...].s..U...:.l.
-00000310: 8e7f 13c6 7148 9290 c605 218c 5cb1 e43c  ....qH....!.\..<
-00000320: e109 900f 190c ecab e12f e5c9 629c 3ad7  ........./..b.:.
-00000330: 63f5 f3c7 e45f 504b 0304 1400 0000 0800  c...._PK........
-00000340: 874e e240 7c52 f707 fe00 0000 7f01 0000  .N.@|R..........
-00000350: 1300 0000 646f 6350 726f 7073 2f63 7573  ....docProps/cus
-00000360: 746f 6d2e 786d 6c9d 90cd 6a84 3018 45f7  tom.xml...j.0.E.
-00000370: 85be 43c8 3e26 a6d8 1925 3a54 9dd9 74d1  ..C.>&...%:T..t.
-00000380: 42a7 b397 1867 02e6 8724 da4a e9bb 3732  B....g...$.J..72
-00000390: fdd9 77f9 713f 0ee7 5eb6 7b57 2398 85f3  ..w.q?..^.{W#...
-000003a0: d2e8 12a6 0981 4068 6e7a a9cf 257c 3d1e  ......@hnz..%|=.
-000003b0: d016 021f 3add 77a3 d1a2 848b f070 57dd  ....:.w......pW.
-000003c0: deb0 6767 ac70 410a 0f22 42fb 125e 42b0  ..gg.pA.."B..^B.
-000003d0: 05c6 9e5f 84ea 7c12 631d 93c1 38d5 8578  ..._..|.c...8..x
-000003e0: ba33 36c3 20b9 680d 9f94 d001 5342 ee31  .36. .h.....SB.1
-000003f0: 9f7c 300a d95f 1cbc f28a 39fc 17d9 1bbe  .|0.._....9.....
-00000400: daf9 d371 b151 b762 dff0 050c 2ac8 be84  ...q.Q.b....*...
-00000410: 1f6d d6b4 6d46 3244 f779 8352 92d6 28bf  .m..mF2D.y.R..(.
-00000420: cb37 886c 09a1 356d 0ef9 c3fe 1302 bb3e  .7.l..5m.......>
-00000430: 5308 74a7 62f5 c797 a788 ed27 1eea 498e  S.t.b......'..I.
-00000440: fd49 b888 9e43 31da 371f 5c45 4946 519a  .I...C1.7.\EIFQ.
-00000450: 2671 c364 bba1 94e1 bf8c e11f 858a e1d5  &q.d............
-00000460: edba 5cf5 0550 4b03 040a 0000 0000 0087  ..\..PK.........
-00000470: 4ee2 4000 0000 0000 0000 0000 0000 0005  N.@.............
-00000480: 0000 0077 6f72 642f 504b 0304 1400 0000  ...word/PK......
-00000490: 0800 874e e240 ae64 84bf 4a14 0000 39a8  ...N.@.d..J...9.
-000004a0: 0000 0f00 0000 776f 7264 2f73 7479 6c65  ......word/style
-000004b0: 732e 786d 6ced 5d4f 6f1c c975 bf07 c877  s.xml.]Oo..u...w
-000004c0: 18cc 2939 70a9 99a1 4489 58ae 2151 62b4  ..)9p...D.X.!Qb.
-000004d0: 0825 2b26 b53e f7cc 34c9 5ef5 744f ba7b  .%+&.>..4.^.tO.{
-000004e0: 4451 e720 86e1 5360 2009 021f e21c 821c  DQ. ..S` .......
-000004f0: 9c5c 821c 82c0 dfc6 96b3 df22 af5e bdea  .\.........".^..
-00000500: aeee eaaa ae7a 4352 6260 fba0 9de6 bc7a  .....zCRb`.....z
-00000510: 55ef cfef fda9 ea9a af7f f461 958e dec7  U..........a....
-00000520: 4599 e4d9 e178 f2d5 83f1 28ce 16f9 32c9  E....x....(...2.
-00000530: 2e0e c76f cf8e 771e 8f47 6515 65cb 28cd  ...o..w..Ge.e.(.
-00000540: b3f8 707c 1d97 e31f 7df3 a77f f2f5 d541  ..p|....}......A
-00000550: 595d a771 3982 01b2 f260 b538 1c5f 56d5  Y].q9....`.8._V.
-00000560: fa60 77b7 5c5c c6ab a8fc 2a5f c719 fcf1  .`w.\\....*_....
-00000570: 3c2f 5651 051f 8b8b dd55 54bc dbac 7716  </VQ.....UT...w.
-00000580: f96a 1d55 c93c 4993 ea7a 77fa e0c1 a331  .j.U.<I..zw....1
-00000590: 0d93 1f8e 3745 7640 43ec ac92 4591 97f9  ....7Ev@C...E...
-000005a0: 7925 480e f2f3 f364 11d3 3f8a a2f0 e12b  y%H....d..?....+
-000005b0: 299f e78b cd2a ce2a e4b8 5bc4 29cc 21cf  )....*.*..[.).!.
-000005c0: cacb 645d aad1 56dc d160 8997 6a90 f7ae  ..d]..V..`..j...
-000005d0: 45bc 5fa5 ea7b 573e ccae f262 b92e f245  E._..{W>...b...E
-000005e0: 5c96 a093 552a 27bf 8a92 ac1e 66b2 670c  \...U*'.....f.g.
-000005f0: 540b ee2b 10dc ae5c feae 180a c827 0ff0  T..+...\.....'..
-00000600: bfb4 794c 1eb8 664c 6217 d48a 6599 1a1c  ..yL..fLb...e...
-00000610: 7bb4 2db5 7892 cc8b a890 6a06 0310 f35e  {.-.x.....j....^
-00000620: 2d0e bebd c8f2 229a a760 5257 93bd f137  -....."..`RW...7
-00000630: 604f cb7c f13c 3e8f 3669 558a 8fc5 9b82  `O.|.<>.6iU.....
-00000640: 3ed2 27fc e738 cfaa 7274 7510 958b 2439  >.'..8..rtu...$9
-00000650: 1cff fe3f 7ef1 bbdf fe72 0c0f 2e9f 6665  ...?~....r....fe
-00000660: eb41 1c95 d5d3 3289 f42f 2dca 0a6c 1378  .A....2../-..l.x
-00000670: ae12 60ff 2c59 26e3 dd6f bede 4566 eadf  ..`.,Y&..o..Ef..
-00000680: 9a29 3cee 4c09 0c06 cce7 54da fdd5 c122  .)<.L.....T...."
-00000690: df64 d5e1 78fa 089c 06be 1b9f ffd5 31da  .d..x.........1.
-000006a0: fae1 583d 789b 5d26 cbf8 a797 71f6 b68c  ..X=x.]&....q...
-000006b0: 97e0 5ff4 c5d3 7895 bc4c 96cb 58f8 1c3d  .._...x..L..X..=
-000006c0: 7bfb ed9b 22c9 0bf0 88c3 f193 27f4 f024  {...".......'..$
-000006d0: 5fbc 8b97 a715 3016 a30a 11a4 e5f2 c587  _.....0.........
-000006e0: 45bc 16b6 0b6c ff5a f1c4 7136 1d86 3891  E....l.Z..q6..8.
-000006f0: 4dd2 8c8c 0f4a 8d3d 3ec8 2221 94d7 62f6  M....J.=>."!..b.
-00000700: a990 c8b6 5c70 fa16 2e97 7124 d065 34f1  ....\p....q$.e4.
-00000710: 61a4 cddc 67cc e92d 8c39 bb85 31f7 6e61  a...g..-.9..1.na
-00000720: cc87 b730 e6a3 5b18 73ff 16c6 7ccc 1953  ...0..[.s...|..S
-00000730: 1abd 32c7 27bd 43e8 ae23 9d52 5225 d932  ..2.'.C..#.RR%.2
-00000740: fe60 3161 374d bf89 ba69 fa4d d04d d36f  .`1a7M...i.M.M.o
-00000750: 626e 9a7e 1372 d3f4 9b88 4963 4103 29c8  bn.~.r....IcA.).
-00000760: 7e9b 3007 d185 dfaf 7337 cdb0 9267 0833  ~.0.....s7...g.3
-00000770: 924f 952f 3c54 dca5 1856 7097 6258 bd5d  .O./<T...Vp.bX.]
-00000780: 8a61 e576 2986 55db a518 566c 9762 588b  .a.v).U...Vl.bX.
-00000790: 5d8a 611d 7629 8635 a8bb a98c 68a3 6fc1  ].a.v).5....h.o.
-000007a0: 5bb3 2ac8 c1cf f3bc caf2 2a1e 55f1 8730  [.*.......*.U..0
-000007b0: ca28 033a cc2c edb4 9da0 ad47 b9a1 3017  .(.:.,.....G..0.
-000007c0: 17bd eb60 8e28 9669 19d1 ed49 049b 8173  ...`.(.i...I...s
-000007d0: 993d 1479 8df4 ae45 8429 4cef 0836 de95  .=.y...E.)L..6..
-000007e0: c818 47f9 f9e8 3cb9 d814 508a f4e5 2a36  ..G...<...P...*6
-000007f0: e238 7b1f a790 a68e a2e5 1268 99c4 455c  .8{........h..E\
-00000800: 4185 12c4 b8b6 a522 3e8f 0b28 afe2 2072  A......">..(.. r
-00000810: cda0 7803 a449 168f b2cd 6a1e a8e9 7574  ..x..I....j...ut
-00000820: c1a2 8bb3 25ba 0e6f b68a 3ad8 f16a e388  ....%..o..:..j..
-00000830: 36d5 a548 a493 4003 5945 506d 06a9 a6ca  6..H..@.YEPm....
-00000840: a391 cb13 6ca6 7892 9461 a022 0846 cf36  ....l.x..a.".F.6
-00000850: 691a 33e8 5e87 ab1e f90d 4732 1d6b 9164  i.3.^.....G2.k.d
-00000860: 3894 1924 7b41 1247 2ec3 c1cc e022 6537  8..${A.G....."e7
-00000870: 622c 8928 192b 234a c602 8992 b14e a96b  b,.(.+#J.....N.k
-00000880: ce3a 8992 b14e a264 ac93 28fb d7d9 0969  .:...N.d..(....i
-00000890: 4395 edc4 55da 9e25 551a 86ba 4769 2e1a  C...U..%U...Gi..
-000008a0: 2e41 c679 9a5c 6411 8487 7e4e 9df5 6841  .A.y.\d...~N..hA
-000008b0: 1f4b 774b 824c ed88 d19b a888 2e8a 687d  .KwK.L........h}
-000008c0: 3912 2d90 a069 3dcb 97d7 a3b3 d03c a6a6  9.-..i=......<..
-000008d0: e2a4 4fe8 a647 30d1 24db f44b c305 8d23  ..O..G0.$..K...#
-000008e0: 45c9 b1e3 9a96 61c9 352d c396 6bda 7e6b  E.....a.5-..k.~k
-000008f0: b6ad f715 6422 22ce be84 b688 253e 770c  ....d"".....%>w.
-00000900: 67d0 115c e674 ba99 57c1 be70 1aa5 1b99  g..\.t..W..p....
-00000910: d206 d9dd 73e8 5a05 1134 2677 9c14 10f0  ....s.Z..4&w....
-00000920: 1879 7bff 1081 76f4 5a24 fe42 21a1 00d0  .y{...v.Z$.B!...
-00000930: 700f 0b34 0d5d 98d1 3674 5254 81eb 34c8  p..4.]..6tRT..4.
-00000940: 03b9 a7d0 9d0c 0796 97d7 ebb8 809c f45d  ...............]
-00000950: 906d 1ce7 699a 5fc5 4b37 75a0 ab4c a7a2  .m..i._.K7u..L..
-00000960: 1eb1 20ef 6955 e496 0010 cac6 159a 5eac  .. .iU........^.
-00000970: d697 5199 9441 d250 5b19 a357 d13a 88f0  ..Q..A.P[..W.:..
-00000980: 4d0a 1df8 709d bdd8 81ce 7d3a 7207 381b  M...p.....}:r.8.
-00000990: c451 15fe 673f 8de7 7f1e 34d9 9767 af4e  .Q..g?....4..g.N
-000009a0: 464f 2129 cfae 570c 4246 9987 1c8f 9240  FO!)..W.BF.....@
-000009b0: dc92 54f9 320c ed90 0ac2 7b92 41a9 9287  ..T.2.....{.A...
-000009c0: 9594 48fb 97f1 f53c 8f60 5726 a40a 46ca  ..H....<.`W&..F.
-000009d0: 3750 9ae1 5645 1533 a84f a3d5 3a30 9b42  7P..VE.3.O..:0.B
-000009e0: ae67 e0f8 5750 9759 c29c cd7c 90f6 bba8  .g..WP.Y...|....
-000009f0: 4844 f1df bbd6 8e3b 6a99 955e 0790 199e  HD.....;j..^....
-00000a00: 5987 b14d 402b c0cb cdfc fb78 1196 7e21  Y..M@+.....x..~!
-00000a10: 4370 1d21 348f 7ea2 3ee5 1669 5848 6991  Cp.!4.~.>..iXHi.
-00000a20: 86e1 ba24 3d4a 23d8 72f4 e980 9a33 56b4  ...$=J#.r....3V.
-00000a30: 9c29 2bda 6de6 1c96 bed1 7af3 342f ce37  .)+.m.....z.4/.7
-00000a40: 294b 4547 8a98 b562 45cc 5a72 9e6e 5659  )KEG...bE.Zr.nVY
-00000a50: c99d 35d2 3227 8db4 dbcc 99a9 26e4 1b96  ..5.2'......&...
-00000a60: 654b 15ff 4591 2c59 8242 428e 9490 9023  eK..E.,Y.BB....#
-00000a70: 2224 e4c8 0709 d9c2 196e fa9b ce8e 1c87  "$.......n......
-00000a80: 7bff 16c2 e12d 0093 10ab cbfe fd63 1b86  {....-.......c..
-00000a90: 4b03 4042 8e1e 9190 a347 24e4 e811 0939  K.@B.....G$....9
-00000aa0: 7a44 428e 1e91 90a3 4724 e4e8 71f6 7c14  zDB.....G$..q.|.
-00000ab0: 9f9f 433c e5c1 9746 ced1 a946 ced1 aca8  ..C<...F...F....
-00000ac0: f7e3 d51a 4eb1 14d7 bd59 89db 145f a4f1  ....N....Y..._..
-00000ad0: 4514 d8c8 9146 fca6 c8cf c569 a03c b31c  E....F.....i.<..
-00000ae0: d670 3316 1d00 6e22 2249 39c2 86dc 9f85  .p3...n""I9.....
-00000af0: bc82 8ecb af5f ab7e c9e2 b308 ca4d 3860  ....._.~.....M8`
-00000b00: 636d 9b75 8619 6aca c87d 4c4b a5d9 4427  cm.u..j..}LK..D'
-00000b10: 8621 9d89 134d fd74 4393 9207 972c 933a  .!...M.tC....,.:
-00000b20: 492e 2eab d1e9 a5a3 0b32 38be ab13 25c7  I........28...%.
-00000b30: 17d8 c19c bcab 7697 838b c8c4 1c7c e668  ......v......|.h
-00000b40: 0cbc 8a97 c966 a544 6333 eb41 e1ec f9b3  .....f.Dc3.A....
-00000b50: b078 c020 0bdc 6eb5 e897 5681 e06d 89a5  .x. ..n...V..m..
-00000b60: 83e3 c3b9 4d6b fb44 1f9f 3bff fde1 f131  ....Mk.D..;....1
-00000b70: fbe0 ce1f 0eb7 0ecd 1fc7 e7ce dfb5 994f  ...............O
-00000b80: f2c1 f1fb 916a f030 dfbe abaf f41c ceda  .....j.0........
-00000b90: 8ef8 eeb5 eff2 ddba dcd9 0a1e f65d 1e5c  .............].\
-00000ba0: b3d8 6209 2e27 aec7 df02 245c e26f c127  ..b..'....$\.o.'
-00000bb0: 34b1 1670 0285 0d15 2e5d 3438 ba2d 1797  4..p.....]48.-..
-00000bc0: 3a1a 40dd 968b 4b29 5d64 dd96 5708 c46e  :.@...K)]d..W..n
-00000bd0: cbcb 1b6b b765 e40d badb 32f2 46df 6d19  ...k.e....2.F.m.
-00000be0: 79c3 f0b6 8cbc f178 4b46 7ec0 bc2d 1317  y......xKF~..-..
-00000bf0: 2ad4 f046 08bd 2d2f 1736 d4bc 3097 d80e  *..F..-/.6..0...
-00000c00: eaf6 5df0 5033 c2a0 b91d 23ff dc57 898e  ..].P3....#..W..
-00000c10: 9b04 b8d4 6482 3797 8b4b 4126 7873 b9b8  ....d.7..KA&xs..
-00000c20: b463 036f 2e2f 0e78 7379 0583 3797 5130  .c.o./.xsy..7.Q0
-00000c30: 7873 1905 8337 9751 3078 7319 0583 3793  xs...7.Q0xs...7.
-00000c40: 5118 7873 99b8 50a1 c6b9 0e78 7379 b9b0  Q.xs..P....xsy..
-00000c50: a1e6 a583 3797 910b 1e6a 463a 7833 1985  ....7....jF:x3..
-00000c60: 8337 b3c2 7ae4 5293 09de 5c2e 2e05 99e0  .7..z.R...\.....
-00000c70: cde5 e2d2 8e0d bcb9 bc38 e0cd e515 0cde  .........8......
-00000c80: 5c46 c1e0 cd65 140c de5c 46c1 e0cd 6514  \F...e...\F...e.
-00000c90: 0cde 4c46 61e0 cd65 e242 851a e73a e0cd  ..LFa..e.B...:..
-00000ca0: e5e5 c286 9a97 0ede 5c46 2e78 a819 e9e0  ........\F.x....
-00000cb0: cd64 140e de96 fdb3 c1f6 a44b 4d26 7873  .d.........KM&xs
-00000cc0: b9b8 1464 8237 978b 4b3b 36f0 e6f2 e280  ...d.7..K;6.....
-00000cd0: 3797 5730 7873 1905 8337 9751 3078 7319  7.W0xs...7.Q0xs.
-00000ce0: 0583 3797 5130 7833 1985 8137 9789 0b15  ..7.Q0x3...7....
-00000cf0: 6a9c eb80 3797 970b 1b6a 5e3a 7873 19b9  j...7....j^:xs..
-00000d00: e0a1 66a4 8337 9351 3878 5bce 30dc 3078  ..f..7.Q8x[.0.0x
-00000d10: 73b9 b814 6482 3797 8b4b 3b36 f0e6 f2e2  s...d.7..K;6....
-00000d20: 8037 9757 3078 7319 0583 3797 5130 7873  .7.W0xs...7.Q0xs
-00000d30: 1905 8337 9751 3078 3319 8581 3797 0907  ...7.Q0x3...7...
-00000d40: bcb9 bc5c d850 63aa 0ede 5c46 2e78 a819  ...\.Pc...\F.x..
-00000d50: e9e0 cd64 140e de96 7364 370c de5c 2e2e  ...d....sd7..\..
-00000d60: 0599 e0cd e5e2 d28e 0dbc b9bc 38e0 cde5  ............8...
-00000d70: 150c de5c 46c1 e0cd 6514 0cde 5c46 c1e0  ...\F...e...\F..
-00000d80: cd65 140c de4c 4661 e0cd 65c2 016f 2e2f  .e...LFa..e..o./
-00000d90: 1736 d498 aa83 3797 910b 1e6a 463a 7823  .6....7....jF:x#
-00000da0: 23b8 5c4c bf4d 4c5c b985 f7e9 c179 a40a  #.\L.ML\.....y..
-00000db0: 5e93 391c afd5 fbbe e288 12dc 2d26 ee45  ^.9.........-&.E
-00000dc0: a3cb c2f0 8bdf e275 6282 4e5c a701 df79  .......ub.N\...y
-00000dd0: 1fc1 a56c fa15 5e74 4211 5f0e 6a8e 84aa  ...l..^tB._.j...
-00000de0: 6f3e 9007 e3d6 6f0a e4bd 8e16 e252 aeab  o>....o......R..
-00000df0: 83b9 7833 08f8 3fc4 c32d f2d3 095c 2051  ..x3..?..-...\ Q
-00000e00: aa47 d139 bcc0 d3fa d0fc 1978 c1c2 684c  .G.9.......x..hL
-00000e10: b8c0 4d0c 5ddc c695 6d57 07ef e242 5c7f  ..M.]...mW...B\.
-00000e20: 86ab a65d 84f2 a37a 30ab 9f1c 89cb e2e4  ...]...z0.......
-00000e30: 97d4 21b1 08d7 89cf e26c e7ed a910 7073  ..!......l....ps
-00000e40: 59dc c7cb 9da3 d7e2 d11c 6e87 3b1c 47c5  Y.........n.;.G.
-00000e50: cee9 5321 2aed 9238 94ff 80c6 6a1d 4df1  ..S!*..8....j.M.
-00000e60: d236 5d47 7461 843a 0c34 8fe0 6ab8 1fd7  .6]Gta.:.4..j...
-00000e70: 6ba1 5966 f0ba b69a b99a 38bc 32a9 1e4d  k.Yf......8.2..M
-00000e80: e9b8 b55b c774 590e e9e3 5d1c af5f c3b0  ...[.tY...].._..
-00000e90: 6810 e203 ea0d 3f95 86fa 677b a87f 52f6  h.....?...g{..R.
-00000ea0: 6c86 9fe0 a54d 6119 fb08 7fe2 c34f 36e2  l....Ma......O6.
-00000eb0: 023f b86f 83ae cdc8 3795 787c f23e 5513  .?.o....7.x|.>U.
-00000ec0: 4533 336c 628e 5ce7 4725 cda5 51e5 1ed5  E33lb.\.G%..Q...
-00000ed0: a58d 2e9b 278d 2ee5 33ae 4a66 5695 90d9  ....'...3.JfV...
-00000ee0: b054 0222 c2d5 b44f ede1 a35b d312 5d3d  .T."...O...[..]=
-00000ef0: 485a a24f 524b 7b13 0cbb 7e5a 420b 33b4  HZ.ORK{...~ZB.3.
-00000f00: d4f6 5c3c 670c 3727 46df e7c5 4b71 d9a2  ..\<g.7'F...Kq..
-00000f10: 7012 bc75 b1f7 2fca a3f4 3fbe a02b 1905  p..u../...?..+..
-00000f20: 6573 15a3 1850 5dc5 086e d732 8dc6 0cfa  es...P]..n.2....
-00000f30: 5c5a 3ee3 9a81 bc75 b2cf 33a9 b1cd 3303  \Z>....u..3...3.
-00000f40: f2d6 fb68 0668 fe86 19dc 9d46 1e5a 1d93  ...h.h.....F.Z..
-00000f50: 5081 a711 f2ea 3bd5 c863 1d3e a74f 34f8  P.....;..c.>.O4.
-00000f60: 9ced 0738 265a a2a1 912f ca31 5528 2a3f  ...8&Z.../.1U(*?
-00000f70: 36f8 2c9f 711d f391 d50c a8ee e599 0179  6.,.q..........y
-00000f80: f57d 3403 347f c30c 6c8e 79f3 1ad9 b76a  .}4.4...l.y....j
-00000f90: 84b2 669e 46c8 abef 5423 adbc e611 d6db  ..f.F...T#......
-00000fa0: 3260 cea6 b593 0ea7 3568 8886 42be 2cbf  2`......5h..B.,.
-00000fb0: ac33 29cd 2f95 2161 6e0e f30f 4a65 1f5b  .3)./.!an...Je.[
-00000fc0: ad80 de1a e459 0139 f53d b402 55c9 b50b  .....Y.9.=..U...
-00000fd0: 1eab 5bde b842 9e58 1542 e501 4f21 e4d3  ..[..B.X.B..O!..
-00000fe0: f750 2168 875f 865b 3699 eb74 0bbd 2f2e  .P!h._.[6..t../.
-00000ff0: a10d b010 3766 40ca 6ceb 0298 f1d2 7569  ....7f@.l.....ui
-00001000: 58b0 5a29 a1bd 8172 1e53 fb46 30be e97b  X.Z)...r.S.F0..{
-00001010: 8537 7638 0460 66f2 e65d 1fcd 5b70 cc2a  .7v8.`f..]..[p.*
-00001020: 8d8a e96a 9eca be06 fcc7 4974 0d15 2f4c  ...j......It../L
-00001030: 4cb6 6cce 930f ea3a 15f8 e351 9ca6 afa2  L.l....:...Q....
-00001040: 42f4 09aa 7c0d 5f82 ebfe 31c2 c82f 2f3f  B...|._...1..//?
-00001050: 4463 9c49 1a9f 8b21 e0af 9307 5858 77fe  Dc.I...!....XXw.
-00001060: 3ecf ab2a 5fd9 e90b 7c4f d33a 0078 833e  >..*_...|O.:.x.>
-00001070: 19f9 51ac 2014 fde1 7e3d b116 bd5e 325f  ..Q. ...~=...^2_
-00001080: 92ed 071c 08b0 75e7 6246 b1e2 a6f4 616d  ......u.bF....am
-00001090: 60e9 0978 7f17 a2b1 c409 e1a5 9ec3 ca67  `..x...........g
-000010a0: 2025 56ac 9c4c 0c69 e977 ed0e cb09 aea6   %V..L.i.w......
-000010b0: dace 5049 30e0 3cf8 730a f02f d810 76bd  ..PI0.<.s../..v.
-000010c0: c4ab 6812 51d6 39b4 f5f6 260f 2935 d6be  ..h.Q.9...&.)5..
-000010d0: 8356 2540 07bf f278 063f d101 d311 d643  .V%@...x.?.....C
-000010e0: e395 59b4 3ecb b1af 49c3 7e06 21f7 37d7  ..Y.>...I.~.!.7.
-000010f0: d4fd 421e 4266 17eb edd6 dafa d912 1dbd  ..B.Bf..........
-00001100: f655 94b3 b83f 126e 2c02 212e c40d 2fd4  .U...?.n,.!.../.
-00001110: 2883 8fe5 c7c3 b1dc 1481 be1b 34d0 7016  (...........4.p.
-00001120: 205b 358c 92b1 a68f dbd4 d9d5 c1f7 8b8e   [5.............
-00001130: 6d48 5db7 f39a 5b75 17b3 27d7 ba19 be5f  mH]...[u..'...._
-00001140: 953d 4dd2 9ee8 66f6 bee1 4611 f42d 5a1f  .=M...f...F..-Z.
-00001150: 7082 e50b 1c06 55c0 afd1 088d 894f 4710  p.....U......OG.
-00001160: 7cc1 3ff0 9126 103b 7082 bea4 beeb eeef  |.?..&.;p.......
-00001170: c46c 699c 892f 8d84 e3c8 4974 9746 d982  .li../....It.F..
-00001180: bb67 08d7 09e8 2b30 fbb7 0ef4 d323 d833  .g....+0.....#.3
-00001190: f851 17f8 f19f 2648 0d1b aedc a294 864b  .Q....&H.......K
-000011a0: 2d4f 0a61 2cda 0097 e9e1 ac82 1f8b 7502  -O.a,.........u.
-000011b0: 4dcc 65fc 5299 bed3 5d7b 784b f2ef 78e4  M.e.R...]{xK..x.
-000011c0: 0249 e7a9 2e7e 7b3a 21bf eb8e d9b5 e92d  .I...~{:!......-
-000011d0: 3625 a40b a7e2 376a 04b0 c0ec 1a63 34cb  6%....7j.....c4.
-000011e0: 78dc 0093 16b9 0fb7 aed2 0d58 f466 9da5  x..........X.f..
-000011f0: b6f7 32d0 8714 be8c f04c bdea fe60 8138  ..2......L...`.8
-00001200: a904 fa70 eff1 545e 185f 892b 2e70 7680  ...p..T^._.+.pv.
-00001210: a1f8 2635 a227 3e16 07f5 60a5 cf8e 293e  ..&5.'>...`...)>
-00001220: 519a 0ac2 4519 bc29 6038 959e c19d a23f  Q...E..)`8.....?
-00001230: c9af 3030 f766 b37a affa 165b dc09 ba6e  ..00.f.z...[...n
-00001240: 42bb 1f0d ac4e 558c 556b 5850 a6b9 d0ec  B....NU.UkXP....
-00001250: 64c0 5ff6 1f3c 7dbe 87fb e016 a189 d863  d._..<}........c
-00001260: 18b3 b030 9d49 7929 1011 9d6a 91c6 1156  ...0.Iy)...j...V
-00001270: 1f9d 1876 9ea4 b0df 788c ff13 5686 ec8e  ...v....x...V...
-00001280: f1e1 3c5a bcbb 28e0 c791 962a b055 b812  ..<Z..(....*.U..
-00001290: 69c7 a416 841c 5349 70e9 dcfd d791 ccf7  i.....SIp.......
-000012a0: fb31 e9be 2be8 5cdc cc0b be88 5e44 dedd  .1..+.\.....^D..
-000012b0: a40f 326d d482 25a5 cfdd 6de0 fbe0 69ee  ..2m..%...m...i.
-000012c0: d872 dff5 281c 4da9 f1de 82a1 33f1 b8ef  .r..(.M.....3...
-000012d0: 1a9a c3af 2e4e be8b 8b0a 5d4d 4228 4473  .....N....]MB(Ds
-000012e0: 5f68 7e31 7d71 fc1c cf0f 69d0 dc8d 9e02  _h~1}q....i.....
-000012f0: b0cf 12f1 2b76 33b5 d5e4 8fd5 38c1 9779  ....+v3.....8..y
-00001300: f1f1 4b9d 6016 8b26 4c6b 76ad 30a7 9b4f  ..K.`..&Lkv.0..O
-00001310: 96e0 2fdf b523 217e a2c4 abc9 282c a12b  ../..#!~....(,.+
-00001320: bb72 736b e1c9 f6ec ca3b 5d5c 796b 8b03  .rsk.....;]\yk..
-00001330: 1963 862a a48a ff51 276c 5e39 adb9 29a1  .c.*...Q'l^9..).
-00001340: e5b4 8f6e 36a7 a56e 8133 a71d 2aa6 87ab  ...n6..n.3..*...
-00001350: af65 bea1 32b2 9372 f5a6 6e70 6242 3508  .e..2..r..npbB5.
-00001360: 31e1 08a3 9629 9996 5ec2 f46c 5d4d f95d  1....)..^..l]M.]
-00001370: 9592 ca7f df3f 4de1 372f ea5c 5136 9664  .....?M.7/.\Q6.d
-00001380: f857 80d5 f84d ad58 cc21 3a99 f81c 9362  .W...M.X.!:....b
-00001390: 7924 0838 7de6 1458 ac75 9b9c 3560 355a  y$.8}..X.u..5`5Z
-000013a0: b268 e8ee 2642 58d0 525a d91d e9a0 6f2d  .h..&BX.RZ....o-
-000013b0: d216 8653 f94e 86c1 1dea 8fa1 100a 60df  ...S.N........`.
-000013c0: 580d bad9 0650 cd4d c508 2e1a bd86 5f28  X....P.M......_(
-000013d0: d859 4655 3496 7eda 39b4 e8d5 13e8 b4dd  .YFU4.~.9.......
-000013e0: 2c4d abd6 91d3 761b 0b00 04db 0727 f23c  ,M....v......'.<
-000013f0: 2a75 9f9a ea83 9aa4 adf2 e38f 787b 38ee  *u..........x{8.
-00001400: c3db faac 823a a857 ff4e 322a 58eb 4aa0  .....:.W.N2*X.J.
-00001410: 6ec1 a85c 90ec 0231 3c1e 0aaa b384 af9e  n..\...1<.......
-00001420: 24ac 1bd3 423b 737d 99d6 d541 a7dd 4719  $...B;s}...A..G.
-00001430: 987a ded3 c7b3 4cb8 4aa7 73d1 55c2 705b  .z....L.J.s.U.p[
-00001440: 8f52 15d3 797d eab5 37bb 0309 f8e6 eec7  .R..y}..7.......
-00001450: 2f8e a747 479d b68a ccdd b177 5367 f4db  /..GG......wSg..
-00001460: e5ee 7571 d12d 0007 6d42 3576 90d0 2718  ..uq.-..mB5v..'.
-00001470: 0804 9fde 31bf 495d 9bdc d1fa 6e88 9fca  ....1.I]....n...
-00001480: 3d3a 4d39 cdc7 6aab f370 9efa bb5b 7945  =:M9..j..p...[yE
-00001490: 3dca 7db3 feed a221 9c09 1375 89be e94d  =.}....!...u...M
-000014a0: bfa0 83bb 3814 f658 5b38 ea5c bbb3 9a80  ....8..X[8.\....
-000014b0: d9d3 dfb7 48a3 7dfc b3a7 efca 4dd6 fe7f  ....H.}.....M...
-000014c0: e690 c713 f1ff 0e24 eb9d 6e51 dd88 7d0a  .......$..nQ..}.
-000014d0: 91a6 d1a6 c4b1 3a50 ed5f 4b6c d953 b9f9  ......:P._Kl.S..
-000014e0: 59da fda7 7536 c9b1 ed34 358f 42fc f0eb  Y...u6...45.B...
-000014f0: fffa c3af 7e3e fafd bfff c31f 7ef3 affd  ....~>......~...
-00001500: 1925 6d3e e947 4726 b4a7 e4de 1a55 5926  .%m>.GG&.....UY&
-00001510: 617e 93c8 6c73 c8c3 7bad e689 0458 ebff  a~..ls..{....X..
-00001520: fecd 3f05 af95 7a0d 9f61 adad 37cf 5c7a  ..?...z..a..7.\z
-00001530: 35f7 ecd7 3be8 fc3b e244 ed8e d8c0 573f  5...;..;.D....W?
-00001540: 70d0 4548 a973 5db9 533a 06ea 5e30 a5fc  p.EH.s].S:..^0..
-00001550: 0666 0a86 70a6 82f6 eee1 833c c21b 7f80  .f..p......<....
-00001560: c373 9297 dce4 c7e9 9de0 97f7 e479 dffa  .s...........y..
-00001570: c991 dced 17fb ff5a 0161 377f 6f31 99a7  .......Z.a7.o1..
-00001580: d35a 6282 9f4a 0e15 151d a1e2 894a bde0  .Zb..J.......J..
-00001590: 3779 889b a8b4 1f4b 9f86 e4a8 e291 5d2c  7y.....K......],
-000015a0: de9e 629e 8c68 8945 5a4f a8db 4ce9 2493  ..b..h.EZO..L.$.
-000015b0: 9768 42b3 42df f38a de96 611e dc6c 89a0  .hB.B.....a..l..
-000015c0: b18c 9da6 b285 daa8 5d7b abe3 a52d 67a2  ........]{...-g.
-000015d0: e321 5e62 309c 4959 887c 0594 0c04 3e60  .!^b0.IY.|....>`
-000015e0: 61e8 aab6 6fc0 2acc 230a 1691 045b 8657  a...o.*.#....[.W
-000015f0: 8b82 1679 5b96 e1ed 1c66 57fb d33f ffec  ...y[....fW..?..
-00001600: 877f f9c7 d124 78dd 526d 6e4b 2073 a165  .....$x.RmnK s.e
-00001610: cf51 d1b7 ff76 a6b7 34cc 9694 c528 c84f  .Q...v..4....(.O
-00001620: 5c32 9a12 78b6 dc85 920d b790 026c 031c  \2..x........l..
-00001630: 0165 b9bd 43c0 5ba5 dd02 842c 61ea 5a25  .e..C.[....,a.Z%
-00001640: bcfc 894a d457 e905 8d6d 4ba8 9b44 51b9  ...J.W...mK..DQ.
-00001650: 4892 3bda b46f 9b5f 93bf 6df3 06a8 afa9  H.;..o._..m.....
-00001660: cdcc 5c95 c43d 0b15 b717 deb4 c5fd 5957  ..\..=........YW
-00001670: 6e66 aeb4 f2bd d095 7b65 72ed 957f 5186  nf......{er...Q.
-00001680: b6cd fb73 de86 6626 cf24 ee87 a1e2 f602  ...s..f&.$......
-00001690: afb6 b86d 8676 272b 37f3 615a f9a3 d095  ...m.v'+7.aZ....
-000016a0: 7be5 c1ed 957f 5986 4618 a1bf 7620 d3b9  {.....Y.F...v ..
-000016b0: 1b0c 2066 9e4d e2de 0f15 77c8 9d13 bda9  .. f.M....w.....
-000016c0: 4483 e52a 69bd d595 9be9 35ad fc71 e8ca  D..*i.....5..q..
-000016d0: c986 dcf9 c117 6068 772c 6033 59ff f4f3  ......`hw,`3Y...
-000016e0: fffe f49f fff6 e9d7 7ffb e9ef 7ff6 e957  ...............W
-000016f0: bf09 9533 bc63 8469 4be7 e5a0 01b9 b705  ...3.c.iK.......
-00001700: dfc8 609b 868f 6f0d 3733 3375 badf 851a  ..`...o.733u....
-00001710: 38dd 6a4d 2e50 cfcb e08d 645c b47b 95f4  8.jM.P....d\.{..
-00001720: 25a3 5883 9142 3b1f fbce ce87 7e80 456c  %.X..B;.....~.El
-00001730: 2fc8 c9f9 deec 52e3 6bb3 85f4 c3ff fcdd  /.....R.k.......
-00001740: ef7e fb4b 39cc 5ced 9b29 4577 aeec 19c6  .~.K9.\..)Ew....
-00001750: 3d6f c598 4503 2986 ba88 1dc5 8022 8d8c  =o..E.)......"..
-00001760: 79cf abe1 68d3 8cad 8c06 11dc 89d2 4096  y...h.........@.
-00001770: 642d 04c6 3ad8 ce30 6b18 16b7 6f3e 0346  d-..:..0k...o>.F
-00001780: dcad 5394 1fb8 4040 251c ba3f 284d 78f9  ..S...@@%..?(Mx.
-00001790: 032d 2dd0 ecf4 cba3 d43e 4c83 1b7d 8506  .--......>L..}..
-000017a0: ebc6 2147 f374 cf2c 3448 5e54 a675 cd93  ..!G.t.,4H^T.u..
-000017b0: 404e 1794 9ab9 97a0 0ce0 b84b f354 a608  @N.........K.T..
-000017c0: ff5a 8ea6 78db 9959 a628 b776 d999 ba9c  .Z..x..Y.(.v....
-000017d0: 4917 9f7a 87ca 4b7c 8376 065e cd29 92ad  I..z..K|.v.^.)..
-000017e0: d720 0d00 a538 4ed1 dceb e0eb cdbe e0b9  . ...8N.........
-000017f0: 6756 2724 65ca 583b d609 d66c 82a7 575d  gV'$e.X;...l..W]
-00001800: f225 80a7 b2ce fa88 4b4b b438 c31b 044a  .%......KK.8...J
-00001810: b3fc 518e ef34 e03e 097b ed11 9184 070d  ..Q..4.>.{......
-00001820: 1815 3814 9f3b 66a7 f637 7170 bb73 7b9b  ..8..;f..7qp.s{.
-00001830: 9d59 ab90 6ca8 a5d0 353b c24a ddab f7bc  .Y..l...5;.J....
-00001840: aa94 50b3 03e1 282b b12f d31b c3cc c244  ..P...(+./.....D
-00001850: 7997 d304 281b 69ad d6ab a9e7 6b02 9f17  y...(.i.....k...
-00001860: c33c 1dcd db98 ccea 84a4 4cc0 d435 26b2  .<........L..5&.
-00001870: b196 78bd 0abf cf6b 4cd6 02c4 d948 92af  ..x....kL....H..
-00001880: 7b60 265a 5fcd b0e7 d5b8 f335 2606 9ec8  {`&Z_......5&...
-00001890: 6cf0 06b1 d65a 0338 5b4d 330a 722d 4bf0  l....Z.8[M3.r-K.
-000018a0: ea35 f9ca e6b3 3a9a 6f87 c9d7 d160 67b0  .5....:.o....`g.
-000018b0: 9bfa af22 78a7 28a9 e065 7869 059d 1d4b  ..."x.(..exi...K
-000018c0: f9d4 7c2f 3fd4 9140 8ca0 2328 7fa7 f256  ..|/?..@..#(...V
-000018d0: 2ff1 a17b 7797 6bbf b20e f881 e583 562a  /..{w.k.......V*
-000018e0: 7896 51de b234 cb82 7233 b78b 52ed ca0e  x.Q..4..r3..R...
-000018f0: c9d2 4b0a dab2 2c81 5dc5 bef2 9bff 0350  ..K...,.]......P
-00001900: 4b03 0414 0000 0008 0087 4ee2 40a6 3496  K.........N.@.4.
-00001910: ede5 0400 0074 0d00 0011 0000 0077 6f72  .....t.......wor
-00001920: 642f 7365 7474 696e 6773 2e78 6d6c b557  d/settings.xml.W
-00001930: 596f db38 107e 5f60 ff83 a177 d7ba 650b  Yo.8.~_`...w..e.
-00001940: 750b eb60 d322 6983 3ad9 7da6 25da e686  u..`."i.:.}.%...
-00001950: 2205 8ab2 ebfc fa0e 75c4 49cd 1445 17cd  ".......u.I..E..
-00001960: 4ba8 f9e6 9ee1 70fc f6fd b78a 4d0e 4436  K.....p.....M.D6
-00001970: 54f0 a5e5 bcb1 ad09 e185 2829 df2d adfb  T.........().-..
-00001980: 3b34 9d5b 9346 615e 6226 3859 5a27 d258  ;4.[.Fa^b&8YZ'.X
-00001990: efdf fdfd d7db 63dc 10a5 80ad 9980 0ade  ......c.........
-000019a0: c455 b1b4 f64a d5f1 6cd6 147b 52e1 e68d  .U...J..l..{R...
-000019b0: a809 0770 2b64 8515 7cca ddac c2f2 a1ad  ...p+d..|.......
-000019c0: a785 a86a ace8 8632 aa4e 33d7 b643 6b50  ...j...2.N3..CkP
-000019d0: 2396 562b 793c a898 56b4 90a2 115b a545  #.V+y<..V....[.E
-000019e0: 62b1 ddd2 820c ff46 09f9 2b76 7bc9 4c14  b......F..+v{.L.
-000019f0: 6d45 b8ea 2cce 2461 e083 e0cd 9ed6 cda8  mE..,.$a........
-00001a00: adfa 5d6d 10e2 7e54 72f8 5910 878a 8d7c  ..]m..~Tr.Y....|
-00001a10: 47c7 fe19 e710 ee51 c8f2 49e2 57dc d302  G......Q..I.W...
-00001a20: b514 0569 1a28 50c5 fa70 2b4c f993 1ac7  ...i.(P..p+L....
-00001a30: bf50 f494 ea37 90ea 596f 7ba6 5581 b863  .P...7..Yo{.U..c
-00001a40: 77a7 b3e7 0dbb 9037 54bb afe2 35dd 482c  w......7T...5.H,
-00001a50: fb32 4303 682f aa22 feb8 e342 e20d 83a6  .2C.h/."...B....
-00001a60: 3a3a bef5 0e3a ea51 886a 728c 6b22 0b28  ::...:.Q.jr.k".(
-00001a70: d2d2 82be b066 1ad8 8017 d0a3 99f8 2cd4  .....f........,.
-00001a80: ba95 52b4 bcbc 2218 68c0 7ec0 e08b f33a  ..R...".h.~....:
-00001a90: 2312 425d 3096 4327 dc4a 000b dd05 a089  #.B]0.C'.J......
-00001aa0: 7068 d582 e80e 595a 83e9 926c 71cb d41d  ph....YZ...lq...
-00001ab0: deac 95a8 4773 be3b c212 1f21 c71f 242d  ....Gs.;...!..$-
-00001ac0: ff21 52d1 02b3 758d 0b20 8dac 4e10 f6be  .!R...u.. ..N...
-00001ad0: 95b4 a919 3e5d 0949 1f05 5798 6567 d91c  ....>].I..W.eg..
-00001ae0: aee0 6994 1855 f7fc a3da d7b8 dd5e 7bb1  ..i..U.......^{.
-00001af0: c712 1710 e860 3e05 1352 b051 a7be 7012  .....`>..R.Q..p.
-00001b00: fae1 b6e5 856a bbb6 1fe4 ba9b a893 dc80  .....j..........
-00001b10: df04 0979 7fdd e71c 33cc 0bb2 8650 1849  ...y....3....P.I
-00001b20: 4e8a 64a2 856a e9d3 bfb4 54fb 8ea9 d415  N.d..j....T.....
-00001b30: b926 f840 125c 3c34 0c37 fb95 1e14 1dd8  .&.@.\<4.7......
-00001b40: b23b 8969 978f 9ed0 71e7 df6a 1827 eb3d  .;.i....q..j.'.=
-00001b50: ddaa af44 c15d ef78 71f9 5fdb a86b cac9  ...D.].xq._..k..
-00001b60: 15a1 bbbd fac8 21e3 6cd0 d310 945f e393  ......!.l...._..
-00001b70: 6855 c7db 0f8f 753f 7e20 408e 2b68 a29e  hU....u?~ @.+h..
-00001b80: 3a8c 941b 5112 0ba0 56d2 8b3e 7db5 cfb5  :...Q...V..>}...
-00001b90: 40df 4cc1 f3dc fc68 4840 ada0 dca4 7370  @.L....hH@....sp
-00001ba0: ad4e 0c92 c6d5 9a3e 9215 2f3f 4114 1486  .N.....>../?A...
-00001bb0: 549f e1df f7e0 670e 10ae 53f3 0586 ebdd  T.....g...S.....
-00001bc0: a926 8860 c822 8ce5 3f63 acab 1962 b4be  .&.`."..?c...b..
-00001bd0: a170 efe4 475e c2ed f863 c6e8 764b 2418  .p..G^...c..vK$.
-00001be0: a058 911b b876 548a 6397 e7fe b6ff 5fbb  .X...vT.c....._.
-00001bf0: b363 dcb7 89ee 7778 f3ca 663c 7c85 2131  .c....wx..f<|.!1
-00001c00: 96df b67d cf0e f261 a468 b633 e284 5e94  ...}...a.h.3..^.
-00001c10: a1be 3a3f 2099 334f 87ab fb12 71c3 d04f  ..:? .3O....q..O
-00001c20: 1726 192f b551 6044 7cd7 0b73 33f2 aa6f  .&./.Q`D|..s3..o
-00001c30: 3e72 5068 9409 16c1 2a30 c613 26be eb18  >rPh....*0..&...
-00001c40: 65a2 c473 c3e1 22bc 8c27 ca9d c07f 0571  e..s.."..'.....q
-00001c50: 1789 1199 2fec 7998 9872 b0c8 fcdc 9f9b  ..../.y..r......
-00001c60: 9024 b39d dc98 d124 0bb3 d5ca 2493 7a51  .$.....$....$.zQ
-00001c70: ba8a 8c48 68e7 8931 0769 e805 7e66 92c9  ...Hh..1.i..~f..
-00001c80: ecc8 718d 3219 7256 816f 92c9 ed28 8d8c  ..q.2.rV.o...(..
-00001c90: dac0 bc17 0d8f c1cb 8ca2 79b8 c88d da50  ..........y....P
-00001ca0: e6a2 c42c 93db eeca 9051 3789 f2c8 770d  ...,.....Q7...w.
-00001cb0: 39f0 508e 506a aa42 e025 f9c2 7387 a7e4  9.P.Pj.B.%..s...
-00001cc0: b96f 2142 793e b7f3 cb48 2327 4b9c 8563  .o!By>...H#'K..c
-00001cd0: 9089 2290 89e6 86ca 4509 f216 a19d 5e6a  ..".....E.....^j
-00001ce0: 4b32 80e0 ef12 c9f2 14e5 abc4 a02d 43ae  K2...........-C.
-00001cf0: b74a 4d1d 8fc2 08ad d0dc d055 08cd 3304  .JM........U..3.
-00001d00: 3daf edc0 34d0 a1c2 0ca8 62bd bddd caf1  =...4.....b.....
-00001d10: a407 faa4 ea1f 8314 571b 49f1 e446 ef77  ........W.I..F.w
-00001d20: 2055 c51b f990 503e e21b 024b 0379 8eac   U....P>...K.y..
-00001d30: dbcd 084e a73d d054 9831 040f f408 74e1  ...N.=.T.1....t.
-00001d40: 54b1 de09 32b2 edd4 b21b 2c77 67bd 0387  T...2.....,wg...
-00001d50: 3452 612b f9f4 a44b 2f4b 447e 80ad a8ee  4Ra+...K/KD~....
-00001d60: ad1d 25ae fb41 3d9a 737c 7fd0 4739 bcb2  ..%..A=.s|..G9..
-00001d70: d548 6fda cd7a 94e2 b0a3 3d83 60c5 fa72  .Ho..z....=.`..r
-00001d80: 905a e1ec 9c9e 63ac 60b5 ef1e bc6b 7cde  .Z....c.`....k|.
-00001d90: 7108 9fde aff5 0344 70a3 560d c54b eb71  q......Dp.V..K.q
-00001da0: 3f4d 3f6b 6918 b94c aef5 2f02 7283 ebba  ?M?ki..L../.r...
-00001db0: df8c 363b 6769 31fd d03b 5a4c c157 09bf  ..6;gi1..;ZL.W..
-00001dc0: 0cba 8fcd ce1d 30b7 c3e0 4b63 dd07 2e74  ......0...Kc...t
-00001dd0: b0c0 3d1c 3443 7f04 aee1 70a6 7923 cd3b  ..=.4C....p.y#.;
-00001de0: d360 efed f9fc 332d 1869 c199 168e 34f8  .`....3-.i....4.
-00001df0: 6572 8cf7 f0d0 4a46 f903 6c13 e351 d3b7  er....JF..l..Q..
-00001e00: 8231 7124 e5d5 485c 5a17 a42e 85e7 9f4b  .1q$..H\Z......K
-00001e10: efbe 0350 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
-00001e20: 407f d10b b4e8 0100 009e 0500 0010 0000  @...............
-00001e30: 0077 6f72 642f 6865 6164 6572 312e 786d  .word/header1.xm
-00001e40: 6ca5 94db 6e9c 3010 86ef 2bf5 1d90 ef17  l...n.0...+.....
-00001e50: c336 892a 1436 52b3 6a95 bb4a 691f c06b  .6.*.6R.j..Ji..k
-00001e60: cc62 057b 2cdb e06e 9fbe 6316 d84d 8956  .b.{,..n..c..M.V
-00001e70: 39dc 003e cc37 ffcc 3073 7bf7 47b5 492f  9..>.7..0s{.G.I/
-00001e80: ac93 a04b 92a7 1949 84e6 5049 bd2f c9ef  ...K...I..PI./..
-00001e90: 5fdf 575f 49e2 3cd3 156b 418b 921c 8423  _.W_I.<..kA....#
-00001ea0: 779b cf9f 6e43 d154 3641 6bed 8a60 7849  w...nC.T6Ak..`xI
-00001eb0: 1aef 4d41 a9e3 8d50 cca5 4a72 0b0e 6a9f  ..MA...P..Jr..j.
-00001ec0: 7250 14ea 5a72 4103 d88a aeb3 3c1b be8c  rP..ZrA.....<...
-00001ed0: 052e 9c43 57f7 4cf7 cc91 11a7 9634 3042  ...CW.L......40B
-00001ee0: a3af 1aac 62de a560 f754 31fb d499 15d2  ....b..`.T1.....
-00001ef0: 0df3 7227 5be9 0fc8 ce6e 260c 94a4 b3ba  ..r'[....n&.....
-00001f00: 1805 ad66 41d1 a438 0a1a 5f93 855d 44f1  ...fA..8.._..]D.
-00001f10: 82df a3e5 1678 a784 f683 476a 458b 1a40  .....x....GjE..@
-00001f20: bb46 9a53 18ef a561 88cd 24a9 bf14 44af  .F.S...a..$...D.
-00001f30: dae9 5e30 f9d5 c2df 1cf2 6b6a b0b5 2c60  ..^0......kj..,`
-00001f40: 294e c005 ee85 6454 4723 d51e f310 eb7b  )N....dTG#.....{
-00001f50: aaea ffc4 3cbb 14cc 5891 8898 35bc 46c2  ....<...X...5.F.
-00001f60: 739f 9312 c5a4 9e31 ef4b cd59 72f3 eb85  s......1.K.Yr...
-00001f70: 928b b95d 0fff f719 c060 377d a441 7e58  ...].....`7}.A~X
-00001f80: e8cc 1c8f 911f a33d e8a7 9915 9bfa 0dca  .......=........
-00001f90: b29b 4568 ee4d 8045 ef3f 36cc 8859 8e71  ..Eh.M.E.?6..Y.q
-00001fa0: f79d f3a0 b6cc b399 1b42 4883 7129 d7e3  .........BH.q)..
-00001fb0: 2039 ebbe fc0b c5a3 9311 4914 2f1e f61a   9........I./...
-00001fc0: 2cdb b518 5bc8 af92 905f 27b1 41c8 06c7  ,...[...._'.A...
-00001fd0: 9619 1e3f edf0 7af4 8756 24a1 e859 8bd3  ...?..z..V$..Y..
-00001fe0: 6f4d e8b0 fbad 1a4e 77e0 51c9 74aa 71fe  oM.....Nw.Q.t.q.
-00001ff0: 115c 7068 0107 05eb 3cc4 a5fb 5b12 1c9a  .\ph....<...[...
-00002000: f861 1847 7f79 6450 7433 42e2 36b6 155e  .a.G.ydPt3B.6..^
-00002010: d809 1c5f f1c6 7ab8 cf6a 2f90 1357 a345  ..._..z..j/..W.E
-00002020: d414 2d87 274e d7cd 3f50 4b03 0414 0000  ..-.'N..?PK.....
-00002030: 0008 0087 4ee2 4096 3d9c 92c5 0100 0051  ....N.@.=......Q
-00002040: 0500 0010 0000 0077 6f72 642f 6865 6164  .......word/head
-00002050: 6572 322e 786d 6ca5 94cb 6edb 3010 45f7  er2.xml...n.0.E.
-00002060: 05f2 0f02 f716 4537 090a 2172 1631 1a64  ......E7..!r.1.d
-00002070: 5720 ed07 d014 6511 e10b 2425 d67f dfa1  W ....e...$%....
-00002080: 2cc9 6e14 1879 6c44 eb31 67ee 9df1 ccdd  ,.n..ylD.1g.....
-00002090: fd5f 25b3 9e3b 2f8c ae10 c90b 9471 cd4c  ._%..;/......q.L
-000020a0: 2df4 be42 7f7e ff5c fd40 990f 54d7 541a  -..B.~.\.@..T.T.
-000020b0: cd2b 74e0 1edd 6fae bedd c5b2 ad5d 06d1  .+t...o......]..
-000020c0: da97 d1b2 0ab5 21d8 1263 cf5a aea8 cf95  ......!..c.Z....
-000020d0: 60ce 78d3 849c 1985 4dd3 08c6 7134 aec6  `.x.....M...q4..
-000020e0: eb82 14c3 2feb 0ce3 de43 aa07 aa7b ead1  ..../....C...{..
-000020f0: 8853 4b9a b15c 43ae c638 4583 cf8d db63  .SK..\C..8E....c
-00002100: 45dd 4b67 5740 b734 889d 9022 1c80 5ddc  E.KgW@.4..."..].
-00002110: 4e18 53a1 cee9 7214 b49a 05a5 90f2 2868  N.S...r.......(h
-00002120: 3ca6 08b7 70f1 46de 63e4 d6b0 4e71 1d86  <...p.F.c...Nq..
-00002130: 8cd8 7109 1a8c f6ad b027 1b9f a581 c576  ..q......'.....v
-00002140: 92d4 5f32 d12b 397d 172d b95e e49b 2dbf  .._2.+9}.-.^..-.
-00002150: a707 5b47 23b4 e204 5ce0 de28 467d 0c52  ..[G#...\..(F}.R
-00002160: f258 87d4 df53 575f 1349 71c9 ccd8 9184  .X...SW_.Iq.....
-00002170: 9835 bc47 c2ff 3927 258a 0a3d 633e 579a  .5.G..9'%..=c>W.
-00002180: b3e2 929b 8592 8bb5 5d0f ffef 3380 8569  ........]...3..i
-00002190: faca 803c 3ad3 d9d9 8f15 5fa3 3de9 9799  ...<:....._.=...
-000021a0: 9586 fa03 ca8a db85 35ff 21c0 62f6 9f5b  ........5.!.b..[
-000021b0: 6af9 2cc7 fa87 ce07 a3b6 34d0 991b 63cc  j.,.......4...c.
-000021c0: a3f5 39d3 e322 399b 3ef2 1dc3 ab53 10ca  ..9.."9.>....S..
-000021d0: 142b 9ff6 da38 ba93 e02d 92eb 2c92 9b2c  .+...8...-..,..,
-000021e0: 0d08 dac0 dab2 c3e5 971b 8ee7 7090 3c8b  ............p.<.
-000021f0: 654f 256c bf35 c2e9 a9b7 94c1 24c0 e31d  eO%l.5......$...
-00002200: 878d 0310 b286 bd18 4bda 040e 3b22 ddc1  ........K...;"..
-00002210: 8718 5809 93ce e10a 0b71 f30f 504b 0304  ..X......q..PK..
-00002220: 1400 0000 0800 874e e240 963d 9c92 c501  .......N.@.=....
-00002230: 0000 5105 0000 1000 0000 776f 7264 2f68  ..Q.......word/h
-00002240: 6561 6465 7233 2e78 6d6c a594 cb6e db30  eader3.xml...n.0
-00002250: 1045 f705 f20f 02f7 1645 3709 0a21 7216  .E.......E7..!r.
-00002260: 311a 6457 20ed 07d0 1465 11e1 0b24 25d6  1.dW ....e...$%.
-00002270: 7fdf a12c c96e 1418 796c 44eb 3167 ee9d  ...,.n..ylD.1g..
-00002280: f1cc ddfd 5f25 b39e 3b2f 8cae 10c9 0b94  ...._%..;/......
-00002290: 71cd 4c2d f4be 427f 7eff 5cfd 4099 0f54  q.L-..B.~.\.@..T
-000022a0: d754 1acd 2b74 e01e dd6f aebe ddc5 b2ad  .T..+t...o......
-000022b0: 5d06 d1da 97d1 b20a b521 d812 63cf 5aae  ]........!..c.Z.
-000022c0: a8cf 9560 ce78 d384 9c19 854d d308 c671  ...`.x.....M...q
-000022d0: 34ae c6eb 8214 c32f eb0c e3de 43aa 07aa  4....../....C...
-000022e0: 7bea d188 534b 9ab1 5c43 aec6 3845 83cf  {...SK..\C..8E..
-000022f0: 8ddb 6345 dd4b 6757 40b7 3488 9d90 221c  ..cE.KgW@.4...".
-00002300: 805d dc4e 1853 a1ce e972 14b4 9a05 a590  .].N.S...r......
-00002310: f228 683c a608 b770 f146 de63 e4d6 b04e  .(h<...p.F.c...N
-00002320: 711d 868c d871 091a 8cf6 adb0 271b 9fa5  q....q......'...
-00002330: 81c5 7692 d45f 32d1 2b39 7d17 2db9 5ee4  ..v.._2.+9}.-.^.
-00002340: 9b2d bfa7 075b 4723 b4e2 045c e0de 2846  .-...[G#...\..(F
-00002350: 7d0c 52f2 5887 d4df 5357 5f13 4971 c9cc  }.R.X...SW_.Iq..
-00002360: d891 8498 35bc 47c2 ff39 2725 8a0a 3d63  ....5.G..9'%..=c
-00002370: 3e57 9ab3 e292 9b85 928b b55d 0fff ef33  >W.........]...3
-00002380: 8085 69fa ca80 3c3a d3d9 d98f 155f a33d  ..i...<:....._.=
-00002390: e997 9995 86fa 03ca 8adb 8535 ff21 c062  ...........5.!.b
-000023a0: f69f 5b6a f92c c7fa 87ce 07a3 b634 d099  ..[j.,.......4..
-000023b0: 1b63 cca3 f539 d3e3 2239 9b3e f21d c3ab  .c...9.."9.>....
-000023c0: 5310 ca14 2b9f f6da 38ba 93e0 2d92 eb2c  S...+...8...-..,
-000023d0: 929b 2c0d 08da c0da b2c3 e597 1b8e e770  ..,............p
-000023e0: 903c 8b65 4f25 6cbf 35c2 e9a9 b794 c124  .<.eO%l.5......$
-000023f0: c0e3 1d87 8d03 10b2 86bd 184b da04 0e3b  ...........K...;
-00002400: 22dd c187 1858 0993 cee1 0a0b 71f3 0f50  "....X......q..P
-00002410: 4b03 0414 0000 0008 0087 4ee2 400b 297d  K.........N.@.)}
-00002420: dfc4 0100 0051 0500 0010 0000 0077 6f72  .....Q.......wor
-00002430: 642f 666f 6f74 6572 312e 786d 6ca5 94c9  d/footer1.xml...
-00002440: 6ee3 300c 86ef 03f4 1d0c dd63 59e9 8281  n.0........cY...
-00002450: 51a7 8706 2d7a 2bd0 ce03 288a 1c0b d506  Q...-z+...(.....
-00002460: 49b6 266f 3f94 633b 99ba 08ba 5cac 78e1  I.&o?.c;....\.x.
-00002470: c7ff 2743 dede fd55 32eb b8f3 c2e8 0a91  ..'C...U2.......
-00002480: bc40 19d7 cc6c 85de 55e8 cfeb c3e2 37ca  .@...l..U.....7.
-00002490: 7ca0 7a4b a5d1 bc42 7bee d1dd eae2 d76d  |.zK...B{......m
-000024a0: 2ceb e032 88d6 be8c 9655 a809 c196 187b  ,..2.....U.....{
-000024b0: d670 457d ae04 73c6 9b3a e4cc 286c ea5a  .pE}..s..:..(l.Z
-000024c0: 308e a371 5bbc 2c48 d1ff b2ce 30ee 3da4  0..q[.,H....0.=.
-000024d0: baa7 baa3 1e0d 3835 a719 cb35 e4aa 8d53  ......85...5...S
-000024e0: 34f8 dcb8 1d56 d4bd b576 0174 4b83 d808  4....V...v.tK...
-000024f0: 29c2 1ed8 c5cd 8831 156a 9d2e 0741 8b49  )......1.j...A.I
-00002500: 500a 290f 8286 638c 7033 171f e43d 44ae  P.)...c.p3...=D.
-00002510: 0d6b 15d7 a1cf 881d 97a0 c168 df08 7bb4  .k.........h..{.
-00002520: f15d 1a58 6c46 49dd 3913 9d92 e377 d192  .].XlFI.9....w..
-00002530: ab59 bec9 f267 7ab0 7634 422b 8ec0 19ee  .Y...gz.v4B+....
-00002540: 8362 6c0f 414a 1eea 90fa 7bec ea7b 2229  .bl.AJ....{..{")
-00002550: ce99 193a 9210 9386 cf48 f83f e7a8 4451  ...:.....H.?..DQ
-00002560: a127 ccf7 4a73 525c 723d 5372 b6b6 cbfe  .'..JsR\r=Sr....
-00002570: ff7d 02b0 304d 3f19 9047 675a 3bf9 b1e2  .}..0M?..GgZ;...
-00002580: 67b4 27fd 36b1 d250 7f41 5971 33b3 e6bf  g.'.6..P.AYq3...
-00002590: 0498 cdfe 4b43 2d9f e458 7fdf fa60 d49a  ....KC-..X...`..
-000025a0: 063a 7163 8c79 b43e 677a 5824 27d3 472e  .:qc.y.>gzX$'.G.
-000025b0: 31bc 3a06 a14c b1f2 69a7 8da3 1b09 de22  1.:..L..i......"
-000025c0: b9ca 22b9 ced2 80a0 15ac 2ddb 5f9e 5d7f  ..".......-._.].
-000025d0: bc84 bde4 592c 3b2a 61fb 1184 d353 6f29  ....Y,;*a....So)
-000025e0: 8349 80c7 1b0e 1b07 2064 097b 3196 b40e  .I...... d.{1...
-000025f0: 1c76 44ba 830f 31b0 1226 9dfd 1516 e2ea  .vD...1..&......
-00002600: 1f50 4b03 0414 0000 0008 0087 4ee2 400b  .PK.........N.@.
-00002610: 297d dfc4 0100 0051 0500 0010 0000 0077  )}.....Q.......w
-00002620: 6f72 642f 666f 6f74 6572 322e 786d 6ca5  ord/footer2.xml.
-00002630: 94c9 6ee3 300c 86ef 03f4 1d0c dd63 59e9  ..n.0........cY.
-00002640: 8281 51a7 8706 2d7a 2bd0 ce03 288a 1c0b  ..Q...-z+...(...
-00002650: d506 49b6 266f 3f94 633b 99ba 08ba 5cac  ..I.&o?.c;....\.
-00002660: 78e1 c7ff 2743 dede fd55 32eb b8f3 c2e8  x...'C...U2.....
-00002670: 0a91 bc40 19d7 cc6c 85de 55e8 cfeb c3e2  ...@...l..U.....
-00002680: 37ca 7ca0 7a4b a5d1 bc42 7bee d1dd eae2  7.|.zK...B{.....
-00002690: d76d 2ceb e032 88d6 be8c 9655 a809 c196  .m,..2.....U....
-000026a0: 187b d670 457d ae04 73c6 9b3a e4cc 286c  .{.pE}..s..:..(l
-000026b0: ea5a 308e a371 5bbc 2c48 d1ff b2ce 30ee  .Z0..q[.,H....0.
-000026c0: 3da4 baa7 baa3 1e0d 3835 a719 cb35 e4aa  =.......85...5..
-000026d0: 8d53 34f8 dcb8 1d56 d4bd b576 0174 4b83  .S4....V...v.tK.
-000026e0: d808 29c2 1ed8 c5cd 8831 156a 9d2e 0741  ..)......1.j...A
-000026f0: 8b49 500a 290f 8286 638c 7033 171f e43d  .IP.)...c.p3...=
-00002700: 44ae 0d6b 15d7 a1cf 881d 97a0 c168 df08  D..k.........h..
-00002710: 7bb4 f15d 1a58 6c46 49dd 3913 9d92 e377  {..].XlFI.9....w
-00002720: d192 ab59 bec9 f267 7ab0 7634 422b 8ec0  ...Y...gz.v4B+..
-00002730: 19ee 8362 6c0f 414a 1eea 90fa 7bec ea7b  ...bl.AJ....{..{
-00002740: 2229 ce99 193a 9210 9386 cf48 f83f e7a8  ")...:.....H.?..
-00002750: 4451 a127 ccf7 4a73 525c 723d 5372 b6b6  DQ.'..JsR\r=Sr..
-00002760: cbfe ff7d 02b0 304d 3f19 9047 675a 3bf9  ...}..0M?..GgZ;.
-00002770: b1e2 67b4 27fd 36b1 d250 7f41 5971 33b3  ..g.'.6..P.AYq3.
-00002780: e6bf 0498 cdfe 4b43 2d9f e458 7fdf fa60  ......KC-..X...`
-00002790: d49a 063a 7163 8c79 b43e 677a 5824 27d3  ...:qc.y.>gzX$'.
-000027a0: 472e 31bc 3a06 a14c b1f2 69a7 8da3 1b09  G.1.:..L..i.....
-000027b0: de22 b9ca 22b9 ced2 80a0 15ac 2ddb 5f9e  ."..".......-._.
-000027c0: 5d7f bc84 bde4 592c 3b2a 61fb 1184 d353  ].....Y,;*a....S
-000027d0: 6f29 8349 80c7 1b0e 1b07 2064 097b 3196  o).I...... d.{1.
-000027e0: b40e 1c76 44ba 830f 31b0 1226 9dfd 1516  ...vD...1..&....
-000027f0: e2ea 1f50 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
-00002800: 400b 297d dfc4 0100 0051 0500 0010 0000  @.)}.....Q......
-00002810: 0077 6f72 642f 666f 6f74 6572 332e 786d  .word/footer3.xm
-00002820: 6ca5 94c9 6ee3 300c 86ef 03f4 1d0c dd63  l...n.0........c
-00002830: 59e9 8281 51a7 8706 2d7a 2bd0 ce03 288a  Y...Q...-z+...(.
-00002840: 1c0b d506 49b6 266f 3f94 633b 99ba 08ba  ....I.&o?.c;....
-00002850: 5cac 78e1 c7ff 2743 dede fd55 32eb b8f3  \.x...'C...U2...
-00002860: c2e8 0a91 bc40 19d7 cc6c 85de 55e8 cfeb  .....@...l..U...
-00002870: c3e2 37ca 7ca0 7a4b a5d1 bc42 7bee d1dd  ..7.|.zK...B{...
-00002880: eae2 d76d 2ceb e032 88d6 be8c 9655 a809  ...m,..2.....U..
-00002890: c196 187b d670 457d ae04 73c6 9b3a e4cc  ...{.pE}..s..:..
-000028a0: 286c ea5a 308e a371 5bbc 2c48 d1ff b2ce  (l.Z0..q[.,H....
-000028b0: 30ee 3da4 baa7 baa3 1e0d 3835 a719 cb35  0.=.......85...5
-000028c0: e4aa 8d53 34f8 dcb8 1d56 d4bd b576 0174  ...S4....V...v.t
-000028d0: 4b83 d808 29c2 1ed8 c5cd 8831 156a 9d2e  K...)......1.j..
-000028e0: 0741 8b49 500a 290f 8286 638c 7033 171f  .A.IP.)...c.p3..
-000028f0: e43d 44ae 0d6b 15d7 a1cf 881d 97a0 c168  .=D..k.........h
-00002900: df08 7bb4 f15d 1a58 6c46 49dd 3913 9d92  ..{..].XlFI.9...
-00002910: e377 d192 ab59 bec9 f267 7ab0 7634 422b  .w...Y...gz.v4B+
-00002920: 8ec0 19ee 8362 6c0f 414a 1eea 90fa 7bec  .....bl.AJ....{.
-00002930: ea7b 2229 ce99 193a 9210 9386 cf48 f83f  .{")...:.....H.?
-00002940: e7a8 4451 a127 ccf7 4a73 525c 723d 5372  ..DQ.'..JsR\r=Sr
-00002950: b6b6 cbfe ff7d 02b0 304d 3f19 9047 675a  .....}..0M?..GgZ
-00002960: 3bf9 b1e2 67b4 27fd 36b1 d250 7f41 5971  ;...g.'.6..P.AYq
-00002970: 33b3 e6bf 0498 cdfe 4b43 2d9f e458 7fdf  3.......KC-..X..
-00002980: fa60 d49a 063a 7163 8c79 b43e 677a 5824  .`...:qc.y.>gzX$
-00002990: 27d3 472e 31bc 3a06 a14c b1f2 69a7 8da3  '.G.1.:..L..i...
-000029a0: 1b09 de22 b9ca 22b9 ced2 80a0 15ac 2ddb  ..."..".......-.
-000029b0: 5f9e 5d7f bc84 bde4 592c 3b2a 61fb 1184  _.].....Y,;*a...
-000029c0: d353 6f29 8349 80c7 1b0e 1b07 2064 097b  .So).I...... d.{
-000029d0: 3196 b40e 1c76 44ba 830f 31b0 1226 9dfd  1....vD...1..&..
-000029e0: 1516 e2ea 1f50 4b03 040a 0000 0000 0087  .....PK.........
-000029f0: 4ee2 4000 0000 0000 0000 0000 0000 000b  N.@.............
-00002a00: 0000 0077 6f72 642f 7468 656d 652f 504b  ...word/theme/PK
-00002a10: 0304 1400 0000 0800 874e e240 c8d4 165a  .........N.@...Z
-00002a20: fe05 0000 2c19 0000 1500 0000 776f 7264  ....,.......word
-00002a30: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
-00002a40: 6ced 594b 6f1b 3710 be17 e87f 58ec bd95  l.YKo.7.....X...
-00002a50: 64eb 1119 9103 5b8f b88d 9d04 9192 2247  d.....[......."G
-00002a60: 6a97 da65 c45d 2e48 ca8e 6e41 722a 0a14  j..e.].H..nAr*..
-00002a70: 2890 1639 3440 d14b 0f45 d100 0dd0 a03d  (..94@.K.E.....=
-00002a80: f4bf d485 8334 fd11 1d72 a515 2951 f503  .....4...r..)Q..
-00002a90: 3e04 4564 1fb4 dc6f 663e ce70 bf21 5757  >.Ed...of>.p.!WW
-00002aa0: af3d 4ca8 7788 b920 2c6d f995 8fcb be87  .=L.w.. ,m......
-00002ab0: d380 8524 8d5a fedd 41ef a32b be27 244a  ...$.Z..A..+.'$J
-00002ac0: 4344 598a 5bfe 140b ffda f687 1f5c 455b  CDY.[........\E[
-00002ad0: 32c6 09f6 c03e 155b a8e5 c752 665b a592  2....>.[...Rf[..
-00002ae0: 0860 1889 8f59 8653 b837 623c 4112 2e79  .`...Y.S.7b<A..y
-00002af0: 540a 393a 02bf 092d 6d94 cbf5 5282 48ea  T.9:...-m...R.H.
-00002b00: 7b29 4ac0 edad d188 04d8 fbeb d5ef 6fbe  {)J...........o.
-00002b10: 7ff6 e7a3 2fe0 dfdf 9ec7 e852 0894 4aa1  ..../......R..J.
-00002b20: 0602 cafb 2a02 b60c 3536 1c57 1442 4c45  ....*...56.W.BLE
-00002b30: 9b72 ef10 d196 0fe1 4276 34c0 0fa5 ef51  .r......Bv4....Q
-00002b40: 2424 dc68 f965 fdf1 4bdb 574b 686b 6644  $$.h.e..K.WKhkfD
-00002b50: e51a 5bc3 aea7 3f33 bb99 4138 ded0 3179  ..[...?3..A8..1y
-00002b60: 342c 8256 abb5 6a7d a7f0 af01 54ae e2ba  4,.V..j}....T...
-00002b70: 8d6e bd5b 2ffc 6900 0a02 9869 cec5 f6d9  .n.[/.i....i....
-00002b80: d868 5767 5803 947f 75f8 ee34 3a9b 150b  .hWgX...u..4:...
-00002b90: 6ff8 df5c e1bc 5353 7f16 5e83 72ff d515  o..\..SS..^.r...
-00002ba0: 7caf d786 2c5a 780d caf1 b515 7c6d b7b9  |...,Zx.....|m..
-00002bb0: dbb1 fd6b 508e afaf e01b e59d 4eb5 61f9  ...kP.......N.a.
-00002bc0: d7a0 9892 74bc 822e d7ea 9bed f96c 0bc8  ....t........l..
-00002bd0: 88d1 3d27 bc59 abf6 1a1b 33e7 0b14 ac86  ..='.Y....3.....
-00002be0: 6275 a910 2396 ca75 6b2d 410f 18ef 0140  bu..#..uk-A....@
-00002bf0: 0129 9224 f5e4 34c3 2314 c062 7efd d3e7  .).$..4.#..b~...
-00002c00: af7f fbc3 db27 512c 5514 b485 9171 3b1f  .....'Q,U....q;.
-00002c10: 0ac4 ca90 0ae8 8980 934c b6fc 4f33 044f  .........L..O3.O
-00002c20: c7c2 e9c9 ab57 c78f 5f1e 3ffe f5f8 c993  .....W.._.?.....
-00002c30: e3c7 3f9b de2d bb3d 9446 a6dd db1f befa  ..?..-.=.F......
-00002c40: e7f9 23ef ef5f be7b fbf4 eb3c f432 5e98  ..#.._.{...<.2^.
-00002c50: f855 f2cb 7078 960c 5adf bc78 fdf2 c5c9  .U..px..Z..x....
-00002c60: b32f dffc f8d4 e17d 87a3 a109 1f90 040b  ./.....}........
-00002c70: ef26 3ef2 eeb0 0426 a8b3 6307 c043 7e3e  .&>....&..c..C~>
-00002c80: 8b41 8c88 69b1 9346 02a5 4845 71f8 efca  .A..i..F..HEq...
-00002c90: d842 df9c 228a 1cb8 5d6c e7f1 1e07 2d71  .B.."...]l....-q
-00002ca0: 01af 4f1e 5884 fb31 9f48 e2f0 7823 4e2c  ..O.X..1.H..x#N,
-00002cb0: e001 6374 9771 6716 6ea8 5846 9a07 9334  ..ct.qg.n.XF...4
-00002cc0: 7207 e713 1377 07a1 4357 ec36 4aad 2a77  r....w..CW.6J.*w
-00002cd0: 2719 8828 71b9 6cc7 d8a2 799b a254 a208  '..(q.l...y..T..
-00002ce0: a758 7aea 1e1b 63ec 98dd 7d42 acbc 1e90  .Xz...c...}B....
-00002cf0: 8033 c146 d2bb 4fbc 5d44 9c29 1990 a1b5  .3.F..O.]D.)....
-00002d00: 9a16 467b 2481 ba4c 5d04 a1de 566e 0eee  ..F{$..L]...Vn..
-00002d10: 79bb 8cba 66dd c187 3612 9e0d 441d e407  y...f...6...D...
-00002d20: 985a 69bc 8e26 1225 2e97 0394 5033 e1fb  .Zi..&.%....P3..
-00002d30: 48c6 2e92 fd29 0f4c 5c57 48a8 7484 29f3  H....).L\WH.t.).
-00002d40: ba21 16c2 6573 8bc3 7c8d a2df 4020 5fce  .!..es..|...@ _.
-00002d50: b21f d069 6223 b924 6397 cf7d c498 89ec  ...ib#.$c..}....
-00002d60: b071 3b46 49e6 c2f6 491a 9bd8 4fc4 1896  .q;FI...I...O...
-00002d70: 28f2 6e33 e982 1f30 fb09 51d7 5007 94ae  (.n3...0..Q.P...
-00002d80: 2df7 3d82 ad72 9fae 0677 4143 4d4a 8b05  -.=..r...wACMJ..
-00002d90: a2ee 4cb8 a396 d731 b3d6 6f7f 4a47 086b  ..L....1..o.JG.k
-00002da0: a901 85b7 843b 21e9 692a 9e07 b81c fd06  .....;!.i*......
-00002db0: 953c f9f6 b983 f2e5 68b6 dbb1 95f0 93f3  .<......h.......
-00002dc0: a9f5 0e27 cec7 656f 49a3 d7e1 9695 b9cd  ...'..eoI.......
-00002dd0: 7848 de7d 61ee a049 7a1b c3b3 b0da 9dde  xH.}a..Iz.......
-00002de0: ebf2 7b5d f6ff f7ba bcee 79be 7c35 5e08  ..{]......y.|5^.
-00002df0: 3068 b3da 07e6 1b6e bdfd 4ed6 eebe 4784  0h.....n..N...G.
-00002e00: d2be 9c52 bc2f f406 5c40 db09 7b30 a8ec  ...R./..\@..{0..
-00002e10: f401 1417 a7b1 2c86 afea 4986 0016 2ee2  ......,...I.....
-00002e20: 48db 789c c9cf 888c fb31 ca60 f35e f195  H.x......1.`.^..
-00002e30: 9348 cc5c 47c2 cb98 8043 a31e 76fa 5678  .H.\G....C..v.Vx
-00002e40: 3a49 0e58 981f 3a2b 1575 c0cc c543 20b9  :I.X..:+.u...C .
-00002e50: 182f d78a 7138 30c8 1c5d 6f2c 0e52 857b  ./..q80..]o,.R.{
-00002e60: cd36 d207 de39 0165 7b1e 1246 309b c4a6  .6...9.e{..F0...
-00002e70: 8344 633e a892 a48f d790 3407 093d b34b  .Dc>......4..=.K
-00002e80: 61d1 74b0 b8a2 dccf 4bb5 c202 a815 5581  a.t.....K.....U.
-00002e90: 7d91 07bb a996 5fab 8209 18c1 b109 511c  }....._.......Q.
-00002ea0: aa3a e5a5 9e57 5717 f332 2bbd 2e99 d60a  .:...WW..2+.....
-00002eb0: 28c3 0b8e d90a 5854 baa9 b8ae 9d9e 9a5d  (.....XT.......]
-00002ec0: bed4 ce50 698b 84b1 dc6c 123a 33ba 8789  ...Pi....l.:3...
-00002ed0: 1885 78b6 3ad5 e859 689c b7d6 cd45 492d  ..x.:..Yh....EI-
-00002ee0: 7a2a 15b3 5c18 341a 57fe 8bc5 456b 0d76  z*..\.4.W...Ek.v
-00002ef0: cbda 4053 5329 68ea 1db5 fcfa 660d 964c  ..@SS)h.....f..L
-00002f00: 80b2 963f 82c3 3b7c 4d32 583b 42ed 6711  ...?..;|M2X;B.g.
-00002f10: 8de0 4558 2079 fec0 5f44 5932 2e64 0789  ..EX y.._DY2.d..
-00002f20: 384f b816 9d5c 0d12 2231 f728 495a be9a  8O...\.."1.(IZ..
-00002f30: 7e51 069a 6a0d d1dc 2a1b 2008 ef2c b926  ~Q..j...*. ..,.&
-00002f40: c8ca bb46 0e8a 6e17 198f 4638 9066 d98d  ...F..n...F8.f..
-00002f50: 1195 e9fc 1214 3ed7 0ae7 5d6d 7e71 b0b2  ......>...]m~q..
-00002f60: 6413 2877 3f0e 8fbc 219d f03b 0896 58ad  d.(w?...!..;..X.
-00002f70: 5151 090c 8980 573c 953c 9b21 8197 9285  QQ....W<.<.!....
-00002f80: 902d d6df 5263 9ac9 aef9 5650 afa1 7c1c  .-..Rc....VP..|.
-00002f90: d12c 46b3 8e62 8a79 0ed7 525e d0d1 5745  .,F..b.y..R^..WE
-00002fa0: 0e8c abd9 9c21 a146 4a66 8d70 18a9 066b  .....!.FJf.p...k
-00002fb0: 26d5 eaa6 45d7 c839 aced baa7 1ba9 cc19  &...E..9........
-00002fc0: a2b9 e899 96aa a8ae e956 312b c2bc 0d2c  .........V1+...,
-00002fd0: e5f2 624d de60 354f 31b4 4bb3 c3e7 d2bd  ..bM.`5O1.K.....
-00002fe0: 2cb9 cdb9 d62d ed13 8a2e 0109 2ff2 e7e8  ,....-....../...
-00002ff0: ba67 6808 06b5 4530 8b9a 62bc 2ac3 4ab3  .gh...E0..b.*.J.
-00003000: 67a3 76ef 984f f014 6a67 6912 86ea d7e7  g.v..O..jgi.....
-00003010: 6e97 f256 f408 6738 18bc 50e7 07bb e555  n..V..g8..P....U
-00003020: 0b43 a3f9 be52 675a ff88 61fe c0c0 860f  .C...RgZ..a.....
-00003030: 403c 3af0 2a77 42a5 c805 4283 b6ff 0550  @<:.*wB...B....P
-00003040: 4b03 0414 0000 0008 0087 4ee2 4081 b4d3  K.........N.@...
-00003050: 50c4 0200 00e7 0700 0011 0000 0077 6f72  P............wor
-00003060: 642f 646f 6375 6d65 6e74 2e78 6d6c a595  d/document.xml..
-00003070: 4b73 db20 10c7 ef9d e977 d070 b725 f991  Ks. .....w.p.%..
-00003080: 3a9a 2899 3669 3239 b493 a99b 7307 2324  :.(.6i29....s.#$
-00003090: 3196 8001 64d5 f9f4 5d84 1e4e e5bc 2f06  1...d...]..N../.
-000030a0: 99dd dffe 975d e0ec e26f 5978 3baa 3413  .....]...oYx;.4.
-000030b0: 3c46 e134 401e e544 248c 6731 baff 7d3d  <F.4@..D$.g1..}=
-000030c0: 5921 4f1b cc13 5c08 4e63 b4a7 1a5d 9c7f  Y!O...\.Nc...]..
-000030d0: fe74 5647 8920 5549 b9f1 00c1 7554 4b12  .tVG. UI....uTK.
-000030e0: a3dc 1819 f9be 2639 2db1 9e96 8c28 a145  ......&9-....(.E
-000030f0: 6aa6 4494 be48 5346 a85f 0b95 f8b3 200c  j.D..HSF._.... .
-00003100: 9a99 5482 50ad 21de 25e6 3bac 518b 2bc7  ..T.P.!.%.;.Q.+.
-00003110: 3421 2987 58a9 5025 367a 2a54 e697 586d  4!).X.P%6z*T..Xm
-00003120: 2b39 01ba c486 6d58 c1cc 1ed8 c149 8711  +9....mX.....I..
-00003130: 31aa 148f 5a41 935e 9075 899c a076 e83c  1...ZA.^.u...v.<
-00003140: d428 8b23 719d e755 bb03 4d44 5fd1 0234  .(.#q..U..MD_..4
-00003150: 08ae 7326 8734 de4b 8314 f34e d2ee b924  ..s&.4.K...N...$
-00003160: 7665 d1d9 d532 5c8c e2f5 29bf a606 570a  ve...2\...)...W.
-00003170: d750 8a01 38c2 1dd9 8cc4 3995 85db 075b  .P..8.....9....[
-00003180: dfa1 aaff 135f 037c 4ce8 b825 66bc 17f6  ....._.|L..%f...
-00003190: be44 0fb6 2a0c 9edb d4b6 33ac 9021 e472  .D..*.....3..!.r
-000031a0: a4fd d9bd 9d35 fd7d 1052 c291 fac8 01b9  .....5.}.R......
-000031b0: 51a2 92bd 1cc9 3e46 bbe5 db9e 654f f61b  Q.....>F....eO..
-000031c0: 9405 27a3 d4f4 9b00 a3b3 bfce b1a4 bd1c  ..'.............
-000031d0: a92f 2b6d 4479 850d eeb9 755d 4f6b a9a7  ./+mDy....u]Ok..
-000031e0: 84b7 17c9 c1e9 0be7 3e2c 0d4e c82b 4974  ........>,.N.+It
-000031f0: 9b71 a1f0 a680 dcea 70e1 d5e1 d2b3 0704  .q......p.......
-00003200: 9dc3 ddb5 11c9 de8e b2f9 b953 7650 ed70  ...........SvP.p
-00003210: 2db8 d15e 1de5 8c9b 1851 accd 57cd 30f2  -..^.....Q..W.0.
-00003220: ad4d 8179 064b 3b5c c00a 9fdc af11 7c75  .M.y.K;\......|u
-00003230: 2631 7ac8 2797 3fad a5df e260 940e bb11  &1z.'.?....`....
-00003240: 626b 6fab b5c1 ca80 134b 6204 976d 1d71  bko......Kb..m.q
-00003250: 5c82 c23f 37e2 1b26 5b17 a5b3 fdce 93de  \..?7..&[.......
-00003260: d241 1bbd 9a12 e3a0 39c5 0955 bf68 4a15  .A......9..U.hJ.
-00003270: dcda d453 0d56 dd26 4b4b 367b 09e4 9429  ...S.V.&KK6{...)
-00003280: 6d1c 3715 c21c 3587 4bfe 88f9 93f4 f960  m.7...5.K......`
-00003290: 9ed0 1457 c54b 7cb8 8e3b fe23 8727 232c  ...W.K|..;.#.'#,
-000032a0: 0607 baa3 fc05 f95f 8e59 cb6c fd00 516b  ......._.Y.l..Qk
-000032b0: 78d5 c253 fb20 4045 617e b29a af1c 4e66  x..S. @Ea~....Nf
-000032c0: 3fb0 b2ba 8484 ff17 8ba6 1a8a 6539 543d  ?...........e9T=
-000032d0: 5c05 cde7 4618 e8c3 61b9 a0e9 c1aa 931f  \...F...a.......
-000032e0: a3d5 32b4 78b7 bd31 3a3d 9dd9 cfac 32b0  ..2.x..1:=....2.
-000032f0: dbb6 ca4d eb10 51d8 aed2 1213 a8ca 62d6  ...M..Q.......b.
-00003300: 9488 5716 ee0c e03d bd51 cc56 dc15 ae60  ..W....=.Q.V...`
-00003310: 1c1e 5bf8 b493 3b66 08c8 9f87 0d9a e458  ..[...;f.......X
-00003320: ad1d a8a1 439b 754d 0153 d7dc 30e9 5ee8  ....C.uM.S..0.^.
-00003330: f37f 504b 0304 0a00 0000 0000 874e e240  ..PK.........N.@
-00003340: 0000 0000 0000 0000 0000 0000 0a00 0000  ................
-00003350: 6375 7374 6f6d 586d 6c2f 504b 0304 1400  customXml/PK....
-00003360: 0000 0800 874e e240 dc7f 3ecf 9500 0000  .....N.@..>.....
-00003370: 0201 0000 1300 0000 6375 7374 6f6d 586d  ........customXm
-00003380: 6c2f 6974 656d 312e 786d 6c9d 8ec1 0ac2  l/item1.xml.....
-00003390: 3010 44ef 82ff 10f6 6eb7 d58b 9424 3db4  0.D.....n....$=.
-000033a0: 7816 d40f 0869 aa85 7653 baa9 d1bf b750  x....i..vS.....P
-000033b0: 10c5 9bd7 9979 c393 c5a3 efc4 dd8d dc7a  .....y.........z
-000033c0: 5290 2529 0847 d6d7 2d5d 155c ce87 cd1e  R.%).G..-].\....
-000033d0: 0407 43b5 e93c 3905 4fc7 50e8 f54a 726e  ..C..<9.O.P..Jrn
-000033e0: 270e beaf 4c30 623e 2156 700b 61c8 1163  '...L0b>!Vp.a..c
-000033f0: 8c49 1c38 b184 be69 5aeb 2a6f a7de 51c0  .I.8...iZ.*o..Q.
-00003400: 6d9a ed70 aeca 370a 0b9b ff49 6bb9 589c  m..p..7....Ik.X.
-00003410: 9c0d c7d1 0ffc 1da0 96f8 33c0 4f75 fd02  ..........3.Ou..
-00003420: 504b 0304 1400 0000 0800 874e e240 6343  PK.........N.@cC
-00003430: 7b45 e500 0000 4701 0000 1800 0000 6375  {E....G.......cu
-00003440: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
-00003450: 7331 2e78 6d6c 658f 516b 8330 1485 df07  s1.xmle.Qk.0....
-00003460: fb0f 72df 3546 ebd4 622c b44e e8eb d860  ..r.5F..b,.N...`
-00003470: af21 5edb 8049 c4c4 da31 f6df 1737 1874  .!^..I...1...7.t
-00003480: 7dba 9c7b b8df 39b7 da5d d510 5c70 b2d2  }..{..9..]..\p..
-00003490: 6806 348a 2140 2d4c 27f5 89c1 db6b 1b16  h.4.!@-L'....k..
-000034a0: 1058 c775 c707 a391 c107 5ad8 d58f 0f55  .X.u......Z....U
-000034b0: 67b7 1d77 dc3a 33e1 d1a1 0afc 42fa 796c  g..w.:3.....B.yl
-000034c0: 187c ee69 99e7 6dde 8449 9ced c34d 5cd0  .|.i..m..I...M\.
-000034d0: b0a4 e921 4c8b 6643 9ff3 2c6b cbe4 0b02  ...!L.fC..,k....
-000034e0: 9fad 3dc6 3238 3b37 6e09 b1e2 8c8a dbc8  ..=.28;7n.......
-000034f0: 8ca8 bdd9 9b49 71e7 e574 22a6 efa5 c0c6  .....Iq..t".....
-00003500: 8859 a176 2489 e327 2266 1faf ded5 00f5  .Y.v$..'"f......
-00003510: dae7 f7fa 057b 7b2b d76a f324 ff52 9665  .....{{+.j.$.R.e
-00003520: 8996 d146 42df 5369 4abc 75f8 0137 fe3f  ...FB.SiJ.u..7.?
-00003530: 2075 45fe b157 7df3 7bfd 0d50 4b03 0414   uE..W}.{..PK...
-00003540: 0000 0008 0087 4ee2 408c af87 adbf 0300  ......N.@.......
-00003550: 0084 1200 0012 0000 0077 6f72 642f 666f  .........word/fo
-00003560: 6e74 5461 626c 652e 786d 6ce5 58dd 4edb  ntTable.xml.X.N.
-00003570: 3014 be9f b477 8872 0f71 d242 4345 41f4  0....w.r.q.BCEA.
-00003580: 2768 d2c4 c560 dab5 9bba ad47 1c57 764a  'h...`.....G.WvJ
-00003590: d727 98a6 5d4d 93f6 06bb d8c5 9026 2e26  .'..]M.......&.&
-000035a0: 6d62 bccc 00f1 163b 7692 d2d2 a46b 5981  mb.....;v....kY.
-000035b0: 4d4b 4569 4fec 83fd f9fb be73 c2e6 f62b  MKEiO......s...+
-000035c0: 1618 4744 48ca c38a 69af 22d3 20a1 cf5b  ..GDH...i.". ..[
-000035d0: 34ec 54cc e707 de8a 6b1a 32c2 610b 073c  4.T.....k.2.a..<
-000035e0: 2415 7348 a4b9 bdf5 f8d1 e6a0 dce6 6124  $.sH..........a$
-000035f0: 0d98 1fca 32f3 2b66 378a 7a65 cb92 7e97  ....2.+f7.ze..~.
-00003600: 302c 5779 8f84 70b3 cd05 c311 7c15 1d8b  0,Wy..p.....|...
-00003610: 6171 d8ef adf8 9cf5 7044 9b34 a0d1 d072  aq......pD.4...r
-00003620: 105a 3793 3462 9e2c bcdd a63e a973 bfcf  .Z7.4b.,...>.s..
-00003630: 4818 e9f9 9620 0164 e4a1 ecd2 9e4c b30d  H.... .d.....L..
-00003640: e6c9 36e0 a2d5 13dc 2752 c29e 5910 e763  ..6.....'R..Y..c
-00003650: 9886 a334 7671 2a11 a3be e092 b7a3 55d8  ...4vq*.......U.
-00003660: 8c15 afc8 52a9 60ba 8df4 2716 9806 f3cb  ....R.`...'.....
-00003670: 4f3a 2117 b819 0076 03bb 686e 25c0 1983  O:!....v..hn%...
-00003680: 7288 1904 0f28 23d2 d823 03e3 1967 38d4  r....(#..#...g8.
-00003690: 037a 38e4 92d8 30e6 0807 1513 39f0 5a47  .z8...0.....9.ZG
-000036a0: 05b4 868a f0e3 c0a7 a269 a94c 7e17 0b49  .........i.L~..I
-000036b0: a2d1 4014 87db 98d1 6098 4685 ceab c7f7  ..@.....`.F.....
-000036c0: 68e4 77d3 f811 1654 2d2c 9e23 6907 6ef4  h.w....T-,.#i.n.
-000036d0: 6513 554c 3812 54da 714b 661c b12b a60b  e.UL8.T.qKf..+..
-000036e0: 1175 2511 0716 155f 400f 3dab 308a e831  .u%...._@.=.0..1
-000036f0: bece a387 d89e a7c6 4004 f224 b3f4 3aad  ........@..$..:.
-00003700: 9842 5388 9c1f bffd 79fa 3e07 081b 8040  .BS.....y.>....@
-00003710: 0080 9dbe 3281 70d7 b380 c0fd 88c7 f109  ....2.p.........
-00003720: 1c5a a48d fb41 340d 43b2 d8c2 350c 8eeb  .Z...A4.C...5...
-00003730: 7a2a 3a05 0330 7826 0c45 9864 2f06 c30b  z*:..0x&.E.d/...
-00003740: a0a3 92a1 cc44 622d 59dc d8af 4c24 90b3  .....Db-Y...L$..
-00003750: 4424 d27d 8f1f 64bc ef6b 42a4 6332 0931  D$.}..d..kB.c2.1
-00003760: 4ea3 f909 b103 3c0d 3251 7050 15f8 50d4  N.....<.2QpP..P.
-00003770: 0251 2271 f284 6167 a120 0754 caf8 c6fc  .Q"q..ag. .T....
-00003780: 8458 862e 141b d084 2e3c b854 50ad 264f  .X.......<.TP.&O
-00003790: 1757 dfdf fd55 bad0 7c06 c350 6c70 5143  .W...U..|..PlpQC
-000037a0: 2f7f 2136 c00c 8dc4 62ba a8f1 bea0 4428  /.!6....b.....D(
-000037b0: cbcc e144 09fc 6143 b341 9965 7121 4e30  ...D..aC.A.eq!N0
-000037c0: de22 22fc 7748 b13f 644d 9e2d 8e35 a815  ."".wH.?dM.-.5..
-000037d0: 3600 60a3 1288 c481 6fa5 785f 37ab 46a6  6.`.....o.x_7.F.
-000037e0: 45e4 558d dfb9 65aa ff7b f688 1a0e 6853  E.U...e..{....hS
-000037f0: 50cd 081c 447b 505b 818b ba7c c6f6 11d7  P...D{P[...|....
-00003800: bfa9 c2ea e982 aa9d 0358 93eb 1f99 85f5  .........X......
-00003810: 56fe 3126 9359 10a5 e2ca b451 9503 d91b  V.1&.Y.....Q....
-00003820: 0bd6 d5cb cf6f 2ebf 9d19 4f69 a71b 65e1  .....o....Oi..e.
-00003830: 94d4 dd1c a01e a0f0 ce41 257b 9ec2 bb64  .........A%{...d
-00003840: 9c76 fbcd 264d 1ce2 069f f4c1 4cbe 654b  .v..&M......L.eK
-00003850: 2e93 4fb7 ec4f e680 69d4 b1e4 d309 56bd  ..O..O..i.....V.
-00003860: 980f c730 a8ee ed66 bbaa 00d0 c67e 8dc4  ...0...f.....~..
-00003870: 9da2 10ff ada4 039b 25aa 14a9 25a2 70f1  ........%...%.p.
-00003880: e1f5 c5c9 9bab 4f67 e73f 8e2f bf9c 408d  ......Og.?./..@.
-00003890: ce29 4aaa 5151 3dbc 9bb4 2bd9 1dfc 721a  .)J.QQ=...+...r.
-000038a0: d786 0dc8 3b0d cdfb b840 af57 eb9e 57f3  ....;....@.W..W.
-000038b0: aa09 48ba 5d53 cd58 61a6 7e60 bd8d 499f  ..H.]S.Xa.~`..I.
-000038c0: a97b f592 3a55 759e 797d ca12 dab5 a5c9  .{..:Uu.y}......
-000038d0: e3e1 bab5 8b8f 5f67 776b 1b40 87fb 788a  ......_gwk.@..x.
-000038e0: d13d b753 1d23 43c1 ad79 a59a b733 4e06  .=.S.#C..y...3N.
-000038f0: 75a8 7399 e982 4f31 fb98 0df1 a1b1 db7f  u.s...O1........
-00003900: 8905 3ca1 e788 03fe 0500 d218 bbee d42f  ..<............/
-00003910: b439 a505 f64f fd62 413c 467e 01d5 f8fc  .9...O.bA<F~....
-00003920: f8f4 3f76 8dc4 3ee4 d62f 504b 0304 0a00  ..?v..>../PK....
-00003930: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
-00003940: 0000 0000 0600 0000 5f72 656c 732f 504b  ........_rels/PK
-00003950: 0304 1400 0000 0800 874e e240 0122 221f  .........N.@."".
-00003960: fd00 0000 e102 0000 0b00 0000 5f72 656c  ............_rel
-00003970: 732f 2e72 656c 73ad 92dd 4a03 3110 85ef  s/.rels...J.1...
-00003980: 05df 21cc 7d37 db2a 22d2 6c6f 44e8 9d48  ..!.}7.*".loD..H
-00003990: 7d80 2199 dd0d ddfc 904c b57d 7b83 7fb8  }.!......L.}{...
-000039a0: b0ae bdf0 7232 67ce 7c73 c87a 7374 8378  ....r2g.|s.zst.x
-000039b0: a194 6df0 0a96 550d 82bc 0ec6 fa4e c1f3  ..m...U......N..
-000039c0: ee61 710b 2233 7a83 43f0 a4e0 4419 36cd  .aq."3z.C...D.6.
-000039d0: e5c5 fa89 06e4 3294 7b1b b328 2e3e 2be8  ......2.{..(.>+.
-000039e0: 99e3 9d94 59f7 e430 5721 922f 9d36 2487  ....Y..0W!./.6$.
-000039f0: 5cca d4c9 887a 8f1d c955 5ddf c8f4 d303  \....z...U].....
-00003a00: 9a91 a7d8 1a05 696b ae41 ec4e b16c fedb  ......ik.A.N.l..
-00003a10: 3bb4 add5 741f f4c1 91e7 8915 72ac 28ce  ;...t.......r.(.
-00003a20: 983a 6205 af21 1969 3e07 ab82 0c72 9a66  .:b..!.i>....r.f
-00003a30: 753e cdef 974a 478c 0619 a50e 8916 3195  u>...JG.......1.
-00003a40: 9c12 db92 ec37 5061 792c cff9 5d31 07b4  .....7Pay,..]1..
-00003a50: 3c1f 687c fc54 3c74 64f2 86cc 3c12 c638  <.h|.T<td...<..8
-00003a60: 4774 f59f 44fa 9039 b879 9e0f cd17 921c  Gt..D..9.y......
-00003a70: 7dcc e60d 504b 0304 0a00 0000 0000 874e  }...PK.........N
-00003a80: e240 0000 0000 0000 0000 0000 0000 1000  .@..............
-00003a90: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
-00003aa0: 732f 504b 0304 1400 0000 0800 874e e240  s/PK.........N.@
-00003ab0: 743f 397a bc00 0000 2801 0000 1e00 0000  t?9z....(.......
-00003ac0: 6375 7374 6f6d 586d 6c2f 5f72 656c 732f  customXml/_rels/
-00003ad0: 6974 656d 312e 786d 6c2e 7265 6c73 85cf  item1.xml.rels..
-00003ae0: c18a 0231 0c06 e0bb e03b 94dc 9dce 7810  ...1.....;....x.
-00003af0: 91e9 7859 16bc 89b8 e0b5 7432 33c5 6953  ..xY......t23.iS
-00003b00: 9a28 faf6 164f 2b2c ec31 09f9 fea4 dd3f  .(...O+,.1.....?
-00003b10: c2ac ee98 d953 34d0 5435 288c 8e7a 1f47  .....S4.T5(..z.G
-00003b20: 033f e7ef d516 148b 8dbd 9d29 a281 2732  .?.........)..'2
-00003b30: ecbb e5a2 3de1 6ca5 2cf1 e413 aba2 4436  ....=.l.,.....D6
-00003b40: 3089 a49d d6ec 260c 962b 4a18 cb64 a01c  0.....&..+J..d..
-00003b50: ac94 328f 3a59 77b5 23ea 755d 6f74 fe6d  ..2.:Yw.#.u]ot.m
-00003b60: 40f7 61aa 436f 201f fa06 d4f9 994a f2ff  @.a.Co ......J..
-00003b70: 360d 8377 f845 ee16 30ca 1f11 dadd 5828  6..w.E..0.....X(
-00003b80: 5cc2 7ccc 94b8 c836 8f28 06bc 6078 b79a  \.|....6.(..`x..
-00003b90: aadc 0bba 6bf5 c77f dd0b 504b 0304 0a00  ....k.....PK....
-00003ba0: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
-00003bb0: 0000 0000 0b00 0000 776f 7264 2f5f 7265  ........word/_re
-00003bc0: 6c73 2f50 4b03 0414 0000 0008 0087 4ee2  ls/PK.........N.
-00003bd0: 40e0 8ea4 be33 0100 0038 0600 001c 0000  @....3...8......
-00003be0: 0077 6f72 642f 5f72 656c 732f 646f 6375  .word/_rels/docu
-00003bf0: 6d65 6e74 2e78 6d6c 2e72 656c 73b5 944b  ment.xml.rels..K
-00003c00: 4fc3 3010 84ef 48fc 07cb 77e2 2485 f250  O.0...H...w.$..P
-00003c10: 935e 1052 af28 485c 8db3 7988 c48e ec2d  .^.R.(H\..y....-
-00003c20: 22ff 9e15 a1a1 952a f7e2 1c77 adcc 371a  "......*...w..7.
-00003c30: c7b3 d97e f71d fb02 eb5a a333 9e44 3167  ...~.....Z.3.D1g
-00003c40: a095 295b 5d67 fcad 78b9 79e0 cca1 d4a5  ..)[]g..x.y.....
-00003c50: ec8c 868c 8fe0 f836 bfbe dabc 4227 913e  .......6....B'.>
-00003c60: 724d 3b38 462a da65 bc41 1c9e 8470 aa81  rM;8F*.e.A...p..
-00003c70: 5eba c80c a0e9 a432 b697 48a3 adc5 20d5  ^......2..H... .
-00003c80: a7ac 41a4 71bc 16f6 5883 e727 9a6c 5766  ..A.q...X..'.lWf
-00003c90: dcee ca47 ce8a 7120 f265 6d53 55ad 8267  ...G..q .emSU..g
-00003ca0: a3f6 3d68 3c83 1048 be80 04a5 ad01 33fe  ..=h<..H......3.
-00003cb0: 3b4e cb24 22a3 5c9c f740 1984 f350 1983  ;N.$".\..@...P..
-00003cc0: 60ff 4d4c f3ca c7bf 5f9e 9ffa f8eb e5f9  `.ML...._.......
-00003cd0: defc ef42 f21b 90e5 71fe d3ec cdff 7679  ...B....q.....vy
-00003ce0: be37 ffd5 f27c 6ffe 6948 be03 446a 1747  .7...|o.iH..Dj.G
-00003cf0: 9a7f cff0 b0f1 fd82 4912 d243 6534 16f2  ........I..Ce4..
-00003d00: a33b ea82 79e5 7541 f518 ae09 d4de a1e9  .;..y.uA........
-00003d10: dfa9 77e6 28a2 48cc 5bd1 22f4 de7b 099a  ..w.(.H.[."..{..
-00003d20: 89c3 b1a3 729f ad4c f321 0d71 d2f7 f90f  ....r..L.!.q....
-00003d30: 504b 0304 1400 0000 0800 874e e240 b2e5  PK.........N.@..
-00003d40: 51b6 9a01 0000 9808 0000 1300 0000 5b43  Q.............[C
-00003d50: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00003d60: 6cc5 964f 4fe3 3010 c5ef 487c 87c8 57d4  l..OO.0...H|..W.
-00003d70: b82d 1242 a829 87dd e5c8 7228 1257 634f  .-.B.)....r(.WcO
-00003d80: 5a6b fd4f 9e29 4bbf 3d93 94f6 0055 db10  Zk.O.)K.=....U..
-00003d90: 2a2e 9112 7bde efe9 cd38 c9e4 f6d5 bbe2  *...{....8......
-00003da0: 0532 da18 2a31 2a87 a280 a0a3 b161 5e89  .2..*1*......a^.
-00003db0: c7d9 dde0 5a14 482a 18e5 6280 4aac 00c5  ....Z.H*..b.J...
-00003dc0: edf4 fc6c 325b 25c0 82ab 0356 6241 946e  ...l2[%....VbA.n
-00003dd0: a444 bd00 afb0 8c09 02af d431 7b45 7c9b  .D.........1{E|.
-00003de0: e732 29fd 4fcd 418e 87c3 2ba9 6320 0834  .2).O.A...+.c .4
-00003df0: a046 434c 27bf a156 4b47 c59f 577e bc76  .FCL'..VKG..W~.v
-00003e00: c2e5 a2f8 b5de d7a0 2aa1 5272 562b 62a3  ........*.RrV+b.
-00003e10: b259 953b eb32 38dc 53f8 12cc 0777 8377  .Y.;.28.S....w.w
-00003e20: 6725 57b6 e2b8 b009 2fde 097f 399a 6c0d  g%W...../...9.l.
-00003e30: 140f 2ad3 bdf2 ec43 ea25 52f4 4fde 494b  ..*....C.%R.O.IK
-00003e40: e01f 724c 382a f7fb dd81 8d75 6d35 98a8  ..rL8*.....um5..
-00003e50: 979e a328 b7a2 8d1e 64b2 b0d7 03d7 b560  ...(....d......`
-00003e60: c9a9 f466 4313 bb01 3348 ddd8 3a66 e80e  ...fC...3H..:f..
-00003e70: dfe4 dd54 7726 b6d1 7767 ee0c fb48 f8ff  ...Tw&..wg...H..
-00003e80: 988d dcf6 a96f 9f1b 358e 5903 221f 31ef  .....o..5.Y.".1.
-00003e90: caad b257 36ec 1bbb d647 cd27 62a6 9edd  ...W6....G.'b...
-00003ea0: 1772 ff90 c127 235b e923 4c44 82dc 7fe6  .r...'#[.#LD....
-00003eb0: 7758 6884 8fe4 8f7b 8f41 3ffe e58f f117  wXh....{.A?.....
-00003ec0: a0cc 49f2 5f0b 1fcc 7fbd ed04 f977 e29f  ..I._........w..
-00003ed0: 20ff 23f9 0844 7c78 f1fb 0760 a37c b005   .#..D|x...`.|..
-00003ee0: 482b 07a7 30d0 ea1e c413 7fe7 41b6 d7fe  H+..0.......A...
-00003ef0: af81 5666 8394 ed7f c5f4 0d50 4b01 0214  ..Vf.......PK...
-00003f00: 0014 0000 0008 0087 4ee2 40b2 e551 b69a  ........N.@..Q..
-00003f10: 0100 0098 0800 0013 0000 0000 0000 0001  ................
-00003f20: 0020 0000 0030 3d00 005b 436f 6e74 656e  . ...0=..[Conten
-00003f30: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
-00003f40: 1400 0a00 0000 0000 874e e240 0000 0000  .........N.@....
-00003f50: 0000 0000 0000 0000 0600 0000 0000 0000  ................
-00003f60: 0000 1000 0000 2a39 0000 5f72 656c 732f  ......*9.._rels/
-00003f70: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
-00003f80: 0122 221f fd00 0000 e102 0000 0b00 0000  ."".............
-00003f90: 0000 0000 0100 2000 0000 4e39 0000 5f72  ...... ...N9.._r
-00003fa0: 656c 732f 2e72 656c 7350 4b01 0214 000a  els/.relsPK.....
-00003fb0: 0000 0000 0087 4ee2 4000 0000 0000 0000  ......N.@.......
-00003fc0: 0000 0000 000a 0000 0000 0000 0000 0010  ................
-00003fd0: 0000 0032 3300 0063 7573 746f 6d58 6d6c  ...23..customXml
-00003fe0: 2f50 4b01 0214 000a 0000 0000 0087 4ee2  /PK...........N.
-00003ff0: 4000 0000 0000 0000 0000 0000 0010 0000  @...............
-00004000: 0000 0000 0000 0010 0000 0074 3a00 0063  ...........t:..c
-00004010: 7573 746f 6d58 6d6c 2f5f 7265 6c73 2f50  ustomXml/_rels/P
-00004020: 4b01 0214 0014 0000 0008 0087 4ee2 4074  K...........N.@t
-00004030: 3f39 7abc 0000 0028 0100 001e 0000 0000  ?9z....(........
-00004040: 0000 0001 0020 0000 00a2 3a00 0063 7573  ..... ....:..cus
-00004050: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
-00004060: 6d31 2e78 6d6c 2e72 656c 7350 4b01 0214  m1.xml.relsPK...
-00004070: 0014 0000 0008 0087 4ee2 40dc 7f3e cf95  ........N.@..>..
-00004080: 0000 0002 0100 0013 0000 0000 0000 0001  ................
-00004090: 0020 0000 005a 3300 0063 7573 746f 6d58  . ...Z3..customX
-000040a0: 6d6c 2f69 7465 6d31 2e78 6d6c 504b 0102  ml/item1.xmlPK..
-000040b0: 1400 1400 0000 0800 874e e240 6343 7b45  .........N.@cC{E
-000040c0: e500 0000 4701 0000 1800 0000 0000 0000  ....G...........
-000040d0: 0100 2000 0000 2034 0000 6375 7374 6f6d  .. ... 4..custom
-000040e0: 586d 6c2f 6974 656d 5072 6f70 7331 2e78  Xml/itemProps1.x
-000040f0: 6d6c 504b 0102 1400 0a00 0000 0000 874e  mlPK...........N
-00004100: e240 0000 0000 0000 0000 0000 0000 0900  .@..............
-00004110: 0000 0000 0000 0000 1000 0000 0000 0000  ................
-00004120: 646f 6350 726f 7073 2f50 4b01 0214 0014  docProps/PK.....
-00004130: 0000 0008 0087 4ee2 404d d85f e75e 0100  ......N.@M._.^..
-00004140: 0072 0200 0010 0000 0000 0000 0001 0020  .r............. 
-00004150: 0000 0027 0000 0064 6f63 5072 6f70 732f  ...'...docProps/
-00004160: 6170 702e 786d 6c50 4b01 0214 0014 0000  app.xmlPK.......
-00004170: 0008 0087 4ee2 4013 fa0c 9254 0100 007e  ....N.@....T...~
-00004180: 0200 0011 0000 0000 0000 0001 0020 0000  ............. ..
-00004190: 00b3 0100 0064 6f63 5072 6f70 732f 636f  .....docProps/co
-000041a0: 7265 2e78 6d6c 504b 0102 1400 1400 0000  re.xmlPK........
-000041b0: 0800 874e e240 7c52 f707 fe00 0000 7f01  ...N.@|R........
-000041c0: 0000 1300 0000 0000 0000 0100 2000 0000  ............ ...
-000041d0: 3603 0000 646f 6350 726f 7073 2f63 7573  6...docProps/cus
-000041e0: 746f 6d2e 786d 6c50 4b01 0214 000a 0000  tom.xmlPK.......
-000041f0: 0000 0087 4ee2 4000 0000 0000 0000 0000  ....N.@.........
-00004200: 0000 0005 0000 0000 0000 0000 0010 0000  ................
-00004210: 0065 0400 0077 6f72 642f 504b 0102 1400  .e...word/PK....
-00004220: 0a00 0000 0000 874e e240 0000 0000 0000  .......N.@......
-00004230: 0000 0000 0000 0b00 0000 0000 0000 0000  ................
-00004240: 1000 0000 9a3b 0000 776f 7264 2f5f 7265  .....;..word/_re
-00004250: 6c73 2f50 4b01 0214 0014 0000 0008 0087  ls/PK...........
-00004260: 4ee2 40e0 8ea4 be33 0100 0038 0600 001c  N.@....3...8....
-00004270: 0000 0000 0000 0001 0020 0000 00c3 3b00  ......... ....;.
-00004280: 0077 6f72 642f 5f72 656c 732f 646f 6375  .word/_rels/docu
-00004290: 6d65 6e74 2e78 6d6c 2e72 656c 7350 4b01  ment.xml.relsPK.
-000042a0: 0214 0014 0000 0008 0087 4ee2 4081 b4d3  ..........N.@...
-000042b0: 50c4 0200 00e7 0700 0011 0000 0000 0000  P...............
-000042c0: 0001 0020 0000 003f 3000 0077 6f72 642f  ... ...?0..word/
-000042d0: 646f 6375 6d65 6e74 2e78 6d6c 504b 0102  document.xmlPK..
-000042e0: 1400 1400 0000 0800 874e e240 8caf 87ad  .........N.@....
-000042f0: bf03 0000 8412 0000 1200 0000 0000 0000  ................
-00004300: 0100 2000 0000 3b35 0000 776f 7264 2f66  .. ...;5..word/f
-00004310: 6f6e 7454 6162 6c65 2e78 6d6c 504b 0102  ontTable.xmlPK..
-00004320: 1400 1400 0000 0800 874e e240 0b29 7ddf  .........N.@.)}.
-00004330: c401 0000 5105 0000 1000 0000 0000 0000  ....Q...........
-00004340: 0100 2000 0000 0f24 0000 776f 7264 2f66  .. ....$..word/f
-00004350: 6f6f 7465 7231 2e78 6d6c 504b 0102 1400  ooter1.xmlPK....
-00004360: 1400 0000 0800 874e e240 0b29 7ddf c401  .......N.@.)}...
-00004370: 0000 5105 0000 1000 0000 0000 0000 0100  ..Q.............
-00004380: 2000 0000 0126 0000 776f 7264 2f66 6f6f   ....&..word/foo
-00004390: 7465 7232 2e78 6d6c 504b 0102 1400 1400  ter2.xmlPK......
-000043a0: 0000 0800 874e e240 0b29 7ddf c401 0000  .....N.@.)}.....
-000043b0: 5105 0000 1000 0000 0000 0000 0100 2000  Q............. .
-000043c0: 0000 f327 0000 776f 7264 2f66 6f6f 7465  ...'..word/foote
-000043d0: 7233 2e78 6d6c 504b 0102 1400 1400 0000  r3.xmlPK........
-000043e0: 0800 874e e240 7fd1 0bb4 e801 0000 9e05  ...N.@..........
-000043f0: 0000 1000 0000 0000 0000 0100 2000 0000  ............ ...
-00004400: 131e 0000 776f 7264 2f68 6561 6465 7231  ....word/header1
-00004410: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
-00004420: 874e e240 963d 9c92 c501 0000 5105 0000  .N.@.=......Q...
-00004430: 1000 0000 0000 0000 0100 2000 0000 2920  .......... ...) 
-00004440: 0000 776f 7264 2f68 6561 6465 7232 2e78  ..word/header2.x
-00004450: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
-00004460: e240 963d 9c92 c501 0000 5105 0000 1000  .@.=......Q.....
-00004470: 0000 0000 0000 0100 2000 0000 1c22 0000  ........ ...."..
-00004480: 776f 7264 2f68 6561 6465 7233 2e78 6d6c  word/header3.xml
-00004490: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
-000044a0: a634 96ed e504 0000 740d 0000 1100 0000  .4......t.......
-000044b0: 0000 0000 0100 2000 0000 ff18 0000 776f  ...... .......wo
-000044c0: 7264 2f73 6574 7469 6e67 732e 786d 6c50  rd/settings.xmlP
-000044d0: 4b01 0214 0014 0000 0008 0087 4ee2 40ae  K...........N.@.
-000044e0: 6484 bf4a 1400 0039 a800 000f 0000 0000  d..J...9........
-000044f0: 0000 0001 0020 0000 0088 0400 0077 6f72  ..... .......wor
-00004500: 642f 7374 796c 6573 2e78 6d6c 504b 0102  d/styles.xmlPK..
-00004510: 1400 0a00 0000 0000 874e e240 0000 0000  .........N.@....
-00004520: 0000 0000 0000 0000 0b00 0000 0000 0000  ................
-00004530: 0000 1000 0000 e529 0000 776f 7264 2f74  .......)..word/t
-00004540: 6865 6d65 2f50 4b01 0214 0014 0000 0008  heme/PK.........
-00004550: 0087 4ee2 40c8 d416 5afe 0500 002c 1900  ..N.@...Z....,..
-00004560: 0015 0000 0000 0000 0001 0020 0000 000e  ........... ....
-00004570: 2a00 0077 6f72 642f 7468 656d 652f 7468  *..word/theme/th
-00004580: 656d 6531 2e78 6d6c 504b 0506 0000 0000  eme1.xmlPK......
-00004590: 1b00 1b00 8d06 0000 fb3e 0000 0000       .........>....
+00000050: 702e 786d 6c9d 91c1 6ec2 3010 44ef 95fa  p.xml...n.0.D...
+00000060: 0f51 ee89 e300 2920 6344 4339 552d 12a1  .Q....) cDC9U-..
+00000070: 1c91 e52c c46a 625b b641 f0f7 7548 05e9  ...,.jb[.A..uH..
+00000080: b5b7 9d59 79fc b443 e697 a60e ce60 ac50  ...Yy..C.....`.P
+00000090: 7216 e238 0903 905c 9542 1e67 e1b6 5845  r..8...\.B.g..XE
+000000a0: e330 b08e c992 d54a c22c bc82 0de7 f4f9  .0.....J.,......
+000000b0: 89ac 8dd2 609c 001b f808 6967 61e5 9c9e  ....`.....iga...
+000000c0: 2264 7905 0db3 b15f 4bbf 3928 d330 e7a5  "dy...._K.9(.0..
+000000d0: 3922 7538 080e 4bc5 4f0d 4887 d224 c910  9"u8..K.O.H..$..
+000000e0: 5c1c c812 ca48 df03 c32e 717a 76ff 0d2d  \....H....qzv..-
+000000f0: 156f f9ec 5771 d51e 9892 021a 5d33 07f4  .o..Wq......]3..
+00000100: a3c5 a9e3 52b9 86a0 bb4b d6ec 0896 6282  ....R....K....b.
+00000110: ba81 ec94 292d 4d08 ea06 9257 cc30 eefc  ....)-M....W.0..
+00000120: 9d5a b3a7 c8bb 90fe a537 bbc1 2719 7634  .Z.......7..'.v4
+00000130: 4c57 37b3 a748 a11c ab0b d100 c569 e63f  LW7..H.......i.?
+00000140: bf4b b2e1 ac86 dc03 d303 ab2d 10f4 30da  .K.........-..0.
+00000150: fc6f bbd5 855a b6f8 bffb bf66 8f6e 275c  .o...Z.....f.n'\
+00000160: b5d1 8c77 480f ce9e 4f16 5ad7 8233 e71b  ...wH...O.Z..3..
+00000170: a7bb f526 f8bc b5b2 c738 f6f5 c718 6793  ...&.....8....g.
+00000180: f17e 85df 06e9 cb6b 1ea5 d924 8f86 8351  .~.....k...$...Q
+00000190: 192d f028 8d92 513e 1a26 e324 49f3 0541  .-.(..Q>.&.$I..A
+000001a0: fd24 e26b dd00 3f19 e1ae ed39 fad2 9ff5  .$.k..?....9....
+000001b0: 5e2e fd01 504b 0304 1400 0000 0800 874e  ^...PK.........N
+000001c0: e240 6120 0ba9 5501 0000 7e02 0000 1100  .@a ..U...~.....
+000001d0: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+000001e0: 786d 6c7d 9251 4f83 3014 85df 4dfc 0fa4  xml}.QO.0...M...
+000001f0: efd0 1696 e908 7489 9a3d 6962 e28c c6b7  ......t..=ib....
+00000200: dade b12a 14d2 7663 fc7b 2963 38a3 f1f1  ...*..vc.{)c8...
+00000210: f69c fbdd 73db 66cb 4355 067b 3056 d53a  ....s.f.CU.{0V.:
+00000220: 4734 2228 002d 6aa9 7491 a3e7 f52a bc46  G4"(.-j.t....*.F
+00000230: 8175 5c4b 5ed6 1a72 d481 454b 7679 9189  .u\K^..r..EKvy..
+00000240: 2615 b581 4753 3760 9c02 1bf4 246d 53d1  &...GS7`....$mS.
+00000250: e468 eb5c 9362 6cc5 162a 6ea3 dea1 7b71  .h.\.bl..*n...{q
+00000260: 539b 8abb be34 056e b8f8 e405 e098 9039  S....4.n.......9
+00000270: aec0 71c9 1dc7 1e18 3613 118d 4829 2664  ..q.....6...H)&d
+00000280: b333 e500 9002 4309 1568 6731 8d28 fef6  .3....C..hg1.(..
+00000290: 3a30 95fd b361 50ce 9c95 725d d3ef 34c6  :0...aP...r]..4.
+000002a0: 3d67 4b71 1427 f7c1 aac9 d8b6 6dd4 2643  =gKq.'......m.&C
+000002b0: 8c3e 3fc5 af0f f74f c3aa a1d2 feae 0420  .>?....O....... 
+000002c0: 9649 318c 4b85 01ee 4006 3d20 3d8e 3b29  .I1.K...@.= =.;)
+000002d0: 2fc9 eddd 7a85 584c e822 2471 4893 35bd  /...z.XL."$qH.5.
+000002e0: 4a69 9212 f296 e193 6bec f7c0 23ab 36ec  Ji......k...#.6.
+000002f0: fde3 6008 f59e e9c8 bf47 c9ad 7be8 9f6e  ..`......G..{..n
+00000300: a340 de74 acd8 d51d d71b d045 867f ab53  .@.t.......E...S
+00000310: c06a ecf8 3761 9c84 641e d2b9 4f38 a329  .j..7a..d...O8.)
+00000320: 999d 253c 0198 cf60 60af fc5f 62c9 6298  ..%<...``.._b.b.
+00000330: 3ad5 43f5 f3c7 b02f 504b 0304 1400 0000  :.C..../PK......
+00000340: 0800 874e e240 c7fb d323 ff00 0000 8001  ...N.@...#......
+00000350: 0000 1300 0000 646f 6350 726f 7073 2f63  ......docProps/c
+00000360: 7573 746f 6d2e 786d 6c9d 90cd 6a84 3018  ustom.xml...j.0.
+00000370: 45f7 85be 43c8 3ee6 a738 1d25 3a54 9dd9  E...C.>..8.%:T..
+00000380: 74d1 42a7 b397 1867 0226 9124 da4a e9bb  t.B....g.&.$.J..
+00000390: 3732 fdd9 77f9 713f 0ee7 5ebe 7bd7 0398  72..w.q?..^.{...
+000003a0: a5f3 ca9a 02d2 8440 208d b09d 32e7 02be  .......@ ...2...
+000003b0: 1e0f 680b 810f ade9 dac1 1a59 c045 7ab8  ..h........Y.Ez.
+000003c0: 2b6f 6ff8 b3b3 a374 4149 0f22 c2f8 025e  +oo....tAI."...^
+000003d0: 4218 738c bdb8 48dd fa24 c626 26bd 75ba  B.s...H..$.&&.u.
+000003e0: 0df1 7467 6cfb 5e09 d958 3169 6902 6684  ..tgl.^..X1ii.f.
+000003f0: 6cb0 987c b01a 8dbf 3878 e5e5 73f8 2fb2  l..|....8x..s./.
+00000400: b362 b5f3 a7e3 3246 dd92 7fc3 17d0 eba0  .b....2F........
+00000410: ba02 7e34 69dd 3429 4911 db67 35a2 8456  ..~4i.4)I..g5..V
+00000420: 28bb cbee 11d9 12c2 2a56 1fb2 87fd 2704  (.......*V....'.
+00000430: e3fa cc20 30ad 8ed5 1f5f 9e22 b69b 44a8  ... 0...._."..D.
+00000440: 2635 7427 e922 7a0e f930 bef9 e04a 4652  &5t'."z..0...JFR
+00000450: 8628 4de2 8609 a59b 6ccb f15f c8f1 8f43  .(M.....l.._...C
+00000460: c9f1 2a77 9dae fc02 504b 0304 0a00 0000  ..*w....PK......
+00000470: 0000 874e e240 0000 0000 0000 0000 0000  ...N.@..........
+00000480: 0000 0500 0000 776f 7264 2f50 4b03 0414  ......word/PK...
+00000490: 0000 0008 0087 4ee2 40a1 43b1 8681 1400  ......N.@.C.....
+000004a0: 0073 a900 000f 0000 0077 6f72 642f 7374  .s.......word/st
+000004b0: 796c 6573 2e78 6d6c ed5d cd6f dc4a 72bf  yles.xml.].o.Jr.
+000004c0: 07c8 ff30 9853 7290 e5f9 9065 0b4f 6f61  ...0.Sr....e.Ooa
+000004d0: cb56 fc10 d9eb ace4 b767 ce0c 47e2 3387  .V.......g..G.3.
+000004e0: 9c90 1c8f e573 90c5 624f c102 4910 ec21  .....s..bO..I..!
+000004f0: 9b43 90c3 2697 2087 20d8 ff66 d79b f75f  .C..&. . ..f..._
+00000500: a4ba ba9a 6cb2 c966 778d 245b 6ff3 de41  ....l..fw.$[o..A
+00000510: 2667 aaab bb3e 7e5d 55fd 315f fde8 c32a  &g...>~]U.1_...*
+00000520: 1ebc 0fb3 3c4a 93e3 e1e8 c1c3 e120 4ce6  ....<J....... L.
+00000530: e922 4a2e 8f87 6f2f 4ef7 1e0f 0779 1124  ."J...o/N....y.$
+00000540: 8b20 4e93 f078 781d e6c3 1f7d fda7 7ff2  . N..xx....}....
+00000550: d5f6 282f aee3 301f 4003 497e b49a 1f0f  ..(/..0.@.I~....
+00000560: af8a 627d b4bf 9fcf afc2 5590 3f48 d761  ..b}......U.?H.a
+00000570: 021f 2ed3 6c15 14f0 985d eeaf 82ec dd66  ....l....].....f
+00000580: bd37 4f57 eba0 8866 511c 15d7 fbe3 870f  .7OW...fQ.......
+00000590: 1f0d a999 f478 b8c9 9223 6a62 6f15 cdb3  .....x...#jbo...
+000005a0: 344f 9785 2039 4a97 cb68 1ed2 1f45 91b9  4O.. 9J..h...E..
+000005b0: f095 94cf d3f9 6615 2605 72dc cfc2 18fa  ......f.&.r.....
+000005c0: 9026 f955 b4ce 556b 2b6e 6b30 c42b d5c8  .&.U..Uk+nk0.+..
+000005d0: 7bdb 20de af62 f5bd ad0b b36d 9a2d d659  {. ..b.....m.-.Y
+000005e0: 3a0f f31c 74b2 8a65 e757 4194 94cd 8ca6  :...t..e.WA.....
+000005f0: 4643 a5e0 1e80 e0f6 e5f0 f745 5340 3e7a  FC.........ES@>z
+00000600: 88ff d2fa 317a 68eb 3189 5d50 2b96 796c  ....1zh.1.]P+.yl
+00000610: 706c d1b6 d4e2 5934 cb82 4caa 190c 40eb  pl....Y4..L...@.
+00000620: f73a 3fd9 e445 ba7a 1e14 41d9 de76 bb7d  .:?..E.z..A..v.}
+00000630: b05d e70f e609 755b d3da 68b2 0f1f 5544  .]....u[..h...UD
+00000640: c3c1 6a7e f4cd 6592 66c1 2c06 e3dc 8ea6  ..j~..e.f.,.....
+00000650: c3af c132 17e9 fc79 b80c 3671 918b c7ec  ...2...y..6q....
+00000660: 4d46 8ff4 847f 4ed3 a4c8 07db a320 9f47  MF....N...... .G
+00000670: d1f1 f0f7 fff1 8bdf fdf6 9743 7871 f534  ...........Cxq.4
+00000680: c96b 2fc2 202f 9ee6 11f4 b1fa d23c 2fc0  .k/. /.......</.
+00000690: ca81 e72a 02f6 cfa2 4534 dcff faab 7d64  ...*....E4....}d
+000006a0: a6fe 6a4c d765 17e4 b71a 3d04 4b04 bb3c  ..jL.e....=.K..<
+000006b0: 970e b53d 9aa7 9ba4 381e 8e1f 8137 c268  ...=....8....7.h
+000006c0: c2e5 5f9d a213 1d0f d58b b7c9 55b4 087f  .._.........U...
+000006d0: 7a15 266f f370 018e 4b5f 3c0f 57d1 cb68  z.&o.p..K_<.W..h
+000006e0: b108 8533 d3bb b7df bcc9 a234 0357 3b1e  ...3.......4.W;.
+000006f0: 3e79 422f cfd2 f9bb 7071 5e00 63d1 aa90  >yB/....pq^.c...
+00000700: 489c 2f5e 7c98 876b e114 c0f6 af15 4f6c  H./^|..k......Ol
+00000710: 67d3 6088 1dd9 4455 cbf8 22d7 d8e3 8b24  g.`...DU.."....$
+00000720: 1032 7a2d 7a1f 0b01 edca 05bb dfc1 e52a  .2z-z..........*
+00000730: 0c04 6c0d 462e 8cb4 9ebb b439 be85 3627  ..l.F......9..6'
+00000740: b7d0 e6f4 16da 3cb8 8536 1fdd 429b 87b7  ......<..6..B...
+00000750: d0e6 634e 9bd2 e895 393e 696d 4277 1de9  ..cN....9>imBw..
+00000760: 9492 2a4a 16e1 870e 13b6 d3b4 9ba8 9da6  ..*J............
+00000770: dd04 ed34 ed26 66a7 6937 213b 8db7 89d8  ...4.&f.i7!;....
+00000780: fc58 8ab5 dd42 ecdd 68b7 003b 4dbf ca27  .X...B..h..;M..'
+00000790: d859 a9f2 229d 3b28 bc49 d1af ee26 45bf  .Y..".;(.I...&E.
+000007a0: b29b 14fd aa6e 52f4 2bba 49d1 ae66 5dbe  .....nR.+.I..f].
+000007b0: 4d8a 7e2d 3629 fa75 d8a4 e8d7 a0ee b472  M.~-6).u.......r
+000007c0: 7e1b 7c03 be9b 145e eebe 4cd3 2249 8b70  ~.|....^..L."I.p
+000007d0: 5084 1ffc 2883 04e8 3080 eda6 6d4c e1fa  P...(...0...mL..
+000007e0: 9c67 7316 815c 61d6 3a0e 668b 6298 1d2d  .gs..\a.:.f.b..-
+000007f0: ea9a d665 2a3d 9640 d4b3 2f93 0311 e548  ...e*=.@../....H
+00000800: ef9a 0718 d0b4 b6d0 c5bb 10e1 e420 5d0e  ............. ].
+00000810: 96d1 e526 838c a72d 72e9 220e 93f7 610c  ...&...-r."...a.
+00000820: d1f0 2058 2c80 9649 9c85 0524 425e 8c4b  .. X,..I...$B^.K
+00000830: 5bca c265 9841 1617 7a91 6b06 c56b 208e  [..e.A..z.k..k .
+00000840: 9270 906c 5633 4f4d af83 4b16 5d98 2cd0  .p.lV3OM..K.].,.
+00000850: 7578 bd55 d4de 8e57 1a47 b029 ae44 581d  ux.U...W.G.).DX.
+00000860: 791a c82a 80a4 d64b 3545 1a0c 6c9e d065  y..*...K5E..l..e
+00000870: 8a67 51ee 072a 8260 f06c 13c7 2183 eeb5  .gQ..*.`.l..!...
+00000880: bfea 915f ff4c a6e3 0292 f44f 6506 c9d4  ..._.L.....Oe...
+00000890: 4be2 c8a5 7f32 33b8 48d9 0d18 4322 4ac6  K....23.H...C"J.
+000008a0: c888 9231 40a2 648c 53ea 9a33 4ea2 648c  ...1@.d.S..3N.d.
+000008b0: 9328 19e3 24ca f671 36a6 b4be 3c77 644b  .(..$..q6...<wdK
+000008c0: 742f a222 f643 dd93 3815 751d 2fe3 3c8f  t/.".C..8.u./.<.
+000008d0: 2e93 00a6 8776 4e8d f168 933e 26f2 1dc9  .....vN..h.>&...
+000008e0: 33d5 2a06 6f82 2cb8 cc82 f5d5 40d4 47bc  3.*.o.,.....@.G.
+000008f0: baf5 2c5d 5c0f 2e7c e398 928a 133e a19b  ..,]\..|.....>..
+00000900: 9e40 47a3 64d3 2e0d 1b34 0e14 25c7 8e4b  .@G.d....4..%..K
+00000910: 5a86 2597 b40c 5b2e 69db adb9 6bbc af20  Z.%...[.i...k.. 
+00000920: 1211 f3ec 4be7 d8ae d711 6ce6 74be 9915  ....K.....l.t...
+00000930: debe 701e c41b 19d2 7ad9 1d94 0ffd 745f  ..p.....z.....t_
+00000940: 99dc 6994 c184 c788 dbdb 9bf0 b4a3 d722  ..i............"
+00000950: f017 0af1 0580 8abb df44 53d1 f919 6d45  .........DS...mE
+00000960: 2745 e539 4e83 dc93 7b0c b54a 7f60 7979  'E.9N...{..J.`yy
+00000970: bd0e 3388 49df 7919 d369 1ac7 e936 5cd8  ..3.I.y..i...6\.
+00000980: a91b 18db e72a e3b1 c847 3a90 f7bc c8d2  .....*...G:.....
+00000990: 8e09 c097 8d6d 6a7a b15a 5f05 7994 7b49  .....mjz.Z_.y.{I
+000009a0: 43d5 de07 af82 b517 e19b 180a fdfe 3a7b  C.............:{
+000009b0: b107 0b04 f1c0 3ec1 7541 1c65 e17f f6d3  ......>.uA.e....
+000009c0: 70f6 e75e 9d7d 79f1 ea6c f014 82f2 e47a  p..^.}y..l.....z
+000009d0: c520 64a4 79c8 f124 f2c4 2d49 952e fcd0  . d.y..$..-I....
+000009e0: 0ea9 607a 8f12 4855 52bf 9412 69ff 32bc  ..`z..HUR...i.2.
+000009f0: 9ea5 012c fef8 64c1 48f9 0652 335c b828  ...,..d.H..R3\.(
+00000a00: 4206 f579 b05a 7b46 53c8 f502 1c7f 0b79  B..y.Z{FS......y
+00000a10: 9967 1a8a b4df 0659 2492 ffd6 b136 dc51  .g.....Y$....6.Q
+00000a20: 8bac f43c 80cc f0a2 b399 2efb d512 f07c  ...<...........|
+00000a30: 33fb 2e9c fb85 5fc8 105c 4708 cda1 9ea8  3....._..\G.....
+00000a40: 77b9 46ea 37a5 d448 fd70 5d92 9ec4 01ac  w.F.7..H.p].....
+00000a50: 6cba 5440 cd1e 2b5a 4e97 15ed 2e7d f60b  l.T@..+ZN....}..
+00000a60: df68 bc69 9c66 cb4d cc52 d189 2266 8d58  .h.i.f.M.R.."f.X
+00000a70: 11b3 869c c69b 5592 737b 8db4 cc4e 23ed  ......U.s{...N#.
+00000a80: 2e7d 66aa 09f9 fa45 d952 c57f 9145 0b96  .}f....E.R...E..
+00000a90: a090 9023 2524 e488 0809 39f2 4142 b670  ...#%$....9.AB.p
+00000aa0: fa8b fea6 b323 c7fe da7f 0761 ff12 8049  .....#.....a...I
+00000ab0: 88d9 65fb 6a72 1786 4b03 4042 8e1e 9190  ..e.jr..K.@B....
+00000ac0: a347 24e4 e811 0939 7a44 428e 1e91 90a3  .G$....9zDB.....
+00000ad0: 4724 e4e8 71f2 7c10 2e97 309f f2e0 4b23  G$..q.|...0...K#
+00000ae0: e7e8 5423 e768 56e4 fbe1 6a0d 5b5c b2eb  ..T#.hV...j.[\..
+00000af0: d6a8 c46e 8a2f e2f0 32f0 2ce4 4823 7e93  ...n./..2.,.H#~.
+00000b00: a54b b1e9 284d 3ab6 6ed8 198b 0a00 3710  .K..(M:.n.....7.
+00000b10: 91a4 1c61 43ec cf42 5e41 c7e5 d7ae 55b7  ...aC..B^A....U.
+00000b20: 60f1 5900 e926 6cb7 e92c 9b35 9ae9 cb34  `.Y..&l..,.5...4
+00000b30: e53a 6647 a659 cd4e 0c43 ba10 db9d dae9  .:fG.Y.N.C......
+00000b40: fa3a 25b7 3175 74ea 2cba bc2a 06e7 5796  .:%.1ut.,..*..W.
+00000b50: 2a48 6ffb b64a 946c 5f60 07b3 f3b6 dc5d  *Ho..J.l_`.....]
+00000b60: 362e 6626 66e3 134b 61e0 55b8 8836 2b25  6.f&f..Ka.U..6+%
+00000b70: 9a2e b3ee 15ce d49d 4587 07f4 b2c0 e5d6  ........E.......
+00000b80: 0efd d228 10bc 3be6 d2de f661 7b68 67f9  ...(..;....a{hg.
+00000b90: 446f 9fdb ffc3 fef6 31fa e0f6 1ff6 d0f6  Do......1.......
+00000ba0: f51f dbe7 f6df b698 4ff2 c1f6 db91 aa77  ........O......w
+00000bb0: 6bdf a1ad aef4 1cb6 f40e f8ee 7568 f3dd  k...........uh..
+00000bc0: 32dd d909 1e0e 6d1e 5cb2 d861 0836 272e  2.....m.\..a.6'.
+00000bd0: dbdf 0124 6ce2 afc1 2714 b1e6 b003 850d  ...$l...'.......
+00000be0: 1536 5d54 38ba 2b17 9b3a 2a40 dd95 8b4d  .6]T8.+..:*@...M
+00000bf0: 294d 64dd 9597 0fc4 eeca cb19 6b77 65e4  )Md.........kwe.
+00000c00: 0cba bb32 7246 df5d 1939 c3f0 ae8c 9cf1  ...2rF.].9......
+00000c10: 7847 466e c0bc 2b13 1b2a 94f0 4608 bd2b  xGFn..+..*..F..+
+00000c20: 2f1b 3694 bc30 96d8 0dea 0e6d f050 32c2  /.6..0.....m.P2.
+00000c30: 4973 3746 eeb1 af12 1d37 08b0 a9c9 046f  Is7F.....7.....o
+00000c40: 2e17 9b82 4cf0 e672 b169 a70b bcb9 bc38  ....L..r.i.....8
+00000c50: e0cd e5e5 0dde 5c46 dee0 cd65 e40d de5c  ......\F...e...\
+00000c60: 46de e0cd 65e4 0dde 4c46 7ee0 cd65 6243  F...e...LF~..ebC
+00000c70: 8512 e71a e0cd e565 c386 9297 0ede 5c46  .......e......\F
+00000c80: 3678 2819 e9e0 cd64 e40f decc 0ceb 914d  6x(....d.......M
+00000c90: 4d26 7873 b9d8 1464 8237 978b 4d3b 5de0  M&xs...d.7..M;].
+00000ca0: cde5 c501 6f2e 2f6f f0e6 32f2 066f 2e23  ....o./o..2..o.#
+00000cb0: 6ff0 e632 f206 6f2e 236f f066 32f2 036f  o..2..o.#o.f2..o
+00000cc0: 2e13 1b2a 9438 d700 6f2e 2f1b 3694 bc74  ...*.8..o./.6..t
+00000cd0: f0e6 32b2 c143 c948 076f 2623 7ff0 ee58  ..2..C.H.o&#...X
+00000ce0: 3feb 2d4f dad4 6482 3797 8b4d 4126 7873  ?.-O..d.7..MA&xs
+00000cf0: b9d8 b4d3 05de 5c5e 1cf0 e6f2 f206 6f2e  ......\^......o.
+00000d00: 236f f0e6 32f2 066f 2e23 6ff0 e632 f206  #o..2..o.#o..2..
+00000d10: 6f26 233f f0e6 32b1 a142 8973 0df0 e6f2  o&#?..2..B.s....
+00000d20: b261 43c9 4b07 6f2e 231b 3c94 8c74 f066  .aC.K.o.#.<..t.f
+00000d30: 32f2 07ef 8e3d 0c37 0cde 5c2e 3605 99e0  2....=.7..\.6...
+00000d40: cde5 62d3 4e17 7873 7971 c09b cbcb 1bbc  ..b.N.xsyq......
+00000d50: b98c bcc1 9bcb c81b bcb9 8cbc c19b cbc8  ................
+00000d60: 1bbc 998c fcc0 9bcb 8403 de5c 5e36 6c28  ...........\^6l(
+00000d70: 3155 076f 2e23 1b3c 948c 74f0 6632 f207  1U.o.#.<..t.f2..
+00000d80: ef8e 7d64 370c de5c 2e36 0599 e0cd e562  ..}d7..\.6.....b
+00000d90: d34e 1778 7379 71c0 9bcb cb1b bcb9 8cbc  .N.xsyq.........
+00000da0: c19b cbc8 1bbc b98c bcc1 9bcb c81b bc99  ................
+00000db0: 8cfc c09b cb84 03de 5c5e 366c 2831 5507  ........\^6l(1U.
+00000dc0: 6f2e 231b 3c94 8c74 f046 4670 2199 7eb7  o.#.<..t.FFp!.~.
+00000dd0: 98b8 800b afed 83fd 4805 1c93 391e aed5  ........H...9...
+00000de0: 795f b145 096e 1a13 97a6 d1d5 61f8 c56f  y_.E.n......a..o
+00000df0: f072 3141 27ae d380 efbc 0fe0 ee37 fd42  .r1A'........7.B
+00000e00: 2fda a188 8783 aa2d a1ea 9b0f e5c6 38b8  /......-......8.
+00000e10: ff0c 79af 83b9 b8a2 6b7b 3413 2783 80ff  ..y.....k{4.'...
+00000e20: 016e 6e91 4f67 7081 44ae 5e05 4b38 c053  .nn.Ogp.D.^.K8.S
+00000e30: 7ba8 3e06 5e30 306a 136e 7713 4d67 b771  {.>.^00j.nw.Mg.q
+00000e40: 9fdb f6e8 5d98 89cb d070 d4b4 8a90 7f54  ....]....p.....T
+00000e50: 2f26 e59b 1371 939c fc92 da24 16e0 38f1  /&...q.....$..8.
+00000e60: 5d98 ecbd 3d17 02ae 6e92 fb78 b577 f25a  ]...=...n..x.w.Z
+00000e70: bc9a c1d5 71c7 c320 db3b 7f2a 44a5 dd20  ....q.. .;.*D.. 
+00000e80: 87f2 efd1 58a9 a331 5ee1 a6eb 882e 8c50  ....X..1^......P
+00000e90: 9b81 6601 5c14 f7e3 722c d4cb 048e 6bab  ..f.\...r,....k.
+00000ea0: 9eab 8ec3 9149 f56a 4cdb aded 3aa6 cb72  .....I.jL...:..r
+00000eb0: 481f efc2 70fd 1a9a 4583 100f a837 7cca  H...p...E....7|.
+00000ec0: 0df5 4fa6 a87f 52f6 6482 4f70 6853 58c6  ..O...R.d.OphSX.
+00000ed0: 21c2 9f78 f8c9 46dc ee07 f76d d0b5 19e9  !..x..F....m....
+00000ee0: a610 afcf dec7 aaa3 6866 864d cc90 ebec  ........hf.M....
+00000ef0: 24a7 be54 aa9c 525e 5ae9 b27a 53e9 52be  $..T..R^Z..zS.R.
+00000f00: e3aa 64d2 a912 321b 964a 4044 389a faae  ..d...2..J@D8...
+00000f10: 3d7c 756b 5aa2 8b08 494b f424 b534 1de1  =|ukZ...IK.$.4..
+00000f20: b4eb a625 b430 434b 75cf c57d c670 ad62  ...%.0CKu..}.p.b
+00000f30: f05d 9abd 1437 310a 27c1 2b19 5b3f 511e  .]...71.'.+.[?Q.
+00000f40: a57f f882 ee6b 1494 d53d 8da2 4175 4f23  .....k...=..AuO#
+00000f50: b85d cd34 2a33 6873 69f9 8e6b 06f2 4aca  .].4*3hsi..k..J.
+00000f60: 36cf a4c2 36cf 0cc8 5bef a319 a0f9 1b66  6...6...[......f
+00000f70: 7077 1a39 e874 4c42 059e 46c8 abef 5423  pw.9.tLB..F...T#
+00000f80: 8f75 f81c 3fd1 e073 72e8 e198 6889 8646  .u..?..sr...h..F
+00000f90: be28 c754 5351 feb1 c267 f98e eb98 8f3a  .(.TSQ...g.....:
+00000fa0: cd80 f25e 9e19 9057 df47 3340 f337 cca0  ...^...W.G3@.7..
+00000fb0: cb31 6f5e 2387 9d1a a1a8 99a7 11f2 ea3b  .1o^#..........;
+00000fc0: d548 2dae 7984 f9b6 9c30 27e3 d249 fbc3  .H-.y....0'..I..
+00000fd0: 1a34 4443 215f 965f 9691 94e6 97ca 9030  .4DC!_._.......0
+00000fe0: 3687 fe7b 85b2 8f3b ad80 4e0d f2ac 809c  6..{...;..N.....
+00000ff0: fa1e 5a81 cae4 ea09 4fa7 5bde b842 9e74  ..Z.....O.[..B.t
+00001000: 2a84 d203 9e42 c8a7 efa1 42d0 0ebf 0cb7  *....B....B.....
+00001010: ac22 d7f1 0e7a 9f5f 4119 602e 6ecc 8090  ."...z._A.`.n...
+00001020: b9ab 0a60 ce97 b64b c3bc d54a 01ed 0da4  ...`...K...J....
+00001030: f318 da57 8271 0ddf 0bbc b1c3 2200 3392  ...W.q......".3.
+00001040: 37ef faa8 4ec1 31b3 344a a68b 592c eb1a  7...N.1.4J..Y,..
+00001050: f08f 9330 8e5f 0599 2805 14e9 1a3a 083f  ...0._..(....:.?
+00001060: 1c80 9388 2ce1 2c3e 0443 6416 874b 91cc  ....,.,>.Cd..K..
+00001070: c3a7 a387 983b 373e 9fa5 05dc b6df 4d9f  .....;7>......M.
+00001080: e151 ccce 06c0 e0f5 cec8 47d1 495f 8087  .Q........G.I_..
+00001090: 2bf4 c458 f494 c83c 07db 8e29 3087 96c5  +..X...<...)0...
+000010a0: 8909 4d07 3725 f2ce 1a95 1e63 b717 1a2a  ..M.7%.....c...*
+000010b0: 631b 1124 ea61 aa7c 0752 624d 87a3 9121  c..$.a.|.RbM...!
+000010c0: 2dfd 3add 7e39 c1ed 53bb d922 0906 fc03  -.:.~9..S.."....
+000010d0: 7f4e 01fe 820d 6161 4b9c 3693 a0b1 4ea1  .N....aaK.6...N.
+000010e0: 7237 1d1d 50f4 ab7d 07ad 4ae0 0a7e e5f1  r7..P..}..J..~..
+000010f0: 047e ec03 ba23 ac87 dacb 9360 7d91 62e9  .~...#.....`}.b.
+00001100: 929a fd0c 426e af9f a92b 841c 84cc cec7  ....Bn...+......
+00001110: ebd5 b3f5 b305 3a7a e9ab 2867 7145 245c  ......:z..(gqE$\
+00001120: 4a04 429c 8b4b 5ca8 1606 8ff9 c7e3 a15c  J.B..K\........\
+00001130: f780 d21a d4c8 b017 205b d58c 92b1 a68f  ........ [......
+00001140: dbd4 d9f6 e8bb 79c3 36a4 aeeb a1cb adba  ......y.6.......
+00001150: 8b59 7693 5749 fb06 8fde 1318 5c20 827e  .Yv.WI......\ .~
+00001160: 4663 05ae 200a 81c9 a016 f88d 1ba1 3df1  Fc.. .........=.
+00001170: 7402 732d f80a bed2 84d3 0da2 a03b a9fb  t.s-.........;..
+00001180: b2d8 3b32 2b18 17e2 4b03 e144 b213 4d8b  ..;2+...K..D..M.
+00001190: a5e0 c05e 2284 db03 f411 98e5 5a0b 12ea  ...^".......Z...
+000011a0: 13d6 33f8 a918 f849 a16a c2ea 3762 b922  ..3....I.j..7b."
+000011b0: 298d 982a 9c34 9db1 683d dca7 85b3 9a08  )..*.4..h=......
+000011c0: 59ac 23a8 592e c297 ca0d acae dbc2 5b92  Y.#.Y.........[.
+000011d0: 7fcb 2317 a83a 8b4b f1cb 47fb 145d 5ad7  ..#..:.K..G..]Z.
+000011e0: 1c7f 8be7 5cfc 068d c011 e840 656f 6662  ....\......@eofb
+000011f0: 8e4b 5ad2 e80e e11e 55ba d38a ceca 7564  .KZ.....U.....ud
+00001200: eb4e 3678 40b3 9531 1b53 f5b9 7d6e 4058  .N6x@..1.S..}n@X
+00001210: 5432 3b98 3e1e cb2b e00b 7169 05f6 0e20  T2;.>..+..qi... 
+00001220: 13cf 4623 58e2 6bb1 f50e 46fa ec94 a623  ..F#X.k...F....#
+00001230: 0a3c 417e 2883 3719 3427 03a8 a5b8 25f4  .<A~(.7.4'....%.
+00001240: 27e9 16e7 e1d6 f854 af3e df62 d13a 42ef  '......T.>.b.:B.
+00001250: 8c68 3da3 42d1 b19a 52d5 18e6 143b ce4b  .h=.B...R....;.K
+00001260: 5380 8ab7 8afe daad faf0 e1d3 e753 5cd9  S............S\.
+00001270: ee10 9a98 6a0c 7b15 16a6 33c9 af04 e821  ....j.{...3....!
+00001280: 8779 1c06 984f 34a6 ac65 14c3 0ae2 29fe  .y...O4..e....).
+00001290: 27ac 0cd9 9de2 cb59 307f 7799 c18f 1f2d  '......Y0.w....-
+000012a0: d43c 56e0 48a4 1d93 5a10 554c 25c1 3572  .<V.H...Z.UL%.5r
+000012b0: f75f 4732 bcff 612a 08bd 087c 11bd 88bc  ._G2..a*...|....
+000012c0: bb8a 1664 94a8 cd87 142d 3717 76ef 83a7  ...d.....-7.v...
+000012d0: d9a7 8f1f 82a3 2935 de5b 30b4 c616 f75d  ......)5.[0....]
+000012e0: 4333 f8b9 c6d1 b761 56a0 ab49 0885 d9dc  C3.....aV..I....
+000012f0: 159a 5f8c 5f9c 3ec7 1d41 1a34 3767 4f01  .._._.>..A.47gO.
+00001300: d817 91f8 95ba 895a 3c72 c76a ece0 cb34  .......Z<r.j...4
+00001310: fbf8 a576 3009 45cd a5d6 bbda 34a7 9b4f  ...v0.E.....4..O
+00001320: 12e1 2fdb d567 427c a2c0 ab8a 283a a6ae  ../..gB|....(:..
+00001330: 646b e756 c393 ddd9 e577 3ab8 fcd6 0607  dk.V.....w:.....
+00001340: 32c6 0855 4815 ff51 066c 4e31 adb9 cca0  2..UH..Q.lN1....
+00001350: c5b4 8f6e 36a6 a5e2 8035 a6ed cb9d fb13  ...n6....5......
+00001360: ac45 baa1 4cb1 1172 b586 6ecd 88d0 8f5a  .E..L..r..n....Z
+00001370: 8664 6578 291f 55d4 29ff be7f 1ac3 0f55  .dex).U.)......U
+00001380: 94e1 a02c 15c9 195e 6152 e51a a5ee da82  ...,...^aR......
+00001390: ed19 c6bd 721f 0f70 facc 51ae 18eb 2e61  ....r..p..Q....a
+000013a0: a9c7 68b4 78d0 50cf 4dcc 525e 43a9 0570  ..h.x.P.M.R^C..p
+000013b0: a483 b6b1 485b e88f d61b 4104 b7a9 ff9f  ....H[....A.....
+000013c0: ed20 c775 9d8e 4137 bb60 a6b9 1218 c0ed  . .u..A7.`......
+000013d0: a0d7 f0b3 027b 0bf8 11df a1f4 d3c6 4e43  .....{........NC
+000013e0: a7b4 bf51 3ceb 283d d5f6 89d6 8b51 0020  ...Q<.(=.....Q. 
+000013f0: 5821 3893 9b48 a986 5425 1854 f6ac 6518  X!8..H..T%.T..e.
+00001400: 7fc4 905a ee21 501b e8ca 1f37 461d 6ab5  ...Z.!P....7F.j.
+00001410: 0554 1fd8 8d0d 756d 3885 db36 413b 1d93  .T....um8..6A;..
+00001420: 504b 28d5 9c99 7c4b 686d f1d2 f6a8 5197  PK(...|Khm....Q.
+00001430: a338 4abd 6f29 b875 74b8 88c7 3351 1bc2  .8J.o).ut...3Q..
+00001440: 2cbd 6ca5 c8c6 b372 376a 6b8c 0612 708d  ,.l....r7jk...p.
+00001450: c04f 5f9c 8e4f 4e1a c511 1981 6305 a68c  .O_..ON.....c...
+00001460: cb77 8bc0 cb14 a199 c6f5 da84 2acf 20a1  .w..........*. .
+00001470: 0bde 0b90 1edf 31bf 5199 61dc d1f8 6e88  ......1.Q.a...n.
+00001480: 9f0a 2f1a a535 cdc7 4aab 7370 9ef2 bb3b  ../..5..J.sp...;
+00001490: 7945 d9ca 7db3 fedd 263c d8ab 25b2 0b7d  yE..}...&<..%..}
+000014a0: a59a 7ed9 0697 5b68 6663 adb5 a8fd e6d6  ..~...[hfc......
+000014b0: 9c00 7a4f 9fef 1029 bbf8 674b f594 1b8f  ..zO...)..gK....
+000014c0: fd30 c3c4 d391 f8bf 01c9 7abd 5a24 3062  .0........z.Z$0b
+000014d0: b541 4462 b4b4 70aa 363a bba7 0b3b 5646  .ADb..p.6:...;VF
+000014e0: 6ebe 97dd fe53 db33 6459 3c1a 9bfb 17be  n....S.3dY<.....
+000014f0: fff5 7ffd e157 3f1f fcfe dfff e10f bff9  .....W?.........
+00001500: d7f6 a091 9690 f4fd 1e23 5a19 b2af 61aa  .........#Z...a.
+00001510: 4092 30bf 0a64 76d9 99e1 3c56 731b 018c  @.0..dv...<Vs...
+00001520: f57f ffe6 9fbc c74a 1583 cf30 d6da 8930  .......J...0...0
+00001530: 9b5e cd85 f6f5 1e3a ff9e d8e9 ba27 56dd  .^.....:.....'V.
+00001540: d50f 0f34 1152 ea5c 57ee 98b6 67da 074c  ...4.R.\W...g..L
+00001550: 51bd 8199 8221 6c84 a045 7678 905b 6bc3  Q....!l..Evx.[k.
+00001560: 0fb0 a94d f292 abf1 d8bd 33fc f254 eec3  ...M......3..T..
+00001570: 2ddf 9cc8 6579 b150 afe5 08dd e6ef 2c26  -...ey.P......,&
+00001580: 73d7 584d 4cf0 13c6 bea2 a29d 0c3c 51a9  s.XML........<Q.
+00001590: 8377 a303 5c0a a555 557a ea93 a39a 8fba  .w..\..UUz......
+000015a0: c5e2 ec29 e616 869a 58a4 f5f8 bacd 98b6  ...)....X.......
+000015b0: 1f39 89c6 372a 74dd 47e8 6c19 e686 ca9a  .9..7*t.G.l.....
+000015c0: 082a cbd8 ab92 57c8 8dea e9b5 daf6 5973  .*....W.......Ys
+000015d0: 26da c7e1 2406 c399 9485 c8a3 9964 20f0  &...$........d .
+000015e0: 8089 a12d a1be 01ab 3037 1a74 88c4 db32  ...-....07.t...2
+000015f0: 9caa 1034 c8db b20c 67e7 306b d39f fef9  ...4....g.0k....
+00001600: 67df ffcb 3f0e 46de e396 6ab3 5b02 990b  g...?.F...j.[...
+00001610: 0d7b 868a befd 5393 ced2 30ab 4e1d 4641  .{....S...0.N.FA
+00001620: 7e62 93d1 98c0 b3e6 2e14 6cd8 85e4 611b  ~b........l...a.
+00001630: e008 28cb dd1d 024e 7b36 1310 b284 b16d  ..(....N{6.....m
+00001640: 9470 2813 95a8 8fd2 091a eb96 5016 8982  .p(.........P...
+00001650: 7c1e 4577 b4f4 5e37 bf2a 7edb e564 a6ab  |.Ew..^7.*~..d..
+00001660: a94d cc58 95c4 3df1 15b7 13de d4c5 fd59  .M.X..=........Y
+00001670: 476e 46ae 34f2 a9ef c89d 22b9 fac8 bf28  GnF.4....."....(
+00001680: 43db e55c 9bb3 a199 c133 89fb c057 dc4e  C..\.....3...W.N
+00001690: e055 1777 97a1 ddc9 c8cd 7898 46fe c877  .U.w......x.F..w
+000016a0: e44e 7170 7de4 5f96 a111 46e8 6705 6438  .Nqp}._...F.g.d8
+000016b0: 7783 1388 1967 93b8 0f7d c5ed 7317 446b  w....g...}..s.Dk
+000016c0: 2851 61b9 0a5a 6f75 e466 784d 237f ec3b  (Qa..Zou.fxM#..;
+000016d0: 72b2 217b 7cf0 0518 da1d 0bd8 0cd6 3ffd  r.!{|.........?.
+000016e0: fcbf 3ffd e7bf 7dfa f5df 7efa fb9f 7dfa  ..?...}...~...}.
+000016f0: d56f 7ce5 0c07 8330 6c69 9ce8 e991 7b5d  .o|....0li....{]
+00001700: f095 0c76 29f8 b8e6 7013 3352 a77b 57a8  ...v)...p.3R.{W.
+00001710: 80d3 ccd6 e400 f5b8 0c4e 0ae3 a0ed a3a4  .........N......
+00001720: 2f19 c91a b4e4 5bf9 38b4 563e f46d 2862  /.....[.8.V>.m(b
+00001730: 7941 76ce f5c6 9512 5fab 25a4 efff e7ef  yAv....._.%.....
+00001740: 7ef7 db5f ca66 666a dd4c 29ba 7195 4e3f  ~.._.ffj.L).q.N?
+00001750: ee39 2bc6 4c1a 4831 5445 6c28 0614 6944  .9+.L.H1TEl(..iD
+00001760: cc53 a782 6397 66ba d268 10c1 9d28 0d64  .S..c.f..h...(.d
+00001770: 49d6 4260 ac83 ed04 a386 7e71 bbc6 3360  I.B`......~q..3`
+00001780: c4cd 3c45 f981 0d04 54c0 a1fb 83d2 8493  ..<E....T.......
+00001790: 3fd0 d03c cd4e bfd4 49ad c354 b8d1 9668  ?..<.N..I..T...h
+000017a0: b06e 02b2 144f a766 a241 f2a2 34ad 699e  .n...O.f.A..4.i.
+000017b0: 0472 baa0 54cf 9d04 6500 c75d 9aa7 3245  .r..T...e..]..2E
+000017c0: f8db b1fb c4d9 cecc 3445 b9b5 cdce d4a5  ........4E......
+000017d0: 49ba f8d4 6127 27f1 f5da 1978 3527 49ee  I...a''....x5'I.
+000017e0: bc9e a807 28c5 768a eabe 0557 6f76 05cf  ....(.v....Wov..
+000017f0: a999 9d90 9429 626d 5827 58b3 099e 4e79  .....)bmX'X...Ny
+00001800: c997 009e ca3a cb2d 2e35 d162 0f6f 1028  .....:.-.5.b.o.(
+00001810: cdf4 4739 bed5 80db 24ec b446 4412 ee35  ..G9....$..FD..5
+00001820: 6054 60df fcdc 303b b5be 898d 773b b7b3  `T`...0;....w;..
+00001830: d999 b90a c986 4a0a 4db3 23ac d4bd 7aea  ......J.M.#...z.
+00001840: 94a5 f89a 1d08 4759 49f7 309d 31cc 4c4c  ......GYI.0.1.LL
+00001850: 9477 594d 80a2 91da 689d 8a7a ae26 f079  .wYM....h..z.&.y
+00001860: 31cc d1d1 9c8d c9cc 4e48 ca04 4c4d 6322  1.......NH..LMc"
+00001870: 1bab 89d7 29f1 fbbc c6d4 9980 580b 49f2  ....).......X.I.
+00001880: d006 46a2 e57d 0a53 a7c2 9dab 3131 f044  ..F..}.S....11.D
+00001890: 4683 3788 b59d 3980 b5d4 34a1 49ae 6609  F.7...9...4.I.f.
+000018a0: 4eb5 2657 d97c 5647 73ad 30b9 3a1a ac0c  N.&W.|VGs.0.:...
+000018b0: 3643 ff55 0027 83a2 024e ad4b 2b68 ac58  6C.U.'...N.K+h.X
+000018c0: cab7 dcbb 62ab 0549 1023 e808 d2df b1bc  ....b..I.#......
+000018d0: 6d4b 3c34 efd4 b2ad 5796 13be 67fa a0a5  mK<4....W...g...
+000018e0: 0a8e 6994 b32c cdb4 20df ccba 45a9 5665  ..i..,.. ...E.Ve
+000018f0: fb64 e924 056d 5837 3cb1 c399 eea6 89ac  .d.$.mX7<.......
+00001900: a379 b1c9 c23d fb4a 5ebb fd10 80eb 77d7  .y...=.J^.....w.
+00001910: ca13 d0db a33e 4154 fbca 7b2c 474d f7a6  .....>AT..{,GM..
+00001920: 8d5c e1a9 3755 df90 3dac 4407 bb9d 64b0  .\..7U..=.D...d.
+00001930: d088 8954 d890 7ffd 7f50 4b03 0414 0000  ...T.....PK.....
+00001940: 0008 0087 4ee2 4058 5aca 1846 0500 0089  ....N.@XZ..F....
+00001950: 0e00 0011 0000 0077 6f72 642f 7365 7474  .......word/sett
+00001960: 696e 6773 2e78 6d6c b557 dd6f db38 0c7f  ings.xml.W.o.8..
+00001970: 3fe0 fe87 c0ef 69fc 153b 0996 0dfe d2ba  ?.....i..;......
+00001980: a1dd 86a5 bb7b 566c 25d1 d596 0c59 ae97  .....{Vl%....Y..
+00001990: fef5 a32c 3bee 5675 1876 585e 2291 fc91  ...,;.Vu.vX^"...
+000019a0: 1449 51f4 ab37 5fab 72f6 4044 4339 db5a  .IQ..7_.r.@DC9.Z
+000019b0: ce95 6dcd 08cb 7941 d971 6b7d b943 f395  ..m...yA.qk}.C..
+000019c0: 356b 2466 052e 3923 5beb 4c1a ebcd ebbf  5k$f..9#[.L.....
+000019d0: ff7a d56d 1a22 2588 3533 50c1 9a4d 956f  .z.m."%.53P..M.o
+000019e0: ad93 94f5 66b1 68f2 13a9 7073 c56b c280  ....f.h...ps.k..
+000019f0: 79e0 a2c2 12b6 e2b8 a8b0 b86f eb79 ceab  y..........o.y..
+00001a00: 1a4b baa7 2595 e785 6bdb 8135 a8e1 5bab  .K..%...k..5..[.
+00001a10: 156c 33a8 9857 3417 bce1 07a9 201b 7e38  .l3..W4..... .~8
+00001a20: d09c 0c7f 2342 fc8a 5d8d 4c79 de56 84c9  ....#B..].Ly.V..
+00001a30: dee2 4290 127c e0ac 39d1 ba19 b555 bfab  ..B..|..9....U..
+00001a40: 0d8e 781a 953c fcec 100f 5539 ca75 8efd  ..x..<....U9.u..
+00001a50: 33c9 e1b8 1d17 c505 f12b ee29 402d 784e  3........+.)@-xN
+00001a60: 9a06 1254 95fa b815 a6ec a2c6 f19f 29ba  ...T..........).
+00001a70: 84fa 0a42 bdd0 b617 4a15 c01d bb5f 4d9e  ...B....J...._M.
+00001a80: 37e5 33bc 21db 3a8b 3774 2fb0 d069 8602  7.3.!.:.7t/..i..
+00001a90: 78e2 45dd 246d 2379 9562 892f faba aebb  x.E.$m#y.b./....
+00001aa0: eaea e62a 6783 134f b2e6 780b 604d 206b  ...*g..O..x.`M k
+00001ab0: 56e5 9b77 47c6 05de 9750 9e9d e35b afa1  V..wG....P...[..
+00001ac0: 361f 39af 66dd a626 2287 7443 6187 b6b5  6.9.f..&".tCa...
+00001ad0: 508c 3d9c 07aa 3de5 1fb8 dcb5 42f0 9615  P.=...=.....B...
+00001ae0: d704 030d c41f 309c ca79 5910 712e 9f09  ......0..yY.q...
+00001af0: 1643 4d7d 12c0 cc55 3d81 26c2 a0e8 73a2  .CM}...U=.&...s.
+00001b00: 6a6d 6b0d a60b 72c0 6d29 eff0 7e27 793d  jmk...r.m)..~'y=
+00001b10: 9af3 dd91 2d70 07d9 7a2b 68f1 0f11 92e6  ....-p..z+h.....
+00001b20: b8dc d538 07d2 28ea 2c03 ed5b 419b bac4  ...8..(.,..[A...
+00001b30: e76b 2ee8 2367 1297 e984 cde0 329f 47c4  .k..#g......2.G.
+00001b40: a85a cb8f 6a5f 9276 b5f6 fc84 05ce e1a0  .Z..j_.v........
+00001b50: 83f9 044c 085e 8e3a d5d5 1550 599f 5a96  ...L.^.:...PY.Z.
+00001b60: cbb6 bf40 1a77 80e8 3088 c127 a102 3dee  ...@.w..0..'..=.
+00001b70: 0046 8b4b 0c7e a0f6 b15e 4cc2 1aaa 9b83  .F.K.~...^L.....
+00001b80: 52d2 4000 08e2 e2cb 8d4e 1e2e 31cb c90e  R.@......N..1...
+00001b90: 6252 92f8 2c49 ca5b 48bb 5afd 4b0b 79ea  bR..,I.[H.Z.K.y.
+00001ba0: 850a 95da 1b82 1f48 8cf3 fba6 c4cd 2952  .......H......)R
+00001bb0: bdab 67b6 e59d c0b4 0fac 26f4 d2d9 d71a  ..g.......&.....
+00001bc0: 3adc ee44 0ff2 3391 d07e 7a59 5cfc 07c5  :..D..3..~zY\...
+00001bd0: 7943 19b9 26f4 7892 ef18 a4ae 1cf4 3404  yC..&.x.......4.
+00001be0: 6537 f8cc 5bd9 cb6a 9777 ba23 c291 19ae  e7..[..j.w.#....
+00001bf0: a01a 3575 e872 b7bc 2016 b05a 412f a53e  ..5u.r.. ..ZA/.>
+00001c00: 36ca 17af 9e02 e8aa 5c0e c9e9 1be7 8f86  6.......\.......
+00001c10: 3824 1dea 86f4 0eee e4b9 84a0 31b9 a38f  8$..........1...
+00001c20: 2462 c57b 3805 85be a953 f5fb 1efc cc01  $b.{8....S......
+00001c30: c254 683e 42bf bf3b d704 110c 5184 97e2  .Th>B..;....Q...
+00001c40: cf18 eb73 864a 5adf 52b8 c0e2 1d2b e09a  ...s.JZ.R....+..
+00001c50: fd31 63f4 7020 020c 502c c92d dc5f 2a78  .1c.p ..P,.-._*x
+00001c60: d7c7 59b7 8dff 6b17 aa7f aa77 7886 8b46  ..Y...k....wx..F
+00001c70: 15be 5a7c 86fb 34a6 dfb6 7dcf 5e66 436f  ..Z|..4...}.^fCo
+00001c80: 52dc 89e3 045e 9822 9d9d 1f38 a9b3 4a86  R....^."...8..J.
+00001c90: 1ef0 3dc7 0d02 3f59 9b30 5e62 a3a5 91e3  ..=...?Y.0^b....
+00001ca0: bb5e 9099 392f fae6 2307 0546 cc72 bd8c  .^..9/..#..F.r..
+00001cb0: 96c6 f304 b1ef 3a46 4c18 7b6e 305c 84ef  ......:FL.{n0\..
+00001cc0: cf13 66ce d27f 81e3 ae63 2367 b5b6 5741  ..f......c#g..WA
+00001cd0: 6c8a c13a f533 7f65 e2c4 a9ed 64c6 88c6  l..:.3.e....d...
+00001ce0: 6990 4691 0993 7861 1285 464e 6067 b131  i.F...xa..FN`g.1
+00001cf0: 0649 e02d fdd4 8449 edd0 718d 9814 39d1  .I.-...I..q...9.
+00001d00: d237 6132 3b4c 42a3 3630 ef85 c3ab f27d  .7a2;LB.60.....}
+00001d10: 44d1 2a58 6746 6d28 7551 6cc6 64b6 1b19  D.*XgFm(uQl.d...
+00001d20: 22ea c661 16fa ae21 061e ca10 4a4c 5958  "..a...!....JLYX
+00001d30: 7a71 b6f6 dce1 4d7a ea5b 9045 e11a c506  zq....Mz.[.E....
+00001d40: 6d01 4259 b6b2 b3e7 3108 1d27 8e8c 710b  m.BY....1..'..q.
+00001d50: 9d34 76d6 8ec1 4e18 82b6 7065 c876 1823  .4v...N...pe.v.#
+00001d60: 6f1d d889 c14e 1a87 ce0a 19ea 204e 0104  o....N...... N..
+00001d70: bfe7 9834 4b50 16c5 063b 2972 bd28 31dd  ...4KP...;)r.(1.
+00001d80: 1f14 8428 422b 438d a255 0628 cf70 1e84  ...(B+C..U.(.p..
+00001d90: 5ce4 c489 c103 8456 2982 5ba7 7c83 7ea4  \......V).[.|.~.
+00001da0: 820d 5da8 daa8 9156 3dc9 7aa5 9e94 59a5  ..]....V=.z...Y.
+00001db0: 9fa3 0457 7b41 f1ec 560d bd80 aa36 7b71  ...W{A..V....6{q
+00001dc0: 1f53 36f2 f704 e61f f294 b36b f723 733e  .S6........k.#s>
+00001dd0: d78c a6c2 6589 60d6 1819 7d08 aa8d 1a6f  ....e.`...}....o
+00001de0: 5272 e8d5 96b7 581c 27bd 8384 3052 61c0  Rr....X.'...0Ra.
+00001df0: 7a7f d1a5 e63e 22de c280 576b 6b9d c0b5  z....>"...Wkk...
+00001e00: 7e2a 4673 8eef 0ffa 2883 77be 1ae9 4dbb  ~*Fs....(.w...M.
+00001e10: df8d 2806 83eb 1316 4c8b 1f1f 8452 b898  ..(.....L....R..
+00001e20: c2d3 6d24 7cef f44f ee0d 9ec6 35c2 e65f  ..m$|..O....5.._
+00001e30: 76ea 0924 b891 5143 61c2 7d3c cd93 0f0a  v..$..QCa.}<....
+00001e40: 0d4d bf14 3bf5 9944 6e71 5deb 216f 7f74  .M..;..Dnq].!o.t
+00001e50: b656 a946 0d47 c124 ec0a f85c ea37 fba3  .V.F.G.$...\.7..
+00001e60: 3bf0 dc9e 073b c5eb 3738 5787 05e9 61a1  ;....;..78W...a.
+00001e70: 04f4 12a4 86c5 44f3 469a 37d1 e063 40cb  ......D.F.7..c@.
+00001e80: f913 6d39 d296 132d 1869 f0b9 d66d 4ef0  ..m9...-.i...mN.
+00001e90: d48b 92b2 7b98 67c6 a5a2 1f78 59f2 8e14  ....{.g....xY...
+00001ea0: d723 716b 3d23 f521 9cbe 215f 7f03 504b  .#qk=#.!..!_..PK
+00001eb0: 0304 1400 0000 0800 874e e240 a0e2 d9ed  .........N.@....
+00001ec0: eb01 0000 3606 0000 1200 0000 776f 7264  ....6.......word
+00001ed0: 2f66 6f6f 746e 6f74 6573 2e78 6d6c ad94  /footnotes.xml..
+00001ee0: db6e db30 0c86 ef07 ec1d 0cdd c7b2 7bc2  .n.0..........{.
+00001ef0: 60c4 e945 830e bd1b d0ed 0114 598e 855a  `..E........Y..Z
+00001f00: a220 c9d1 f2f6 a3cf 591d 043d ddd8 8644  . ......Y..=...D
+00001f10: 7efc 499a 5cdf ff55 7574 10d6 49d0 3949  ~.I.\..Uut..I.9I
+00001f20: e384 4442 7328 a4de e7e4 cfef c7d5 0f12  ..DBs(..........
+00001f30: 39cf 74c1 6ad0 2227 47e1 c8fd e6fb b775  9.t.j."'G......u
+00001f40: c84a 00af c10b 1721 43bb 2c18 9e93 ca7b  .J.....!C.,....{
+00001f50: 9351 ea78 2514 73b1 92dc 8283 d2c7 1c14  .Q.x%.s.........
+00001f60: 85b2 945c d000 b6a0 5749 9a74 5fc6 0217  ...\....WI.t_...
+00001f70: ce61 c007 a60f cc91 01a7 9634 3042 63ac  .a.........40Bc.
+00001f80: 12ac 62de c560 f754 31fb d298 15d2 0df3  ..b..`.T1.......
+00001f90: 7227 6be9 8fc8 4eee 460c e4a4 b13a 1b04  r'k...N.F....:..
+00001fa0: ad26 41ad 4bd6 0b1a 5ea3 875d 6471 266e  .&A.K...^..]dq&n
+00001fb0: efb9 05de 28a1 7d17 915a 51a3 06d0 ae92  ....(.}..ZQ.....
+00001fc0: 664e e3a3 344c b11a 251d 2e25 7150 f568  fN..4L..%..%qP.h
+00001fd0: 174c 7ab3 8837 a5fc 961e 6c2d 0bd8 8a19  .Lz..7....l-....
+00001fe0: b8c0 9d29 46d1 3ba9 baaf 43db dfb9 abaf  ...)F.;...C.....
+00001ff0: 896f 01fe 4f18 b98a 493d 09fb 58a2 27a5  .o..O...I=..X.'.
+00002000: 4a6f 174a 2e56 eaaa fb5b 4f01 c9a5 ae0c  Jo.J.V...[O.....
+00002010: bf56 9bc9 a4d9 e04c 7d66 407e 5a68 cc4c  .V.....L}f@~Zh.L
+00002020: 939f a33d e997 89d5 8ef6 3b94 2577 af8b  ...=......;.%w..
+00002030: 61dc bb00 8bd9 7fae 9811 931c e31e 1ae7  a...............
+00002040: 416d 9967 1337 8410 07e3 62ae 8745 7232  Am.g.7....b..Er2
+00002050: 7de9 35c5 abd9 8944 8a67 4f7b 0d96 ed6a  }.5....D.gO{...j
+00002060: cc2d a437 5148 6fa3 7640 c8e6 6479 4521  .-.7QHo.v@..dyE!
+00002070: f347 8316 4e18 6699 074b f048 1639 493a  .G..N.f..K.H.9I:
+00002080: 3bd3 1a9b 5fb6 7d39 c338 ce06 deef 04ee  ;..._.}9.8......
+00002090: 2074 c26d 1932 567a 813b 2321 74b3 a693   t.m.2Vz.;#!t...
+000020a0: 71ef 3142 fb2b 3c6b 0dba e7b8 3dcf 8ae1  q.1B.+<k....=...
+000020b0: a0bd d44d b74d 9e47 c628 2cfd 0261 6703  ...M.M.G.(,..ag.
+000020c0: 5c12 89ba 47c5 6ef3 0f50 4b03 0414 0000  \...G.n..PK.....
+000020d0: 0008 0087 4ee2 407f d10b b4e8 0100 009e  ....N.@.........
+000020e0: 0500 0010 0000 0077 6f72 642f 6865 6164  .......word/head
+000020f0: 6572 312e 786d 6ca5 94db 6e9c 3010 86ef  er1.xml...n.0...
+00002100: 2bf5 1d90 ef17 c336 892a 1436 52b3 6a95  +......6.*.6R.j.
+00002110: bb4a 691f c06b cc62 057b 2cdb e06e 9fbe  .Ji..k.b.{,..n..
+00002120: 6316 d84d 8956 39dc 003e cc37 ffcc 3073  c..M.V9..>.7..0s
+00002130: 7bf7 47b5 492f ac93 a04b 92a7 1949 84e6  {.G.I/...K...I..
+00002140: 5049 bd2f c9ef 5fdf 575f 49e2 3cd3 156b  PI./.._.W_I.<..k
+00002150: 418b 921c 8423 779b cf9f 6e43 d154 3641  A....#w...nC.T6A
+00002160: 6bed 8a60 7849 1aef 4d41 a9e3 8d50 cca5  k..`xI..MA...P..
+00002170: 4a72 0b0e 6a9f 7250 14ea 5a72 4103 d88a  Jr..j.rP..ZrA...
+00002180: aeb3 3c1b be8c 052e 9c43 57f7 4cf7 cc91  ..<......CW.L...
+00002190: 11a7 9634 3042 a3af 1aac 62de a560 f754  ...40B....b..`.T
+000021a0: 31fb d499 15d2 0df3 7227 5be9 0fc8 ce6e  1.......r'[....n
+000021b0: 260c 94a4 b3ba 1805 ad66 41d1 a438 0a1a  &........fA..8..
+000021c0: 5f93 855d 44f1 82df a3e5 1678 a784 f683  _..]D......x....
+000021d0: 476a 458b 1a40 bb46 9a53 18ef a561 88cd  GjE..@.F.S...a..
+000021e0: 24a9 bf14 44af dae9 5e30 f9d5 c2df 1cf2  $...D...^0......
+000021f0: 6b6a b0b5 2c60 294e c005 ee85 6454 4723  kj..,`)N....dTG#
+00002200: d51e f310 eb7b aaea ffc4 3cbb 14cc 5891  .....{....<...X.
+00002210: 8898 35bc 46c2 739f 9312 c5a4 9e31 ef4b  ..5.F.s......1.K
+00002220: cd59 72f3 eb85 928b b95d 0fff f719 c060  .Yr......].....`
+00002230: 377d a441 7e58 e8cc 1c8f 911f a33d e8a7  7}.A~X.......=..
+00002240: 9915 9bfa 0dca b29b 4568 ee4d 8045 ef3f  ........Eh.M.E.?
+00002250: 36cc 8859 8e71 f79d f3a0 b6cc b399 1b42  6..Y.q.........B
+00002260: 4883 7129 d7e3 2039 ebbe fc0b c5a3 9311  H.q).. 9........
+00002270: 4914 2f1e f61a 2cdb b518 5bc8 af92 905f  I./...,...[...._
+00002280: 27b1 41c8 06c7 9619 1e3f edf0 7af4 8756  '.A......?..z..V
+00002290: 24a1 e859 8bd3 6f4d e8b0 fbad 1a4e 77e0  $..Y..oM.....Nw.
+000022a0: 51c9 74aa 71fe 115c 7068 0107 05eb 3cc4  Q.t.q..\ph....<.
+000022b0: a5fb 5b12 1c9a f861 1847 7f79 6450 7433  ..[....a.G.ydPt3
+000022c0: 42e2 36b6 155e d809 1c5f f1c6 7ab8 cf6a  B.6..^..._..z..j
+000022d0: 2f90 1357 a345 d414 2d87 274e d7cd 3f50  /..W.E..-.'N..?P
+000022e0: 4b03 0414 0000 0008 0087 4ee2 4096 3d9c  K.........N.@.=.
+000022f0: 92c5 0100 0051 0500 0010 0000 0077 6f72  .....Q.......wor
+00002300: 642f 6865 6164 6572 322e 786d 6ca5 94cb  d/header2.xml...
+00002310: 6edb 3010 45f7 05f2 0f02 f716 4537 090a  n.0.E.......E7..
+00002320: 2172 1631 1a64 5720 ed07 d014 6511 e10b  !r.1.dW ....e...
+00002330: 2425 d67f dfa1 2cc9 6e14 1879 6c44 eb31  $%....,.n..ylD.1
+00002340: 67ee 9df1 ccdd fd5f 25b3 9e3b 2f8c ae10  g......_%..;/...
+00002350: c90b 9471 cd4c 2df4 be42 7f7e ff5c fd40  ...q.L-..B.~.\.@
+00002360: 990f 54d7 541a cd2b 74e0 1edd 6fae bedd  ..T.T..+t...o...
+00002370: c5b2 ad5d 06d1 da97 d1b2 0ab5 21d8 1263  ...]........!..c
+00002380: cf5a aea8 cf95 60ce 78d3 849c 1985 4dd3  .Z....`.x.....M.
+00002390: 08c6 7134 aec6 eb82 14c3 2feb 0ce3 de43  ..q4....../....C
+000023a0: aa07 aa7b ead1 8853 4b9a b15c 43ae c638  ...{...SK..\C..8
+000023b0: 4583 cf8d db63 45dd 4b67 5740 b734 889d  E....cE.KgW@.4..
+000023c0: 9022 1c80 5ddc 4e18 53a1 cee9 7214 b49a  ."..].N.S...r...
+000023d0: 05a5 90f2 2868 3ca6 08b7 70f1 46de 63e4  ....(h<...p.F.c.
+000023e0: d6b0 4e71 1d86 8cd8 7109 1a8c f6ad b027  ..Nq....q......'
+000023f0: 1b9f a581 c576 92d4 5f32 d12b 397d 172d  .....v.._2.+9}.-
+00002400: b95e e49b 2dbf a707 5b47 23b4 e204 5ce0  .^..-...[G#...\.
+00002410: de28 467d 0c52 f258 87d4 df53 575f 1349  .(F}.R.X...SW_.I
+00002420: 71c9 ccd8 9184 9835 bc47 c2ff 3927 258a  q......5.G..9'%.
+00002430: 0a3d 633e 579a b3e2 929b 8592 8bb5 5d0f  .=c>W.........].
+00002440: ffef 3380 8569 faca 803c 3ad3 d9d9 8f15  ..3..i...<:.....
+00002450: 5fa3 3de9 9799 9586 fa03 ca8a db85 35ff  _.=...........5.
+00002460: 21c0 62f6 9f5b 6af9 2cc7 fa87 ce07 a3b6  !.b..[j.,.......
+00002470: 34d0 991b 63cc a3f5 39d3 e322 399b 3ef2  4...c...9.."9.>.
+00002480: 1dc3 ab53 10ca 142b 9ff6 da38 ba93 e02d  ...S...+...8...-
+00002490: 92eb 2c92 9b2c 0d08 dac0 dab2 c3e5 971b  ..,..,..........
+000024a0: 8ee7 7090 3c8b 654f 256c bf35 c2e9 a9b7  ..p.<.eO%l.5....
+000024b0: 94c1 24c0 e31d 878d 0310 b286 bd18 4bda  ..$...........K.
+000024c0: 040e 3b22 ddc1 8718 5809 93ce e10a 0b71  ..;"....X......q
+000024d0: f30f 504b 0304 1400 0000 0800 874e e240  ..PK.........N.@
+000024e0: 963d 9c92 c501 0000 5105 0000 1000 0000  .=......Q.......
+000024f0: 776f 7264 2f68 6561 6465 7233 2e78 6d6c  word/header3.xml
+00002500: a594 cb6e db30 1045 f705 f20f 02f7 1645  ...n.0.E.......E
+00002510: 3709 0a21 7216 311a 6457 20ed 07d0 1465  7..!r.1.dW ....e
+00002520: 11e1 0b24 25d6 7fdf a12c c96e 1418 796c  ...$%....,.n..yl
+00002530: 44eb 3167 ee9d f1cc ddfd 5f25 b39e 3b2f  D.1g......_%..;/
+00002540: 8cae 10c9 0b94 71cd 4c2d f4be 427f 7eff  ......q.L-..B.~.
+00002550: 5cfd 4099 0f54 d754 1acd 2b74 e01e dd6f  \.@..T.T..+t...o
+00002560: aebe ddc5 b2ad 5d06 d1da 97d1 b20a b521  ......]........!
+00002570: d812 63cf 5aae a8cf 9560 ce78 d384 9c19  ..c.Z....`.x....
+00002580: 854d d308 c671 34ae c6eb 8214 c32f eb0c  .M...q4....../..
+00002590: e3de 43aa 07aa 7bea d188 534b 9ab1 5c43  ..C...{...SK..\C
+000025a0: aec6 3845 83cf 8ddb 6345 dd4b 6757 40b7  ..8E....cE.KgW@.
+000025b0: 3488 9d90 221c 805d dc4e 1853 a1ce e972  4..."..].N.S...r
+000025c0: 14b4 9a05 a590 f228 683c a608 b770 f146  .......(h<...p.F
+000025d0: de63 e4d6 b04e 711d 868c d871 091a 8cf6  .c...Nq....q....
+000025e0: adb0 271b 9fa5 81c5 7692 d45f 32d1 2b39  ..'.....v.._2.+9
+000025f0: 7d17 2db9 5ee4 9b2d bfa7 075b 4723 b4e2  }.-.^..-...[G#..
+00002600: 045c e0de 2846 7d0c 52f2 5887 d4df 5357  .\..(F}.R.X...SW
+00002610: 5f13 4971 c9cc d891 8498 35bc 47c2 ff39  _.Iq......5.G..9
+00002620: 2725 8a0a 3d63 3e57 9ab3 e292 9b85 928b  '%..=c>W........
+00002630: b55d 0fff ef33 8085 69fa ca80 3c3a d3d9  .]...3..i...<:..
+00002640: d98f 155f a33d e997 9995 86fa 03ca 8adb  ..._.=..........
+00002650: 8535 ff21 c062 f69f 5b6a f92c c7fa 87ce  .5.!.b..[j.,....
+00002660: 07a3 b634 d099 1b63 cca3 f539 d3e3 2239  ...4...c...9.."9
+00002670: 9b3e f21d c3ab 5310 ca14 2b9f f6da 38ba  .>....S...+...8.
+00002680: 93e0 2d92 eb2c 929b 2c0d 08da c0da b2c3  ..-..,..,.......
+00002690: e597 1b8e e770 903c 8b65 4f25 6cbf 35c2  .....p.<.eO%l.5.
+000026a0: e9a9 b794 c124 c0e3 1d87 8d03 10b2 86bd  .....$..........
+000026b0: 184b da04 0e3b 22dd c187 1858 0993 cee1  .K...;"....X....
+000026c0: 0a0b 71f3 0f50 4b03 0414 0000 0008 0087  ..q..PK.........
+000026d0: 4ee2 400b 297d dfc4 0100 0051 0500 0010  N.@.)}.....Q....
+000026e0: 0000 0077 6f72 642f 666f 6f74 6572 312e  ...word/footer1.
+000026f0: 786d 6ca5 94c9 6ee3 300c 86ef 03f4 1d0c  xml...n.0.......
+00002700: dd63 59e9 8281 51a7 8706 2d7a 2bd0 ce03  .cY...Q...-z+...
+00002710: 288a 1c0b d506 49b6 266f 3f94 633b 99ba  (.....I.&o?.c;..
+00002720: 08ba 5cac 78e1 c7ff 2743 dede fd55 32eb  ..\.x...'C...U2.
+00002730: b8f3 c2e8 0a91 bc40 19d7 cc6c 85de 55e8  .......@...l..U.
+00002740: cfeb c3e2 37ca 7ca0 7a4b a5d1 bc42 7bee  ....7.|.zK...B{.
+00002750: d1dd eae2 d76d 2ceb e032 88d6 be8c 9655  .....m,..2.....U
+00002760: a809 c196 187b d670 457d ae04 73c6 9b3a  .....{.pE}..s..:
+00002770: e4cc 286c ea5a 308e a371 5bbc 2c48 d1ff  ..(l.Z0..q[.,H..
+00002780: b2ce 30ee 3da4 baa7 baa3 1e0d 3835 a719  ..0.=.......85..
+00002790: cb35 e4aa 8d53 34f8 dcb8 1d56 d4bd b576  .5...S4....V...v
+000027a0: 0174 4b83 d808 29c2 1ed8 c5cd 8831 156a  .tK...)......1.j
+000027b0: 9d2e 0741 8b49 500a 290f 8286 638c 7033  ...A.IP.)...c.p3
+000027c0: 171f e43d 44ae 0d6b 15d7 a1cf 881d 97a0  ...=D..k........
+000027d0: c168 df08 7bb4 f15d 1a58 6c46 49dd 3913  .h..{..].XlFI.9.
+000027e0: 9d92 e377 d192 ab59 bec9 f267 7ab0 7634  ...w...Y...gz.v4
+000027f0: 422b 8ec0 19ee 8362 6c0f 414a 1eea 90fa  B+.....bl.AJ....
+00002800: 7bec ea7b 2229 ce99 193a 9210 9386 cf48  {..{")...:.....H
+00002810: f83f e7a8 4451 a127 ccf7 4a73 525c 723d  .?..DQ.'..JsR\r=
+00002820: 5372 b6b6 cbfe ff7d 02b0 304d 3f19 9047  Sr.....}..0M?..G
+00002830: 675a 3bf9 b1e2 67b4 27fd 36b1 d250 7f41  gZ;...g.'.6..P.A
+00002840: 5971 33b3 e6bf 0498 cdfe 4b43 2d9f e458  Yq3.......KC-..X
+00002850: 7fdf fa60 d49a 063a 7163 8c79 b43e 677a  ...`...:qc.y.>gz
+00002860: 5824 27d3 472e 31bc 3a06 a14c b1f2 69a7  X$'.G.1.:..L..i.
+00002870: 8da3 1b09 de22 b9ca 22b9 ced2 80a0 15ac  ....."..".......
+00002880: 2ddb 5f9e 5d7f bc84 bde4 592c 3b2a 61fb  -._.].....Y,;*a.
+00002890: 1184 d353 6f29 8349 80c7 1b0e 1b07 2064  ...So).I...... d
+000028a0: 097b 3196 b40e 1c76 44ba 830f 31b0 1226  .{1....vD...1..&
+000028b0: 9dfd 1516 e2ea 1f50 4b03 0414 0000 0008  .......PK.......
+000028c0: 0087 4ee2 400b 297d dfc4 0100 0051 0500  ..N.@.)}.....Q..
+000028d0: 0010 0000 0077 6f72 642f 666f 6f74 6572  .....word/footer
+000028e0: 322e 786d 6ca5 94c9 6ee3 300c 86ef 03f4  2.xml...n.0.....
+000028f0: 1d0c dd63 59e9 8281 51a7 8706 2d7a 2bd0  ...cY...Q...-z+.
+00002900: ce03 288a 1c0b d506 49b6 266f 3f94 633b  ..(.....I.&o?.c;
+00002910: 99ba 08ba 5cac 78e1 c7ff 2743 dede fd55  ....\.x...'C...U
+00002920: 32eb b8f3 c2e8 0a91 bc40 19d7 cc6c 85de  2........@...l..
+00002930: 55e8 cfeb c3e2 37ca 7ca0 7a4b a5d1 bc42  U.....7.|.zK...B
+00002940: 7bee d1dd eae2 d76d 2ceb e032 88d6 be8c  {......m,..2....
+00002950: 9655 a809 c196 187b d670 457d ae04 73c6  .U.....{.pE}..s.
+00002960: 9b3a e4cc 286c ea5a 308e a371 5bbc 2c48  .:..(l.Z0..q[.,H
+00002970: d1ff b2ce 30ee 3da4 baa7 baa3 1e0d 3835  ....0.=.......85
+00002980: a719 cb35 e4aa 8d53 34f8 dcb8 1d56 d4bd  ...5...S4....V..
+00002990: b576 0174 4b83 d808 29c2 1ed8 c5cd 8831  .v.tK...)......1
+000029a0: 156a 9d2e 0741 8b49 500a 290f 8286 638c  .j...A.IP.)...c.
+000029b0: 7033 171f e43d 44ae 0d6b 15d7 a1cf 881d  p3...=D..k......
+000029c0: 97a0 c168 df08 7bb4 f15d 1a58 6c46 49dd  ...h..{..].XlFI.
+000029d0: 3913 9d92 e377 d192 ab59 bec9 f267 7ab0  9....w...Y...gz.
+000029e0: 7634 422b 8ec0 19ee 8362 6c0f 414a 1eea  v4B+.....bl.AJ..
+000029f0: 90fa 7bec ea7b 2229 ce99 193a 9210 9386  ..{..{")...:....
+00002a00: cf48 f83f e7a8 4451 a127 ccf7 4a73 525c  .H.?..DQ.'..JsR\
+00002a10: 723d 5372 b6b6 cbfe ff7d 02b0 304d 3f19  r=Sr.....}..0M?.
+00002a20: 9047 675a 3bf9 b1e2 67b4 27fd 36b1 d250  .GgZ;...g.'.6..P
+00002a30: 7f41 5971 33b3 e6bf 0498 cdfe 4b43 2d9f  .AYq3.......KC-.
+00002a40: e458 7fdf fa60 d49a 063a 7163 8c79 b43e  .X...`...:qc.y.>
+00002a50: 677a 5824 27d3 472e 31bc 3a06 a14c b1f2  gzX$'.G.1.:..L..
+00002a60: 69a7 8da3 1b09 de22 b9ca 22b9 ced2 80a0  i......"..".....
+00002a70: 15ac 2ddb 5f9e 5d7f bc84 bde4 592c 3b2a  ..-._.].....Y,;*
+00002a80: 61fb 1184 d353 6f29 8349 80c7 1b0e 1b07  a....So).I......
+00002a90: 2064 097b 3196 b40e 1c76 44ba 830f 31b0   d.{1....vD...1.
+00002aa0: 1226 9dfd 1516 e2ea 1f50 4b03 0414 0000  .&.......PK.....
+00002ab0: 0008 0087 4ee2 400b 297d dfc4 0100 0051  ....N.@.)}.....Q
+00002ac0: 0500 0010 0000 0077 6f72 642f 666f 6f74  .......word/foot
+00002ad0: 6572 332e 786d 6ca5 94c9 6ee3 300c 86ef  er3.xml...n.0...
+00002ae0: 03f4 1d0c dd63 59e9 8281 51a7 8706 2d7a  .....cY...Q...-z
+00002af0: 2bd0 ce03 288a 1c0b d506 49b6 266f 3f94  +...(.....I.&o?.
+00002b00: 633b 99ba 08ba 5cac 78e1 c7ff 2743 dede  c;....\.x...'C..
+00002b10: fd55 32eb b8f3 c2e8 0a91 bc40 19d7 cc6c  .U2........@...l
+00002b20: 85de 55e8 cfeb c3e2 37ca 7ca0 7a4b a5d1  ..U.....7.|.zK..
+00002b30: bc42 7bee d1dd eae2 d76d 2ceb e032 88d6  .B{......m,..2..
+00002b40: be8c 9655 a809 c196 187b d670 457d ae04  ...U.....{.pE}..
+00002b50: 73c6 9b3a e4cc 286c ea5a 308e a371 5bbc  s..:..(l.Z0..q[.
+00002b60: 2c48 d1ff b2ce 30ee 3da4 baa7 baa3 1e0d  ,H....0.=.......
+00002b70: 3835 a719 cb35 e4aa 8d53 34f8 dcb8 1d56  85...5...S4....V
+00002b80: d4bd b576 0174 4b83 d808 29c2 1ed8 c5cd  ...v.tK...).....
+00002b90: 8831 156a 9d2e 0741 8b49 500a 290f 8286  .1.j...A.IP.)...
+00002ba0: 638c 7033 171f e43d 44ae 0d6b 15d7 a1cf  c.p3...=D..k....
+00002bb0: 881d 97a0 c168 df08 7bb4 f15d 1a58 6c46  .....h..{..].XlF
+00002bc0: 49dd 3913 9d92 e377 d192 ab59 bec9 f267  I.9....w...Y...g
+00002bd0: 7ab0 7634 422b 8ec0 19ee 8362 6c0f 414a  z.v4B+.....bl.AJ
+00002be0: 1eea 90fa 7bec ea7b 2229 ce99 193a 9210  ....{..{")...:..
+00002bf0: 9386 cf48 f83f e7a8 4451 a127 ccf7 4a73  ...H.?..DQ.'..Js
+00002c00: 525c 723d 5372 b6b6 cbfe ff7d 02b0 304d  R\r=Sr.....}..0M
+00002c10: 3f19 9047 675a 3bf9 b1e2 67b4 27fd 36b1  ?..GgZ;...g.'.6.
+00002c20: d250 7f41 5971 33b3 e6bf 0498 cdfe 4b43  .P.AYq3.......KC
+00002c30: 2d9f e458 7fdf fa60 d49a 063a 7163 8c79  -..X...`...:qc.y
+00002c40: b43e 677a 5824 27d3 472e 31bc 3a06 a14c  .>gzX$'.G.1.:..L
+00002c50: b1f2 69a7 8da3 1b09 de22 b9ca 22b9 ced2  ..i......".."...
+00002c60: 80a0 15ac 2ddb 5f9e 5d7f bc84 bde4 592c  ....-._.].....Y,
+00002c70: 3b2a 61fb 1184 d353 6f29 8349 80c7 1b0e  ;*a....So).I....
+00002c80: 1b07 2064 097b 3196 b40e 1c76 44ba 830f  .. d.{1....vD...
+00002c90: 31b0 1226 9dfd 1516 e2ea 1f50 4b03 040a  1..&.......PK...
+00002ca0: 0000 0000 0087 4ee2 4000 0000 0000 0000  ......N.@.......
+00002cb0: 0000 0000 000b 0000 0077 6f72 642f 7468  .........word/th
+00002cc0: 656d 652f 504b 0304 1400 0000 0800 874e  eme/PK.........N
+00002cd0: e240 c8d4 165a fe05 0000 2c19 0000 1500  .@...Z....,.....
+00002ce0: 0000 776f 7264 2f74 6865 6d65 2f74 6865  ..word/theme/the
+00002cf0: 6d65 312e 786d 6ced 594b 6f1b 3710 be17  me1.xml.YKo.7...
+00002d00: e87f 58ec bd95 64eb 1119 9103 5b8f b88d  ..X...d.....[...
+00002d10: 9d04 9192 2247 6a97 da65 c45d 2e48 ca8e  ...."Gj..e.].H..
+00002d20: 6e41 722a 0a14 2890 1639 3440 d14b 0f45  nAr*..(..94@.K.E
+00002d30: d100 0dd0 a03d f4bf d485 8334 fd11 1d72  .....=.....4...r
+00002d40: a515 2951 f503 3e04 4564 1fb4 dc6f 663e  ..)Q..>.Ed...of>
+00002d50: ce70 bf21 5757 af3d 4ca8 7788 b920 2c6d  .p.!WW.=L.w.. ,m
+00002d60: f995 8fcb be87 d380 8524 8d5a fedd 41ef  .........$.Z..A.
+00002d70: a32b be27 244a 4344 598a 5bfe 140b ffda  .+.'$JCDY.[.....
+00002d80: f687 1f5c 455b 32c6 09f6 c03e 155b a8e5  ...\E[2....>.[..
+00002d90: c752 665b a592 0860 1889 8f59 8653 b837  .Rf[...`...Y.S.7
+00002da0: 623c 4112 2e79 540a 393a 02bf 092d 6d94  b<A..yT.9:...-m.
+00002db0: cbf5 5282 48ea 7b29 4ac0 edad d188 04d8  ..R.H.{)J.......
+00002dc0: fbeb d5ef 6fbe 7ff6 e7a3 2fe0 dfdf 9ec7  ....o...../.....
+00002dd0: e852 0894 4aa1 0602 cafb 2a02 b60c 3536  .R..J.....*...56
+00002de0: 1c57 1442 4c45 9b72 ef10 d196 0fe1 4276  .W.BLE.r......Bv
+00002df0: 34c0 0fa5 ef51 2424 dc68 f965 fdf1 4bdb  4....Q$$.h.e..K.
+00002e00: 574b 686b 6644 e51a 5bc3 aea7 3f33 bb99  WKhkfD..[...?3..
+00002e10: 4138 ded0 3179 342c 8256 abb5 6a7d a7f0  A8..1y4,.V..j}..
+00002e20: af01 54ae e2ba 8d6e bd5b 2ffc 6900 0a02  ..T....n.[/.i...
+00002e30: 9869 cec5 f6d9 d868 5767 5803 947f 75f8  .i.....hWgX...u.
+00002e40: ee34 3a9b 150b 6ff8 df5c e1bc 5353 7f16  .4:...o..\..SS..
+00002e50: 5e83 72ff d515 7caf d786 2c5a 780d caf1  ^.r...|...,Zx...
+00002e60: b515 7c6d b7b9 dbb1 fd6b 508e afaf e01b  ..|m.....kP.....
+00002e70: e59d 4eb5 61f9 d7a0 9892 74bc 822e d7ea  ..N.a.....t.....
+00002e80: 9bed f96c 0bc8 88d1 3d27 bc59 abf6 1a1b  ...l....='.Y....
+00002e90: 33e7 0b14 ac86 6275 a910 2396 ca75 6b2d  3.....bu..#..uk-
+00002ea0: 410f 18ef 0140 0129 9224 f5e4 34c3 2314  A....@.).$..4.#.
+00002eb0: c062 7efd d3e7 af7f fbc3 db27 512c 5514  .b~........'Q,U.
+00002ec0: b485 9171 3b1f 0ac4 ca90 0ae8 8980 934c  ...q;..........L
+00002ed0: b6fc 4f33 044f c7c2 e9c9 ab57 c78f 5f1e  ..O3.O.....W.._.
+00002ee0: 3ffe f5f8 c993 e3c7 3f9b de2d bb3d 9446  ?.......?..-.=.F
+00002ef0: a6dd db1f befa e7f9 23ef ef5f be7b fbf4  ........#.._.{..
+00002f00: eb3c f432 5e98 f855 f2cb 7078 960c 5adf  .<.2^..U..px..Z.
+00002f10: bc78 fdf2 c5c9 b32f dffc f8d4 e17d 87a3  .x...../.....}..
+00002f20: a109 1f90 040b ef26 3ef2 eeb0 0426 a8b3  .......&>....&..
+00002f30: 6307 c043 7e3e 8b41 8c88 69b1 9346 02a5  c..C~>.A..i..F..
+00002f40: 4845 71f8 efca d842 df9c 228a 1cb8 5d6c  HEq....B.."...]l
+00002f50: e7f1 1e07 2d71 01af 4f1e 5884 fb31 9f48  ....-q..O.X..1.H
+00002f60: e2f0 7823 4e2c e001 6374 9771 6716 6ea8  ..x#N,..ct.qg.n.
+00002f70: 5846 9a07 9334 7207 e713 1377 07a1 4357  XF...4r....w..CW
+00002f80: ec36 4aad 2a77 2719 8828 71b9 6cc7 d8a2  .6J.*w'..(q.l...
+00002f90: 799b a254 a208 a758 7aea 1e1b 63ec 98dd  y..T...Xz...c...
+00002fa0: 7d42 acbc 1e90 8033 c146 d2bb 4fbc 5d44  }B.....3.F..O.]D
+00002fb0: 9c29 1990 a1b5 9a16 467b 2481 ba4c 5d04  .)......F{$..L].
+00002fc0: a1de 566e 0eee 79bb 8cba 66dd c187 3612  ..Vn..y...f...6.
+00002fd0: 9e0d 441d e407 985a 69bc 8e26 1225 2e97  ..D....Zi..&.%..
+00002fe0: 0394 5033 e1fb 48c6 2e92 fd29 0f4c 5c57  ..P3..H....).L\W
+00002ff0: 48a8 7484 29f3 ba21 16c2 6573 8bc3 7c8d  H.t.)..!..es..|.
+00003000: a2df 4020 5fce b21f d069 6223 b924 6397  ..@ _....ib#.$c.
+00003010: cf7d c498 89ec b071 3b46 49e6 c2f6 491a  .}.....q;FI...I.
+00003020: 9bd8 4fc4 1896 28f2 6e33 e982 1f30 fb09  ..O...(.n3...0..
+00003030: 51d7 5007 94ae 2df7 3d82 ad72 9fae 0677  Q.P...-.=..r...w
+00003040: 4143 4d4a 8b05 a2ee 4cb8 a396 d731 b3d6  ACMJ....L....1..
+00003050: 6f7f 4a47 086b a901 85b7 843b 21e9 692a  o.JG.k.....;!.i*
+00003060: 9e07 b81c fd06 953c f9f6 b983 f2e5 68b6  .......<......h.
+00003070: dbb1 95f0 93f3 a9f5 0e27 cec7 656f 49a3  .........'..eoI.
+00003080: d7e1 9695 b9cd 7848 de7d 61ee a049 7a1b  ......xH.}a..Iz.
+00003090: c3b3 b0da 9dde ebf2 7b5d f6ff f7ba bcee  ........{]......
+000030a0: 79be 7c35 5e08 3068 b3da 07e6 1b6e bdfd  y.|5^.0h.....n..
+000030b0: 4ed6 eebe 4784 d2be 9c52 bc2f f406 5c40  N...G....R./..\@
+000030c0: db09 7b30 a8ec f401 1417 a7b1 2c86 afea  ..{0........,...
+000030d0: 4986 0016 2ee2 48db 789c c9cf 888c fb31  I.....H.x......1
+000030e0: ca60 f35e f195 9348 cc5c 47c2 cb98 8043  .`.^...H.\G....C
+000030f0: a31e 76fa 5678 3a49 0e58 981f 3a2b 1575  ..v.Vx:I.X..:+.u
+00003100: c0cc c543 20b9 182f d78a 7138 30c8 1c5d  ...C ../..q80..]
+00003110: 6f2c 0e52 857b cd36 d207 de39 0165 7b1e  o,.R.{.6...9.e{.
+00003120: 1246 309b c4a6 8344 633e a892 a48f d790  .F0....Dc>......
+00003130: 3407 093d b34b 61d1 74b0 b8a2 dccf 4bb5  4..=.Ka.t.....K.
+00003140: c202 a815 5581 7d91 07bb a996 5fab 8209  ....U.}....._...
+00003150: 18c1 b109 511c aa3a e5a5 9e57 5717 f332  ....Q..:...WW..2
+00003160: 2bbd 2e99 d60a 28c3 0b8e d90a 5854 baa9  +.....(.....XT..
+00003170: b8ae 9d9e 9a5d bed4 ce50 698b 84b1 dc6c  .....]...Pi....l
+00003180: 123a 33ba 8789 1885 78b6 3ad5 e859 689c  .:3.....x.:..Yh.
+00003190: b7d6 cd45 492d 7a2a 15b3 5c18 341a 57fe  ...EI-z*..\.4.W.
+000031a0: 8bc5 456b 0d76 cbda 4053 5329 68ea 1db5  ..Ek.v..@SS)h...
+000031b0: fcfa 660d 964c 80b2 963f 82c3 3b7c 4d32  ..f..L...?..;|M2
+000031c0: 583b 42ed 6711 8de0 4558 2079 fec0 5f44  X;B.g...EX y.._D
+000031d0: 5932 2e64 0789 384f b816 9d5c 0d12 2231  Y2.d..8O...\.."1
+000031e0: f728 495a be9a 7e51 069a 6a0d d1dc 2a1b  .(IZ..~Q..j...*.
+000031f0: 2008 ef2c b926 c8ca bb46 0e8a 6e17 198f   ..,.&...F..n...
+00003200: 4638 9066 d98d 1195 e9fc 1214 3ed7 0ae7  F8.f........>...
+00003210: 5d6d 7e71 b0b2 6413 2877 3f0e 8fbc 219d  ]m~q..d.(w?...!.
+00003220: f03b 0896 58ad 5151 090c 8980 573c 953c  .;..X.QQ....W<.<
+00003230: 9b21 8197 9285 902d d6df 5263 9ac9 aef9  .!.....-..Rc....
+00003240: 5650 afa1 7c1c d12c 46b3 8e62 8a79 0ed7  VP..|..,F..b.y..
+00003250: 525e d0d1 5745 0e8c abd9 9c21 a146 4a66  R^..WE.....!.FJf
+00003260: 8d70 18a9 066b 26d5 eaa6 45d7 c839 aced  .p...k&...E..9..
+00003270: baa7 1ba9 cc19 a2b9 e899 96aa a8ae e956  ...............V
+00003280: 312b c2bc 0d2c e5f2 624d de60 354f 31b4  1+...,..bM.`5O1.
+00003290: 4bb3 c3e7 d2bd 2cb9 cdb9 d62d ed13 8a2e  K.....,....-....
+000032a0: 0109 2ff2 e7e8 ba67 6808 06b5 4530 8b9a  ../....gh...E0..
+000032b0: 62bc 2ac3 4ab3 67a3 76ef 984f f014 6a67  b.*.J.g.v..O..jg
+000032c0: 6912 86ea d7e7 6e97 f256 f408 6738 18bc  i.....n..V..g8..
+000032d0: 50e7 07bb e555 0b43 a3f9 be52 675a ff88  P....U.C...RgZ..
+000032e0: 61fe c0c0 860f 403c 3af0 2a77 42a5 c805  a.....@<:.*wB...
+000032f0: 4283 b6ff 0550 4b03 0414 0000 0008 0087  B....PK.........
+00003300: 4ee2 4035 16cd 05c5 0200 00e7 0700 0011  N.@5............
+00003310: 0000 0077 6f72 642f 646f 6375 6d65 6e74  ...word/document
+00003320: 2e78 6d6c a595 c96e db30 1086 ef05 fa0e  .xml...n.0......
+00003330: 02ef b62c c74e 6d21 4ad0 264d 9043 83a0  ...,.Nm!J.&M.C..
+00003340: 6ece 054d 5112 6189 2448 caac f3f4 1d8a  n..MQ.a.$H......
+00003350: 5adc dad9 2f26 65ce 7cf3 cf0c 97b3 8b3f  Z.../&e.|......?
+00003360: 5519 6ca9 d24c f004 45e3 090a 2827 2265  U.l..L..E...('"e
+00003370: 3c4f d0c3 afeb d102 05da 609e e252 709a  <O........`..Rp.
+00003380: a01d d5e8 e2fc f3a7 331b a782 d415 e526  ........3......&
+00003390: 0004 d7b1 9524 4185 3132 0e43 4d0a 5a61  .....$A.12.CM.Za
+000033a0: 3dae 1851 428b cc8c 89a8 4291 658c d0d0  =..QB.....B.e...
+000033b0: 0a95 86d3 4934 6966 5209 42b5 8678 9798  ....I4ifR.B..x..
+000033c0: 6fb1 462d ae3a a409 4939 c4ca 84aa b0d1  o.F-.:..I9......
+000033d0: 63a1 f2b0 c26a 53cb 11d0 2536 6ccd 4a66  c....jS...%6l.Jf
+000033e0: 76c0 9e9c 7618 91a0 5af1 b815 34ea 0539  v...v...Z...4..9
+000033f0: 97d8 0b6a 87ce 431d 6471 24ae f7bc 6a2b  ...j..C.dq$...j+
+00003400: d044 0c15 2d41 83e0 ba60 7248 e3bd 3448  .D..-A...`rH..4H
+00003410: b1e8 246d 9f4b 625b 959d 9d95 d1ec 205e  ..$m.Kb[...... ^
+00003420: 9ff2 6b7a 70a5 b085 560c c003 dc91 62a4  ..kzp...V.....b.
+00003430: dea9 2a7d 1d5c 7f87 aefe 4f7c 0df0 5f42  ..*}.\....O|.._B
+00003440: c7ad 30e3 bdb0 f725 ba57 aa68 f25c 51db  ..0....%.W.h.\Q.
+00003450: 9de1 840c 21e7 07da 9fad edb4 d9df 7b21  ....!.........{!
+00003460: 251c a98f 1c90 1b25 6ad9 cb91 ec63 b45b  %......%j....c.[
+00003470: bee9 59ee 64bf 41d9 e4f4 2035 fd26 c0c1  ..Y.d.A... 5.&..
+00003480: d95f 1558 d25e 8ed4 97b5 36a2 bac2 06f7  ._.X.^....6.....
+00003490: 5c6b edd8 4a3d 26bc bd48 f64e 5f74 12c2  \k..J=&..H.N_t..
+000034a0: d2e0 8482 8ac4 b739 170a af4b c8cd 46b3  .......9...K..F.
+000034b0: c046 f3c0 1d10 740e 77d7 5aa4 3b37 cae6  .F....t.w.Z.;7..
+000034c0: e75e b941 b5c3 b5e0 4607 362e 1837 09a2  .^.A....F.6..7..
+000034d0: 589b af9a 6114 3a9b 12f3 1c96 b6b8 8415  X...a.:.........
+000034e0: 3e7a 5821 f8ea 4c12 f458 8c2e ef9c 65d8  >zX!..L..X....e.
+000034f0: e260 941e bb16 62e3 6eab 95c1 ca80 134b  .`....b.n......K
+00003500: 1304 97ad 8d39 ae40 e1ef 1bf1 0d93 8d8f  .....9.@........
+00003510: d2d9 7ee7 696f e9a1 8d5e 4d89 f1d0 82e2  ..~.io...^M.....
+00003520: 94aa 9f34 a30a 6e6d 1aa8 06ab 6e53 b8ff  ...4..nm....nS..
+00003530: 6c6c 7612 c819 53da 786e 2684 396a be3c  llv...S.xn&.9j.<
+00003540: 6afe 247d 3698 a734 c375 f912 ffcb 130e  j.$}6..4.u......
+00003550: 4f46 980f 0e74 4bf9 0bf2 e18d eab2 1dac  OF...tK.........
+00003560: 65be 7a84 bf2d bc6a d1d2 3d08 d051 989f  e.z..-.j..=..Q..
+00003570: 2e4e 161e 27f3 1f58 3947 21e1 ffd9 ace9  .N..'..X9G!.....
+00003580: 8662 7901 5d8f 1693 e673 2d0c ecc3 61b9  .by.]....s-...a.
+00003590: a4d9 deaa 979f a0c5 3c72 785f de04 2d97  ........<rx_..-.
+000035a0: 53f7 99d7 06aa edba dc6c 1d22 4ab7 abb4  S........l."J...
+000035b0: c404 ba32 9b36 29f2 dac1 bd01 bca7 378a  ...2.6).......7.
+000035c0: b98e fbc6 958c c363 0b9f 6e72 cf0c 01f9  .......c..nr....
+000035d0: 2751 8326 0556 2b0f 6ae8 b0cd ba4d 0153  'Q.&.V+.j....M.S
+000035e0: bfb9 61d2 bdd0 e77f 0150 4b03 0414 0000  ..a......PK.....
+000035f0: 0008 0087 4ee2 40c8 cae8 592a 0400 0099  ....N.@...Y*....
+00003600: 1000 0012 0000 0077 6f72 642f 666f 6e74  .......word/font
+00003610: 5461 626c 652e 786d 6cc5 5741 6fdb 3614  Table.xml.WAo.6.
+00003620: be0f d87f 1074 6f44 c98a ad18 750a d98a  .....toD....u...
+00003630: 8001 4350 acd9 7aa6 65da e62a 899a 28c7  ..CP..z.e..*..(.
+00003640: f30f 1886 a2a7 a140 2f3b eeb4 43bb 436f  .......@/;..C.Co
+00003650: 1bba fe99 355d fec5 1e49 c996 23da 9333  ....5]...I..#..3
+00003660: 6fa3 10db 7926 1fc8 8fdf f7bd e787 8fbe  o...y&..........
+00003670: 4d62 e39a e49c b274 60da 27c8 3448 1ab1  Mb.....t`.'.4H..
+00003680: 094d 6703 f3cb abf0 8167 1abc c0e9 04c7  .Mg......g......
+00003690: 2c25 0373 45b8 f9e8 fcd3 4f1e 2efb 5396  ,%.sE.....O...S.
+000036a0: 16dc 80f5 29ef 27d1 c09c 1745 d6b7 2c1e  ....).'....E..,.
+000036b0: cd49 82f9 09cb 480a 5f4e 599e e002 fecd  .I....H._NY.....
+000036c0: 6756 82f3 678b ec41 c492 0c17 744c 635a  gV..g..A....tLcZ
+000036d0: ac2c 07a1 ae59 a6c9 db64 61d3 298d 48c0  .,...Y...da.).H.
+000036e0: a245 42d2 42ae b772 1243 4696 f239 cd78  .EB.B..r.CF..9.x
+000036f0: 956d d926 db92 e593 2c67 11e1 1cce 9cc4  .m.&....,g......
+00003700: 2a5f 8269 ba4e 63bb 8d44 098d 72c6 d9b4  *_.i.Nc..D..r...
+00003710: 3881 c358 6a47 9648 05cb 6d24 3f25 b169  8..XjG.H..m$?%.i
+00003720: 2451 ffb3 59ca 723c 8e01 bba5 ed9a e725  $Q..Y.r<.......%
+00003730: 70c6 b29f e204 8257 3421 dcb8 244b e30b  p......W4!..$K..
+00003740: 96e0 544e c870 ca38 b161 ce35 8e07 2672  ..TN.p.8.a.5..&r
+00003750: e0e9 a20e 3a45 2efc 39f0 c935 2d91 299a  ....:E..9..5-.).
+00003760: e39c 9362 3d11 a9f0 1427 345e 55d1 5ce6  ...b=....'4^U.\.
+00003770: 95f3 335a 44f3 2a7e 8d73 2a36 a6d6 703a  ..3ZD.*~.s*6..p:
+00003780: 832f 167c 8c06 265c 09ea f95e cf54 117b  ./.|..&\...^.T.{
+00003790: 607a 1011 a38c 38b0 2935 801e 7255 671d  `z....8.)5..rUg.
+000037a0: 9173 2299 474e b1c3 50cc 8108 e429 57c9  .s".GN..P....)W.
+000037b0: 7d5a 8a42 0d44 3ebc 79f1 c7bb 973b 80b0  }Z.B.D>.y....;..
+000037c0: 0108 0400 d8d5 a305 c2eb ea80 c08b 82a9  ................
+000037d0: f816 0e13 32c5 8bb8 68c2 506e b6b3 81c1  ....2...h.Pn....
+000037e0: f1bc 5044 1b30 0083 f7c2 e0c2 22fb 3018  ..PD.0......".0.
+000037f0: 9e02 1d85 0cb9 1689 d372 73b5 372d 12c8  .........rs.7-..
+00003800: 3922 12d5 b9eb 17a9 cebd 2144 3547 4b88  9"........!D5GK.
+00003810: 3a8d da13 c207 9ec6 5a14 1c34 443d 1085  :.......Z..4D=..
+00003820: 1088 7a76 08c3 d6a1 c097 9473 f545 7b42  ..zv.......s.E{B
+00003830: 1c43 1782 0d68 4b17 210c 1114 bbd9 a58b  .C...hK.!.......
+00003840: dbdf 7ed8 af8b 33d0 c67f a10b 798b ce50  ..~...3.....y..P
+00003850: ca1a 0c03 d8d0 f146 616f 14fa 7775 61ff  .......Fao..wua.
+00003860: 0bba 18b1 454e 492e 2c53 7202 c7c5 2538  ....ENI.,Sr...%8
+00003870: 29f0 509a 6540 bec6 5f2d 8c27 38ad aeb6  ).P.e@.._-.'8...
+00003880: 61a6 3df0 8f33 c917 61a6 ee2e 33d5 7226  a.=..3..a...3.r&
+00003890: 6113 92a7 8790 e602 aed5 f195 092a b446  a............*.F
+000038a0: 10e9 796e e52b 1bed 9ced 7391 fb91 e6c9  ..yn.+....s.....
+000038b0: 2a19 b35d e281 ca0b 40d4 863a d7dd aaa2  *..]....@..:....
+000038c0: b590 5d55 65a7 9b2a edfb 35d6 8813 01fe  ..]Ue..*..5.....
+000038d0: 0dd6 acfd 55eb 21a2 3889 7198 9b8e 704c  ....U.!.8.q...pL
+000038e0: c739 d531 e6c3 ef6f fe7c f7cb ed8f df81  .9.1...o.|......
+000038f0: c0ca 8b6d 5026 9475 5758 8c0b e481 573d  ...mP&.uWX....W=
+00003900: 52da fa7b 2f9b a94e a818 230f 5c9e 1922  R..{/..N..#.\.."
+00003910: 1bc6 c89a 0211 2d52 7295 7d26 116f efb6  ......-Rr.}&.o..
+00003920: 5b70 88e2 dcec 4686 8086 4041 a021 5fb5  [p....F...@A.!_.
+00003930: 681c a708 2bb3 a9f7 228e 3f0a 3ba3 d3aa  h...+...".?.;...
+00003940: d0ac c168 6336 f681 607c 7cfd fce3 afef  ...hc6..`||.....
+00003950: 8dcf e96c 5e68 b9a3 7a15 d55c 3558 f33f  ...l^h..z..\5X.?
+00003960: 342b 152a 7b4a 741b 9cd0 9171 7a8c 9f5d  4+.*{Jt....qz..]
+00003970: ad32 7289 bfe1 73bd c62a 8ad7 deb5 ac52  .2r...s..*.....R
+00003980: 3512 5ac7 ad1e f79e ad5d 0bb4 f69b 51b5  5.Z......]....Q.
+00003990: dbc3 cc68 0b0d 9dc4 445a e9f7 55fe ead4  ...h....DZ..U...
+000039a0: 77ad 596b 3887 82e1 43d3 e0a0 d39a 330b  w.Yk8...C.....3.
+000039b0: d181 b89d ad7a 6e43 706f 8512 9d39 b203  .....znCpo...9..
+000039c0: 59d7 94df f841 208a ddde b6a6 5eb0 7558  Y....A .....^.uX
+000039d0: 881e af0b 4f07 797b eda6 82e8 9f11 e3a2  ....O.y{........
+000039e0: 0727 bfa8 57eb 000a 4e18 ac23 c26e 7cc7  .'..W...N..#.n|.
+000039f0: ed22 a705 16f5 9f3e 90e2 6f5b bc9b 57df  .".....>..o[..W.
+00003a00: dfbc 7d7e fbf3 fb9b d73f 896a a4c7 4394  ..}~.....?.j..C.
+00003a10: ed8e 80b5 1a5a a11c c77e 657b b0d5 eb39  .....Z...~e{...9
+00003a20: c320 ec05 e170 8b1b b093 4eb7 8c68 6b11  . ...p....N..hk.
+00003a30: ec58 3442 c146 2881 1300 d677 b851 f6be  .X4B.F(....w.Q..
+00003a40: fcfc 2f50 4b03 040a 0000 0000 0087 4ee2  ../PK.........N.
+00003a50: 4000 0000 0000 0000 0000 0000 0006 0000  @...............
+00003a60: 005f 7265 6c73 2f50 4b03 0414 0000 0008  ._rels/PK.......
+00003a70: 0087 4ee2 4001 2222 1ffd 0000 00e1 0200  ..N.@.""........
+00003a80: 000b 0000 005f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
+00003a90: ad92 dd4a 0331 1085 ef05 df21 cc7d 37db  ...J.1.....!.}7.
+00003aa0: 2a22 d26c 6f44 e89d 487d 8021 99dd 0ddd  *".loD..H}.!....
+00003ab0: fc90 4cb5 7d7b 837f b8b0 aebd f072 3267  ..L.}{.......r2g
+00003ac0: ce7c 73c8 7a73 7483 78a1 946d f00a 9655  .|s.zst.x..m...U
+00003ad0: 0d82 bc0e c6fa 4ec1 f3ee 6171 0b22 337a  ......N...aq."3z
+00003ae0: 8343 f0a4 e044 1936 cde5 c5fa 8906 e432  .C...D.6.......2
+00003af0: 947b 1bb3 282e 3e2b e899 e39d 9459 f7e4  .{..(.>+.....Y..
+00003b00: 3057 2192 2f9d 3624 875c cad4 c988 7a8f  0W!./.6$.\....z.
+00003b10: 1dc9 555d dfc8 f4d3 039a 91a7 d81a 0569  ..U]...........i
+00003b20: 6bae 41ec 4eb1 6cfe db3b b4ad d574 1ff4  k.A.N.l..;...t..
+00003b30: c191 e789 1572 ac28 ce98 3a62 05af 2119  .....r.(..:b..!.
+00003b40: 693e 07ab 820c 729a 6675 3ecd ef97 4a47  i>....r.fu>...JG
+00003b50: 8c06 19a5 0e89 1631 959c 12db 92ec 3750  .......1......7P
+00003b60: 6179 2ccf f95d 3107 b43c 1f68 7cfc 543c  ay,..]1..<.h|.T<
+00003b70: 7464 f286 cc3c 12c6 3847 74f5 9f44 fa90  td...<..8Gt..D..
+00003b80: 39b8 799e 0fcd 1792 1c7d cce6 0d50 4b03  9.y......}...PK.
+00003b90: 040a 0000 0000 0087 4ee2 4000 0000 0000  ........N.@.....
+00003ba0: 0000 0000 0000 000b 0000 0077 6f72 642f  ...........word/
+00003bb0: 5f72 656c 732f 504b 0304 1400 0000 0800  _rels/PK........
+00003bc0: 874e e240 d3ee 090a 2b01 0000 2f06 0000  .N.@....+.../...
+00003bd0: 1c00 0000 776f 7264 2f5f 7265 6c73 2f64  ....word/_rels/d
+00003be0: 6f63 756d 656e 742e 786d 6c2e 7265 6c73  ocument.xml.rels
+00003bf0: b594 dd4a c430 1085 ef05 df21 e4de a6ed  ...J.0.....!....
+00003c00: eafa c3a6 7b23 c2de cafa 00b1 9dfe 609b  ....{#........`.
+00003c10: 9464 14fb f68e ad0b 5958 e24d 7a13 9829  .d......YX.Mz..)
+00003c20: 39df e961 32bb fdf7 d0b3 2fb0 ae33 5af2  9..a2...../..3Z.
+00003c30: 2c49 3903 5d9a aad3 8de4 6fc7 979b 07ce  ,I9.].....o.....
+00003c40: 1c2a 5da9 de68 907c 02c7 f7c5 f5d5 ee15  .*]..h.|........
+00003c50: 7a85 74c9 b5dd e818 a968 2779 8b38 3e09  z.t......h'y.8>.
+00003c60: e1ca 1606 e512 3382 a62f b5b1 8342 2a6d  ......3../...B*m
+00003c70: 2346 557e a806 449e a65b 617d 0d5e 9c69  #FU~..D..[a}.^.i
+00003c80: b243 25b9 3d54 8f9c 1da7 91c8 ff6b 9bba  .C%.=T.......k..
+00003c90: ee4a 7836 e5e7 001a 2f20 446d 0c82 2545  .Jx6..../ Dm..%E
+00003ca0: 651b 40c9 977a 9390 492e 2ef3 e9ff d7e6  e.@..z..I.......
+00003cb0: e721 fefd fafc 2cc4 dfc6 e4b7 a02a 3fff  .!....,......*?.
+00003cc0: a50e e67f b73e 3f98 ffed fafc 60fe 9b98  .....>?.....`...
+00003cd0: fcdf 79d7 f404 1c89 7a4f 606e 8586 208f  ..y.....zO`n.. .
+00003ce0: 69c2 0122 ad17 cfc3 a913 b290 6531 3dd4  i.."........e1=.
+00003cf0: 46e3 51bd f7e0 07f1 d70a baa0 fd18 6f1d  F.Q...........o.
+00003d00: 20ad 49cf c15c 8af9 0c8e 44d4 241c 4ebd   .I..\....D.$.N.
+00003d10: 3f0f 4b7d ca40 9cad f9e2 0750 4b03 0414  ?.K}.@.....PK...
+00003d20: 0000 0008 0087 4ee2 401b 7cb3 a295 0100  ......N.@.|.....
+00003d30: 0099 0800 0013 0000 005b 436f 6e74 656e  .........[Conten
+00003d40: 745f 5479 7065 735d 2e78 6d6c c596 cd6e  t_Types].xml...n
+00003d50: c230 1084 ef95 fa0e 91af 1531 50a9 aa2a  .0.........1P..*
+00003d60: 0287 fe1c 5b0e f401 5c7b 0351 13db f22e  ....[...\{.Q....
+00003d70: 14de be9b a470 a014 92a2 884b a4c4 f67c  .....p.....K...|
+00003d80: e3f1 28c9 68b2 2ef2 6805 0133 6713 3188  ..(.h...h..3g.1.
+00003d90: fb22 02ab 9dc9 ec3c 11ef b397 debd 8890  .".....<........
+00003da0: 9435 2a77 1612 b101 1493 f1f5 d568 b6f1  .5*w.........h..
+00003db0: 8011 afb6 9888 0591 7f90 12f5 020a 85b1  ................
+00003dc0: f360 7924 75a1 50c4 b761 2ebd d29f 6a0e  .`y$u.P..a....j.
+00003dd0: 72d8 efdf 49ed 2c81 a51e 951a 623c 7a82  r...I.,.....b<z.
+00003de0: 542d 738a 9ed7 fcb8 7612 2047 113d d613  T-s.....v. G.=..
+00003df0: 4b56 2294 f779 a615 b153 b9b2 668f d2fb  KV"..y...S..f...
+00003e00: 21c4 bcb2 9a83 8bcc e30d db10 f220 a11c  !............ ..
+00003e10: f91b f0b3 ee8d a309 9981 68aa 02bd aa82  ..........h.....
+00003e20: 6d48 e3f4 3438 8f92 0dc5 c755 0ed8 7469  mH..48.....U..ti
+00003e30: 9a69 608d 65c1 11c4 506e d980 e979 9684  .i`.e...Pn...y..
+00003e40: 4019 ec3c 1f65 6b17 a03d 7c9b 51b9 ba35  @..<.ek..=|.Q..5
+00003e50: 7189 e48a f6cc bd0d eb4a a621 fccb 0553  q........J.!...S
+00003e60: e65d 6775 6ed6 a51a c7ac 0191 eb5d e4f1  .]gun........]..
+00003e70: 4eb9 5099 dd56 e550 ec95 8f94 cb38 531f  N.P..V.P.....8S.
+00003e80: f93f 72df cbe0 9791 9d74 0313 8e20 0cce  .?r......t... ..
+00003e90: 3e86 0316 4ae1 86fc e185 f9b7 17e5 5b4e  >...J.........[N
+00003ea0: 0abb 7150 499f 3c84 0528 d349 096a e186  ..qPI.<..(.I.j..
+00003eb0: fc0e 4ad0 8adf 4109 1af2 1188 f80d d241  ..J...A........A
+00003ec0: 07b6 ca27 8f00 6993 7751 c25a f724 9ef8  ...'..i.wQ.Z.$..
+00003ed0: 430f b2ba 9eff 2eaa 64b6 4859 fd58 8cbf  C.......d.HY.X..
+00003ee0: 0150 4b01 0214 0014 0000 0008 0087 4ee2  .PK...........N.
+00003ef0: 401b 7cb3 a295 0100 0099 0800 0013 0000  @.|.............
+00003f00: 0000 0000 0001 0020 0000 001b 3d00 005b  ....... ....=..[
+00003f10: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
+00003f20: 6d6c 504b 0102 1400 0a00 0000 0000 874e  mlPK...........N
+00003f30: e240 0000 0000 0000 0000 0000 0000 0b00  .@..............
+00003f40: 0000 0000 0000 0000 1000 0000 8d3b 0000  .............;..
+00003f50: 776f 7264 2f5f 7265 6c73 2f50 4b01 0214  word/_rels/PK...
+00003f60: 0014 0000 0008 0087 4ee2 4035 16cd 05c5  ........N.@5....
+00003f70: 0200 00e7 0700 0011 0000 0000 0000 0001  ................
+00003f80: 0020 0000 00f5 3200 0077 6f72 642f 646f  . ....2..word/do
+00003f90: 6375 6d65 6e74 2e78 6d6c 504b 0102 1400  cument.xmlPK....
+00003fa0: 1400 0000 0800 874e e240 d3ee 090a 2b01  .......N.@....+.
+00003fb0: 0000 2f06 0000 1c00 0000 0000 0000 0100  ../.............
+00003fc0: 2000 0000 b63b 0000 776f 7264 2f5f 7265   ....;..word/_re
+00003fd0: 6c73 2f64 6f63 756d 656e 742e 786d 6c2e  ls/document.xml.
+00003fe0: 7265 6c73 504b 0102 1400 1400 0000 0800  relsPK..........
+00003ff0: 874e e240 c8d4 165a fe05 0000 2c19 0000  .N.@...Z....,...
+00004000: 1500 0000 0000 0000 0100 2000 0000 c42c  .......... ....,
+00004010: 0000 776f 7264 2f74 6865 6d65 2f74 6865  ..word/theme/the
+00004020: 6d65 312e 786d 6c50 4b01 0214 000a 0000  me1.xmlPK.......
+00004030: 0000 0087 4ee2 4000 0000 0000 0000 0000  ....N.@.........
+00004040: 0000 000b 0000 0000 0000 0000 0010 0000  ................
+00004050: 009b 2c00 0077 6f72 642f 7468 656d 652f  ..,..word/theme/
+00004060: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00004070: 0b29 7ddf c401 0000 5105 0000 1000 0000  .)}.....Q.......
+00004080: 0000 0000 0100 2000 0000 b728 0000 776f  ...... ....(..wo
+00004090: 7264 2f66 6f6f 7465 7232 2e78 6d6c 504b  rd/footer2.xmlPK
+000040a0: 0102 1400 1400 0000 0800 874e e240 0b29  ...........N.@.)
+000040b0: 7ddf c401 0000 5105 0000 1000 0000 0000  }.....Q.........
+000040c0: 0000 0100 2000 0000 c526 0000 776f 7264  .... ....&..word
+000040d0: 2f66 6f6f 7465 7231 2e78 6d6c 504b 0102  /footer1.xmlPK..
+000040e0: 1400 1400 0000 0800 874e e240 c7fb d323  .........N.@...#
+000040f0: ff00 0000 8001 0000 1300 0000 0000 0000  ................
+00004100: 0100 2000 0000 3803 0000 646f 6350 726f  .. ...8...docPro
+00004110: 7073 2f63 7573 746f 6d2e 786d 6c50 4b01  ps/custom.xmlPK.
+00004120: 0214 0014 0000 0008 0087 4ee2 4096 3d9c  ..........N.@.=.
+00004130: 92c5 0100 0051 0500 0010 0000 0000 0000  .....Q..........
+00004140: 0001 0020 0000 00d2 2400 0077 6f72 642f  ... ....$..word/
+00004150: 6865 6164 6572 332e 786d 6c50 4b01 0214  header3.xmlPK...
+00004160: 0014 0000 0008 0087 4ee2 407f d10b b4e8  ........N.@.....
+00004170: 0100 009e 0500 0010 0000 0000 0000 0001  ................
+00004180: 0020 0000 00c9 2000 0077 6f72 642f 6865  . .... ..word/he
+00004190: 6164 6572 312e 786d 6c50 4b01 0214 0014  ader1.xmlPK.....
+000041a0: 0000 0008 0087 4ee2 4001 2222 1ffd 0000  ......N.@.""....
+000041b0: 00e1 0200 000b 0000 0000 0000 0001 0020  ............... 
+000041c0: 0000 0067 3a00 005f 7265 6c73 2f2e 7265  ...g:.._rels/.re
+000041d0: 6c73 504b 0102 1400 1400 0000 0800 874e  lsPK...........N
+000041e0: e240 c8ca e859 2a04 0000 9910 0000 1200  .@...Y*.........
+000041f0: 0000 0000 0000 0100 2000 0000 e935 0000  ........ ....5..
+00004200: 776f 7264 2f66 6f6e 7454 6162 6c65 2e78  word/fontTable.x
+00004210: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
+00004220: e240 0b29 7ddf c401 0000 5105 0000 1000  .@.)}.....Q.....
+00004230: 0000 0000 0000 0100 2000 0000 a92a 0000  ........ ....*..
+00004240: 776f 7264 2f66 6f6f 7465 7233 2e78 6d6c  word/footer3.xml
+00004250: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00004260: a0e2 d9ed eb01 0000 3606 0000 1200 0000  ........6.......
+00004270: 0000 0000 0100 2000 0000 ae1e 0000 776f  ...... .......wo
+00004280: 7264 2f66 6f6f 746e 6f74 6573 2e78 6d6c  rd/footnotes.xml
+00004290: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+000042a0: 585a ca18 4605 0000 890e 0000 1100 0000  XZ..F...........
+000042b0: 0000 0000 0100 2000 0000 3919 0000 776f  ...... ...9...wo
+000042c0: 7264 2f73 6574 7469 6e67 732e 786d 6c50  rd/settings.xmlP
+000042d0: 4b01 0214 0014 0000 0008 0087 4ee2 40a1  K...........N.@.
+000042e0: 43b1 8681 1400 0073 a900 000f 0000 0000  C......s........
+000042f0: 0000 0001 0020 0000 008b 0400 0077 6f72  ..... .......wor
+00004300: 642f 7374 796c 6573 2e78 6d6c 504b 0102  d/styles.xmlPK..
+00004310: 1400 0a00 0000 0000 874e e240 0000 0000  .........N.@....
+00004320: 0000 0000 0000 0000 0500 0000 0000 0000  ................
+00004330: 0000 1000 0000 6804 0000 776f 7264 2f50  ......h...word/P
+00004340: 4b01 0214 0014 0000 0008 0087 4ee2 4061  K...........N.@a
+00004350: 200b a955 0100 007e 0200 0011 0000 0000   ..U...~........
+00004360: 0000 0001 0020 0000 00b4 0100 0064 6f63  ..... .......doc
+00004370: 5072 6f70 732f 636f 7265 2e78 6d6c 504b  Props/core.xmlPK
+00004380: 0102 1400 0a00 0000 0000 874e e240 0000  ...........N.@..
+00004390: 0000 0000 0000 0000 0000 0600 0000 0000  ................
+000043a0: 0000 0000 1000 0000 433a 0000 5f72 656c  ........C:.._rel
+000043b0: 732f 504b 0102 1400 1400 0000 0800 874e  s/PK...........N
+000043c0: e240 5855 5a17 5f01 0000 7302 0000 1000  .@XUZ._...s.....
+000043d0: 0000 0000 0000 0100 2000 0000 2700 0000  ........ ...'...
+000043e0: 646f 6350 726f 7073 2f61 7070 2e78 6d6c  docProps/app.xml
+000043f0: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00004400: 963d 9c92 c501 0000 5105 0000 1000 0000  .=......Q.......
+00004410: 0000 0000 0100 2000 0000 df22 0000 776f  ...... ...."..wo
+00004420: 7264 2f68 6561 6465 7232 2e78 6d6c 504b  rd/header2.xmlPK
+00004430: 0102 1400 0a00 0000 0000 874e e240 0000  ...........N.@..
+00004440: 0000 0000 0000 0000 0000 0900 0000 0000  ................
+00004450: 0000 0000 1000 0000 0000 0000 646f 6350  ............docP
+00004460: 726f 7073 2f50 4b05 0600 0000 0017 0017  rops/PK.........
+00004470: 0084 0500 00e1 3e00 0000 00              ......>....
```

## Comparing `tabdoc-1.0.3.dist-info/LICENSE` & `tabdoc-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tabdoc-1.0.3.dist-info/METADATA` & `tabdoc-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabdoc
-Version: 1.0.3
+Version: 1.0.4
 Summary: tabular datasets to excel,word,pdf
 Home-page: https://github.com/tinybees/tabdoc
 Author: TinyBees
 Author-email: a598824322@qq.com
 License: MIT
 Keywords: tabular,datasets,excel,word,pdf
 Platform: UNKNOWN
```

## Comparing `tabdoc-1.0.3.dist-info/RECORD` & `tabdoc-1.0.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-tabdoc/__init__.py,sha256=LXoOGF8wbXsqHi2lgLX1qoNLzOt88va6ieAvPSQ6CKw,205
+tabdoc/__init__.py,sha256=Pwf9OuOHDd8_wkFzQiJOWgunBjRWDfqThYLCMAS_Q7s,205
 tabdoc/tabexcel.py,sha256=QJwNiRgX_QE8MVs4zgnJVKGPM9ZYYQt7a2cBGPZ9V7I,7681
 tabdoc/tabpdf.py,sha256=bu4aNprhWiWA12Mhz_CtLJBX_KfC6AwmNOaHvNXQ0g8,10330
-tabdoc/tabword.py,sha256=Qo9apQgNFEbpvBP3vBw8HaA7G1B6qC-tlcSRuZtnjnk,16014
+tabdoc/tabword.py,sha256=XOiAoQqEG63L_P0A5UVRcNlgOl0j7tB79PtTfYf9iTg,16022
 tabdoc/templates/SimHei.ttf,sha256=rccIEeST9Ktnzjhw7HH7fosL7jgIsCp9cg7W6A654xA,10063973
 tabdoc/templates/__init__.py,sha256=KWhgTfEXeHp242vVpo5sLjZQv5EKTok52kk2n87PnQ4,112
-tabdoc/templates/template.docx,sha256=2Jk0zRUzNg9HN9srGXmsxDw_N9hStFPhnTcF8C6gnoo,17822
-tabdoc-1.0.3.dist-info/LICENSE,sha256=Zhqbr5LXiWdCR27qxTV0fnscCrUfsMNZmwX7b2YuxrE,1066
-tabdoc-1.0.3.dist-info/METADATA,sha256=jJ_LRY9tfItHOCnynsn_m_TeKaiJQ3lnhbZv48Z2Vtg,1272
-tabdoc-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tabdoc-1.0.3.dist-info/top_level.txt,sha256=LC-DKh-j0Rlc6U2wIkElDY4Z_ZOV6GopgaqcDtYgH3s,7
-tabdoc-1.0.3.dist-info/RECORD,,
+tabdoc/templates/template.docx,sha256=Lzi6gq9PUhuJtJp_vQ8gFZzx6iWMi0mEWtpD74d_Unw,17531
+tabdoc-1.0.4.dist-info/LICENSE,sha256=Zhqbr5LXiWdCR27qxTV0fnscCrUfsMNZmwX7b2YuxrE,1066
+tabdoc-1.0.4.dist-info/METADATA,sha256=PaL_5SVeJq1rR9Al5FjGUqVp4ZTMVowEQnVh9nRb7Jk,1272
+tabdoc-1.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tabdoc-1.0.4.dist-info/top_level.txt,sha256=LC-DKh-j0Rlc6U2wIkElDY4Z_ZOV6GopgaqcDtYgH3s,7
+tabdoc-1.0.4.dist-info/RECORD,,
```

