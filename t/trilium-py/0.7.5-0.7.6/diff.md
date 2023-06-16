# Comparing `tmp/trilium_py-0.7.5-py3-none-any.whl.zip` & `tmp/trilium_py-0.7.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 27426 bytes, number of entries: 12
+Zip file size: 27592 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      141 b- defN 23-Apr-04 07:07 trilium_py/__init__.py
--rw-r--r--  2.0 unx    30967 b- defN 23-May-06 05:44 trilium_py/client.py
+-rw-r--r--  2.0 unx    31298 b- defN 23-Jun-16 08:33 trilium_py/client.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-04 07:07 trilium_py/utils/__init__.py
 -rw-r--r--  2.0 unx     8656 b- defN 23-Apr-04 07:07 trilium_py/utils/markdown_math.py
 -rw-r--r--  2.0 unx      675 b- defN 23-Apr-04 07:07 trilium_py/utils/param_util.py
 -rw-r--r--  2.0 unx      208 b- defN 23-Apr-04 07:07 trilium_py/utils/time_util.py
 -rw-r--r--  2.0 unx      470 b- defN 23-Apr-04 07:07 trilium_py/utils/url_util.py
--rwxrwx---  2.0 unx    35184 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    10488 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      990 b- defN 23-May-06 05:53 trilium_py-0.7.5.dist-info/RECORD
-12 files, 87882 bytes uncompressed, 25756 bytes compressed:  70.7%
+-rwxrwx---  2.0 unx    35184 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    11024 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Jun-16 08:49 trilium_py-0.7.6.dist-info/RECORD
+12 files, 88749 bytes uncompressed, 25922 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: trilium_py/utils/time_util.py
 Comment: 
 
 Filename: trilium_py/utils/url_util.py
 Comment: 
 
-Filename: trilium_py-0.7.5.dist-info/LICENSE.txt
+Filename: trilium_py-0.7.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: trilium_py-0.7.5.dist-info/METADATA
+Filename: trilium_py-0.7.6.dist-info/METADATA
 Comment: 
 
-Filename: trilium_py-0.7.5.dist-info/WHEEL
+Filename: trilium_py-0.7.6.dist-info/WHEEL
 Comment: 
 
-Filename: trilium_py-0.7.5.dist-info/top_level.txt
+Filename: trilium_py-0.7.6.dist-info/top_level.txt
 Comment: 
 
-Filename: trilium_py-0.7.5.dist-info/RECORD
+Filename: trilium_py-0.7.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## trilium_py/client.py

```diff
@@ -4,17 +4,18 @@
 
 import magic
 import markdown2
 import requests
 from bs4 import BeautifulSoup
 from natsort import natsort
 
+from .utils.markdown_math import sanitizeInput, reconstructMath
 from .utils.param_util import format_query_string, clean_param
 from .utils.time_util import get_yesterday, get_today
-from .utils.markdown_math import sanitizeInput, reconstructMath
+
 
 class ETAPI:
 
     def __init__(self, server_url: str, token: str = None):
         self.server_url = server_url
         self.token = token
 
@@ -128,15 +129,15 @@
             "isExpanded": isExpanded,
             "noteId": noteId,
             "branchId": branchId
         }
         res = requests.post(url, json=clean_param(params), headers=self.get_header())
 
         return res.json()
-    
+
     def create_file_note(self, parentNoteId: str, title: str, file_data: str, content_file: str,
                          type: str = 'file', mime: str = None,
                          content=None, notePosition: int = None, prefix: str = None,
                          isExpanded: str = None, noteId: str = None,
                          branchId: str = None):
         '''
         Create a note
@@ -679,25 +680,26 @@
         # convert md to html
         with open(md_file, 'r', encoding='utf-8') as f:
             content = f.read()
 
             # fix logseq image size format
             logseq_image_pat = r'(\!\[.*\]\(.*\))\{.*?:height.*width.*}'
             content = re.sub(logseq_image_pat, r'\1', content)
-            
-            if not re.search(re.escape("$"),content):
+
+            if not re.search(re.escape("$"), content):
                 # extra format support
                 # https://github.com/trentm/python-markdown2/wiki/Extras
                 html = markdown2.markdown(content, extras=['fenced-code-blocks', 'strike', 'tables', 'task_list'])
                 # print(html)
             else:
                 no_latex_part, latex_code_part = sanitizeInput(content)
-                html = reconstructMath(markdown2.markdown(no_latex_part, 
-                                                          extras=['fenced-code-blocks', 'strike', 'tables', 'task_list']),
-                                      latex_code_part)
+                html = reconstructMath(markdown2.markdown(no_latex_part,
+                                                          extras=['fenced-code-blocks', 'strike', 'tables',
+                                                                  'task_list']),
+                                       latex_code_part)
 
         # detect images
         pat = '<img (.*?) />'
         images = re.findall(pat, html)
 
         if not images:
             res = self.create_note(
@@ -839,7 +841,16 @@
                         type="text",
                         content=name,
                     )
                     res['note']['noteId']
                     note_tree[rel_path] = res['note']['noteId']
 
         return True
+
+    def backup(self, backup_name):
+        url = f'{self.server_url}/etapi/backup/{backup_name}'
+
+        res = requests.put(url, headers=self.get_header())
+        if res.status_code == 204:
+            print('backup successfully')
+            return True
+        return False
```

## Comparing `trilium_py-0.7.5.dist-info/LICENSE.txt` & `trilium_py-0.7.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `trilium_py-0.7.5.dist-info/METADATA` & `trilium_py-0.7.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trilium-py
-Version: 0.7.5
+Version: 0.7.6
 Summary: Python client for ETAPI of Trilium Note. With some extra features powered by Python :)
 Home-page: https://github.com/nriver/trilium-py
 Author: Nriver
 Author-email: 
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues
 Project-URL: Funding, https://github.com/nriver/trilium-py
 Project-URL: Say Thanks!, https://github.com/nriver/trilium-py
@@ -49,38 +49,40 @@
 
 <!--ts-->
 
 - [🐍 trilium-py](#-trilium-py)
 - [🦮 Table of Contents](#-table-of-contents)
 - [🔧 Installation](#-installation)
 - [📖 (Basic) Usage](#-basic-usage)
-  - [🚀 Initialization](#-initialization)
-  - [📊 Application Information](#-application-information)
-  - [🔍 Search note](#-search-note)
-  - [🏭 Create Note](#-create-note)
-    - [🖼️ Create Image note](#️-create-image-note)
-  - [👀 Get note](#-get-note)
-  - [🔄 Update note](#-update-note)
-  - [🗑️ Delete note](#️-delete-note)
-  - [📅 Day note](#-day-note)
-  - [📤 Export note](#-export-note)
+    - [🚀 Initialization](#-initialization)
+    - [📊 Application Information](#-application-information)
+    - [🔍 Search note](#-search-note)
+    - [🏭 Create Note](#-create-note)
+        - [🖼️ Create Image note](#️-create-image-note)
+    - [👀 Get note](#-get-note)
+    - [🔄 Update note](#-update-note)
+    - [🗑️ Delete note](#️-delete-note)
+    - [📅 Day note](#-day-note)
+    - [📤 Export note](#-export-note)
+    - [💾Create data backup](#-create-data-backup)
 - [(Advanced Usage) ✅ TODO List](#advanced-usage--todo-list)
-  - [Add TODO item](#add-todo-item)
-  - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
-  - [Update a TODO item](#update-a-todo-item)
-  - [Delete a TDOO item](#delete-a-tdoo-item)
-  - [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
+    - [Add TODO item](#add-todo-item)
+    - [Check/Uncheck a TODO item](#checkuncheck-a-todo-item)
+    - [Update a TODO item](#update-a-todo-item)
+    - [Delete a TDOO item](#delete-a-tdoo-item)
+    - [Move yesterday's unfinished todo to today](#move-yesterdays-unfinished-todo-to-today)
 - [(Advanced Usage) 🚚 Upload Markdown files](#advanced-usage--upload-markdown-files)
-  - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
-  - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
-    - [Import from VNote](#import-from-vnote)
-    - [Import from Logseq](#import-from-logseq)
-    - [Import from Obsidian](#import-from-obsidian)
-    - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
-    - [Import from other markdown software](#import-from-other-markdown-software)
+    - [Upload single Markdown file with images](#upload-single-markdown-file-with-images)
+    - [Bulk upload Markdown files in a folder](#bulk-upload-markdown-files-in-a-folder)
+        - [Import from VNote](#import-from-vnote)
+        - [Import from Joplin](#import-from-joplin)
+        - [Import from Logseq](#import-from-logseq)
+        - [Import from Obsidian](#import-from-obsidian)
+        - [Import from Youdao Note/有道云笔记](#import-from-youdao-note有道云笔记)
+        - [Import from other markdown software](#import-from-other-markdown-software)
 - [🛠️ Develop](#️-develop)
 - [🔗 Original OpenAPI Documentation](#-original-openapi-documentation)
 
 <!--te-->
 
 # 🔧 Installation
 
@@ -237,14 +239,22 @@
 res = ea.export_note(
     noteId='sK5fn4T6yZRI',
     format='md',
     savePath='/home/nate/data/1/test.zip',
 )
 ```
 
+## 💾 Create data backup
+
+This example will create a database backup file like this `trilium-data/backup/backup-test.db`.
+
+```python
+res = ea.backup("test")
+```
+
 # (Advanced Usage) ✅ TODO List
 
 With the power of Python, I have expanded the basic usage of ETAPI. You can do something with todo list now.
 
 ## Add TODO item
 
 You can use `add_todo` to add a TODO item, param is the TODO description
@@ -313,14 +323,26 @@
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="~/data/vnotebook/",
     ignoreFolder=['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'],
 )
 ```
 
+### Import from Joplin
+
+Joplin can be imported effortlessly.
+
+```python
+res = ea.upload_md_folder(
+    parentNoteId="root",
+    mdFolder="/home/nate/data/joplin_data/",
+    ignoreFolder=['_resources', ],
+)
+```
+
 ### Import from Logseq
 
 ```python
 res = ea.upload_md_folder(
     parentNoteId="root",
     mdFolder="/home/nate/data/logseq_data/",
     ignoreFolder=['assets', 'logseq'],
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trilium-py Version: 0.7.5 Summary: Python client
+Metadata-Version: 2.1 Name: trilium-py Version: 0.7.6 Summary: Python client
 for ETAPI of Trilium Note. With some extra features powered by Python :) Home-
 page: https://github.com/nriver/trilium-py Author: Nriver Author-email:
 Project-URL: Bug Reports, https://github.com/nriver/trilium-py/issues Project-
 URL: Funding, https://github.com/nriver/trilium-py Project-URL: Say Thanks!,
 https://github.com/nriver/trilium-py Project-URL: Source, https://github.com/
 nriver/trilium-py/ Keywords: trilium,etapi,api client Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
@@ -31,25 +31,26 @@
 # ð¦® Table of Contents  - [ð trilium-py](#-trilium-py) - [ð¦® Table of
 Contents](#-table-of-contents) - [ð§ Installation](#-installation) - [ð
 (Basic) Usage](#-basic-usage) - [ð Initialization](#-initialization) - [ð
 Application Information](#-application-information) - [ð Search note](#-
 search-note) - [ð­ Create Note](#-create-note) - [ð¼ï¸ Create Image note]
 (#ï¸-create-image-note) - [ð Get note](#-get-note) - [ð Update note](#-
 update-note) - [ðï¸ Delete note](#ï¸-delete-note) - [ð Day note](#-day-
-note) - [ð¤ Export note](#-export-note) - [(Advanced Usage) â TODO List]
-(#advanced-usage--todo-list) - [Add TODO item](#add-todo-item) - [Check/Uncheck
-a TODO item](#checkuncheck-a-todo-item) - [Update a TODO item](#update-a-todo-
-item) - [Delete a TDOO item](#delete-a-tdoo-item) - [Move yesterday's
-unfinished todo to today](#move-yesterdays-unfinished-todo-to-today) - [
-(Advanced Usage) ð Upload Markdown files](#advanced-usage--upload-markdown-
-files) - [Upload single Markdown file with images](#upload-single-markdown-
-file-with-images) - [Bulk upload Markdown files in a folder](#bulk-upload-
-markdown-files-in-a-folder) - [Import from VNote](#import-from-vnote) - [Import
-from Logseq](#import-from-logseq) - [Import from Obsidian](#import-from-
-obsidian) - [Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
+note) - [ð¤ Export note](#-export-note) - [ð¾Create data backup](#-create-
+data-backup) - [(Advanced Usage) â TODO List](#advanced-usage--todo-list) -
+[Add TODO item](#add-todo-item) - [Check/Uncheck a TODO item](#checkuncheck-a-
+todo-item) - [Update a TODO item](#update-a-todo-item) - [Delete a TDOO item]
+(#delete-a-tdoo-item) - [Move yesterday's unfinished todo to today](#move-
+yesterdays-unfinished-todo-to-today) - [(Advanced Usage) ð Upload Markdown
+files](#advanced-usage--upload-markdown-files) - [Upload single Markdown file
+with images](#upload-single-markdown-file-with-images) - [Bulk upload Markdown
+files in a folder](#bulk-upload-markdown-files-in-a-folder) - [Import from
+VNote](#import-from-vnote) - [Import from Joplin](#import-from-joplin) -
+[Import from Logseq](#import-from-logseq) - [Import from Obsidian](#import-
+from-obsidian) - [Import from Youdao Note/æéäºç¬è®°](#import-from-youdao-
 noteæéäºç¬è®°) - [Import from other markdown software](#import-from-
 other-markdown-software) - [ð ï¸ Develop](#ï¸-develop) - [ð Original
 OpenAPI Documentation](#-original-openapi-documentation)  # ð§ Installation
 ```bash python3 -m pip install trilium-py --user ``` # ð (Basic) Usage These
 are basic function that Trilium's ETAPI provides. Down below are some simple
 example code to use this package. ## ð Initialization If you have a ETAPI
 token, change the `server_url` and `token` to yours. ```python from
@@ -83,46 +84,51 @@
 note You can get the content of a certain date with `get_day_note`. The date
 string should be in format of "%Y-%m-%d", e.g. " 2022-02-25". ```python
 es.get_day_note("2022-02-25") ``` Then set/update a day note with
 `set_day_note`. The content should be a (html) string. ```python
 self.set_day_note(date, new_content) ``` ## ð¤ Export note Export note comes
 in two formats `html` or `markdown`/`md`. ```python res = ea.export_note
 ( noteId='sK5fn4T6yZRI', format='md', savePath='/home/nate/data/1/test.zip', )
-``` # (Advanced Usage) â TODO List With the power of Python, I have expanded
-the basic usage of ETAPI. You can do something with todo list now. ## Add TODO
-item You can use `add_todo` to add a TODO item, param is the TODO description
-```python ea.add_todo("ä¹°æå®å®") ``` ## Check/Uncheck a TODO item param is
-the index of the TODO item ```python ea.todo_check(0) ea.todo_uncheck(1) ``` ##
-Update a TODO item Use `update_todo` to update a TODO item description at
-certain index. ```python ea.update_todo(0, "å»ç å¤´æ´ç¹è¯æ¡") ``` ##
-Delete a TDOO item Remove a TODO item by its index. ```python ea.delete_todo(1)
-``` ## Move yesterday's unfinished todo to today As the title suggests, you can
-move yesterday's unfinished things to today. Unfinished todos will be deleted
-from yesterday's note. ```python ea.move_yesterday_unfinished_todo_to_today()
-``` # (Advanced Usage) ð Upload Markdown files ## Upload single Markdown
-file with images You can import Markdown file with images into Trilium now!
-Trilium-py will help you to upload the images and fix the links for you!
-```python res = ea.upload_md_file( parentNoteId="root", file="./md-demo/manjaro
-ä¿®æ¹caps lock.md", ) ``` ## Bulk upload Markdown files in a folder You can
-upload a folder with lots of Markdown files to Trilium and preserve the folder
-structure! ### Import from VNote Say, upload all the notes from [VNote](https:/
-/github.com/vnotex/vnote), simply do this: ```python res = ea.upload_md_folder
-( parentNoteId="root", mdFolder="~/data/vnotebook/", ignoreFolder=
-['vx_notebook', 'vx_recycle_bin', 'vx_images', '_v_images'], ) ``` ### Import
-from Logseq ```python res = ea.upload_md_folder( parentNoteId="root",
-mdFolder="/home/nate/data/logseq_data/", ignoreFolder=['assets', 'logseq'], )
-``` ### Import from Obsidian Obsidian has a very unique linking system for
-files. You should use [obsidian-export ](https://github.com/zoni/obsidian-
-export) to convert a Obsidian vault to regular Markdown files. Then you should
-be able to import the note into Trilium with trilium-py. Convert it first.
-```bash obsidian-export /path/to/your/vault /out ``` Then import just like a
-normal markdown, trilium-py will handle the images for you. ```python res =
-ea.upload_md_folder( parentNoteId="root", mdFolder="E:/data/out", ) ``` ###
-Import from Youdao Note/æéäºç¬è®° Youdao does not provide an export
-feature anymore. Luckily, you can use
+``` ## ð¾ Create data backup This example will create a database backup file
+like this `trilium-data/backup/backup-test.db`. ```python res = ea.backup
+("test") ``` # (Advanced Usage) â TODO List With the power of Python, I have
+expanded the basic usage of ETAPI. You can do something with todo list now. ##
+Add TODO item You can use `add_todo` to add a TODO item, param is the TODO
+description ```python ea.add_todo("ä¹°æå®å®") ``` ## Check/Uncheck a TODO
+item param is the index of the TODO item ```python ea.todo_check(0)
+ea.todo_uncheck(1) ``` ## Update a TODO item Use `update_todo` to update a TODO
+item description at certain index. ```python ea.update_todo(0,
+"å»ç å¤´æ´ç¹è¯æ¡") ``` ## Delete a TDOO item Remove a TODO item by its
+index. ```python ea.delete_todo(1) ``` ## Move yesterday's unfinished todo to
+today As the title suggests, you can move yesterday's unfinished things to
+today. Unfinished todos will be deleted from yesterday's note. ```python
+ea.move_yesterday_unfinished_todo_to_today() ``` # (Advanced Usage) ð Upload
+Markdown files ## Upload single Markdown file with images You can import
+Markdown file with images into Trilium now! Trilium-py will help you to upload
+the images and fix the links for you! ```python res = ea.upload_md_file
+( parentNoteId="root", file="./md-demo/manjaro ä¿®æ¹caps lock.md", ) ``` ##
+Bulk upload Markdown files in a folder You can upload a folder with lots of
+Markdown files to Trilium and preserve the folder structure! ### Import from
+VNote Say, upload all the notes from [VNote](https://github.com/vnotex/vnote),
+simply do this: ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="~/data/vnotebook/", ignoreFolder=['vx_notebook', 'vx_recycle_bin',
+'vx_images', '_v_images'], ) ``` ### Import from Joplin Joplin can be imported
+effortlessly. ```python res = ea.upload_md_folder( parentNoteId="root",
+mdFolder="/home/nate/data/joplin_data/", ignoreFolder=['_resources', ], ) ```
+### Import from Logseq ```python res = ea.upload_md_folder
+( parentNoteId="root", mdFolder="/home/nate/data/logseq_data/", ignoreFolder=
+['assets', 'logseq'], ) ``` ### Import from Obsidian Obsidian has a very unique
+linking system for files. You should use [obsidian-export ](https://github.com/
+zoni/obsidian-export) to convert a Obsidian vault to regular Markdown files.
+Then you should be able to import the note into Trilium with trilium-py.
+Convert it first. ```bash obsidian-export /path/to/your/vault /out ``` Then
+import just like a normal markdown, trilium-py will handle the images for you.
+```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="E:/data/
+out", ) ``` ### Import from Youdao Note/æéäºç¬è®° Youdao does not provide
+an export feature anymore. Luckily, you can use
 github.com/DeppWang/youdaonote-pull> to download your notes and convert them
 into markdown files. After that, trilium-py should be able to help you import
 them. ```python res = ea.upload_md_folder( parentNoteId="root", mdFolder="/
 home/nate/gitRepo/youdaonote-pull/out/", ) ``` ### Import from other markdown
 software In general, markdown files have variety of standards. You can always
 try import them with ```python res = ea.upload_md_folder( parentNoteId="root",
 mdFolder="/home/nate/data/your_markdown_files/", ) ``` If there is any problem,
```

## Comparing `trilium_py-0.7.5.dist-info/RECORD` & `trilium_py-0.7.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 trilium_py/__init__.py,sha256=uSMH49RW2MFU_LVKKKm6lt3xOBsDWo0cb8--nMcNlgY,141
-trilium_py/client.py,sha256=bY7OgceY6RAgdNv4VNXYoKh6yOnzmyNLvpYoNj0CEi4,30967
+trilium_py/client.py,sha256=Tb7_ozH_C5AWNINpmZyj2klxCfuutyNDZagf5pI2hGA,31298
 trilium_py/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 trilium_py/utils/markdown_math.py,sha256=ORQwEXAPtcf2-NaYKx4Pr5q5B8CtupVRYt04JD-c3EY,8656
 trilium_py/utils/param_util.py,sha256=BOiblP1F-jMgggx8L_QxCH3s8-FIdG1kAM-4ykSbZ5E,675
 trilium_py/utils/time_util.py,sha256=DIFQmCKZ_wL5lCdeTMJZAtFolZw_dic6NKZ8CCJTa1A,208
 trilium_py/utils/url_util.py,sha256=U1Qn5UFzQO-Bi9DGjq2OEiVzCi6x5KXsyRKF-AOJV64,470
-trilium_py-0.7.5.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
-trilium_py-0.7.5.dist-info/METADATA,sha256=RmEkxI8yHd-Hv5zstISOfL_Ehug_oq_58nV8mxfu2xw,10488
-trilium_py-0.7.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-trilium_py-0.7.5.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
-trilium_py-0.7.5.dist-info/RECORD,,
+trilium_py-0.7.6.dist-info/LICENSE.txt,sha256=bx5iLIKjgAdYQ7sISn7DsfHRKkoCUm1154sJJKhgqnU,35184
+trilium_py-0.7.6.dist-info/METADATA,sha256=rsBP9AAbt2thtfHGK75duLbVWSzCM8Gusxtnwes6_lQ,11024
+trilium_py-0.7.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+trilium_py-0.7.6.dist-info/top_level.txt,sha256=nm0WM9tsACU6iD5bbVQgo-LgS3xkDUFPK87VYZfaToo,11
+trilium_py-0.7.6.dist-info/RECORD,,
```

