# Comparing `tmp/tt_wizard_core-0.1.1b0.tar.gz` & `tmp/tt_wizard_core-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tt_wizard_core-0.1.1b0.tar", last modified: Fri Jun  9 10:44:20 2023, max compression
+gzip compressed data, was "tt_wizard_core-1.0.0rc1.tar", last modified: Fri Jun 16 15:51:24 2023, max compression
```

## Comparing `tt_wizard_core-0.1.1b0.tar` & `tt_wizard_core-1.0.0rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1853 2023-06-09 10:36:29.000000 tt_wizard_core-0.1.1b0/Example.py
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)    35129 2023-06-02 16:17:46.000000 tt_wizard_core-0.1.1b0/LICENSE
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       84 2023-06-02 11:53:29.000000 tt_wizard_core-0.1.1b0/MANIFEST.in
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4513 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/PKG-INFO
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3521 2023-06-09 10:42:12.000000 tt_wizard_core-0.1.1b0/README.md
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       38 2023-06-09 10:44:20.483319 tt_wizard_core-0.1.1b0/setup.cfg
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1479 2023-06-09 10:39:31.000000 tt_wizard_core-0.1.1b0/setup.py
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.481319 tt_wizard_core-0.1.1b0/src/
-drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-09 10:44:20.482319 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4513 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/PKG-INFO
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)      280 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/SOURCES.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)        1 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/dependency_links.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       17 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/requires.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       15 2023-06-09 10:44:20.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/top_level.txt
--rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     7342 2023-06-09 10:09:31.000000 tt_wizard_core-0.1.1b0/src/tt_wizard_core.py
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-16 15:51:24.714991 tt_wizard_core-1.0.0rc1/
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1856 2023-06-16 15:18:20.000000 tt_wizard_core-1.0.0rc1/Example.py
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)    35129 2023-06-02 16:17:46.000000 tt_wizard_core-1.0.0rc1/LICENSE
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       84 2023-06-02 11:53:29.000000 tt_wizard_core-1.0.0rc1/MANIFEST.in
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4536 2023-06-16 15:51:24.714991 tt_wizard_core-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     3544 2023-06-16 15:21:54.000000 tt_wizard_core-1.0.0rc1/README.md
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       38 2023-06-16 15:51:24.714991 tt_wizard_core-1.0.0rc1/setup.cfg
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     1496 2023-06-16 15:41:40.000000 tt_wizard_core-1.0.0rc1/setup.py
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-16 15:51:24.712991 tt_wizard_core-1.0.0rc1/src/
+drwxr-xr-x   0 bumblebee  (1000) bumblebee  (1000)        0 2023-06-16 15:51:24.713991 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     4536 2023-06-16 15:51:24.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/PKG-INFO
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)      280 2023-06-16 15:51:24.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)        1 2023-06-16 15:51:24.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       31 2023-06-16 15:51:24.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/requires.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)       15 2023-06-16 15:51:24.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/top_level.txt
+-rw-r--r--   0 bumblebee  (1000) bumblebee  (1000)     7845 2023-06-16 15:49:02.000000 tt_wizard_core-1.0.0rc1/src/tt_wizard_core.py
```

### Comparing `tt_wizard_core-0.1.1b0/Example.py` & `tt_wizard_core-1.0.0rc1/Example.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 #from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
 from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
-# Create an tt_wizard_core object and provide it with the path to your pen,
-# otherwise the current directory is used.
+# Create an tt_wizard_core object and try to auto dectect pen
 # A list of all available media files is downloaded automatically.
-print("What is the path to your TipToi pen?")
-penPath = str(input())
-ttwiz = tt_wizard_core(penPath)
-#if len(penPath) < 1:
-#    penPath = ""
-#    ttwiz = tt_wizard_core()
+ttwiz = tt_wizard_core()
+if ttwiz.autoDetectPenMountPoint() is False:
+    # If pen is not detected automatically, set mount point manually.
+    print("What is the path to your TipToi pen?")
+    ttwiz.setPenMountPoint(str(input()))
 
 # Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
```

### Comparing `tt_wizard_core-0.1.1b0/LICENSE` & `tt_wizard_core-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `tt_wizard_core-0.1.1b0/PKG-INFO` & `tt_wizard_core-1.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tt_wizard_core
-Version: 0.1.1b0
+Version: 1.0.0rc1
 Summary: Tool to download and manage gme-files. Core of TT_WIZARD.
 Home-page: https://github.com/BumblebeeMan/tt_wizard_core
 Author: BumblebeeMan (Dennis Schweer)
 Author-email: dennis@bumblebeeman.engineer
 Keywords: TipToi,TipTio,tip,toi,tio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,17 +27,18 @@
 This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
 - Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
 - Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
 - Auto update of media files that are already loaded to the TipToi pen
+- Auto detect of pen mount point (tests ongoing)
 
 ## Planned features
-- Auto detect of pen mount point
+n/a
 
 ## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
@@ -52,23 +53,21 @@
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
 #from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
-# Create an tt_wizard_core object and provide it with the path to your pen,
-# otherwise the current directory is used.
+# Create an tt_wizard_core object and try to auto dectect pen
 # A list of all available media files is downloaded automatically.
-print("What is the path to your TipToi pen?")
-penPath = str(input())
-ttwiz = tt_wizard_core(penPath)
-#if len(penPath) < 1:
-#    penPath = ""
-#    ttwiz = tt_wizard_core()
+ttwiz = tt_wizard_core()
+if ttwiz.autoDetectPenMountPoint() is False:
+    # If pen is not detected automatically, set mount point manually.
+    print("What is the path to your TipToi pen?")
+    ttwiz.setPenMountPoint(str(input()))
 
 # Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
```

### Comparing `tt_wizard_core-0.1.1b0/README.md` & `tt_wizard_core-1.0.0rc1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
 - Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
 - Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
 - Auto update of media files that are already loaded to the TipToi pen
+- Auto detect of pen mount point (tests ongoing)
 
 ## Planned features
-- Auto detect of pen mount point
+n/a
 
 ## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
@@ -28,23 +29,21 @@
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
 #from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
-# Create an tt_wizard_core object and provide it with the path to your pen,
-# otherwise the current directory is used.
+# Create an tt_wizard_core object and try to auto dectect pen
 # A list of all available media files is downloaded automatically.
-print("What is the path to your TipToi pen?")
-penPath = str(input())
-ttwiz = tt_wizard_core(penPath)
-#if len(penPath) < 1:
-#    penPath = ""
-#    ttwiz = tt_wizard_core()
+ttwiz = tt_wizard_core()
+if ttwiz.autoDetectPenMountPoint() is False:
+    # If pen is not detected automatically, set mount point manually.
+    print("What is the path to your TipToi pen?")
+    ttwiz.setPenMountPoint(str(input()))
 
 # Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
```

### Comparing `tt_wizard_core-0.1.1b0/setup.py` & `tt_wizard_core-1.0.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name = 'tt_wizard_core',
-    version = '0.1.1-beta',
+    version = '1.0.0-rc1',
     description = 'Tool to download and manage gme-files. Core of TT_WIZARD.',
     long_description = long_description,
     long_description_content_type='text/markdown',
 
     py_modules = ["tt_wizard_core"],
     package_dir = {'': 'src'},
 
     author="BumblebeeMan (Dennis Schweer)", 
     author_email="dennis@bumblebeeman.engineer",     
     url="https://github.com/BumblebeeMan/tt_wizard_core",
 
-    install_requires=["requests >= 2.30.0"],
+    install_requires=["requests >= 2.30.0", "psutil >= 5.9.0"],
 
     python_requires=">=3.7",
 
     keywords=["TipToi", "TipTio", "tip", "toi", "tio"],
 
-    classifiers=["Development Status :: 3 - Alpha",
+    classifiers=["Development Status :: 4 - Beta",
                  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
                  "Operating System :: OS Independent",
                  "Programming Language :: Python :: 3",
                  "Programming Language :: Python :: 3 :: Only",
                  "Programming Language :: Python :: 3.7",
                  "Programming Language :: Python :: 3.8",
                  "Programming Language :: Python :: 3.9",
```

### Comparing `tt_wizard_core-0.1.1b0/src/tt_wizard_core.egg-info/PKG-INFO` & `tt_wizard_core-1.0.0rc1/src/tt_wizard_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: tt-wizard-core
-Version: 0.1.1b0
+Version: 1.0.0rc1
 Summary: Tool to download and manage gme-files. Core of TT_WIZARD.
 Home-page: https://github.com/BumblebeeMan/tt_wizard_core
 Author: BumblebeeMan (Dennis Schweer)
 Author-email: dennis@bumblebeeman.engineer
 Keywords: TipToi,TipTio,tip,toi,tio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -27,17 +27,18 @@
 This projects provides an operating system independent backend to download and manage *.gme-files / audio files for the TipToi pen sold by Ravensburger. By removing the hassle to deal with file versioning and download servers, it especially enables the creation of tools for operating systems that are currently not officially supported by the manufacturer itself (like Linux). **TT_WIZARD_CORE** only uses the official servers (i.e. hosted by the manufacturer) to download any media files! 
 
 ## Following operations are currently supported:
 - Searching the names of all currently published TipToi media for a keyword (e.g. "puzzle" to get all puzzles listed).
 - Picking and downloading selected media from the search results above.
 - Checking whether an already downloaded media file needs an update or not. (Attention: Files without recent updates may be flagged to require an update, even though no newer versions are available. This is a known issue.) 
 - Auto update of media files that are already loaded to the TipToi pen
+- Auto detect of pen mount point (tests ongoing)
 
 ## Planned features
-- Auto detect of pen mount point
+n/a
 
 ## Installation of released version
 
 Use pip to install:
 
 ```python
 pip install tt_wizard_core
@@ -52,23 +53,21 @@
 from tt_wizard_core import tt_wizard_core
 
 # if not installed using pip and using source code
 #from src.tt_wizard_core import tt_wizard_core
 
 print("Welcome to an example of TT_WIZARD_CORE!")
 
-# Create an tt_wizard_core object and provide it with the path to your pen,
-# otherwise the current directory is used.
+# Create an tt_wizard_core object and try to auto dectect pen
 # A list of all available media files is downloaded automatically.
-print("What is the path to your TipToi pen?")
-penPath = str(input())
-ttwiz = tt_wizard_core(penPath)
-#if len(penPath) < 1:
-#    penPath = ""
-#    ttwiz = tt_wizard_core()
+ttwiz = tt_wizard_core()
+if ttwiz.autoDetectPenMountPoint() is False:
+    # If pen is not detected automatically, set mount point manually.
+    print("What is the path to your TipToi pen?")
+    ttwiz.setPenMountPoint(str(input()))
 
 # Provide a string to search in the list of available media. 
 print("Please enter keyword to search avaiable media for: ")
 keyword = str(input())
 
 # Search for string and receive a python list of media titles that partially match.
 print("Found following media:")
```

### Comparing `tt_wizard_core-0.1.1b0/src/tt_wizard_core.py` & `tt_wizard_core-1.0.0rc1/src/tt_wizard_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,67 +11,88 @@
             "User-Agent": "Chrome/33.0.1750.152",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,*/*;q=0.8",
             "Cache-Control": "max-age=0",
             "Connection": "keep-alive"}
 
     __mediaDict = {}
 
-    __downloadPath = ""
+    __mediaNameList = []
 
-    def __init__(self, downloadPath = ""):
-        """ __init__(self, downloadPath = "")
+    __penMountPoint = ""
+
+    def __init__(self, penMountPoint = ""):
+        """
         Contructor.
 
         (optional) param: String. Specifies path to storage location of gme files.
         """
-        self.__downloadPath = downloadPath
+        self.__penMountPoint = penMountPoint
         self.__mediaDict = {}
-        self.__getAvailableMedia(self.__LIST_PATH)
+        self.__loadAvailableMedia(self.__LIST_PATH)
 
-    def __getAvailableMedia(self, path):
+    def __loadAvailableMedia(self, path):
         """ 
         Downloads csv of available gme-files from __LIST_PATH and decodes them into a dictionary, where title name is used as key.
         """
         response = self.requests.get(path, headers=self.__HEADER__)
         lines = response.content.splitlines()
         response.close()
-        self.__mediaList = []
         for line in lines:
             entries = line.decode('ISO-8859-1').split(',')
             url = entries[2]
             name = entries[3]
             if ".gme" in url:
                 id = int(entries[0])
                 version = int(entries[1])
                 qualifiedName = (name + ".gme")
+                self.__mediaNameList.append(qualifiedName)
                 self.__mediaDict[qualifiedName] = (qualifiedName, url, id, version)
     
     def __isDateString(self, dataBytes, position):
         """
         Checks whether >>position<< is located at the end of 8 ASCII integers (i.e. the timestamp) or not.
 
         return: True/False
         """
         for index in range(position, position - 8, -1):
             if (dataBytes[index] >= 58) or (dataBytes[index] < 48):
                 return False
-        return True
+        return True 
+
+    def autoDetectPenMountPoint(self):
+        """
+        Tries to find mount point of pen. If mount point is found, __penMountPoint is set to mount point path and True returned.
+
+        return: True -- Bool. Mountpoint found.
+                False -- Bool. Mountpoint NOT found.
+        """
+        import psutil
+        for disk in psutil.disk_partitions():
+            mnt = str(disk.mountpoint) + "/"
+            if "tiptoi" in mnt.lower():
+                self.__penMountPoint = mnt
+                return True
+        return False
+
+    def setPenMountPoint(self, penMountPoint = ""):
+        """ 
+        Overwrites path to pen / download location. For example, to be used when auto detection fails.
+
+        param: >>penMountPoint<< -- String. New path value.
+        return: None
+        """
+        self.__penMountPoint = penMountPoint
 
     def getAllAvailableTitles(self):
         """ 
         Return list of all titles that are available for download.
 
         return: [] -- List of String. List of titles (i.e. fileName + ".gme") that can be downloaded.
         """
-        result = []
-        for item in self.__mediaDict.keys():
-            qualifiedName, url, id, version = self.__mediaDict[item] 
-            result.append(qualifiedName)
-        return result
-
+        return self.__mediaNameList
     
     def searchEntry(self, searchString):
         """ 
         Search available media files for specified keyword.
 
         param: >>searchString<< -- String. Keyword to be searched in available titles.
         return: a.) [] -- Empty list if string is NOT found in any title.
@@ -89,34 +110,33 @@
         Downloads media files into specified folder location.
 
         param1: [fileNames] -- List of Strings. File name of title that shall be downloaded to specified path.
         param2: >>filePath<< -- (Optional) String. Path to download location.
         return: No return value.
         """
         if filePath is None:
-            path = self.__downloadPath
+            path = self.__penMountPoint
         else:
             path = filePath
         for title in fileNameList:
             (qualifiedName, url, id, versionRemote) = self.__mediaDict[title]
-            print(f"Downloading: {qualifiedName}")
             response = self.requests.get(url, headers=self.__HEADER__)
             open((path + title), 'wb+').write(response.content)
 
     def checkForUpdate(self, fileName, filePath=None):
         """
         Checks whether an update for title named >>fileName<<, which is stored at location >>filePath<<, is required or not.
 
         param1: >>fileName<< -- String. Name of file to check its update status.
         param2: >>filePath<< -- (Optional) String. Path to storage location of gme-files.
         return: TRUE -- Update is required.
                 FALSE -- Update is NOT required.
         """ 
         if filePath is None:
-            path = self.__downloadPath
+            path = self.__penMountPoint
         else:
             path = filePath
             
         with open((path + fileName), mode='rb') as file:
             fileContent = file.read()
         # search end of timestamp
         dataString = "CopyRight"
@@ -138,16 +158,14 @@
                       ((fileContent[endOfVersion - 6] - 48) * 1000000) + \
                       ((fileContent[endOfVersion - 7] - 48) * 10000000)
         (qualifiedName, url, id, versionRemote) = self.__mediaDict[fileName]
         # Theoretically updates should only be required, when versionRemote > versionLocal
         # but we are choosing the currently hosted version to be the golden master.
         # Hence, whenever a version mismatch is detected, an update is suggested. 
         if versionRemote != versionLocal:
-            print(f"Medium: {fileName} = Local Version: {versionLocal} vs. Remote Version: {versionRemote}")
-            print("Type: " + str(type(fileContent)))
             return True
         else:
             return False
 
     def performAutoUpdate(self, filePath=None, dryRun=False):
         """ 
         Iterates through all downloaded gme-files and updates all that are outdated
@@ -157,15 +175,15 @@
                 If >>true<<: Evaluate which files require an update only (without downloading the updates). 
                 If >>False<<: Perform evaluation and OVERWRITE old files with their update (default).
         return: a.) [] -- Empty list if no titles was updated.
                 b.) [] -- List of all titles that received an update.
         """
         from os import listdir
         if filePath is None:
-            path = self.__downloadPath
+            path = self.__penMountPoint
         else:
             path = filePath
 
         gmeFiles = [gme for gme in listdir(path) if "gme" in gme]
         updatedFiles = []
 
         for title in gmeFiles:
```

