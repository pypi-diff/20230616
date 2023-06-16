# Comparing `tmp/pypipr-0.1.95.tar.gz` & `tmp/pypipr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypipr-0.1.95.tar", max compression
+gzip compressed data, was "pypipr-1.0.2.tar", max compression
```

## Comparing `pypipr-0.1.95.tar` & `pypipr-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0        0 2022-10-24 06:22:00.291550 pypipr-0.1.95/pypipr/__init__.py
--rw-r--r--   0        0        0    35790 2023-05-18 05:33:43.263472 pypipr-0.1.95/pypipr/pypipr.py
--rw-r--r--   0        0        0      631 2023-05-18 07:58:10.393265 pypipr-0.1.95/pyproject.toml
--rw-r--r--   0        0        0    15948 2023-05-18 07:55:46.464798 pypipr-0.1.95/README.md
--rw-r--r--   0        0        0    16885 1970-01-01 00:00:00.000000 pypipr-0.1.95/setup.py
--rw-r--r--   0        0        0    15743 1970-01-01 00:00:00.000000 pypipr-0.1.95/PKG-INFO
+-rw-r--r--   0        0        0    34252 2023-06-16 08:34:35.919415 pypipr-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 07:50:31.475417 pypipr-1.0.2/pypipr/__init__.py
+-rw-r--r--   0        0        0    43701 2023-06-16 07:50:31.479416 pypipr-1.0.2/pypipr/pypipr.py
+-rw-r--r--   0        0        0      538 2023-06-16 08:34:38.779415 pypipr-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    34657 1970-01-01 00:00:00.000000 pypipr-1.0.2/PKG-INFO
```

### Comparing `pypipr-0.1.95/pypipr/pypipr.py` & `pypipr-1.0.2/pypipr/pypipr.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 import os
 import pathlib
 import platform
 import pprint
 import queue
 import random
 import re
+import io
 import shutil
 import subprocess
 import sys
 import threading
 import time
 import timeit
-import urllib
+import urllib.request
+import urllib.parse
 import uuid
 import warnings
 import webbrowser
 import zoneinfo
 import textwrap
 
 
@@ -55,14 +57,15 @@
 if WINDOWS:
     import msvcrt as _getch
 
 
 """PYPI Module"""
 import colorama
 import lxml.html
+import lxml.etree
 import requests
 import yaml
 import pint
 
 if LINUX:
     import getch as _getch
 
@@ -75,90 +78,62 @@
 format variabel: __[function]__[var_name]__
 """
 # is_empty()
 __is_empty__empty_list__ = [None, False, 0, -0]
 __is_empty__empty_list__ += ["0", "", "-0", "\n", "\t"]
 __is_empty__empty_list__ += [set(), dict(), list(), tuple()]
 # batchmaker()
-__batchmaker__regex_pattern__ = r"\{([0-9a-zA-Z]+)\-([0-9a-zA-Z]+)(?:\-(\d+))?\}"
+__batchmaker__regex_pattern__ = r"{(?:[^a-zA-Z0-9{}]+)?([a-zA-Z]|\d+)[^a-zA-Z0-9{}]+([a-zA-Z]|\d+)(?:[^a-zA-Z0-9{}]+(\d+))?(?:[^a-zA-Z0-9{}]+)?}"
 __batchmaker__regex_compile__ = re.compile(__batchmaker__regex_pattern__)
 # calculate()
 __calculate__ureg__ = pint.UnitRegistry()
-__calculate__Quantity__ = __calculate__ureg__.Quantity
+__calculate__quantity__ = __calculate__ureg__.Quantity
+# is_valid_url()
+__is_valid_url__pattern__ = "^(?:(?:(?:https?|ftp):)?\/\/)(?:\S+(?::\S*)?@)?(?:(?!(?:10|127)(?:\.\d{1,3}){3})(?!(?:169\.254|192\.168)(?:\.\d{1,3}){2})(?!172\.(?:1[6-9]|2\d|3[0-1])(?:\.\d{1,3}){2})(?:[1-9]\d?|1\d\d|2[01]\d|22[0-3])(?:\.(?:1?\d{1,2}|2[0-4]\d|25[0-5])){2}(?:\.(?:[1-9]\d?|1\d\d|2[0-4]\d|25[0-4]))|(?:(?:[a-z0-9\u00a1-\uffff][a-z0-9\u00a1-\uffff_-]{0,62})?[a-z0-9\u00a1-\uffff]\.)+(?:[a-z\u00a1-\uffff]{2,}\.?))(?::\d{2,5})?(?:[/?#]\S*)?$"
+__is_valid_url__regex__ = re.compile(__is_valid_url__pattern__, flags=re.IGNORECASE)
 
 
 class generator:
     """
     Class ini menyediakan beberapa fungsi yang bisa mengembalikan generator.
     Digunakan untuk mengoptimalkan program.
 
     Class ini dibuat karena python generator yang disimpan dalam variabel
     hanya dapat diakses satu kali.
     """
 
-    def iscandir(folder_name=".", glob_pattern="*", recursive=True):
+    @staticmethod
+    def iscandir(
+        folder_name=".",
+        glob_pattern="*",
+        recursive=True,
+        scan_file=True,
+        scan_folder=True,
+    ):
         """
-        Mempermudah scandir untuk mengumpulkan folder, subfolder dan file
+        Mempermudah scandir untuk mengumpulkan folder dan file.
 
-        ```py
-        for i in generator.iscandir():
-            print(i)
-
-        for i in iscandir():
-            print(i)
+        ```python
+        print(generator.iscandir())
+        print(iscandir("./", recursive=False, scan_file=False))
         ```
         """
+        path_obj = pathlib.Path(folder_name)
         if recursive:
-            return pathlib.Path(folder_name).rglob(glob_pattern)
+            path_obj = path_obj.rglob(glob_pattern)
         else:
-            return pathlib.Path(folder_name).glob(glob_pattern)
-
-    def scan_folder(folder_name="", glob_pattern="*", recursive=True):
-        """
-        Mengumpulkan nama-nama folder dan subfolder.
-        Tidak termasuk [".", ".."] dan file.
+            path_obj = path_obj.glob(glob_pattern)
 
-        ```python
-        for i in generator.scan_folder(recursive=False):
-            print(i)
-
-        for i in scan_folder(recursive=False):
-            print(i)
-        ```
-        """
-        p = generator.iscandir(
-            folder_name=folder_name,
-            glob_pattern=glob_pattern,
-            recursive=recursive,
-        )
-        for i in p:
-            if i.is_dir():
+        for i in path_obj:
+            if scan_folder and i.is_dir():
                 yield i
-
-    def scan_file(folder_name="", glob_pattern="*", recursive=True):
-        """
-        Mengumpulkan nama-nama file dalam folder dan subfolder.
-
-        ```py
-        for i in generator.scan_file():
-            print(i)
-
-        for i in scan_file():
-            print(i)
-        ```
-        """
-        p = generator.iscandir(
-            folder_name=folder_name,
-            glob_pattern=glob_pattern,
-            recursive=recursive,
-        )
-        for i in p:
-            if i.is_file():
+            if scan_file and i.is_file():
                 yield i
 
+    @staticmethod
     def get_class_method(cls):
         """
         Mengembalikan berupa tuple yg berisi list dari method dalam class
 
         ```python
         class ExampleGetClassMethod:
             def a():
@@ -169,36 +144,37 @@
 
             def c():
                 return [x for x in range(10)]
 
             def d():
                 return [x for x in range(10)]
 
-        if __name__ == "__main__":
-            print(get_class_method(ExampleGetClassMethod))
+        print(get_class_method(ExampleGetClassMethod))
         ```
         """
         for x in dir(cls):
             a = getattr(cls, x)
             if not x.startswith("__") and callable(a):
                 yield a
 
+    @staticmethod
     def chunck_array(array, size, start=0):
         """
         Membagi array menjadi potongan-potongan dengan besaran yg diinginkan
 
         ```python
         array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
         print(generator.chunck_array(array, 5))
         print(chunck_array(array, 5))
         ```
         """
         for i in range(start, len(array), size):
             yield array[i : i + size]
 
+    @staticmethod
     def irange(start, finish, step=1):
         """
         Meningkatkan fungsi range() dari python untuk pengulangan menggunakan huruf
 
         ```python
         print(generator.irange('a', 'c'))
         print(irange('z', 'a', 10))
@@ -264,48 +240,53 @@
         faktor = 1 if finish > start else -1
         step *= faktor
         finish += faktor
 
         for i in range(start, finish, step):
             yield converter_class(i)
 
+    @staticmethod
     def sets_ordered(iterator):
         """
         Hanya mengambil nilai unik dari suatu list
 
         ```python
         array = [2, 3, 12, 3, 3, 42, 42, 1, 43, 2, 42, 41, 4, 24, 32, 42, 3, 12, 32, 42, 42]
         print(generator.sets_ordered(array))
         print(sets_ordered(array))
         ```
         """
         for i in dict.fromkeys(iterator):
             yield i
 
+    @staticmethod
     def filter_empty(iterable, zero_is_empty=True, str_strip=True):
         for i in iterable:
             if i == 0 and zero_is_empty:
                 continue
             if isinstance(i, str) and str_strip:
                 i = i.strip()
             if not is_iterable(i) and not to_str(i):
                 continue
             yield i
 
+    @staticmethod
     def batchmaker(text: str):
         """
         Alat Bantu untuk membuat teks yang berulang.
-        Gunakan {[start]-[finish][-[step]]}.
+        Gunakan {[start][separator][finish]([separator][step])}.
         ```
         [start] dan [finish]    -> bisa berupa huruf maupun angka
-        [-[step]]               -> bersifat optional
+        ([separator][step])     -> bersifat optional
+        [separator]             -> selain huruf dan angka
+        [step]                  -> berupa angka positif
         ```
 
         ```python
-        s = "Urutan {1-30-5} dan {3-1} dan {a-d} dan {Z-A-10} saja."
+        s = "Urutan {1/6/3} dan {10:9} dan {j k} dan {Z - A - 15} saja."
         print(generator.batchmaker(s))
         print(batchmaker(s))
         ```
         """
         s = __batchmaker__regex_compile__.search(text)
         if s is None:
             yield text
@@ -326,44 +307,43 @@
     color_end=colorama.Style.RESET_ALL,
     text_start="",
     text_end="\n",
 ):
     """
     Print text dengan warna untuk menunjukan text penting
 
-    ```python
+    ```py
     print_colorize("Print some text")
     print_colorize("Print some text", color=colorama.Fore.RED)
     ```
     """
     print(f"{text_start}{color + bright}{text}{color_end}", end=text_end, flush=True)
 
 
 def log(text=None):
     """
     Decorator untuk mempermudah pembuatan log karena tidak perlu mengubah fungsi yg sudah ada.
     Melakukan print ke console untuk menginformasikan proses yg sedang berjalan didalam program.
 
-    ```python
+    ```py
     @log
     def some_function():
         pass
 
     @log()
     def some_function_again():
         pass
 
     @log("Calling some function")
     def some_function_more():
         pass
 
-    if __name__ == "__main__":
-        some_function()
-        some_function_again()
-        some_function_more()
+    some_function()
+    some_function_again()
+    some_function_more()
     ```
     """
 
     def inner_log(func=None):
         def callable_func(*args, **kwargs):
             main_function(text)
             result = func(*args, **kwargs)
@@ -386,31 +366,41 @@
 
 
 def print_log(text):
     """
     Akan melakukan print ke console.
     Berguna untuk memberikan informasi proses program yg sedang berjalan.
 
-    ```python
+    ```py
     print_log("Standalone Log")
     ```
     """
     print_colorize(f">>> {text}")
 
 
-def console_run(command):
+def console_run(info, command=None, print_info=True, capture_output=False):
     """
     Menjalankan command seperti menjalankan command di Command Terminal
 
-    ```python
+    ```py
     console_run('dir')
     console_run('ls')
     ```
     """
-    return subprocess.run(command, shell=True)
+    if command is None:
+        command = info
+
+    if print_info:
+        print_log(info)
+
+    param = dict(shell=True)
+    if capture_output:
+        param |= dict(capture_output=True, text=True)
+
+    return subprocess.run(command, **param)
 
 
 def input_char(
     prompt=None,
     prompt_ending="",
     newline_after_input=True,
     echo_char=True,
@@ -477,81 +467,41 @@
     Menjalankan command status, add, commit dan push
 
     ```py
     github_push('Commit Message')
     ```
     """
 
-    def console(t, c):
-        print_log(t)
-        console_run(c)
-
     def console_input(prompt, default):
         print_colorize(prompt, text_end="")
         if default:
             print(default)
             return default
         else:
             return input()
 
     print_log("Menjalankan Github Push")
-    console("Checking files", "git status")
+    console_run("Checking files", "git status")
     msg = console_input("Commit Message if any or empty to exit : ", commit)
     if msg:
-        console("Mempersiapkan files", "git add .")
-        console("Menyimpan files", f'git commit -m "{msg}"')
-        console("Mengirim files", "git push")
+        console_run("Mempersiapkan files", "git add .")
+        console_run("Menyimpan files", f'git commit -m "{msg}"')
+        console_run("Mengirim files", "git push")
     print_log("Selesai Menjalankan Github Push")
 
 
 def github_pull():
     """
     Menjalankan command `git pull`
 
     ```py
     github_pull()
     ```
     """
-    print_log("Git Pull")
-    console_run("git pull")
-
-
-def file_get_contents(filename):
-    """
-    Membaca seluruh isi file ke memory.
-    Apabila file tidak ada maka akan return None.
-    Apabila file ada tetapi kosong, maka akan return empty string
-
-    ```py
-    print(file_get_contents("ifile_test.txt"))
-    ```
-    """
-    try:
-        f = open(filename, "r")
-        r = f.read()
-        f.close()
-        return r
-    except:
-        return None
-
-
-def file_put_contents(filename, contents):
-    """
-    Menuliskan content ke file.
-    Apabila file tidak ada maka file akan dibuat.
-    Apabila file sudah memiliki content maka akan di overwrite.
-
-    ```py
-    file_put_contents("ifile_test.txt", "Contoh menulis content")
-    ```
-    """
-    f = open(filename, "w")
-    r = f.write(contents)
-    f.close()
-    return r
+    console_run("Git Pull", "git pull")
 
 
 def create_folder(folder_name):
     """
     Membuat folder.
     Membuat folder secara recursive dengan permission.
 
@@ -560,137 +510,32 @@
     create_folder("contoh/membuat/folder/recursive")
     create_folder("./contoh_membuat_folder/secara/recursive")
     ```
     """
     pathlib.Path(folder_name).mkdir(parents=True, exist_ok=True)
 
 
-def iscandir(folder_name=".", glob_pattern="*", recursive=True):
+def iscandir(
+    folder_name=".",
+    glob_pattern="*",
+    recursive=True,
+    scan_file=True,
+    scan_folder=True,
+):
     return tuple(
         generator.iscandir(
             folder_name=folder_name,
             glob_pattern=glob_pattern,
             recursive=recursive,
+            scan_file=scan_file,
+            scan_folder=scan_folder,
         )
     )
 
 
-def scan_folder(folder_name="", glob_pattern="*", recursive=True):
-    return tuple(
-        generator.scan_folder(
-            folder_name=folder_name,
-            glob_pattern=glob_pattern,
-            recursive=recursive,
-        )
-    )
-
-
-def scan_file(folder_name="", glob_pattern="*", recursive=True):
-    return tuple(
-        generator.scan_file(
-            folder_name=folder_name,
-            glob_pattern=glob_pattern,
-            recursive=recursive,
-        )
-    )
-
-
-def html_get_contents(url, xpath=None, regex=None, css_select=None):
-    """
-    Mengambil content html dari url.
-
-    RETURN:
-    - String: Apabila hanya url saja yg diberikan
-    - List of etree: Apabila xpath diberikan
-    - False: Apabila terjadi error
-
-    ```py
-    print(html_get_contents("https://arbadzukhron.deta.dev/"))
-    ```
-    ```python
-    # Using XPATH
-    a = html_get_contents("https://www.google.com/", xpath="//a")
-    for i in a:
-        print(i.text)
-        print(i.attrib.get('href'))
-
-    # Using REGEX
-    a = html_get_contents("https://www.google.com/", regex=r"(<a.[^>]+>(?:(?:\s+)?(.[^<]+)(?:\s+)?)<\/a>)")
-    for i in a:
-        print(i)
-
-    # Using cssselect
-    a = html_get_contents("https://www.google.com/", css_select="a")
-    for i in a:
-        print(i.text)
-        print(i.attrib.get("href"))
-    ```
-    """
-    url_req = urllib.request.Request(
-        url=url,
-        headers={
-            "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Mobile Safari/537.36"
-        },
-    )
-    url_open = urllib.request.urlopen(url_req)
-    try:
-        if xpath:
-            return lxml.html.parse(url_open).findall(xpath)
-        if regex:
-            return re.findall(regex, url_open.read().decode())
-        if css_select:
-            return lxml.html.parse(url_open).getroot().cssselect(css_select)
-        return url_open.read().decode()
-    except:
-        return False
-
-
-def html_put_contents(url, data):
-    """
-    Fungsi untuk mengirim data ke URL dengan method POST dan mengembalikan
-    respon dari server sebagai string.
-
-    Parameters:
-        url (str): URL tujuan.
-        data (dict): Data yang akan dikirim.
-
-    Returns:
-    - str: Respon dari server dalam bentuk string.
-
-    ```python
-    data = dict(pengirim="saya", penerima="kamu")
-    print(html_put_contents("https://arbadzukhron.deta.dev/", data))
-    ```
-    """
-
-    # Encode data ke dalam format yang bisa dikirim
-    data = urllib.parse.urlencode(data).encode()
-
-    # Buat objek request
-    req = (
-        urllib.request.Request(
-            url=url,
-            data=data,
-            headers={
-                "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Mobile Safari/537.36"
-            },
-        ),
-    )
-
-    # Kirim request dan terima respon
-    response = urllib.request.urlopen(req)
-    html = response.read().decode()
-
-    # Tutup koneksi
-    response.close()
-
-    # Kembalikan respon sebagai string
-    return html
-
-
 def get_filesize(filename):
     """
     Mengambil informasi file size dalam bytes
 
     ```python
     print(get_filesize(__file__))
     ```
@@ -705,35 +550,38 @@
     ```python
     print(get_filemtime(__file__))
     ```
     """
     return os.stat(filename).st_mtime_ns
 
 
-def dict_first(d: dict) -> tuple:
+def dict_first(d: dict, remove=False):
     """
-    Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple
+    Mengambil nilai (key, value) pertama dari dictionary dalam bentuk tuple.
 
     ```python
     d = {
-        "key1": "value1",
         "key2": "value2",
         "key3": "value3",
+        "key1": "value1",
     }
+    print(dict_first(d, remove=True))
     print(dict_first(d))
     ```
     """
     for k in d:
-        return (k, d[k])
+        return (k, d.pop(k) if remove else d[k])
 
 
-def random_bool() -> bool:
+def random_bool():
     """
     Menghasilkan nilai random True atau False.
     Fungsi ini merupakan fungsi tercepat untuk mendapatkan random bool.
+    Fungsi ini sangat cepat, tetapi pemanggilan fungsi ini membutuhkan
+    overhead yg besar.
 
     ```python
     print(random_bool())
     ```
     """
     return bool(random.getrandbits(1))
 
@@ -762,15 +610,16 @@
 def get_class_method(cls):
     return tuple(generator.get_class_method(cls))
 
 
 class ComparePerformance:
     """
     Menjalankan seluruh method dalam class,
-    kemudian membandingkan waktu yg diperlukan.
+    Kemudian membandingkan waktu yg diperlukan.
+    Nilai 100 berarti yang tercepat.
 
     ```python
     class ExampleComparePerformance(ComparePerformance):
         # number = 1
         z = 10
 
         def a(self):
@@ -781,21 +630,20 @@
 
         def c(self):
             return [x for x in range(self.z)]
 
         def d(self):
             return list(x for x in range(self.z))
 
-    if __name__ == "__main__":
-        print(ExampleComparePerformance().compare_result())
-        print(ExampleComparePerformance().compare_performance())
-        print(ExampleComparePerformance().compare_performance())
-        print(ExampleComparePerformance().compare_performance())
-        print(ExampleComparePerformance().compare_performance())
-        print(ExampleComparePerformance().compare_performance())
+    pprint.pprint(ExampleComparePerformance().compare_result(), depth=100)
+    print(ExampleComparePerformance().compare_performance())
+    print(ExampleComparePerformance().compare_performance())
+    print(ExampleComparePerformance().compare_performance())
+    print(ExampleComparePerformance().compare_performance())
+    print(ExampleComparePerformance().compare_performance())
     ```
     """
 
     number = 1
 
     def get_all_instance_methods(self):
         c = set(dir(__class__))
@@ -816,15 +664,14 @@
         s = time.perf_counter_ns()
         for _ in range(self.number):
             c()
         f = time.perf_counter_ns()
         return f - s
 
     def calculate_average(self, d: dict):
-        # avg = lambda v: sum(v) / len(v)
         r1 = {i: avg(v) for i, v in d.items()}
         min_value = min(r1.values())
         persen = lambda v: int(v / min_value * 100)
         r2 = {i: persen(v) for i, v in r1.items()}
         return r2
 
     def compare_performance(self):
@@ -838,24 +685,25 @@
         return {x: getattr(self, x)() for x in m}
 
 
 class RunParallel:
     """
     Menjalankan program secara bersamaan.
 
-    Structure:
-    - Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`
-    - Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunaan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.
-    - Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.
-    - Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi
-
-    Note:
     - `class RunParallel` didesain hanya untuk pemrosesan data saja.
     - Penggunaannya `class RunParallel` dengan cara membuat instance sub class beserta data yg akan diproses, kemudian panggil fungsi yg dipilih `run_asyncio / run_multi_threading / run_multi_processing`, kemudian dapatkan hasilnya.
     - `class RunParallel` tidak didesain untuk menyimpan data, karena setiap module terutama module `multiprocessing` tidak dapat mengakses data kelas dari proses yg berbeda.
+    - Semua methods akan dijalankan secara paralel kecuali method dengan nama yg diawali underscore `_`
+    - Method untuk multithreading/multiprocessing harus memiliki 2 parameter, yaitu: `result: dict` dan `q: queue.Queue`. Parameter `result` digunakan untuk memberikan return value dari method, dan Parameter `q` digunakan untuk mengirim data antar proses.
+    - Method untuk asyncio harus menggunakan keyword `async def`, dan untuk perpindahan antar kode menggunakan `await asyncio.sleep(0)`, dan keyword `return` untuk memberikan return value.
+    - Return Value berupa dictionary dengan key adalah nama function, dan value adalah return value dari setiap fungsi
+    - Menjalankan Multiprocessing harus berada dalam blok `if __name__ == "__main__":` karena area global pada program akan diproses lagi. Terutama pada sistem operasi windows.
+    - `run_asyncio()` akan menjalankan kode dalam satu program, hanya saja alur program dapat berpindah-pindah menggunkan `await asyncio.sleep(0)`.
+    - `run_multi_threading()` akan menjalankan program dalam satu CPU, hanya saja dalam thread yang berbeda. Walaupun tidak benar-benar berjalan secara bersamaan namun bisa meningkatkan kecepatan penyelesaian program, dan dapat saling mengakses resource antar program.  Akses resource antar program bisa secara langsung maupun menggunakan parameter yang sudah disediakan yaitu `result: dict` dan `q: queue.Queue`.
+    - `run_multi_processing()` akan menjalankan program dengan beberapa CPU. Program akan dibuatkan environment sendiri yang terpisah dari program induk. Keuntungannya adalah program dapat benar-benar berjalan bersamaan, namun tidak dapat saling mengakses resource secara langsung. Akses resource menggunakan parameter yang sudah disediakan yaitu `result: dict` dan `q: queue.Queue`.
 
     ```python
     class ExampleRunParallel(RunParallel):
         z = "ini"
 
         def __init__(self) -> None:
             self.pop = random.randint(0, 100)
@@ -986,15 +834,15 @@
 
 
 def exit_if_empty(*args):
     """
     Keluar dari program apabila seluruh variabel
     setara dengan empty
 
-    ```python
+    ```py
     var1 = None
     var2 = '0'
     exit_if_empty(var1, var2)
     ```
     """
     for i in args:
         if not is_empty(i):
@@ -1006,14 +854,15 @@
     iterable,
     separator="",
     start="",
     end="",
     remove_empty=False,
     recursive=True,
     recursive_flat=False,
+    str_strip=False,
 ):
     """
     Simplify Python join functions like PHP function.
     Iterable bisa berupa sets, tuple, list, dictionary.
 
     ```python
     arr = {'asd','dfs','weq','qweqw'}
@@ -1052,76 +901,79 @@
             recursive=recursive,
             recursive_flat=recursive_flat,
         )
         iterable = ((rec(i) if is_iterable(i) else i) for i in iterable)
 
     iterable = (str(i) for i in iterable)
 
+    if str_strip:
+        iterable = (i.strip() for i in iterable)
+
     result = start
 
     for index, value in enumerate(iterable):
         if index:
             result += separator
         result += value
 
     result += end
 
     return result
 
 
-def strtr(string: str, replacements: dict):
+def strtr(
+    string: str,
+    replacements: dict,
+    flags=re.DOTALL | re.MULTILINE | re.IGNORECASE,
+):
     """
-    STRing TRanslate, mengubah string menggunakan kamus dari dict.
+    STRing TRanslate mengubah string menggunakan kamus dari dict.
+    Replacement dapat berupa text biasa ataupun regex pattern.
+    Apabila replacement berupa regex, gunakan raw string `r"..."`
+    Untuk regex capturing gunakan `(...)`, dan untuk mengaksesnya gunakan `\\1`, `\\2`, .., dst.
 
     ```python
-    text = 'aku disini mau kemana saja'
+    text = 'aku ini mau ke sini'
     replacements = {
-        "disini": "disitu",
-        "kemana": "kesini",
+        "sini": "situ",
+        r"(ini)": r"itu dan \\1",
     }
     print(strtr(text, replacements))
     ```
     """
     for i, v in replacements.items():
-        string = string.replace(i, v)
-    return string
-
-
-def strtr_regex(string: str, replacements: dict, flags=0):
-    """
-    STRing TRanslate metode Regex, mengubah string menggunakan kamus dari dict.
-
-    ```python
-    text = 'aku {{ ini }} mau ke {{ sini }} mau kemana saja'
-    replacements = {
-        r"\{\{\s*(ini)\s*\}\}": r"itu dan \\1",
-        r"\{\{\s*sini\s*\}\}": r"situ",
-    }
-    print(strtr_regex(text, replacements))
-    ```
-    """
-    for i, v in replacements.items():
         string = re.sub(i, v, string, flags=flags)
     return string
 
 
-def print_dir(var):
+def print_dir(var, colorize=True):
     """
     Print property dan method yang tersedia pada variabel
 
     ```python
-    p = pathlib.Path("c:/arba/dzukhron.dz")
-    print_dir(p)
+    p = pathlib.Path("https://www.google.com/")
+    print_dir(p, colorize=False)
     ```
     """
-    for i in dir(var):
+    d = dir(var)
+    m = max(len(i) for i in d)
+    for i in d:
         try:
             a = getattr(var, i)
             r = a() if callable(a) else a
-            print(f"{i: >20} : {r}")
+            if colorize:
+                color = colorama.Fore.GREEN
+                if is_empty(r):
+                    color = colorama.Fore.LIGHTRED_EX
+                if i.startswith("__"):
+                    color = colorama.Fore.CYAN
+                print_colorize(f"{i: >{m}}", text_end=" : ", color=color)
+                print(r)
+            else:
+                print(f"{i: >{m}} : {r}")
         except:
             pass
 
 
 def is_iterable(var, str_is_iterable=False):
     """
     Mengecek apakah suatu variabel bisa dilakukan forloop atau tidak
@@ -1176,29 +1028,36 @@
     print(irange(-10, 4, 3))
     print(irange(1, 5))
     ```
     """
     return list(generator.irange(start, finish, step))
 
 
-def serialize(data):
+def serialize(data, syntax="yaml", indent=4):
     """
     Mengubah variabel data menjadi string untuk yang dapat dibaca untuk disimpan.
-    String yang dihasilkan berbentuk syntax YAML.
+    String yang dihasilkan berbentuk syntax YAML/JSON/HTML.
 
     ```python
     data = {
         'a': 123,
         't': ['disini', 'senang', 'disana', 'senang'],
-        'l': (12, 23, [12, 42])
+        'l': (12, 23, [12, 42]),
     }
     print(serialize(data))
+    print(serialize(data, syntax='html'))
     ```
     """
-    return yaml.safe_dump(data)
+    if syntax == "yaml":
+        return yaml.dump(data, indent=indent)
+    if syntax == "json":
+        return json.dumps(data, indent=indent)
+    if syntax == "html":
+        return serialize_html(data, indent=indent)
+    raise Exception(f"Syntax tidak didukung {syntax}")
 
 
 def unserialize(data):
     """
     Mengubah string data hasil dari serialize menjadi variabel.
     String data adalah berupa syntax YAML.
 
@@ -1322,21 +1181,366 @@
     Mengembalikan hasil dari perhitungan teks menggunakan modul pint.
     Mendukung perhitungan matematika dasar dengan satuan.
 
     Return value:
     - Berupa class Quantity dari modul pint
 
     Format:
-    - f"{fx:~P}"            -> pretty
-    - f"{fx:~H}"            -> html
-    - fx.to_base_units()    -> SI
-    - fx.to_compact()       -> human readable
+    - f"{result:~P}"            -> pretty
+    - f"{result:~H}"            -> html
+    - result.to_base_units()    -> SI
+    - result.to_compact()       -> human readable
 
     ```python
     fx = "3 meter * 10 cm * 3 km"
     res = calculate(fx)
     print(res)
     print(res.to_base_units())
     print(res.to_compact())
+    print(f"{res:~P}")
+    print(f"{res:~H}")
+    ```
+    """
+    return __calculate__quantity__(teks)
+
+
+def iexec(python_syntax, import_pypipr=True):
+    """
+    improve exec() python function untuk mendapatkan outputnya
+
+    ```python
+    print(iexec('print(9*9)'))
+    ```
+    """
+    if import_pypipr:
+        python_syntax = f"from pypipr.pypipr import *\n\n{python_syntax}"
+
+    stdout_backup = sys.stdout
+
+    sys.stdout = io.StringIO()
+    exec(python_syntax)
+    output = sys.stdout.getvalue()
+
+    sys.stdout = stdout_backup
+
+    return output
+
+
+def is_valid_url(path):
+    """
+    Mengecek apakah path merupakan URL yang valid atau tidak.
+    Cara ini merupakan cara yang paling efektif.
+
+    ```python
+    print(is_valid_url("https://chat.openai.com/?model=text-davinci-002-render-sha"))
+    print(is_valid_url("https://chat.openai.com/?model/=text-dav/inci-002-render-sha"))
+    ```
+    """
+    return bool(__is_valid_url__regex__.fullmatch(path))
+
+
+def iopen(path, data=None, regex=None, css_select=None, xpath=None, file_append=False):
+    """
+    Membaca atau Tulis pada path yang bisa merupakan FILE maupun URL.
+
+    Baca File :
+    - Membaca seluruh file.
+    - Jika berhasil content dapat diparse dengan regex.
+    - Apabila File berupa html, dapat diparse dengan css atau xpath.
+
+    Tulis File :
+    - Menulis pada file.
+    - Jika file tidak ada maka akan dibuat.
+    - Jika file memiliki content maka akan di overwrite.
+
+    Membaca URL :
+    - Mengakses URL dan mengembalikan isi html nya berupa teks.
+    - Content dapat diparse dengan regex, css atau xpath.
+
+    Tulis URL :
+    - Mengirimkan data dengan metode POST ke url.
+    - Jika berhasil dan response memiliki content, maka dapat diparse dengan regex, css atau xpath.
+
+
+    ```python
+    # FILE
+    print(iopen("__iopen.txt", "mana aja"))
+    print(iopen("__iopen.txt", regex="(\w+)"))
+    # URL
+    print(iopen("https://www.google.com/", css_select="a"))
+    print(iopen("https://www.google.com/", dict(coba="dulu"), xpath="//a"))
     ```
     """
-    return __calculate__Quantity__(teks)
+    path = to_str(path)
+    content = ""
+
+    if is_valid_url(path):
+        req = dict(
+            url=path,
+            headers={
+                "User-Agent": "Mozilla/5.0 (Linux; Android 6.0; Nexus 5 Build/MRA58N) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Mobile Safari/537.36"
+            },
+        )
+
+        if data:
+            req["data"] = urllib.parse.urlencode(data).encode()
+
+        req = urllib.request.Request(**req)
+
+        # Connect to URL
+        try:
+            with urllib.request.urlopen(req) as url_open:
+                content = url_open.read().decode()
+        except Exception as e:
+            # print(f"An error occurred: {str(e)}")
+            return False
+
+    else:
+        # Write File
+        if data is not None:
+            mode = "a" if file_append else "w"
+            with open(path, mode, encoding="utf-8") as f:
+                content = f.write(data)
+        # Read File
+        else:
+            try:
+                with open(path, "r") as f:
+                    content = f.read()
+            except Exception as e:
+                # print(f"An error occurred: {str(e)}")
+                return False
+
+    """ Parse """
+    if regex:
+        return re.findall(regex, content)
+    if css_select:
+        return lxml.html.fromstring(content).cssselect(css_select)
+    if xpath:
+        return lxml.html.fromstring(content).xpath(xpath)
+
+    """ Return """
+    return content
+
+
+def serialize_html(data, indent=None):
+    """
+    Serialisasi python variabel menjadi HTML.
+    ```
+    List -> <ul>...</ul>
+    Dict -> <table>...</table>
+    ```
+
+    ```python
+    data = {
+        'abc': 123,
+        'list': [1, 2, 3, 4, 5],
+        'dict': {'a': 1, 'b':2, 'c':3},
+    }
+    print(serialize_html(data))
+    ```
+    """
+
+    def to_ul(data):
+        ul = lxml.etree.Element("ul")
+        for i in data:
+            li = lxml.etree.SubElement(ul, "li")
+            li.append(to_html(i))
+        return ul
+
+    def to_table(data: dict):
+        table = lxml.etree.Element("table")
+        tbody = lxml.etree.SubElement(table, "tbody")
+        for i, v in data.items():
+            tr = lxml.etree.SubElement(tbody, "tr")
+            th = lxml.etree.SubElement(tr, "th")
+            th.text = str(i)
+            td = lxml.etree.SubElement(tr, "td")
+            td.append(to_html(v))
+        return table
+
+    def to_text(data):
+        span = lxml.etree.Element("span")
+        span.text = str(data)
+        return span
+
+    def to_html(data):
+        struct = {
+            dict: to_table,
+            list: to_ul,
+            tuple: to_ul,
+            set: to_ul,
+        }
+        return struct.get(type(data), to_text)(data)
+
+    html = to_html(data)
+    if indent:
+        lxml.etree.indent(html, space=" " * indent)
+    return lxml.etree.tostring(html, pretty_print=True, encoding="unicode")
+
+
+def str_cmp(t1, t2):
+    """
+    Membandingakan string secara incase-sensitive menggunakan lower().
+    Lebih cepat dibandingkan upper(), casefold(), re.fullmatch(), len().
+    perbandingan ini sangat cepat, tetapi pemanggilan fungsi ini membutuhkan
+    overhead yg besar.
+    ```python
+    print(str_cmp('teks1', 'Teks1'))
+    ```
+    """
+    return t1.lower() == t2.lower()
+
+
+def unserialize_html(html):
+    """
+    Mengambil data yang berupa list `<ul>`, dan table `<table>` dari html
+    dan menjadikannya data python berupa list.
+    setiap data yang ditemukan akan dibungkus dengan tuple sebagai separator.
+    ```
+    list (<ul>)     -> list         -> list satu dimensi
+    table (<table>) -> list[list]   -> list satu dimensi didalam list
+    ```
+    apabila data berupa ul maka dapat dicek type(data) -> html_ul
+    apabila data berupa ol maka dapat dicek type(data) -> html_ol
+    apabila data berupa dl maka dapat dicek type(data) -> html_dl
+    apabila data berupa table maka dapat dicek type(data) -> html_table
+
+    ```python
+    pprint.pprint(unserialize_html(iopen("https://harga-emas.org/")), depth=10)
+    pprint.pprint(unserialize_html(iopen("https://harga-emas.org/1-gram/")), depth=10)
+    ```
+    """
+
+    def xpath(e, x):
+        """
+        Fungsi ini sangat krusial/menentukan. Fungsi ini dibuat
+        supaya xpath yang diberikan diproses dari element saat ini.
+        Sedangkan xpath pada element lxml akan mengecek syntax xpath dari
+        root paling awal document.
+        """
+        if not isinstance(e, str):
+            e = lxml.html.tostring(e, encoding="unicode")
+        e = lxml.html.fromstring(e)
+        return (e, e.xpath(x))
+
+    def parse(e):
+        parser = {
+            "ul": parse_ul,
+            "ol": parse_ol,
+            "dl": parse_dl,
+            "table": parse_table,
+        }
+        try:
+            return parser[e.tag.lower()](e)
+        except:
+            raise Exception("Tidak ditemukan parse fungsi untuk element : ", e)
+
+    def parse_list(ul):
+        """
+        Simple parse html list.
+        """
+        result = []
+        _, li = xpath(ul, "li")
+        for i in li:
+            u = unserialize_html(i)
+            t = i.text.strip() if i.text else ""
+            if t and t != u:
+                result.append({t: u})
+            else:
+                result.append(u)
+        return result
+
+    def parse_ul(ul):
+        return html_ul(parse_list(ul))
+
+    def parse_ol(ol):
+        return html_ol(parse_list(ol))
+
+    def parse_dl(dl):
+        """
+        Simple parse dl-dt-dd.
+        """
+        result = html_dl()
+        _, di = xpath(dl, "dt|dd")
+        d = iter(di)
+        try:
+            while True:
+                i = next(d)
+                k = i.tag.lower()
+                v = unserialize_html(i)
+                if k == "dt":
+                    result.append(["", []])
+                    result[-1][0] = v
+                elif k == "dd":
+                    result[-1][-1].append(v)
+        except:
+            pass
+
+        return result
+
+    def parse_table(table):
+        """
+        Mengambil children tr dari table.
+        tr diambil dari thead atau tbody atau langsung tr.
+        tr dari thead atau tbody akan dianggap sama.
+        """
+        result = html_table()
+        _, tr = xpath(table, "//tr[not(ancestor::tr)]")
+        for itr in tr:
+            d = []
+            _, td = xpath(itr, "th|td")
+            for itd in td:
+                d.append(unserialize_html(itd))
+            result.append(d.copy())
+        return result
+
+    def text_content(e):
+        """
+        mengambil semua text dalam element secara recursive.
+        karena tidak ditemukan data dalam element.
+        """
+        return implode(e.itertext(), str_strip=True)
+
+    element, childs = xpath(
+        html,
+        "//*[self::ul | self::ol | self::dl | self::table][not(ancestor::ul | ancestor::ol | ancestor::dl | ancestor::table)]",
+    )
+    if childs:
+        return tuple((parse(data) for data in childs))
+    else:
+        return text_content(element)
+
+
+class html_ul(list):
+    """
+    Class ini digunakan untuk serialize dan unserialize html
+    """
+
+    pass
+
+
+class html_ol(list):
+    """
+    Class ini digunakan untuk serialize dan unserialize html
+    """
+
+    pass
+
+
+class html_dl(list):
+    """
+    Class ini digunakan untuk serialize dan unserialize html
+    """
+
+    pass
+
+
+class html_table(list):
+    """
+    Class ini digunakan untuk serialize dan unserialize html
+    """
+
+    pass
+
+
+if __name__ == "__main__":
+    print_colorize("Anda menjalankan module pypipr", color=colorama.Fore.RED)
```

### Comparing `pypipr-0.1.95/pyproject.toml` & `pypipr-1.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 [tool.poetry]
 name = "pypipr"
-version = "0.1.95"
+version = "1.0.2"
 description = "The Python Package Index Project"
 authors = ["ufiapjj <ufiapjj@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
+
+[tool.poetry.group.dev.dependencies]
 getch = { version = "*", markers = "platform_system == 'Linux'" }
 colorama = "*"
 lxml = "*"
 cssselect = "*"
 tzdata = "*"
-requests = "^2.30.0"
-pyyaml = "^6.0"
-pint = "^0.21"
-
-[tool.poetry.dev-dependencies]
+requests = "*"
+pyyaml = "*"
+pint = "*"
 pytest = "*"
-
-[tool.poetry.group.dev.dependencies]
-black = {version = "^22.12.0", allow-prereleases = true}
+black = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

