# Comparing `tmp/araste-3.0-py3-none-any.whl.zip` & `tmp/araste-3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 32172 bytes, number of entries: 14
--rw-rw-r--  2.0 unx    10346 b- defN 23-Jun-06 15:24 araste/__init__.py
+Zip file size: 35138 bytes, number of entries: 15
+-rw-rw-r--  2.0 unx    10346 b- defN 23-Jun-16 16:17 araste/__init__.py
 -rw-rw-r--  2.0 unx     6731 b- defN 23-Jun-06 15:24 araste/filters.py
 -rw-rw-r--  2.0 unx    21914 b- defN 22-Nov-05 11:36 araste/fonts/aipara.aff
 -rw-rw-r--  2.0 unx     4767 b- defN 22-Nov-05 11:36 araste/fonts/aipara_mini.aff
--rw-rw-r--  2.0 unx     8907 b- defN 22-Nov-05 12:06 araste/fonts/naqshe.aff
--rw-rw-r--  2.0 unx    15400 b- defN 22-Nov-05 11:36 araste/fonts/nima.aff
+-rw-rw-r--  2.0 unx     7851 b- defN 23-Jun-16 11:57 araste/fonts/naqshe.aff
+-rw-rw-r--  2.0 unx    22358 b- defN 23-Jun-16 13:23 araste/fonts/nima.aff
+-rw-rw-r--  2.0 unx    22232 b- defN 23-Jun-16 16:15 araste/fonts/nima2.aff
 -rw-rw-r--  2.0 unx    20050 b- defN 22-Nov-05 11:36 araste/fonts/zivar.aff
--rwxrwxr-x  2.0 unx     2776 b- defN 23-Jun-06 15:24 araste-3.0.data/scripts/araste
--rwxrwxr-x  2.0 unx     3797 b- defN 23-Jun-06 15:24 araste-3.0.data/scripts/araste-get
--rw-rw-r--  2.0 unx    34523 b- defN 23-Jun-06 15:24 araste-3.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2215 b- defN 23-Jun-06 15:24 araste-3.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:24 araste-3.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-06 15:24 araste-3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1104 b- defN 23-Jun-06 15:24 araste-3.0.dist-info/RECORD
-14 files, 132629 bytes uncompressed, 30366 bytes compressed:  77.1%
+-rwxrwxr-x  2.0 unx     2778 b- defN 23-Jun-16 16:18 araste-3.1.data/scripts/araste
+-rwxrwxr-x  2.0 unx     3797 b- defN 23-Jun-16 16:18 araste-3.1.data/scripts/araste-get
+-rw-rw-r--  2.0 unx    34523 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2215 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1184 b- defN 23-Jun-16 16:18 araste-3.1.dist-info/RECORD
+15 files, 160845 bytes uncompressed, 33212 bytes compressed:  79.4%
```

## zipnote {}

```diff
@@ -12,32 +12,35 @@
 
 Filename: araste/fonts/naqshe.aff
 Comment: 
 
 Filename: araste/fonts/nima.aff
 Comment: 
 
+Filename: araste/fonts/nima2.aff
+Comment: 
+
 Filename: araste/fonts/zivar.aff
 Comment: 
 
-Filename: araste-3.0.data/scripts/araste
+Filename: araste-3.1.data/scripts/araste
 Comment: 
 
-Filename: araste-3.0.data/scripts/araste-get
+Filename: araste-3.1.data/scripts/araste-get
 Comment: 
 
-Filename: araste-3.0.dist-info/LICENSE
+Filename: araste-3.1.dist-info/LICENSE
 Comment: 
 
-Filename: araste-3.0.dist-info/METADATA
+Filename: araste-3.1.dist-info/METADATA
 Comment: 
 
-Filename: araste-3.0.dist-info/WHEEL
+Filename: araste-3.1.dist-info/WHEEL
 Comment: 
 
-Filename: araste-3.0.dist-info/top_level.txt
+Filename: araste-3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: araste-3.0.dist-info/RECORD
+Filename: araste-3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## araste/__init__.py

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/python3
-__version__ = "3.0"
+__version__ = "3.1"
 
 import os
 import sys
 from araste.filters import apply_filter
 
 # copy a block into the board
 def copyboard_glyph(blockstr: str, cursor: int, board: list, korsi: int) -> tuple:
```

## araste/fonts/naqshe.aff

```diff
@@ -1,8 +1,8 @@
-aff3 3 1 5 6 275 1
+aff3 3 1 5 6 242 1
 naqshe
     this is a font file for araste
     designed by Erfan Kheyrollahi <ekm507@gmail.com>
     English glyphs are added from "smbraille" font of figlet.
 
 ا
 3 1
@@ -661,30 +661,15 @@
 ⠈⠈
 ی
 4 1
 ⠀⠀⠀⠀
 ⢠⠀⣔⡂
 ⠈⠒⠒⠁
  
-3 1
-⠀⠀
-⠀⠀
-⠀⠀
- 
-2 1
-⠀⠀
-⠀⠀
-⠀⠀
- 
-1 1
-⠀⠀
-⠀⠀
-⠀⠀
- 
-4 1
+0 0
 ⠀⠀
 ⠀⠀
 ⠀⠀
 (
 3 1
 ⢠⠀
 ⠀⡇
@@ -861,210 +846,60 @@
 ⠀⠁⠈
 »
 4 1
 ⠀⠀⠀
 ⢰⠁⡎
 ⠀⠁⠈
 ۰
-3 1
-⠀⠀
-⠠⡢
-⠀⠀
-۰
-2 1
-⠀⠀
-⠠⡢
-⠀⠀
-۰
-1 1
-⠀⠀
-⠠⡢
-⠀⠀
-۰
-4 1
+0 2
 ⠀⠀
 ⠠⡢
 ⠀⠀
 ۱
-3 1
-⢀⠀
-⠀⡇
-⠀⠀
-۱
-2 1
-⢀⠀
-⠀⡇
-⠀⠀
-۱
-1 1
-⢀⠀
-⠀⡇
-⠀⠀
-۱
-4 1
+0 2
 ⢀⠀
 ⠀⡇
 ⠀⠀
 ۲
-3 1
-⢀⢀
-⢸⠁
-⠀⠀
-۲
-2 1
-⢀⢀
-⢸⠁
-⠀⠀
-۲
-1 1
-⢀⢀
-⢸⠁
-⠀⠀
-۲
-4 1
+0 2
 ⢀⢀
 ⢸⠁
 ⠀⠀
 ۳
-3 1
-⢀⢀⢀
-⠀⡇⠁
-⠀⠀⠀
-۳
-2 1
-⢀⢀⢀
-⠀⡇⠁
-⠀⠀⠀
-۳
-1 1
-⢀⢀⢀
-⠀⡇⠁
-⠀⠀⠀
-۳
-4 1
+0 2
 ⢀⢀⢀
 ⠀⡇⠁
 ⠀⠀⠀
 ۴
-3 1
-⠀⢀
-⢰⠓
-⠀⠀
-۴
-2 1
-⠀⢀
-⢰⠓
-⠀⠀
-۴
-1 1
-⠀⢀
-⢰⠓
-⠀⠀
-۴
-4 1
+0 2
 ⠀⢀
 ⢰⠓
 ⠀⠀
 ۵
-3 1
-⠀⢀⠀
-⠰⡡⡱
-⠀⠀⠀
-۵
-2 1
-⠀⢀⠀
-⠰⡡⡱
-⠀⠀⠀
-۵
-1 1
-⠀⢀⠀
-⠰⡡⡱
-⠀⠀⠀
-۵
-4 1
+0 2
 ⠀⢀⠀
 ⠰⡡⡱
 ⠀⠀⠀
 ۶
-3 1
-⠀⢀⡀
-⢀⠕⠂
-⠀⠀⠀
-۶
-2 1
-⠀⢀⡀
-⢀⠕⠂
-⠀⠀⠀
-۶
-1 1
-⠀⢀⡀
-⢀⠕⠂
-⠀⠀⠀
-۶
-4 1
+0 2
 ⠀⢀⡀
 ⢀⠕⠂
 ⠀⠀⠀
 ۷
-3 1
-⢀⠀⢀
-⠈⢆⠎
-⠀⠀⠀
-۷
-2 1
-⢀⠀⢀
-⠈⢆⠎
-⠀⠀⠀
-۷
-1 1
-⢀⠀⢀
-⠈⢆⠎
-⠀⠀⠀
-۷
-4 1
+0 2
 ⢀⠀⢀
 ⠈⢆⠎
 ⠀⠀⠀
 ۸
-3 1
-⠀⢀⠀
-⢠⠃⢣
-⠀⠀⠀
-۸
-2 1
-⠀⢀⠀
-⢠⠃⢣
-⠀⠀⠀
-۸
-1 1
-⠀⢀⠀
-⢠⠃⢣
-⠀⠀⠀
-۸
-4 1
+0 2
 ⠀⢀⠀
 ⢠⠃⢣
 ⠀⠀⠀
 ۹
-3 1
-⠀⣀
-⠘⢺
-⠀⠀
-۹
-2 1
-⠀⣀
-⠘⢺
-⠀⠀
-۹
-1 1
-⠀⣀
-⠘⢺
-⠀⠀
-۹
-4 1
+0 2
 ⠀⣀
 ⠘⢺
 ⠀⠀
 a
 0 2
  ⢀⣀
  ⠣⠼
```

## araste/fonts/nima.aff

```diff
@@ -1,8 +1,8 @@
-aff3 8 8 4 40 142 1
+aff3 8 8 4 40 204 1
 Nima font
     this is a font file for araste
     designed by Nima Fanniasl <smartnima.com>
 
 آ
 4 1
  ●●● 
@@ -346,25 +346,25 @@
 ح
 2 1
       
       
    ●  
     ● 
 ●●●●● 
-  ●   
+      
       
       
 ح
 1 1
       
       
    ●  
     ● 
 ●●●●● 
-  ●   
+      
       
       
 خ
 4 1
      ●   
          
      ●   
@@ -386,25 +386,25 @@
 خ
 2 1
    ●  
       
    ●  
     ● 
 ●●●●● 
-  ●   
+      
       
       
 خ
 1 1
    ●  
       
    ●  
     ● 
 ●●●●● 
-  ●   
+      
       
       
 د
 4 1
       
       
   ●   
@@ -1111,22 +1111,22 @@
      ● 
 ●●●●●● 
        
        
        
 ل
 1 1
-       
      ● 
      ● 
      ● 
      ● 
 ●●●●●● 
        
        
+       
 م
 4 1
          
          
      ●●  
     ●  ● 
   ●●●●●● 
@@ -1272,41 +1272,41 @@
   ● 
   ● 
     
     
 ه
 1 1
           
-          
      ● ●  
     ●   ● 
      ● ●  
 ●●●●●●●●  
           
           
+          
 ی
 4 1
           
           
         ● 
   ●   ●   
   ●     ● 
   ●     ● 
    ●●●●●  
           
 ی
 3 1
           
           
+          
         ● 
   ●   ●   
   ●     ● 
   ●     ● 
    ●●●●●  
-          
 ی
 2 1
      
      
      
    ● 
 ●●●● 
@@ -1419,7 +1419,627 @@
    ● ● 
        
      ● 
      ● 
      ● 
     ●  
   ●    
+a
+0 2
+          
+          
+ ●●●●●●  
+●     ●  
+●     ●  
+ ●●●●●●  
+          
+          
+b
+0 2
+          
+●        
+●●●●●    
+●    ●  
+●    ●  
+●●●●●    
+          
+          
+c
+0 2
+          
+          
+ ●●●●●●  
+●        
+●        
+ ●●●●●●  
+          
+          
+d
+0 2
+          
+     ●  
+ ●●●●●  
+●    ●  
+●    ●  
+ ●●●●●  
+          
+          
+e
+0 2
+          
+          
+ ●●●●    
+●●●●●●  
+●        
+ ●●●●●  
+          
+          
+f
+0 2
+          
+   ●●●●  
+  ●      
+●●●●●●●  
+  ●      
+  ●      
+          
+          
+g
+0 2
+          
+          
+ ●●●●●●  
+●    ●  
+●    ●  
+ ●●●●●  
+     ●  
+ ●●●●    
+h
+0 2
+          
+●        
+●●●●●    
+●    ●  
+●    ●  
+●    ●  
+          
+          
+i
+0 2
+    
+●  
+    
+●  
+●  
+●  
+    
+    
+j
+0 2
+      
+   ●  
+      
+   ●  
+   ●  
+   ●  
+●  ●  
+ ●●    
+k
+0 2
+          
+●        
+●  ●    
+●●●      
+●  ●    
+●   ●  
+          
+          
+l
+0 2
+    
+●  
+●  
+●  
+●  
+●  
+    
+    
+m
+0 2
+                
+                
+●●●●● ●●●●   
+●    ●    ●  
+●    ●    ●  
+●    ●    ●  
+                
+                
+n
+0 2
+          
+          
+●●●●●   
+●    ●  
+●    ●  
+●    ●  
+          
+          
+o
+0 2
+          
+          
+ ●●●●   
+●    ●  
+●    ●  
+ ●●●●   
+          
+          
+p
+0 2
+          
+          
+●●●●●   
+●    ●  
+●    ●  
+●●●●●   
+●        
+●        
+q
+0 2
+          
+          
+ ●●●●●  
+●    ●  
+●    ●  
+ ●●●●●  
+     ●  
+     ●  
+r
+0 2
+          
+          
+●  ●●●  
+●●●      
+●        
+●        
+          
+          
+s
+0 2
+          
+          
+ ●●●●●  
+●●●     
+   ●●●  
+●●●●●   
+          
+          
+t
+0 2
+          
+  ●      
+●●●●●●  
+  ●      
+  ●      
+   ●●●  
+          
+          
+u
+0 2
+          
+          
+●    ●  
+●    ●  
+●    ●  
+ ●●●●●  
+          
+          
+v
+0 2
+            
+            
+●     ●  
+●     ●  
+ ●   ●    
+   ●      
+            
+            
+w
+0 2
+                    
+                    
+●     ●     ●  
+ ●   ● ●   ●  
+  ● ●   ● ●    
+   ●     ●      
+                    
+                    
+x
+0 2
+          
+●    ●  
+●    ●  
+ ●●●●   
+●    ●  
+●    ●  
+          
+          
+y
+0 2
+          
+          
+●    ●  
+●    ●  
+●    ●  
+ ●●●●●  
+     ●  
+ ●●●●   
+z
+0 2
+          
+          
+●●●●●●  
+   ●    
+  ●      
+●●●●●●  
+          
+          
+A
+0 2
+          
+ ●●●●   
+●    ●  
+●●●●●●  
+●    ●  
+●    ●  
+          
+          
+B
+0 2
+          
+●●●●●   
+●    ●  
+●●●●●   
+●    ●  
+●●●●●   
+          
+          
+C
+0 2
+          
+ ●●●●●  
+●        
+●        
+●        
+ ●●●●●  
+          
+          
+D
+0 2
+          
+●●●●●   
+●    ●  
+●    ●  
+●    ●  
+●●●●●   
+          
+          
+E
+0 2
+          
+●●●●●●  
+●       
+●●●●    
+●       
+●●●●●●  
+          
+          
+F
+0 2
+          
+●●●●●●  
+●       
+●●●●    
+●       
+●       
+          
+          
+G
+0 2
+          
+ ●●●●●  
+●       
+●  ●●●  
+●    ●  
+ ●●●●●  
+          
+          
+H
+0 2
+          
+●    ●  
+●    ●  
+●●●●●●  
+●    ●  
+●    ●  
+          
+          
+I
+0 2
+        
+●●●●●  
+  ●    
+  ●    
+  ●    
+●●●●●  
+        
+        
+J
+0 2
+          
+     ●  
+     ●  
+     ●  
+●    ●  
+ ●●●●   
+          
+          
+K
+0 2
+          
+●   ●  
+●  ●   
+●●●     
+●  ●    
+●   ●  
+          
+          
+L
+0 2
+          
+●        
+●        
+●        
+●        
+●●●●●●  
+          
+          
+M
+0 2
+            
+●    ●  
+●●  ●●  
+● ●● ●  
+●    ●  
+●    ●  
+            
+            
+N
+0 2
+            
+●●    ●  
+● ●   ●  
+●  ●  ●  
+●   ● ●  
+●    ●●  
+            
+            
+O
+0 2
+          
+ ●●●●   
+●    ●  
+●    ●  
+●    ●  
+ ●●●●   
+          
+          
+P
+0 2
+          
+●●●●●   
+●    ●  
+●●●●●   
+●        
+●        
+          
+          
+Q
+0 2
+            
+ ●●●●     
+●    ●    
+●  ●●●    
+●    ●    
+ ●●●● ●●  
+            
+            
+R
+0 2
+          
+●●●●●   
+●    ●  
+●●●●●   
+●    ●  
+●    ●  
+          
+          
+S
+0 2
+          
+ ●●●●●  
+●       
+ ●●●●   
+     ●  
+●●●●●   
+          
+          
+T
+0 2
+            
+●●●●●●●  
+   ●     
+   ●     
+   ●     
+   ●     
+            
+            
+U
+0 2
+          
+●    ●  
+●    ●  
+●    ●  
+●    ●  
+ ●●●●   
+          
+          
+V
+0 2
+            
+●      ●  
+●      ●  
+●      ●  
+ ●    ●   
+   ●●     
+            
+            
+W
+0 2
+                
+●       ●  
+●       ●  
+●   ●   ●  
+ ●  ●  ●   
+  ●● ●●    
+                
+                
+X
+0 2
+            
+●    ●  
+ ●  ●   
+  ●●    
+ ●  ●   
+●    ●  
+            
+            
+Y
+0 2
+            
+●     ●  
+  ● ●    
+   ●      
+   ●      
+   ●      
+            
+            
+Z
+0 2
+            
+●●●●●  
+   ●   
+  ●    
+ ●     
+●●●●●  
+            
+            
+0
+0 2
+        
+ ●●    
+●  ●  
+●  ●  
+●  ●  
+ ●●   
+        
+        
+1
+0 2
+      
+  ●  
+●●●  
+  ●  
+  ●  
+  ●  
+      
+      
+2
+0 2
+          
+ ●●●  
+●   ● 
+  ●●  
+ ●    
+●●●●● 
+          
+          
+3
+0 2
+          
+●●●●   
+    ●  
+ ●●●   
+    ●  
+●●●●   
+          
+          
+4
+0 2
+          
+●  ●    
+●  ●    
+●●●●●●  
+   ●    
+   ●    
+          
+          
+5
+0 2
+          
+●●●●●●  
+●       
+●●●●●   
+     ●  
+●●●●●   
+          
+          
+6
+0 2
+          
+ ●●●●●  
+●       
+●●●●●   
+●    ●  
+ ●●●●   
+          
+          
+7
+0 2
+            
+●●●●●  
+    ●  
+   ●    
+  ●     
+ ●      
+            
+            
+8
+0 2
+          
+ ●●●●   
+●    ●  
+ ●●●●   
+●    ●  
+ ●●●●   
+          
+          
+9
+0 2
+          
+ ●●●●   
+●    ●  
+ ●●●●●  
+     ●  
+●●●●●   
+          
+
```

## Comparing `araste-3.0.data/scripts/araste` & `araste-3.1.data/scripts/araste`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     parser.add_argument("-w", "--width", help="specify width maximum of text", default=None, type=int)
     parser.add_argument("text", help="Text", nargs='*', default='')
 
     args = parser.parse_args()
 
     # default dir where fonts are stored
     # there are 2 possible options. root directory or home directory
-    fonts_dir = araste.__file__.replace("araste.py", "") + "fonts"
+    fonts_dir = araste.__file__.replace("__init__.py", "") + "fonts"
     if args.get_font_list:
         fonts_list = filter(lambda x: x.endswith('aff'), os.listdir(fonts_dir))
         for font_name in fonts_list:
             print(os.path.splitext(font_name)[0])
         exit(0)
     
     elif args.get_filter_list:
```

## Comparing `araste-3.0.data/scripts/araste-get` & `araste-3.1.data/scripts/araste-get`

 * *Files identical despite different names*

## Comparing `araste-3.0.dist-info/LICENSE` & `araste-3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `araste-3.0.dist-info/METADATA` & `araste-3.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: araste
-Version: 3.0
+Version: 3.1
 Summary: Convert persian text to ascii art
 Home-page: https://github.com/ekm507/araste
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: figlet
 Platform: UNKNOWN
```

## Comparing `araste-3.0.dist-info/RECORD` & `araste-3.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-araste/__init__.py,sha256=d8FLFbdbzzdKna8XO5nBhQ4AM_vE-3Y5bR15anQm4x4,10346
+araste/__init__.py,sha256=IQR7JHBsVV3aQWcT9lrEurogaKXhl4lL6Up0zfZgKvs,10346
 araste/filters.py,sha256=Gvi89NFKDm04D7FB1oCU4N4-N3TNs5YzcKB_wtWg6qk,6731
 araste/fonts/aipara.aff,sha256=l2P0fP8LvXe31wkuhrDTbFrmBzPr304y2RkaLFVwAsQ,21914
 araste/fonts/aipara_mini.aff,sha256=lXrk1OpVJLtc45K5lqN74KXw8n5KfLi0NdQrDCU_M-c,4767
-araste/fonts/naqshe.aff,sha256=tBlgkCjVUBAwiT4sVhRdKJD3RNHER4RIR-NE2rQZn3w,8907
-araste/fonts/nima.aff,sha256=pMi1keVEzA-lV019HsoW3QS17dur6rgPfu_kU5iJe3c,15400
+araste/fonts/naqshe.aff,sha256=dAd4UKA_R64f7tKPnsah0g6GlRqwUoQmsdnZK5OaAp8,7851
+araste/fonts/nima.aff,sha256=KNiuYeyiPZzKqpodgOJVUcP5TQ-GEMms4J_aw0SQBA4,22358
+araste/fonts/nima2.aff,sha256=xPLJ3tqKBW4z0Jwt_iYdjjl93ih7NPi6HZpj_zZMcBA,22232
 araste/fonts/zivar.aff,sha256=rBTpxxJ_AAFx9KuDb6lZplq3DVM8PyzN_IsgFoTX4Ps,20050
-araste-3.0.data/scripts/araste,sha256=Gi93OF6CBwi7GR85NcRpy8RauWfcEPqLuFPrtKaCYLo,2776
-araste-3.0.data/scripts/araste-get,sha256=i14FcpyzNO0gIQUYxMpGAeLb2fmXxuiCIIPHmlP-NaQ,3797
-araste-3.0.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-araste-3.0.dist-info/METADATA,sha256=i2Lr-OQAfWxb3ZnyEJSIrmycqzxG_mGbzTsO8Xn4vdA,2215
-araste-3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-araste-3.0.dist-info/top_level.txt,sha256=4kgusdipgAhPRJu18_01Rx9zsgSwu5uApfskLdcopIw,7
-araste-3.0.dist-info/RECORD,,
+araste-3.1.data/scripts/araste,sha256=mbO-pzer332TrjpBLQZPEOYILzZUZ7AhmuHBspoXQsw,2778
+araste-3.1.data/scripts/araste-get,sha256=i14FcpyzNO0gIQUYxMpGAeLb2fmXxuiCIIPHmlP-NaQ,3797
+araste-3.1.dist-info/LICENSE,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+araste-3.1.dist-info/METADATA,sha256=cNxw8j9FFFtaiCKU5nGmb03qns9HtwFjpmsvQU65xbQ,2215
+araste-3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+araste-3.1.dist-info/top_level.txt,sha256=4kgusdipgAhPRJu18_01Rx9zsgSwu5uApfskLdcopIw,7
+araste-3.1.dist-info/RECORD,,
```

