# Comparing `tmp/slidesgen-0.2.tar.gz` & `tmp/slidesgen-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidesgen-0.2.tar", last modified: Sat Apr  1 13:12:09 2023, max compression
+gzip compressed data, was "slidesgen-0.3.tar", last modified: Fri Jun 16 03:46:53 2023, max compression
```

## Comparing `slidesgen-0.2.tar` & `slidesgen-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-01 13:12:09.180445 slidesgen-0.2/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      130 2023-04-01 13:12:09.179943 slidesgen-0.2/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      703 2022-12-18 01:17:43.000000 slidesgen-0.2/README.md
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-04-01 13:12:09.180621 slidesgen-0.2/setup.cfg
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      448 2023-04-01 13:11:18.000000 slidesgen-0.2/setup.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-01 13:12:09.172004 slidesgen-0.2/slidesgen/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       73 2022-12-17 04:41:31.000000 slidesgen-0.2/slidesgen/__init__.py
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)   579182 2023-04-01 13:11:18.000000 slidesgen-0.2/slidesgen/slidesgen.py
-drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-04-01 13:12:09.179121 slidesgen-0.2/slidesgen.egg-info/
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      130 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/PKG-INFO
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)      263 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/SOURCES.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/dependency_links.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       45 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/entry_points.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       15 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/requires.txt
--rw-r--r--   0 junqiang.zhang   (510) staff       (20)       10 2023-04-01 13:12:09.000000 slidesgen-0.2/slidesgen.egg-info/top_level.txt
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-06-16 03:46:53.962243 slidesgen-0.3/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      130 2023-06-16 03:46:53.961229 slidesgen-0.3/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      703 2022-12-18 01:17:43.000000 slidesgen-0.3/README.md
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       38 2023-06-16 03:46:53.962704 slidesgen-0.3/setup.cfg
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      448 2023-06-16 03:46:08.000000 slidesgen-0.3/setup.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-06-16 03:46:53.951369 slidesgen-0.3/slidesgen/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       73 2022-12-17 04:41:31.000000 slidesgen-0.3/slidesgen/__init__.py
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)   579456 2023-06-16 03:46:08.000000 slidesgen-0.3/slidesgen/slidesgen.py
+drwxr-xr-x   0 junqiang.zhang   (510) staff       (20)        0 2023-06-16 03:46:53.960344 slidesgen-0.3/slidesgen.egg-info/
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      130 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/PKG-INFO
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)      263 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/SOURCES.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)        1 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/dependency_links.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       45 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/entry_points.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       15 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/requires.txt
+-rw-r--r--   0 junqiang.zhang   (510) staff       (20)       10 2023-06-16 03:46:53.000000 slidesgen-0.3/slidesgen.egg-info/top_level.txt
```

### Comparing `slidesgen-0.2/README.md` & `slidesgen-0.3/README.md`

 * *Files identical despite different names*

### Comparing `slidesgen-0.2/slidesgen/slidesgen.py` & `slidesgen-0.3/slidesgen/slidesgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import base64
 
 
 pattern_slides = re.compile(r'^[\-]{3,}\n|<![\-]{4,}>', re.MULTILINE)
 
 pattern_section_raw = re.compile(r"```section([\s\S]+?)```|```([\s\S]+?)```", re.MULTILINE)
 
-pattern_images = re.compile(r"!\[.*?\]\((.*?)\)", re.MULTILINE)
+pattern_images = re.compile(r'!\[.*?\]\((.*?)\)|data-background-image="([^"]+?)"', re.MULTILINE)
 
 pattern_comments = re.compile(r'<!--[\s\S]+?-->', re.MULTILINE)
 pattern_scripts_src = re.compile(r'<script src="(.+?)"></script>', re.MULTILINE)
 pattern_css_href = re.compile(r'<link[\s\S]+?href="(.*)?">', re.MULTILINE)
 pattern_reveal_initialization = re.compile(r'<!--revealjs([\s\S]*?)-->', re.MULTILINE)
 
 style_map = {'global': '', 'preview': ''}
@@ -265,15 +265,18 @@
         comment = get_comment(slide)
         options = get_slide_options_from_comment(comment)
         options = options.strip()
 
         if images:
 
             try:
-                rsp=requests.get(images[0])
+                if len(images)>0 and len(images[0])>0 and images[0][0].startswith('http'):
+                    rsp=requests.get(images[0][0])
+                if len(images)>0 and len(images[0])>1  and images[0][1].startswith('http'):
+                    rsp=requests.get(images[0][1])
                 img64=base64.b64encode( rsp.content)
                 options=options+' data-background-image="data:image/png;base64,'+img64.decode()+'"'+ ' data-background-opacity="'+transparency+'" '
 
             except Exception as  er:
                 print(er)
 
         # if options!='':
```

