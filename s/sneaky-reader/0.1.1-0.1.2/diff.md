# Comparing `tmp/sneaky_reader-0.1.1.tar.gz` & `tmp/sneaky_reader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaky_reader-0.1.1.tar", last modified: Fri Jun 16 10:53:43 2023, max compression
+gzip compressed data, was "sneaky_reader-0.1.2.tar", last modified: Fri Jun 16 12:24:20 2023, max compression
```

## Comparing `sneaky_reader-0.1.1.tar` & `sneaky_reader-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 10:53:43.905127 sneaky_reader-0.1.1/
--rw-r--r--   0 gus        (501) staff       (20)       45 2023-06-16 10:53:18.000000 sneaky_reader-0.1.1/MANIFEST.in
--rw-r--r--   0 gus        (501) staff       (20)     2677 2023-06-16 10:53:43.904414 sneaky_reader-0.1.1/PKG-INFO
--rw-r--r--   0 gus        (501) staff       (20)     2289 2023-06-16 10:46:58.000000 sneaky_reader-0.1.1/readme.md
--rw-r--r--   0 gus        (501) staff       (20)       38 2023-06-16 10:53:43.905393 sneaky_reader-0.1.1/setup.cfg
--rw-r--r--   0 gus        (501) staff       (20)     1246 2023-06-16 10:51:04.000000 sneaky_reader-0.1.1/setup.py
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 10:53:43.899134 sneaky_reader-0.1.1/sneaky_reader/
--rw-r--r--   0 gus        (501) staff       (20)      126 2023-06-16 10:53:29.000000 sneaky_reader-0.1.1/sneaky_reader/__init__.py
--rw-r--r--   0 gus        (501) staff       (20)       62 2023-06-16 09:23:51.000000 sneaky_reader-0.1.1/sneaky_reader/__main__.py
--rw-r--r--   0 gus        (501) staff       (20)      517 2023-06-15 08:59:02.000000 sneaky_reader-0.1.1/sneaky_reader/code_browser.css
--rw-r--r--   0 gus        (501) staff       (20)     3075 2023-06-16 10:00:07.000000 sneaky_reader-0.1.1/sneaky_reader/main.py
--rw-r--r--   0 gus        (501) staff       (20)     7445 2023-06-16 09:56:23.000000 sneaky_reader-0.1.1/sneaky_reader/reader.py
-drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 10:53:43.903046 sneaky_reader-0.1.1/sneaky_reader.egg-info/
--rw-r--r--   0 gus        (501) staff       (20)     2677 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/PKG-INFO
--rw-r--r--   0 gus        (501) staff       (20)      383 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/SOURCES.txt
--rw-r--r--   0 gus        (501) staff       (20)        1 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/dependency_links.txt
--rw-r--r--   0 gus        (501) staff       (20)       53 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/entry_points.txt
--rw-r--r--   0 gus        (501) staff       (20)        8 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/requires.txt
--rw-r--r--   0 gus        (501) staff       (20)       14 2023-06-16 10:53:43.000000 sneaky_reader-0.1.1/sneaky_reader.egg-info/top_level.txt
+drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 12:24:20.359832 sneaky_reader-0.1.2/
+-rw-r--r--   0 gus        (501) staff       (20)       45 2023-06-16 10:53:18.000000 sneaky_reader-0.1.2/MANIFEST.in
+-rw-r--r--   0 gus        (501) staff       (20)     2645 2023-06-16 12:24:20.359052 sneaky_reader-0.1.2/PKG-INFO
+-rw-r--r--   0 gus        (501) staff       (20)     2257 2023-06-16 12:21:04.000000 sneaky_reader-0.1.2/readme.md
+-rw-r--r--   0 gus        (501) staff       (20)       38 2023-06-16 12:24:20.360071 sneaky_reader-0.1.2/setup.cfg
+-rw-r--r--   0 gus        (501) staff       (20)     1246 2023-06-16 10:51:04.000000 sneaky_reader-0.1.2/setup.py
+drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 12:24:20.354044 sneaky_reader-0.1.2/sneaky_reader/
+-rw-r--r--   0 gus        (501) staff       (20)      126 2023-06-16 12:22:52.000000 sneaky_reader-0.1.2/sneaky_reader/__init__.py
+-rw-r--r--   0 gus        (501) staff       (20)       62 2023-06-16 09:23:51.000000 sneaky_reader-0.1.2/sneaky_reader/__main__.py
+-rw-r--r--   0 gus        (501) staff       (20)      517 2023-06-16 12:03:09.000000 sneaky_reader-0.1.2/sneaky_reader/code_browser.css
+-rw-r--r--   0 gus        (501) staff       (20)     3645 2023-06-16 12:17:43.000000 sneaky_reader-0.1.2/sneaky_reader/main.py
+-rw-r--r--   0 gus        (501) staff       (20)     6935 2023-06-16 12:18:19.000000 sneaky_reader-0.1.2/sneaky_reader/reader.py
+drwxr-xr-x   0 gus        (501) staff       (20)        0 2023-06-16 12:24:20.357757 sneaky_reader-0.1.2/sneaky_reader.egg-info/
+-rw-r--r--   0 gus        (501) staff       (20)     2645 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/PKG-INFO
+-rw-r--r--   0 gus        (501) staff       (20)      383 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 gus        (501) staff       (20)        1 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 gus        (501) staff       (20)       53 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/entry_points.txt
+-rw-r--r--   0 gus        (501) staff       (20)        8 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/requires.txt
+-rw-r--r--   0 gus        (501) staff       (20)       14 2023-06-16 12:24:20.000000 sneaky_reader-0.1.2/sneaky_reader.egg-info/top_level.txt
```

### Comparing `sneaky_reader-0.1.1/PKG-INFO` & `sneaky_reader-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneaky_reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: undercover book-reader in your terminal
 Home-page: https://github.com/gusye1234/sneaky-reader
 Author: JianbaiYe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,19 +15,18 @@
   <p><strong>上班看书的幻影坦克 | Hide your book under a fancy terminal</strong></p>
   <a href="https://pypi.org/project/sneaky-reader/"><img src="https://img.shields.io/pypi/v/sneaky_reader.svg"></a>
 </div>
 
 
 <div align="center">
   <div class="row" align="center">
-      <img src="./assets/en-1.png" width="32%" align="center"/>
-      <img src="./assets/en-2.png" width="32%" align="center"/>
-      <img src="./assets/en-3.png" width="32%" align="center"/>
+      <img src="./assets/en-1.png" width="40%" align="center"/>
+      👉 BOSS 👉
+      <img src="./assets/en-3.png" width="40%" align="center"/>
   </div>
-  <a align="center"> Find dickens in those images</a>
 </div>
 
 
 
 
 ## Features
 ### History saving
@@ -42,21 +41,22 @@
 ```
 ### Intuitive usage
 
 Greate thanks to the wonderful projects: [`rich`](https://github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/textual), sneaky-reader can build a (relatively) complex UI in terminal with few lines:
 
 * You can press `f` to show/hide the chapters pane
 * You can press `m`, `n` to forward/backward the current chapter
-* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet.
+* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet. *You can pass `-f <PYTHON FILE>` to use your own fake code!*
 
 ### Smart spliting
 
 Sneaky-reader supports you to use regluar expression (refer to the `re` module in python) to split your TXT into chapters. Using the command line option `-e` to pass your regluar expression. 
 
-Remember, always group your chapter name in first in your regular expression! *group the title with `()`*
+Remember, always group your chapter name in first in your regular expression!  *group the title with `(.*)`*
+
 ## Quick Start
 
 * Via `pip`: `pip install sneaky-reader`
 * Via sources: clone and enter this repo, then install with `pip install -e .`. 
 Then you have a shell command `sneaky_reader` to use!
 
 For the demo books, you could start with commands
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: sneaky_reader Version: 0.1.1 Summary: undercover
+Metadata-Version: 2.1 Name: sneaky_reader Version: 0.1.2 Summary: undercover
 book-reader in your terminal Home-page: https://github.com/gusye1234/sneaky-
 reader Author: JianbaiYe Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown
                        ****** Sneaky-Reader ð¤« ******
       ä¸ç­çä¹¦çå¹»å½±å¦å | Hide your book under a fancy terminal
                [https://img.shields.io/pypi/v/sneaky_reader.svg]
-          [./assets/en-1.png] [./assets/en-2.png] [./assets/en-3.png]
-                         Find dickens in those images
+            [./assets/en-1.png] ð BOSS ð [./assets/en-3.png]
 ## Features ### History saving Sneaky-reader implements a simple cache
 mechanism. You can use `-l` to list all the previous books, and use `-b ID` to
 quickly get the book. For example: ```shell $ sneaky_reader -l [0]
 CharlesDickens-OliverTwist [1] çº¢æ¥¼æ¢¦ $ sneaky_reader -b0 ... ``` ###
 Intuitive usage Greate thanks to the wonderful projects: [`rich`](https://
 github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/
 textual), sneaky-reader can build a (relatively) complex UI in terminal with
 few lines: * You can press `f` to show/hide the chapters pane * You can press
 `m`, `n` to forward/backward the current chapter * You can press `/` to enable
 BOSS mode! It will hide all the sneaky things and only leave a fake Python
-snippet. ### Smart spliting Sneaky-reader supports you to use regluar
-expression (refer to the `re` module in python) to split your TXT into
-chapters. Using the command line option `-e` to pass your regluar expression.
-Remember, always group your chapter name in first in your regular expression!
-*group the title with `()`* ## Quick Start * Via `pip`: `pip install sneaky-
-reader` * Via sources: clone and enter this repo, then install with `pip
-install -e .`. Then you have a shell command `sneaky_reader` to use! For the
-demo books, you could start with commands ```/shell #demo in english
-sneaky_reader -p="./assets/CharlesDickens-OliverTwist.txt" -e="^CHAPTER (.*)" #
-demo in chinese sneaky_reader -p="./assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ```
-For the first time you import a book, `sneaky_reader` will require the book
-path and the spliting expression. After that, the book will be cached and you
-can read it with command `-b ID`.
+snippet. *You can pass `-f ` to use your own fake code!* ### Smart spliting
+Sneaky-reader supports you to use regluar expression (refer to the `re` module
+in python) to split your TXT into chapters. Using the command line option `-e`
+to pass your regluar expression. Remember, always group your chapter name in
+first in your regular expression! *group the title with `(.*)`* ## Quick Start
+* Via `pip`: `pip install sneaky-reader` * Via sources: clone and enter this
+repo, then install with `pip install -e .`. Then you have a shell command
+`sneaky_reader` to use! For the demo books, you could start with commands ```/
+shell #demo in english sneaky_reader -p="./assets/CharlesDickens-
+OliverTwist.txt" -e="^CHAPTER (.*)" # demo in chinese sneaky_reader -p="./
+assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ``` For the first time you import a
+book, `sneaky_reader` will require the book path and the spliting expression.
+After that, the book will be cached and you can read it with command `-b ID`.
```

### Comparing `sneaky_reader-0.1.1/readme.md` & `sneaky_reader-0.1.2/readme.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,19 +3,18 @@
   <p><strong>上班看书的幻影坦克 | Hide your book under a fancy terminal</strong></p>
   <a href="https://pypi.org/project/sneaky-reader/"><img src="https://img.shields.io/pypi/v/sneaky_reader.svg"></a>
 </div>
 
 
 <div align="center">
   <div class="row" align="center">
-      <img src="./assets/en-1.png" width="32%" align="center"/>
-      <img src="./assets/en-2.png" width="32%" align="center"/>
-      <img src="./assets/en-3.png" width="32%" align="center"/>
+      <img src="./assets/en-1.png" width="40%" align="center"/>
+      👉 BOSS 👉
+      <img src="./assets/en-3.png" width="40%" align="center"/>
   </div>
-  <a align="center"> Find dickens in those images</a>
 </div>
 
 
 
 
 ## Features
 ### History saving
@@ -30,21 +29,22 @@
 ```
 ### Intuitive usage
 
 Greate thanks to the wonderful projects: [`rich`](https://github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/textual), sneaky-reader can build a (relatively) complex UI in terminal with few lines:
 
 * You can press `f` to show/hide the chapters pane
 * You can press `m`, `n` to forward/backward the current chapter
-* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet.
+* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet. *You can pass `-f <PYTHON FILE>` to use your own fake code!*
 
 ### Smart spliting
 
 Sneaky-reader supports you to use regluar expression (refer to the `re` module in python) to split your TXT into chapters. Using the command line option `-e` to pass your regluar expression. 
 
-Remember, always group your chapter name in first in your regular expression! *group the title with `()`*
+Remember, always group your chapter name in first in your regular expression!  *group the title with `(.*)`*
+
 ## Quick Start
 
 * Via `pip`: `pip install sneaky-reader`
 * Via sources: clone and enter this repo, then install with `pip install -e .`. 
 Then you have a shell command `sneaky_reader` to use!
 
 For the demo books, you could start with commands
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
                        ****** Sneaky-Reader ð¤« ******
       ä¸ç­çä¹¦çå¹»å½±å¦å | Hide your book under a fancy terminal
                [https://img.shields.io/pypi/v/sneaky_reader.svg]
-          [./assets/en-1.png] [./assets/en-2.png] [./assets/en-3.png]
-                         Find dickens in those images
+            [./assets/en-1.png] ð BOSS ð [./assets/en-3.png]
 ## Features ### History saving Sneaky-reader implements a simple cache
 mechanism. You can use `-l` to list all the previous books, and use `-b ID` to
 quickly get the book. For example: ```shell $ sneaky_reader -l [0]
 CharlesDickens-OliverTwist [1] çº¢æ¥¼æ¢¦ $ sneaky_reader -b0 ... ``` ###
 Intuitive usage Greate thanks to the wonderful projects: [`rich`](https://
 github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/
 textual), sneaky-reader can build a (relatively) complex UI in terminal with
 few lines: * You can press `f` to show/hide the chapters pane * You can press
 `m`, `n` to forward/backward the current chapter * You can press `/` to enable
 BOSS mode! It will hide all the sneaky things and only leave a fake Python
-snippet. ### Smart spliting Sneaky-reader supports you to use regluar
-expression (refer to the `re` module in python) to split your TXT into
-chapters. Using the command line option `-e` to pass your regluar expression.
-Remember, always group your chapter name in first in your regular expression!
-*group the title with `()`* ## Quick Start * Via `pip`: `pip install sneaky-
-reader` * Via sources: clone and enter this repo, then install with `pip
-install -e .`. Then you have a shell command `sneaky_reader` to use! For the
-demo books, you could start with commands ```/shell #demo in english
-sneaky_reader -p="./assets/CharlesDickens-OliverTwist.txt" -e="^CHAPTER (.*)" #
-demo in chinese sneaky_reader -p="./assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ```
-For the first time you import a book, `sneaky_reader` will require the book
-path and the spliting expression. After that, the book will be cached and you
-can read it with command `-b ID`.
+snippet. *You can pass `-f ` to use your own fake code!* ### Smart spliting
+Sneaky-reader supports you to use regluar expression (refer to the `re` module
+in python) to split your TXT into chapters. Using the command line option `-e`
+to pass your regluar expression. Remember, always group your chapter name in
+first in your regular expression! *group the title with `(.*)`* ## Quick Start
+* Via `pip`: `pip install sneaky-reader` * Via sources: clone and enter this
+repo, then install with `pip install -e .`. Then you have a shell command
+`sneaky_reader` to use! For the demo books, you could start with commands ```/
+shell #demo in english sneaky_reader -p="./assets/CharlesDickens-
+OliverTwist.txt" -e="^CHAPTER (.*)" # demo in chinese sneaky_reader -p="./
+assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ``` For the first time you import a
+book, `sneaky_reader` will require the book path and the spliting expression.
+After that, the book will be cached and you can read it with command `-b ID`.
```

### Comparing `sneaky_reader-0.1.1/setup.py` & `sneaky_reader-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `sneaky_reader-0.1.1/sneaky_reader/code_browser.css` & `sneaky_reader-0.1.2/sneaky_reader/code_browser.css`

 * *Files identical despite different names*

### Comparing `sneaky_reader-0.1.1/sneaky_reader/main.py` & `sneaky_reader-0.1.2/sneaky_reader/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,28 @@
                         type=str, help="Regular Expression to split your txt!")
     parser.add_argument('-l', '--list', action="store_true",
                         help="Show all cached books")
     parser.add_argument('-b', '--book', default=-1, type=int,
                         help="Pick the book from the cached list(use `-l` to look the list)")
     parser.add_argument('-r', '--reload', action="store_true",
                         help="Ignore cache")
+    parser.add_argument('-d', '--delete', default=-1, type=int,
+                        help="Delete a book cache")
+    parser.add_argument('-f', '--fake_file', default=__file__, type=str,
+                        help="Ignore cache")
     return parser.parse_args()
 
 
 def get_root_dir():
-    return os.path.dirname(os.path.dirname(__file__))
+    return os.path.expanduser("~")
 
 
 def get_cache_dir():
     root = get_root_dir()
-    cache_dir = os.path.join(root, "book_cache")
+    cache_dir = os.path.join(root, ".book_cache")
     if not os.path.exists(cache_dir):
         os.mkdir(cache_dir)
     return cache_dir
 
 
 def get_cache_path(book_path):
     parent = get_cache_dir()
@@ -58,14 +62,21 @@
         print(f"[{i}] {b}")
 
 def main():
     args = commandline()
     if args.list:
         print_cache_name()
         exit()
+    if args.delete != -1:
+        book_paths = get_cache_books()
+        assert 0 <= args.delete <= len(
+            book_paths), f"Wrong index for book, expected in [0, {len(book_paths)}]"
+        cache_path = book_paths[args.delete]
+        os.remove(cache_path)
+        exit()
     if args.book != -1:
         book_paths = get_cache_books()
         assert 0 <= args.book <= len(
             book_paths), f"Wrong index for book, expected in [0, {len(book_paths)}]"
         cache_path = book_paths[args.book]
     else:
         assert args.path != "", "Must input your book path"
@@ -81,10 +92,11 @@
             with open(cache_path, 'rb') as f:
                 file_name = pickle.load(f)["txt"]
             raise FileNotFoundError(
                 f"Expect a TXT file in {file_name}, but found none!")
     else:
         if args.re == "":
             raise ValueError("Import a new book must set your `-e`")
-        abs_path = os.path.abspath(args.path)
+        abs_path = os.path.expanduser(args.path)
+        abs_path = os.path.abspath(abs_path)
         reader = Reader(abs_path, args.re)
-    TxtBrowser(reader=reader, save_path=cache_path).run()
+    TxtBrowser(reader=reader, save_path=cache_path, fake_file=args.fake_file).run()
```

### Comparing `sneaky_reader-0.1.1/sneaky_reader/reader.py` & `sneaky_reader-0.1.2/sneaky_reader/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,46 +10,14 @@
 from textual import events
 from textual.app import App, CSSPathType, ComposeResult
 from textual.containers import Container, VerticalScroll
 from textual.driver import Driver
 from textual.reactive import var
 from textual.widgets import DirectoryTree, Footer, Header, Static, ListItem, Label, TextLog, LoadingIndicator, OptionList
 
-FAKE_CODE = '''\
-def loop_first_last(values: Iterable[T]) -> Iterable[tuple[bool, bool, T]]:
-    """Iterate and generate a tuple with a flag for first and last value."""
-    iter_values = iter(values)
-    try:
-        previous_value = next(iter_values)
-    except StopIteration:
-        return
-    first = True
-    for value in iter_values:
-        yield first, False, previous_value
-        first = False
-        previous_value = value
-    yield first, True, previous_value
-
-class Reader:
-    def __init__(self, txt, split_term):
-        self._txt = txt
-        with open(txt) as f:
-            self.content = list(f.readlines())
-        self.split_term = re.compile(split_term)
-        self.history = 0
-        self.find_chapters()
-    def find_chapters(self):
-        lines = []
-        names = []
-        for i, l in enumerate(self.content):
-            if re.match(self.split_term, l):
-                lines.append(i)
-'''
-
-
 class Reader:
     def __init__(self, txt, split_term, history_cache=0):
         self._txt = txt
         with open(txt) as f:
             self.content = list(f.readlines())
         self.split_term = re.compile(split_term)
         self.history = history_cache
@@ -113,44 +81,53 @@
         ("m", "forward_chapter", "Forward"),
         ("n", "backward_chapter", "Backward"),
         ("/", "switch", "Switch"),
     ]
 
     show_tree = var(True)
     current_index = var(0)
-    boss_mode = var(True)
+    boss_mode = var(False)
 
     def __init__(self, *args, **kwargs):
         reader = kwargs.pop("reader", None)
         if reader is None:
             raise ValueError("Must input your reader")
         self.reader = reader
         self.save_path = kwargs.pop("save_path", "./default.pkl")
+        fake_file = kwargs.pop("fake_file", None)
+        with open(fake_file) as f:
+            fake_code = "".join(f.readlines())
+        self.fake_code = Syntax(fake_code, "python")
         super().__init__(*args, **kwargs)
 
     def watch_show_tree(self, show_tree: bool) -> None:
         """Called when show_tree is modified."""
         self.set_class(show_tree, "-show-tree")
         self.query_one(Footer).visible = show_tree
 
     def watch_boss_mode(self, boss_mode: bool) -> None:
         """Called when show_tree is modified."""
-        if not boss_mode:
+        if boss_mode:
             self.show_tree = False
-        self.query_one("#code-view", VerticalScroll).visible = boss_mode
+            self.query_one("#fake-code", Static).visible = True
+            self.query_one("#fake-code", Static).update(self.fake_code)
+        else:
+            self.query_one("#fake-code", Static).update("")
+            self.query_one("#fake-code", Static).visible = False
+        self.query_one("#code-view", VerticalScroll).visible = not boss_mode
 
     def watch_current_index(self, current_index):
         # self.query_one(ListView).index = current_index
         self.query_one(OptionList).highlighted = current_index
 
     def compose(self) -> ComposeResult:
         """Compose our UI."""
         with Container():
             yield OptionList(*self.reader.ch_names, id="tree-view")
-            yield Static(Syntax(FAKE_CODE, "python"), expand=True, id="fake-code")
+            yield Static(id="fake-code")
             with VerticalScroll(id="code-view"):
                 yield Static(id="code", expand=True)
                 # yield TextLog(highlight=True, markup=True, id="code")
         yield Footer()
 
     def on_mount(self, event: events.Mount) -> None:
         self.current_index = self.reader.history
```

### Comparing `sneaky_reader-0.1.1/sneaky_reader.egg-info/PKG-INFO` & `sneaky_reader-0.1.2/sneaky_reader.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sneaky-reader
-Version: 0.1.1
+Version: 0.1.2
 Summary: undercover book-reader in your terminal
 Home-page: https://github.com/gusye1234/sneaky-reader
 Author: JianbaiYe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -15,19 +15,18 @@
   <p><strong>上班看书的幻影坦克 | Hide your book under a fancy terminal</strong></p>
   <a href="https://pypi.org/project/sneaky-reader/"><img src="https://img.shields.io/pypi/v/sneaky_reader.svg"></a>
 </div>
 
 
 <div align="center">
   <div class="row" align="center">
-      <img src="./assets/en-1.png" width="32%" align="center"/>
-      <img src="./assets/en-2.png" width="32%" align="center"/>
-      <img src="./assets/en-3.png" width="32%" align="center"/>
+      <img src="./assets/en-1.png" width="40%" align="center"/>
+      👉 BOSS 👉
+      <img src="./assets/en-3.png" width="40%" align="center"/>
   </div>
-  <a align="center"> Find dickens in those images</a>
 </div>
 
 
 
 
 ## Features
 ### History saving
@@ -42,21 +41,22 @@
 ```
 ### Intuitive usage
 
 Greate thanks to the wonderful projects: [`rich`](https://github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/textual), sneaky-reader can build a (relatively) complex UI in terminal with few lines:
 
 * You can press `f` to show/hide the chapters pane
 * You can press `m`, `n` to forward/backward the current chapter
-* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet.
+* You can press `/` to enable BOSS mode! It will hide all the sneaky things and only leave a fake Python snippet. *You can pass `-f <PYTHON FILE>` to use your own fake code!*
 
 ### Smart spliting
 
 Sneaky-reader supports you to use regluar expression (refer to the `re` module in python) to split your TXT into chapters. Using the command line option `-e` to pass your regluar expression. 
 
-Remember, always group your chapter name in first in your regular expression! *group the title with `()`*
+Remember, always group your chapter name in first in your regular expression!  *group the title with `(.*)`*
+
 ## Quick Start
 
 * Via `pip`: `pip install sneaky-reader`
 * Via sources: clone and enter this repo, then install with `pip install -e .`. 
 Then you have a shell command `sneaky_reader` to use!
 
 For the demo books, you could start with commands
```

#### html2text {}

```diff
@@ -1,34 +1,33 @@
-Metadata-Version: 2.1 Name: sneaky-reader Version: 0.1.1 Summary: undercover
+Metadata-Version: 2.1 Name: sneaky-reader Version: 0.1.2 Summary: undercover
 book-reader in your terminal Home-page: https://github.com/gusye1234/sneaky-
 reader Author: JianbaiYe Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown
                        ****** Sneaky-Reader ð¤« ******
       ä¸ç­çä¹¦çå¹»å½±å¦å | Hide your book under a fancy terminal
                [https://img.shields.io/pypi/v/sneaky_reader.svg]
-          [./assets/en-1.png] [./assets/en-2.png] [./assets/en-3.png]
-                         Find dickens in those images
+            [./assets/en-1.png] ð BOSS ð [./assets/en-3.png]
 ## Features ### History saving Sneaky-reader implements a simple cache
 mechanism. You can use `-l` to list all the previous books, and use `-b ID` to
 quickly get the book. For example: ```shell $ sneaky_reader -l [0]
 CharlesDickens-OliverTwist [1] çº¢æ¥¼æ¢¦ $ sneaky_reader -b0 ... ``` ###
 Intuitive usage Greate thanks to the wonderful projects: [`rich`](https://
 github.com/Textualize/rich) and [`textual`](https://github.com/Textualize/
 textual), sneaky-reader can build a (relatively) complex UI in terminal with
 few lines: * You can press `f` to show/hide the chapters pane * You can press
 `m`, `n` to forward/backward the current chapter * You can press `/` to enable
 BOSS mode! It will hide all the sneaky things and only leave a fake Python
-snippet. ### Smart spliting Sneaky-reader supports you to use regluar
-expression (refer to the `re` module in python) to split your TXT into
-chapters. Using the command line option `-e` to pass your regluar expression.
-Remember, always group your chapter name in first in your regular expression!
-*group the title with `()`* ## Quick Start * Via `pip`: `pip install sneaky-
-reader` * Via sources: clone and enter this repo, then install with `pip
-install -e .`. Then you have a shell command `sneaky_reader` to use! For the
-demo books, you could start with commands ```/shell #demo in english
-sneaky_reader -p="./assets/CharlesDickens-OliverTwist.txt" -e="^CHAPTER (.*)" #
-demo in chinese sneaky_reader -p="./assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ```
-For the first time you import a book, `sneaky_reader` will require the book
-path and the spliting expression. After that, the book will be cached and you
-can read it with command `-b ID`.
+snippet. *You can pass `-f ` to use your own fake code!* ### Smart spliting
+Sneaky-reader supports you to use regluar expression (refer to the `re` module
+in python) to split your TXT into chapters. Using the command line option `-e`
+to pass your regluar expression. Remember, always group your chapter name in
+first in your regular expression! *group the title with `(.*)`* ## Quick Start
+* Via `pip`: `pip install sneaky-reader` * Via sources: clone and enter this
+repo, then install with `pip install -e .`. Then you have a shell command
+`sneaky_reader` to use! For the demo books, you could start with commands ```/
+shell #demo in english sneaky_reader -p="./assets/CharlesDickens-
+OliverTwist.txt" -e="^CHAPTER (.*)" # demo in chinese sneaky_reader -p="./
+assets/çº¢æ¥¼æ¢¦.txt" -e="^ç¬¬(.*)å" ``` For the first time you import a
+book, `sneaky_reader` will require the book path and the spliting expression.
+After that, the book will be cached and you can read it with command `-b ID`.
```

