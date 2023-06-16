# Comparing `tmp/better_face-1.0.1-py3-none-any.whl.zip` & `tmp/better_face-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3874 bytes, number of entries: 8
+Zip file size: 3901 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       28 b- defN 23-Jun-16 18:46 betterface/__init__.py
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-16 19:10 betterface/__main__.py
--rw-rw-r--  2.0 unx     5963 b- defN 23-Jun-16 18:46 betterface/interface.py
--rw-rw-r--  2.0 unx      903 b- defN 23-Jun-16 19:27 better_face-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 19:27 better_face-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       56 b- defN 23-Jun-16 19:27 better_face-1.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-16 19:27 better_face-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      646 b- defN 23-Jun-16 19:27 better_face-1.0.1.dist-info/RECORD
-8 files, 7770 bytes uncompressed, 2734 bytes compressed:  64.8%
+-rw-rw-r--  2.0 unx     6146 b- defN 23-Jun-16 21:51 betterface/interface.py
+-rw-rw-r--  2.0 unx      903 b- defN 23-Jun-16 21:53 better_face-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-16 21:53 better_face-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jun-16 21:53 better_face-1.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-16 21:53 better_face-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      646 b- defN 23-Jun-16 21:53 better_face-1.0.2.dist-info/RECORD
+8 files, 7953 bytes uncompressed, 2761 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: betterface/__main__.py
 Comment: 
 
 Filename: betterface/interface.py
 Comment: 
 
-Filename: better_face-1.0.1.dist-info/METADATA
+Filename: better_face-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: better_face-1.0.1.dist-info/WHEEL
+Filename: better_face-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: better_face-1.0.1.dist-info/entry_points.txt
+Filename: better_face-1.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: better_face-1.0.1.dist-info/top_level.txt
+Filename: better_face-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: better_face-1.0.1.dist-info/RECORD
+Filename: better_face-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## betterface/interface.py

```diff
@@ -79,30 +79,36 @@
         tile_pad=10,
         pre_pad=0,
         half=half,
         gpu_id=0)
 
 
 def select_face_enhancer(version, scale, upsampler):
+    device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+
     if 'v1.2' in version:
         model_path = download_model_gfpgan('GFPGANv1.2.pth')
         return GFPGANer(
-            model_path=model_path, upscale=scale, arch='clean', channel_multiplier=2, bg_upsampler=upsampler)
+            model_path=model_path, upscale=scale, arch='clean',
+            channel_multiplier=2, bg_upsampler=upsampler, device=device)
     elif 'v1.3' in version:
         model_path = download_model_gfpgan('GFPGANv1.3.pth')
         return GFPGANer(
-            model_path=model_path, upscale=scale, arch='clean', channel_multiplier=2, bg_upsampler=upsampler)
+            model_path=model_path, upscale=scale, arch='clean',
+            channel_multiplier=2, bg_upsampler=upsampler, device=device)
     elif 'v1.4' in version:
         model_path = download_model_gfpgan('GFPGANv1.4.pth')
         return GFPGANer(
-            model_path=model_path, upscale=scale, arch='clean', channel_multiplier=2, bg_upsampler=upsampler)
+            model_path=model_path, upscale=scale, arch='clean',
+            channel_multiplier=2, bg_upsampler=upsampler, device=device)
     elif 'RestoreFormer' in version:
         model_path = download_model_gfpgan('RestoreFormer.pth')
         return GFPGANer(
-            model_path=model_path, upscale=scale, arch='RestoreFormer', channel_multiplier=2, bg_upsampler=upsampler)
+            model_path=model_path, upscale=scale, arch='RestoreFormer',
+            channel_multiplier=2, bg_upsampler=upsampler, device=device)
 
 
 def predict(image, version_upsampler, version_enhancer, scale):
     scale = int(scale)
 
     upsampler = select_upsampler(version_upsampler)
```

## Comparing `better_face-1.0.1.dist-info/METADATA` & `better_face-1.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: better-face
-Version: 1.0.1
+Version: 1.0.2
 Summary: General image  and face restoration
 Home-page: https://github.com/leonelhs
 Author: Leonel Hernandez
 Author-email: leonelhs@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

## Comparing `better_face-1.0.1.dist-info/RECORD` & `better_face-1.0.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 betterface/__init__.py,sha256=Be6dKroLZh0X6LgaBIJQrzJAg1K6MnLj2jhUbkFH5DI,28
 betterface/__main__.py,sha256=Wua2SXNjPjsx3gUt3KGf2wwN_y6Wk1O_GS6eb7F2Jck,71
-betterface/interface.py,sha256=j0RiPil6tewLcN7Icd7I-OORHEu6OFy9e0q4w2SyCWk,5963
-better_face-1.0.1.dist-info/METADATA,sha256=PThFAYZJJPJkQMEzcfsQCePJfJVjFjNC5ZsBOGxEnAk,903
-better_face-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-better_face-1.0.1.dist-info/entry_points.txt,sha256=FvbD28ZN661smV_7mk5d4o-5J6XFuvEjgEZre9lzVIU,56
-better_face-1.0.1.dist-info/top_level.txt,sha256=u40NbiHm-DmI-y2tkwbTlLZ9uICKPGxxNGnNOd-KenQ,11
-better_face-1.0.1.dist-info/RECORD,,
+betterface/interface.py,sha256=Si6c4W7ahv8nprcgXjtO-kmgSbg-CZ6Y_zenJF4Zvy8,6146
+better_face-1.0.2.dist-info/METADATA,sha256=1-2tWKhuCzHSNy3pMwA_7ww2BHxHBa2Hc-S0tyY3fb4,903
+better_face-1.0.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+better_face-1.0.2.dist-info/entry_points.txt,sha256=FvbD28ZN661smV_7mk5d4o-5J6XFuvEjgEZre9lzVIU,56
+better_face-1.0.2.dist-info/top_level.txt,sha256=u40NbiHm-DmI-y2tkwbTlLZ9uICKPGxxNGnNOd-KenQ,11
+better_face-1.0.2.dist-info/RECORD,,
```

