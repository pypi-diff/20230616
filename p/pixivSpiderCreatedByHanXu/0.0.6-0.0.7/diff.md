# Comparing `tmp/pixivSpiderCreatedByHanXu-0.0.6.tar.gz` & `tmp/pixivSpiderCreatedByHanXu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.6.tar", last modified: Wed Apr 26 10:28:32 2023, max compression
+gzip compressed data, was "pixivSpiderCreatedByHanXu-0.0.7.tar", last modified: Fri Jun 16 14:41:35 2023, max compression
```

## Comparing `pixivSpiderCreatedByHanXu-0.0.6.tar` & `pixivSpiderCreatedByHanXu-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2818 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1845 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.360945 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/
--rw-rw-rw-   0        0        0    11319 2023-04-26 10:23:15.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.370946 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/
--rw-rw-rw-   0        0        0     2818 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-26 10:28:32.000000 pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 10:28:32.374349 pixivSpiderCreatedByHanXu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     4308 2023-04-26 10:28:29.000000 pixivSpiderCreatedByHanXu-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 10:28:32.373340 pixivSpiderCreatedByHanXu-0.0.6/tests/
--rw-rw-rw-   0        0        0      991 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/tests/test.py
--rw-rw-rw-   0        0        0       83 2023-04-26 10:08:28.000000 pixivSpiderCreatedByHanXu-0.0.6/tests/test2.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:41:35.039323 pixivSpiderCreatedByHanXu-0.0.7/
+-rw-rw-rw-   0        0        0     1090 2023-06-16 14:24:24.000000 pixivSpiderCreatedByHanXu-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     2818 2023-06-16 14:41:35.039323 pixivSpiderCreatedByHanXu-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1845 2023-06-16 14:24:24.000000 pixivSpiderCreatedByHanXu-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 14:41:35.020323 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu/
+-rw-rw-rw-   0        0        0    11525 2023-06-16 14:35:22.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:41:35.036323 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/
+-rw-rw-rw-   0        0        0     2818 2023-06-16 14:41:34.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-16 14:41:34.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 14:41:34.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 14:41:34.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-06-16 14:41:34.000000 pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 14:41:35.039323 pixivSpiderCreatedByHanXu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     4308 2023-06-16 14:41:08.000000 pixivSpiderCreatedByHanXu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:41:35.038324 pixivSpiderCreatedByHanXu-0.0.7/tests/
+-rw-rw-rw-   0        0        0      991 2023-06-16 14:24:24.000000 pixivSpiderCreatedByHanXu-0.0.7/tests/test.py
+-rw-rw-rw-   0        0        0       83 2023-06-16 14:24:24.000000 pixivSpiderCreatedByHanXu-0.0.7/tests/test2.py
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/LICENSE` & `pixivSpiderCreatedByHanXu-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package can crawl the images at pixiv in two ways.
 Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/README.md` & `pixivSpiderCreatedByHanXu-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu/__init__.py` & `pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,17 @@
                 print("It seems that you have typed in a wrong answer.Please try again.")
 
         self.path = input("type in the path where you want to reserve the images:\n")
         self.headers = {
             'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.48',
             "referer": "https://www.pixiv.net/",
         }
-        self.maximages = eval(input("Type in the number of images you want:\n"))
+
+        self.maximages = int(input("Type in the number of images you want:\n"))
+
 
         if (self.searchTarget == "1"):
             DateMode_dict = {"1": "daily", "2": "weekly", "3": "monthly", "4": "rookie", "5": "daily_ai", "6": "male",
                              "7": "female"}
             print(DateMode_dict)
             DateMode = ""
             while (True):
@@ -80,28 +82,35 @@
 
             self.paginator = int(self.maximages / 50) + 1
             self.date = input("Type in the date you want to search.Follow the format like this:20230423\n")
             self.url_front = "https://www.pixiv.net/ranking.php?mode={}&date={}&format=json&p=".format(DateMode,
                                                                                                        self.date)
 
         elif (self.searchTarget == "2"):
-            heat_dic = {"1": "500", "2": "1000", "3": "5000", "4": "10000", }
+            heat_dic = {"0":"0","1": "500", "2": "1000", "3": "5000", "4": "10000", }
             print(heat_dic)
             heat_require = ""
             while (True):
                 DateMode_key = input("Type in the requirement of heat.Larger the number is,Less the results are.\n")
                 if (DateMode_key in heat_dic):
                     heat_require = heat_dic[DateMode_key]
                     break
                 else:
                     print("It seems that you have typed in a wrong answer.Please try again.")
 
             self.url_front = "https://www.pixiv.net/ajax/search/artworks/"
             self.paginator = int(self.maximages / 60) + 1
-            self.keyword = input("type in the keywords used to search in pixiv:\n") + " " + heat_require + "users入り"
+
+            self.keyword = input("type in the keywords used to search in pixiv:\n")
+            while(True):
+                if (heat_require=="0"):
+                    break
+                else:
+                    self.keyword = self.keyword + " " + heat_require + "users入り"
+                    break
 
     def get_urls(self):
         """
         @:brief Get the URLs that you need to visit.
         @:return return a list of the URLs
         """
         urls = []
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO` & `pixivSpiderCreatedByHanXu-0.0.7/pixivSpiderCreatedByHanXu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixivSpiderCreatedByHanXu
-Version: 0.0.6
+Version: 0.0.7
 Summary: This package can crawl the images at pixiv in two ways.
 Home-page: https://gitee.com/UnderTurrets/pixiv-spider
 Author: Han Xu
 Author-email: 736946693@qq.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/setup.py` & `pixivSpiderCreatedByHanXu-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
 
     #如果上传时出现ERROR：The user '' isn't allowed to upload to project ''，换个名字，长一点无所谓，不能跟别人重复
     name="pixivSpiderCreatedByHanXu",
-    version="0.0.6",
+    version="0.0.7",
     author="Han Xu",
     author_email="736946693@qq.com",
     description="This package can crawl the images at pixiv in two ways.",
 
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

### Comparing `pixivSpiderCreatedByHanXu-0.0.6/tests/test.py` & `pixivSpiderCreatedByHanXu-0.0.7/tests/test.py`

 * *Files identical despite different names*

