# Comparing `tmp/sponsorblock.py-0.2.2.tar.gz` & `tmp/sponsorblock.py-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sponsorblock.py-0.2.2.tar", last modified: Sat Apr 16 03:16:04 2022, max compression
+gzip compressed data, was "sponsorblock.py-0.2.3.tar", last modified: Fri Jun 16 08:37:13 2023, max compression
```

## Comparing `sponsorblock.py-0.2.2.tar` & `sponsorblock.py-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.893172 sponsorblock.py-0.2.2/
--rw-rw-rw-   0        0        0       66 2021-08-23 17:06:28.000000 sponsorblock.py-0.2.2/.gitattributes
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.839681 sponsorblock.py-0.2.2/.github/
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.867787 sponsorblock.py-0.2.2/.github/workflows/
--rw-rw-rw-   0        0        0     1096 2021-09-12 15:11:02.000000 sponsorblock.py-0.2.2/.github/workflows/python-publish.yml
--rw-rw-rw-   0        0        0     1499 2021-08-23 17:08:18.000000 sponsorblock.py-0.2.2/.gitignore
--rw-rw-rw-   0        0        0      515 2021-08-26 07:16:30.000000 sponsorblock.py-0.2.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2021-08-23 17:06:28.000000 sponsorblock.py-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     7962 2022-04-16 03:16:04.893172 sponsorblock.py-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6899 2022-01-19 16:43:27.000000 sponsorblock.py-0.2.2/README.md
--rw-rw-rw-   0        0        0     1064 2022-01-19 17:28:51.000000 sponsorblock.py-0.2.2/TODO.md
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.873827 sponsorblock.py-0.2.2/docs/
--rw-rw-rw-   0        0        0     1136 2022-04-16 03:13:52.000000 sponsorblock.py-0.2.2/docs/api_reference.rst
--rw-rw-rw-   0        0        0     2021 2022-04-16 03:13:52.000000 sponsorblock.py-0.2.2/docs/conf.py
--rw-rw-rw-   0        0        0     1708 2022-04-16 03:13:52.000000 sponsorblock.py-0.2.2/docs/index.rst
--rw-rw-rw-   0        0        0       15 2021-08-26 07:28:09.000000 sponsorblock.py-0.2.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.874825 sponsorblock.py-0.2.2/images/
--rw-rw-rw-   0        0        0   244938 2021-10-07 18:13:39.000000 sponsorblock.py-0.2.2/images/logo.png
--rw-rw-rw-   0        0        0      362 2021-08-25 16:51:46.000000 sponsorblock.py-0.2.2/pylama.ini
--rw-rw-rw-   0        0        0       52 2022-04-16 03:13:52.000000 sponsorblock.py-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0     1227 2022-04-16 03:16:04.894172 sponsorblock.py-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-11-07 14:49:52.000000 sponsorblock.py-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.884369 sponsorblock.py-0.2.2/sponsorblock/
--rw-rw-rw-   0        0        0      474 2022-04-16 03:15:17.000000 sponsorblock.py-0.2.2/sponsorblock/__init__.py
--rw-rw-rw-   0        0        0     1934 2022-01-19 17:39:05.000000 sponsorblock.py-0.2.2/sponsorblock/__main__.py
--rw-rw-rw-   0        0        0    46021 2022-04-16 03:14:23.000000 sponsorblock.py-0.2.2/sponsorblock/client.py
--rw-rw-rw-   0        0        0        0 2022-01-27 06:07:55.000000 sponsorblock.py-0.2.2/sponsorblock/database.py
--rw-rw-rw-   0        0        0     1132 2021-08-25 17:06:03.000000 sponsorblock.py-0.2.2/sponsorblock/errors.py
--rw-rw-rw-   0        0        0    10382 2022-01-19 17:52:36.000000 sponsorblock.py-0.2.2/sponsorblock/models.py
--rw-rw-rw-   0        0        0     4023 2022-04-16 03:13:52.000000 sponsorblock.py-0.2.2/sponsorblock/utils.py
-drwxrwxrwx   0        0        0        0 2022-04-16 03:16:04.892170 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/
--rw-rw-rw-   0        0        0     7962 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       54 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-04-16 03:16:04.000000 sponsorblock.py-0.2.2/sponsorblock.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 08:37:13.862419 sponsorblock.py-0.2.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     7956 2023-06-16 08:37:13.862419 sponsorblock.py-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/README.md
+-rw-rw-rw-   0        0        0     1227 2023-06-16 08:37:13.863921 sponsorblock.py-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:37:13.853831 sponsorblock.py-0.2.3/sponsorblock/
+-rw-rw-rw-   0        0        0      474 2023-06-16 08:32:52.000000 sponsorblock.py-0.2.3/sponsorblock/__init__.py
+-rw-rw-rw-   0        0        0     1934 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/__main__.py
+-rw-rw-rw-   0        0        0    40631 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/client.py
+-rw-rw-rw-   0        0        0       45 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/database.py
+-rw-rw-rw-   0        0        0     1481 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/errors.py
+-rw-rw-rw-   0        0        0    10444 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/models.py
+-rw-rw-rw-   0        0        0     4023 2023-06-16 08:31:46.000000 sponsorblock.py-0.2.3/sponsorblock/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:37:13.860921 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/
+-rw-rw-rw-   0        0        0     7956 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       54 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-16 08:37:13.000000 sponsorblock.py-0.2.3/sponsorblock.py.egg-info/top_level.txt
```

### Comparing `sponsorblock.py-0.2.2/LICENSE` & `sponsorblock.py-0.2.3/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `sponsorblock.py-0.2.2/PKG-INFO` & `sponsorblock.py-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sponsorblock.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: An unofficial wrapper for the SponsorBlock API
 Home-page: https://wasi-master.github.io/sponsorblock.py/
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Keywords: sponsorblock.py,documentation,sponsorblock,python,api,wrapper,sponsor,block,youtube,youtube-dl,youtube-dlp
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -147,15 +146,21 @@
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 See the [documentation](https://sponsorblockpy.readthedocs.io/en/latest/)
 
 There is also a cli that you can use to get segments from the command line (beta).\
-To use that run `sponsorblock video_id` and pass your desired video_id
+To use that run:
+
+```sh
+sponsorblock video_id
+```
+
+and pass your desired video_id
 
 ## Roadmap
 
 See the [todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of features yet to be added and features already added.
 Also see the [open issues](https://github.com/wasi-master/sponsorblock.py/issues) for issues.
 
 <!-- CONTRIBUTING -->
@@ -178,9 +183,7 @@
 ## Contact
 
 Project Link: [https://github.com/wasi-master/sponsorblock.py](https://github.com/wasi-master/sponsorblock.py)
 
 Discord: [Wasi Master#6969](https://discord.com/users/723234115746398219)
 
 Email: [arianmollik323@gmail.com](mailto:arianmollik323@gmail.com)
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: sponsorblock.py Version: 0.2.2 Summary: An
+Metadata-Version: 2.1 Name: sponsorblock.py Version: 0.2.3 Summary: An
 unofficial wrapper for the SponsorBlock API Home-page: https://wasi-
 master.github.io/sponsorblock.py/ Author: Wasi Master Author-email:
 arianmollik323@gmail.com License: MIT Keywords:
 sponsorblock.py,documentation,sponsorblock,python,api,wrapper,sponsor,block,youtube,youtube-
-dl,youtube-dlp Platform: UNKNOWN Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Internet Requires-
-Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
+dl,youtube-dlp Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Internet Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
                           ***** sponsorblock.py *****
                       A wrapper for the SponsorBlock API
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
   [Contributors] [Forks] [Stargazers] [Issues] [Code_Size] [MIT_License] [Say
@@ -43,23 +43,23 @@
 ```sh pip install sponsorblock.py ``` 2. Installing using pip and git ```sh pip
 install git+https://github.com/wasi-master/sponsorblock.py.git ``` * Cloning
 then installing 1. Clone the repo ```sh git clone https://github.com/wasi-
 master/sponsorblock.py.git ``` 2. Changing the current working directory to the
 directory of the project ```sh cd sponsorblock.py ``` 3. Install using pip
 ```sh pip install . ```  ## Usage See the [documentation](https://
 sponsorblockpy.readthedocs.io/en/latest/) There is also a cli that you can use
-to get segments from the command line (beta).\ To use that run `sponsorblock
-video_id` and pass your desired video_id ## Roadmap See the [todo list](https:/
-/github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of
-features yet to be added and features already added. Also see the [open issues]
-(https://github.com/wasi-master/sponsorblock.py/issues) for issues.  ##
-Contributing Contributions are what make the open source community such an
-amazing place to be learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
-(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
--m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See [`LICENSE`](LICENSE) for more information.  ## Contact Project
-Link: [https://github.com/wasi-master/sponsorblock.py](https://github.com/wasi-
-master/sponsorblock.py) Discord: [Wasi Master#6969](https://discord.com/users/
-723234115746398219) Email: [arianmollik323@gmail.com](mailto:
+to get segments from the command line (beta).\ To use that run: ```sh
+sponsorblock video_id ``` and pass your desired video_id ## Roadmap See the
+[todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md)
+for a list of features yet to be added and features already added. Also see the
+[open issues](https://github.com/wasi-master/sponsorblock.py/issues) for
+issues.  ## Contributing Contributions are what make the open source community
+such an amazing place to be learn, inspire, and create. Any contributions you
+make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
+Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
+commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
+feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
+the MIT License. See [`LICENSE`](LICENSE) for more information.  ## Contact
+Project Link: [https://github.com/wasi-master/sponsorblock.py](https://
+github.com/wasi-master/sponsorblock.py) Discord: [Wasi Master#6969](https://
+discord.com/users/723234115746398219) Email: [arianmollik323@gmail.com](mailto:
 arianmollik323@gmail.com)
```

### Comparing `sponsorblock.py-0.2.2/README.md` & `sponsorblock.py-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,21 @@
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 See the [documentation](https://sponsorblockpy.readthedocs.io/en/latest/)
 
 There is also a cli that you can use to get segments from the command line (beta).\
-To use that run `sponsorblock video_id` and pass your desired video_id
+To use that run:
+
+```sh
+sponsorblock video_id
+```
+
+and pass your desired video_id
 
 ## Roadmap
 
 See the [todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of features yet to be added and features already added.
 Also see the [open issues](https://github.com/wasi-master/sponsorblock.py/issues) for issues.
 
 <!-- CONTRIBUTING -->
```

#### html2text {}

```diff
@@ -30,23 +30,23 @@
 ```sh pip install sponsorblock.py ``` 2. Installing using pip and git ```sh pip
 install git+https://github.com/wasi-master/sponsorblock.py.git ``` * Cloning
 then installing 1. Clone the repo ```sh git clone https://github.com/wasi-
 master/sponsorblock.py.git ``` 2. Changing the current working directory to the
 directory of the project ```sh cd sponsorblock.py ``` 3. Install using pip
 ```sh pip install . ```  ## Usage See the [documentation](https://
 sponsorblockpy.readthedocs.io/en/latest/) There is also a cli that you can use
-to get segments from the command line (beta).\ To use that run `sponsorblock
-video_id` and pass your desired video_id ## Roadmap See the [todo list](https:/
-/github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of
-features yet to be added and features already added. Also see the [open issues]
-(https://github.com/wasi-master/sponsorblock.py/issues) for issues.  ##
-Contributing Contributions are what make the open source community such an
-amazing place to be learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
-(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
--m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See [`LICENSE`](LICENSE) for more information.  ## Contact Project
-Link: [https://github.com/wasi-master/sponsorblock.py](https://github.com/wasi-
-master/sponsorblock.py) Discord: [Wasi Master#6969](https://discord.com/users/
-723234115746398219) Email: [arianmollik323@gmail.com](mailto:
+to get segments from the command line (beta).\ To use that run: ```sh
+sponsorblock video_id ``` and pass your desired video_id ## Roadmap See the
+[todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md)
+for a list of features yet to be added and features already added. Also see the
+[open issues](https://github.com/wasi-master/sponsorblock.py/issues) for
+issues.  ## Contributing Contributions are what make the open source community
+such an amazing place to be learn, inspire, and create. Any contributions you
+make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
+Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
+commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
+feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
+the MIT License. See [`LICENSE`](LICENSE) for more information.  ## Contact
+Project Link: [https://github.com/wasi-master/sponsorblock.py](https://
+github.com/wasi-master/sponsorblock.py) Discord: [Wasi Master#6969](https://
+discord.com/users/723234115746398219) Email: [arianmollik323@gmail.com](mailto:
 arianmollik323@gmail.com)
```

### Comparing `sponsorblock.py-0.2.2/setup.cfg` & `sponsorblock.py-0.2.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 706f 6e73 6f72 626c 6f63 6b2e   = sponsorblock.
 00000020: 7079 0d0a 7665 7273 696f 6e20 3d20 302e  py..version = 0.
-00000030: 322e 320d 0a64 6573 6372 6970 7469 6f6e  2.2..description
+00000030: 322e 330d 0a64 6573 6372 6970 7469 6f6e  2.3..description
 00000040: 203d 2041 6e20 756e 6f66 6669 6369 616c   = An unofficial
 00000050: 2077 7261 7070 6572 2066 6f72 2074 6865   wrapper for the
 00000060: 2053 706f 6e73 6f72 426c 6f63 6b20 4150   SponsorBlock AP
 00000070: 490d 0a6c 6f6e 675f 6465 7363 7269 7074  I..long_descript
 00000080: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
 00000090: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 000000a0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
```

### Comparing `sponsorblock.py-0.2.2/sponsorblock/__main__.py` & `sponsorblock.py-0.2.3/sponsorblock/__main__.py`

 * *Files identical despite different names*

### Comparing `sponsorblock.py-0.2.2/sponsorblock/client.py` & `sponsorblock.py-0.2.3/sponsorblock/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,52 @@
     set_env_var,
     cache,
     Singleton,
     __version__,
 )
 
 
+def raise_request_exception(response: requests.Response):
+    """
+    If the server returns a status code, which is not 200,
+    it needs to raise an exception:
+
+    Every exception inherits from HTTPException
+
+    :param response:
+    :return:
+    """
+    code = response.status_code
+
+    if code == 200:
+        return
+
+    if code == 400:
+        raise BadRequest("Your inputs are wrong/impossible", response)
+
+    if code == 403:
+        raise Forbidden("Rejected by auto moderator", response)
+
+    if code == 429:
+        raise RateLimitException("Rate Limit (Too many for the same user or IP)", response)
+
+    if code == 409:
+        raise DuplicateException("Duplicate", response)
+
+    if code == 404:
+        raise NotFoundException("Not Found", response)
+
+    if code > 500:
+        raise ServerException("Server Error", response)
+
+    raise UnexpectedException(
+        "Unexpected response from server", response
+    )
+
+
 class Client(metaclass=Singleton):
     """A client for making requests to the sponsorblock server."""
 
     def __init__(
         self,
         user_id=None,
         *,
@@ -81,14 +119,15 @@
             else:
                 self.user_id = user_id or secrets.token_hex(32)
                 set_env_var("SPONSORBLOCK_USER_ID", user_id)
         self.debug = debug
         self.default_categories = default_categories or ALL_CATEGORIES
         self.hash_length = hashed_video_id_length
         self.session = session or requests.Session()
+        self.session.headers.update({"Content-Type": "application/json"})
 
     @cache(ttl=300)  # 5 minutes
     def get_skip_segments(
         self,
         video_id: str,
         *,
         category: Category = None,
@@ -170,39 +209,29 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return [Segment.from_dict(d) for d in data]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 400:
-                    raise BadRequest("Your inputs are wrong/impossible", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=300)  # 5 minutes
     def get_skip_segments_with_hash(
         self,
         video_id: str ,
         video_hash: str = None,
         *,
         category: Category = None,
         categories: List[str] = None,
         required_segments: List[str] = None,
         service: str = "YouTube",
     ) -> List[Segment]:
-        """Gets the skip segments for a given video using a K-Anonymity system.
+        """
+        Gets the skip segments for a given video using a K-Anonymity system.
 
         Parameters
         ----------
         video_id : str
             The id of the video to get the skip segments for, can be a video url too.
         video_hash : str
             The sha256 hash of the id of the video to get the skip segments for, if not given uses video_id to generate a hash with the length 32.
@@ -291,26 +320,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return [Segment.from_dict(d) for d in data]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 400:
-                    raise BadRequest("Your inputs are wrong/impossible", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     def add_skip_segments(
         self,
         video_id: str,
         *,
         segment: Segment = None,
         segments: List[Segment] = None,
@@ -385,30 +403,15 @@
                     "category": segment.category,
                 }
                 for segment in segments
             ],
         }
         url = self.base_url + "/api/skipSegments"
         response = self.session.post(url, data=body)
-        code = response.status_code
-        if code != 200:
-            if code == 400:
-                raise BadRequest("Your inputs are wrong/impossible", response)
-            if code == 403:
-                raise Forbidden("Rejected by auto moderator", response)
-            if code == 429:
-                raise RateLimitException(
-                    "Rate Limit (Too many for the same user or IP)", response
-                )
-            if code == 409:
-                raise DuplicateException("Duplicate", response)
-            if code > 500:
-                raise ServerException("Server Error", response)
-            else:
-                raise UnexpectedException("Unexpected response from server", response)
+        raise_request_exception(response)
 
     def vote_skip_segment(
         self,
         uuid: Union[Segment, str],
         *,
         vote: Union[str, int, bool] = None,
         category: Category = None,
@@ -416,15 +419,18 @@
         """Votes on a skip segment.
 
         Parameters
         ----------
         uuid : Union[Segment, str]
             segment or uuid of the segment being voted on
         vote : Union[str, int, bool], optional
-            The vote to vote on the skip segment. Can be truthy or falsey or even basic english, by default None
+            The vote to vote on the skip segment.
+            Can be any of ``yes``, ``upvote``, ``up``, ``good``, ``1``, ``True`` for upvoting,
+            ``no``, ``downvote``, ``down``, ``bad``, ``0``, ``False`` for downvoting,
+            and ``undo`` for undoing a given vote
         category : Category, optional
             The category of the skip segment. This can be used as an alternative to the vote parameter, by default None
 
         Raises
         ------
         ValueError
             You passed both vote and category.
@@ -444,18 +450,20 @@
         >>> segments = client.get_skip_segments("https://www.youtube.com/watch?v=kJQP7kiw5Fk")
         >>> client.vote_skip_segment(segments[0], 'yes')
         """
 
         if category is None and vote is None:
             raise ValueError("At least one argument is required")
 
-        if vote in ("yes", "upvote", "up", "good", 1, True):
+        if vote in ("yes", "upvote", "up", "good", 1, "1", True, "True"):
             vote = 1
-        elif vote in ("no", "downvote", "down", "bad", 0, False):
+        elif vote in ("no", "downvote", "down", "bad", 0, "0", False, "False"):
             vote = 0
+        elif vote in ("undo", 20):
+            vote = 20
         else:
             vote = int(bool(vote))
 
         parameters = {
             "UUID": uuid.uuid if isinstance(uuid, Segment) else uuid,
             "userID": self.user_id,
         }
@@ -463,24 +471,15 @@
         if vote is not None:
             parameters["type"] = vote
         if category is not None:
             parameters["category"] = category
 
         url = self.base_url + "/api/voteOnSponsorTime"
         response = self.session.post(url, data=parameters)
-        code = response.status_code
-        if code != 200:
-            if code == 400:
-                raise BadRequest("Your inputs are wrong/impossible", response)
-            if code == 403:
-                raise Forbidden("Rejected by auto moderator", response)
-            if code > 500:
-                raise ServerException("Server Error", response)
-            else:
-                raise UnexpectedException("Unexpected response from server", response)
+        raise_request_exception(response)
 
     def post_viewed_video_sponsor_time(self, uuid: Union[Segment, str]):
         """Notifies the server that a segment has been skipped.
 
         Parameters
         ----------
         uuid : Union[Segment, str]
@@ -500,23 +499,17 @@
         >>> import sponsorblock as sb
         >>> client = sb.Client()
         >>> segments = client.get_skip_segments("https://www.youtube.com/watch?v=kJQP7kiw5Fk")
         >>> client.post_viewed_video_sponsor_time(segments[1])
         """
         parameters = {"UUID": uuid.uuid if isinstance(uuid, Segment) else uuid}
         url = self.base_url + "/api/viewedVideoSponsorTime"
+
         response = self.session.post(url, params=parameters)
-        code = response.status_code
-        if code != 200:
-            if code == 400:
-                raise BadRequest("Your inputs are wrong/impossible", response)
-            if code > 500:
-                raise ServerException("Server Error", response)
-            else:
-                raise UnexpectedException("Unexpected response from server", response)
+        raise_request_exception(response)
 
     @cache(ttl=900)  # 15 minutes
     def get_user_info(self, public_userid: str = None) -> User:
         """Gets the user info for the current user.
 
         Parameters
         ----------
@@ -593,26 +586,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return User(data)
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 400:
-                    raise BadRequest("Your inputs are wrong/impossible", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=60)  # a minute
     def get_views_for_user(self):
         """Gets the view count for the current user.
 
         Returns
         -------
@@ -647,24 +629,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return data["viewCount"]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=60)  # a minute
     def get_saved_time_for_user(self):
         """Gets the view count for the current user.
 
         Returns
         -------
@@ -699,24 +672,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return data["timeSaved"]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     def set_user_name(self, user_name: str):
         """Sets the user name for the current user.
 
         Parameters
         ----------
         user_name : str
@@ -740,22 +704,15 @@
         parameters = {
             "userID": self.user_id,
             "username": user_name,
         }
 
         url = self.base_url + "/api/setUsername"
         response = self.session.post(url, data=parameters)
-        code = response.status_code
-        if code != 200:
-            if code == 400:
-                raise BadRequest("Your inputs are wrong/impossible", response)
-            if code > 500:
-                raise ServerException("Server Error", response)
-            else:
-                raise UnexpectedException("Unexpected response from server", response)
+        raise_request_exception(response)
 
     @cache(ttl=60)  # a minute
     def get_user_name(self) -> str:
         """Gets the user name for the current user.
 
         Returns
         -------
@@ -792,26 +749,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return data["userName"]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 400:
-                    raise BadRequest("Your inputs are wrong/impossible", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=3600)  # a minute
     def get_top_users(self, sort_type: SortType) -> List[TopUser]:
         """Gets the top users.
 
         Paremeters
         ----------
@@ -877,24 +823,15 @@
                     data["userNames"],
                     data["viewCounts"],
                     data["totalSubmissions"],
                     data["minutesSaved"],
                 )
             ]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code == 400:
-                    raise BadRequest("Your inputs are wrong/impossible", response)
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=60)  # a minute
     def get_total_stats(self, count_contributing_users: bool = False) -> TotalStats:
         """Gets total stats for the api
 
         Parameters
         ----------
@@ -941,22 +878,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return TotalStats(data)
         finally:
-            code = response.status_code
-            if code != 200:
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(ttl=60)  # a minute
     def get_saved_days_formatted(self) -> float:
         """Returns the amount of days that have been saved.
 
         Returns
         -------
@@ -987,22 +917,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return float(data["daysSaved"])
         finally:
-            code = response.status_code
-            if code != 200:
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(max_entries=300)  # 5 minutes
     def get_segment_info(
         self,
         segment: Union[Segment, str] = None,
         segments: List[Union[Segment, str]] = None,
     ) -> List[SegmentInfo]:
@@ -1083,29 +1006,15 @@
         except json.JSONDecodeError as exc:
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return [SegmentInfo(segment_info) for segment_info in data]
         finally:
-            code = response.status_code
-            if code != 200:
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code == 400:
-                    raise BadRequest(
-                        "Bad Request (Your inputs are wrong/impossible) or exceed the character limits",
-                        response,
-                    )
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
 
     @cache(max_entries=300)  # 5 minutes
     def search_for_user(
         self, user_name: str, exact: bool = False
     ) -> List[SearchedUser]:
         """Searches for a user based on their name.
 
@@ -1154,20 +1063,8 @@
             raise InvalidJSONException(
                 "The server returned invalid JSON", response
             ) from exc
         else:
             return [SearchedUser(d) for d in data]
         finally:
             code = response.status_code
-            if code != 200:
-                if code > 500:
-                    raise ServerException("Server Error", response)
-                if code == 404:
-                    raise NotFoundException("Not Found", response)
-                if code == 400:
-                    raise BadRequest(
-                        "Bad Request (Your inputs are wrong/impossible)", response
-                    )
-                else:
-                    raise UnexpectedException(
-                        "Unexpected response from server", response
-                    )
+            raise_request_exception(response)
```

### Comparing `sponsorblock.py-0.2.2/sponsorblock/errors.py` & `sponsorblock.py-0.2.3/sponsorblock/errors.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,54 @@
+from requests import Response
+
 class InvalidJSONException(Exception):
     """Raised when the JSON gotten from the server is invalid"""
 
     def __init__(self, message, response):
         self.response = response
         super().__init__(f"{message}: {response.text}")
 
 
 class HTTPException(Exception):
     """Raised when the server returns an error code"""
 
-    def __init__(self, message, response):
-        self.response = response
-        super().__init__(f"{message}: {response.status_code} {response.reason}")
+    def __init__(self, message, response: Response):
+        self.response: Response = response
+        super().__init__(f"{message}: {response.status_code} {response.reason} - {response.text}")
+
+    def __str__(self):
+        newline = "\n"
+
+        return f"""
+{super().__str__()}
+{self.response.url} {self.response.url}
+{newline.join(f'{key}: {value}' for key, value in self.response.request.headers.items())}
+{self.response.content}
+        """
 
 
 class Forbidden(HTTPException):
-    """Raised if the status code is 403"""
+    """Raised when the status code is 403."""
 
 
 class BadRequest(HTTPException):
-    """Raised if the status code is 400"""
+    """Raised when the status code is 400."""
 
 
 class NotFoundException(HTTPException):
-    """Raised when the status code is 404"""
+    """Raised when the status code is 404."""
 
 
 class RateLimitException(HTTPException):
-    """Raised when the status code is 429"""
+    """Raised when the status code is 429."""
 
 
 class UnexpectedException(HTTPException):
-    """Raised if an unknown error has occurred."""
+    """Raised when an unknown error has occurred."""
 
 
 class ServerException(HTTPException):
-    """Raised if the status code is bigger than 500"""
+    """Raised if the status code is bigger than 500."""
 
 
 class DuplicateException(HTTPException):
-    """Raised if the status code is 409"""
+    """Raised when the status code is 409."""
```

### Comparing `sponsorblock.py-0.2.2/sponsorblock/models.py` & `sponsorblock.py-0.2.3/sponsorblock/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     action_type : Optional[str], optional
         The action_type of the segment, by default None
     data : Optional[dict], optional
         The raw data that was used to create the segment, can be None if the segment was created manually
 
     Note
     ----
-    While creating your own instance you should only pass the category, start and end time. The other attributes won't do anything
+    While creating your own instance you should only pass the category, start and end time.
+    The other attributes won't do anything, those are only useful for segments gotten from the API.
     """
 
     def __init__(
         self,
         category: Category,
         start: Union[float, timedelta],
         end: Union[float, timedelta],
```

### Comparing `sponsorblock.py-0.2.2/sponsorblock/utils.py` & `sponsorblock.py-0.2.3/sponsorblock/utils.py`

 * *Files identical despite different names*

### Comparing `sponsorblock.py-0.2.2/sponsorblock.py.egg-info/PKG-INFO` & `sponsorblock.py-0.2.3/sponsorblock.py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: sponsorblock.py
-Version: 0.2.2
+Version: 0.2.3
 Summary: An unofficial wrapper for the SponsorBlock API
 Home-page: https://wasi-master.github.io/sponsorblock.py/
 Author: Wasi Master
 Author-email: arianmollik323@gmail.com
 License: MIT
 Keywords: sponsorblock.py,documentation,sponsorblock,python,api,wrapper,sponsor,block,youtube,youtube-dl,youtube-dlp
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
@@ -147,15 +146,21 @@
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 See the [documentation](https://sponsorblockpy.readthedocs.io/en/latest/)
 
 There is also a cli that you can use to get segments from the command line (beta).\
-To use that run `sponsorblock video_id` and pass your desired video_id
+To use that run:
+
+```sh
+sponsorblock video_id
+```
+
+and pass your desired video_id
 
 ## Roadmap
 
 See the [todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of features yet to be added and features already added.
 Also see the [open issues](https://github.com/wasi-master/sponsorblock.py/issues) for issues.
 
 <!-- CONTRIBUTING -->
@@ -178,9 +183,7 @@
 ## Contact
 
 Project Link: [https://github.com/wasi-master/sponsorblock.py](https://github.com/wasi-master/sponsorblock.py)
 
 Discord: [Wasi Master#6969](https://discord.com/users/723234115746398219)
 
 Email: [arianmollik323@gmail.com](mailto:arianmollik323@gmail.com)
-
-
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: sponsorblock.py Version: 0.2.2 Summary: An
+Metadata-Version: 2.1 Name: sponsorblock.py Version: 0.2.3 Summary: An
 unofficial wrapper for the SponsorBlock API Home-page: https://wasi-
 master.github.io/sponsorblock.py/ Author: Wasi Master Author-email:
 arianmollik323@gmail.com License: MIT Keywords:
 sponsorblock.py,documentation,sponsorblock,python,api,wrapper,sponsor,block,youtube,youtube-
-dl,youtube-dlp Platform: UNKNOWN Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
-:: English Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3 :: Only Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Topic :: Internet Requires-
-Python: >=3.6 Description-Content-Type: text/markdown License-File: LICENSE
+dl,youtube-dlp Classifier: Intended Audience :: Developers Classifier: License
+:: OSI Approved :: MIT License Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Topic :: Internet Requires-Python: >=3.6
+Description-Content-Type: text/markdown License-File: LICENSE
                                     [Logo]
                           ***** sponsorblock.py *****
                       A wrapper for the SponsorBlock API
                              Explore_the_docs_Â»
 
                   View_Demo Â· Report_Bug Â· Request_Feature
   [Contributors] [Forks] [Stargazers] [Issues] [Code_Size] [MIT_License] [Say
@@ -43,23 +43,23 @@
 ```sh pip install sponsorblock.py ``` 2. Installing using pip and git ```sh pip
 install git+https://github.com/wasi-master/sponsorblock.py.git ``` * Cloning
 then installing 1. Clone the repo ```sh git clone https://github.com/wasi-
 master/sponsorblock.py.git ``` 2. Changing the current working directory to the
 directory of the project ```sh cd sponsorblock.py ``` 3. Install using pip
 ```sh pip install . ```  ## Usage See the [documentation](https://
 sponsorblockpy.readthedocs.io/en/latest/) There is also a cli that you can use
-to get segments from the command line (beta).\ To use that run `sponsorblock
-video_id` and pass your desired video_id ## Roadmap See the [todo list](https:/
-/github.com/wasi-master/sponsorblock.py/blob/main/TODO.md) for a list of
-features yet to be added and features already added. Also see the [open issues]
-(https://github.com/wasi-master/sponsorblock.py/issues) for issues.  ##
-Contributing Contributions are what make the open source community such an
-amazing place to be learn, inspire, and create. Any contributions you make are
-**greatly appreciated**. 1. Fork the Project 2. Create your Feature Branch
-(`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git commit
--m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin feature/
-AmazingFeature`) 5. Open a Pull Request  ## License Distributed under the MIT
-License. See [`LICENSE`](LICENSE) for more information.  ## Contact Project
-Link: [https://github.com/wasi-master/sponsorblock.py](https://github.com/wasi-
-master/sponsorblock.py) Discord: [Wasi Master#6969](https://discord.com/users/
-723234115746398219) Email: [arianmollik323@gmail.com](mailto:
+to get segments from the command line (beta).\ To use that run: ```sh
+sponsorblock video_id ``` and pass your desired video_id ## Roadmap See the
+[todo list](https://github.com/wasi-master/sponsorblock.py/blob/main/TODO.md)
+for a list of features yet to be added and features already added. Also see the
+[open issues](https://github.com/wasi-master/sponsorblock.py/issues) for
+issues.  ## Contributing Contributions are what make the open source community
+such an amazing place to be learn, inspire, and create. Any contributions you
+make are **greatly appreciated**. 1. Fork the Project 2. Create your Feature
+Branch (`git checkout -b feature/AmazingFeature`) 3. Commit your Changes (`git
+commit -m 'Add some AmazingFeature'`) 4. Push to the Branch (`git push origin
+feature/AmazingFeature`) 5. Open a Pull Request  ## License Distributed under
+the MIT License. See [`LICENSE`](LICENSE) for more information.  ## Contact
+Project Link: [https://github.com/wasi-master/sponsorblock.py](https://
+github.com/wasi-master/sponsorblock.py) Discord: [Wasi Master#6969](https://
+discord.com/users/723234115746398219) Email: [arianmollik323@gmail.com](mailto:
 arianmollik323@gmail.com)
```

