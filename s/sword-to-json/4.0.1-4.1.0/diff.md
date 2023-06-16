# Comparing `tmp/sword_to_json-4.0.1.tar.gz` & `tmp/sword_to_json-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sword_to_json-4.0.1.tar", max compression
+gzip compressed data, was "sword_to_json-4.1.0.tar", max compression
```

## Comparing `sword_to_json-4.0.1.tar` & `sword_to_json-4.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1794 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/README.md
--rw-r--r--   0        0        0      768 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/__init__.py
--rw-r--r--   0        0        0      875 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/__main__.py
--rw-r--r--   0        0        0     1344 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/books_from_sword.py
--rw-r--r--   0        0        0        0 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/__init__.py
--rw-r--r--   0        0        0      207 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/metadata.py
--rw-r--r--   0        0        0      498 2023-05-31 07:57:24.173336 sword_to_json-4.0.1/sword_to_json/utils/progress.py
--rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 sword_to_json-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1794 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/README.md
+-rw-r--r--   0        0        0      768 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/__init__.py
+-rw-r--r--   0        0        0     1217 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/__main__.py
+-rw-r--r--   0        0        0     1349 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/books_from_sword.py
+-rw-r--r--   0        0        0        0 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/utils/__init__.py
+-rw-r--r--   0        0        0      207 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/utils/metadata.py
+-rw-r--r--   0        0        0      717 2023-06-16 08:51:24.158869 sword_to_json-4.1.0/sword_to_json/utils/progress.py
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 sword_to_json-4.1.0/PKG-INFO
```

### Comparing `sword_to_json-4.0.1/README.md` & `sword_to_json-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sword_to_json-4.0.1/pyproject.toml` & `sword_to_json-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sword-to-json"
-version = "4.0.1"
+version = "4.1.0"
 description = "Generate JSON Files of Bible Translations from SWORD Modules"
 license = "GPL-3.0-or-later"
 authors = ["Evans <evans@fundi.dev>"]
 readme = "README.md"
 homepage = "https://github.com/evnskc/sword-to-json"
 repository = "https://github.com/evnskc/sword-to-json"
 documentation = "https://github.com/evnskc/sword-to-json"
```

### Comparing `sword_to_json-4.0.1/sword_to_json/books_from_sword.py` & `sword_to_json-4.1.0/sword_to_json/books_from_sword.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,32 +8,31 @@
     modules.parse_modules()
     bible = modules.get_bible_from_module(module)
 
     book_structure = bible.get_structure().get_books()
 
     books = {}
 
-    progress = Progress(sum([len(v) for v in book_structure.values()]))
-
     for testament, testament_books in book_structure.items():
         books[testament] = []
         for number, book in enumerate(testament_books, start=sum([len(v) for v in books.values()]) + 1):
-            books[testament].append({
+            progress = Progress(book.name, book.num_chapters)
+            _book = {
                 "number": number,
                 "name": book.name,
                 "abbreviation": book.preferred_abbreviation,
-                "chapters": [
-                    {
-                        "number": chapter,
-                        "verses": [
-                            {
-                                "number": verse,
-                                "text": bible.get(books=book.name, chapters=chapter, verses=verse).rstrip()
-                            } for verse in range(1, book.chapter_lengths[chapter - 1] + 1)
-                        ]
-                    } for chapter in range(1, book.num_chapters + 1)
-                ]
-            })
-
-            progress.update(number)
+                "chapters": []
+            }
+            for chapter in range(1, book.num_chapters + 1):
+                _book["chapters"].append({
+                    "number": chapter,
+                    "verses": [
+                        {
+                            "number": verse,
+                            "text": bible.get(books=book.name, chapters=chapter, verses=verse).rstrip()
+                        } for verse in range(1, book.chapter_lengths[chapter - 1] + 1)
+                    ]
+                })
+                progress.update(chapter)
+            books[testament].append(_book)
 
     return books
```

### Comparing `sword_to_json-4.0.1/PKG-INFO` & `sword_to_json-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sword-to-json
-Version: 4.0.1
+Version: 4.1.0
 Summary: Generate JSON Files of Bible Translations from SWORD Modules
 Home-page: https://github.com/evnskc/sword-to-json
 License: GPL-3.0-or-later
 Keywords: sword,bible text,json
 Author: Evans
 Author-email: evans@fundi.dev
 Requires-Python: >=3.11,<4.0
```

