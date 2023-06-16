# Comparing `tmp/ao3-cli-0.1.5.tar.gz` & `tmp/ao3-cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/arbaaz/Projects/Personal/Projects/Python/CLI/ao3-cli/dist/tmpr3t5qbdy/ao3-cli-0.1.5.tar", last modified: Sat Jan 29 16:09:28 2022, max compression
+gzip compressed data, was "D:\Projects\Personal\Projects\Langs\Python\CLI\ao3-cli\dist\.tmp-pdwnb8d1\ao3-cli-0.1.6.tar", last modified: Fri Jun 16 15:27:05 2023, max compression
```

## Comparing `ao3-cli-0.1.5.tar` & `ao3-cli-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 arbaaz    (1000) arbaaz    (1000)        0 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     1070 2021-05-13 19:13:54.000000 ao3-cli-0.1.5/LICENSE.txt
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     2629 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/PKG-INFO
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     2177 2021-06-15 15:03:48.000000 ao3-cli-0.1.5/README.md
-drwxrwxr-x   0 arbaaz    (1000) arbaaz    (1000)        0 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/ao3_cli/
--rw-r--r--   0 arbaaz    (1000) arbaaz    (1000)        0 2021-04-21 05:35:36.000000 ao3-cli-0.1.5/ao3_cli/__init__.py
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     2667 2022-01-29 16:06:37.000000 ao3-cli-0.1.5/ao3_cli/cli.py
-drwxrwxr-x   0 arbaaz    (1000) arbaaz    (1000)        0 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/ao3_cli/utils/
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)        0 2021-06-15 11:55:19.000000 ao3-cli-0.1.5/ao3_cli/utils/__init__.py
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     3262 2021-12-24 07:56:52.000000 ao3-cli-0.1.5/ao3_cli/utils/ao3.py
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     9712 2021-12-24 08:26:52.000000 ao3-cli-0.1.5/ao3_cli/utils/fetch_data.py
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)      779 2021-08-05 18:24:43.000000 ao3-cli-0.1.5/ao3_cli/utils/logging.py
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     3145 2022-01-12 00:11:37.000000 ao3-cli-0.1.5/ao3_cli/utils/processing.py
-drwxrwxr-x   0 arbaaz    (1000) arbaaz    (1000)        0 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/ao3_cli.egg-info/
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     2629 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)      406 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)        1 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)       67 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)      108 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/requires.txt
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)        8 2022-01-29 16:09:28.000000 ao3-cli-0.1.5/ao3_cli.egg-info/top_level.txt
--rw-r--r--   0 arbaaz    (1000) arbaaz    (1000)      229 2021-04-21 05:35:36.000000 ao3-cli-0.1.5/pyproject.toml
--rw-r--r--   0 arbaaz    (1000) arbaaz    (1000)      106 2022-01-29 16:09:28.942202 ao3-cli-0.1.5/setup.cfg
--rw-rw-r--   0 arbaaz    (1000) arbaaz    (1000)     1015 2022-01-29 16:06:37.000000 ao3-cli-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:27:05.954530 ao3-cli-0.1.6/
+-rw-rw-rw-   0        0        0    11357 2022-02-09 15:53:43.000000 ao3-cli-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2721 2023-06-16 15:27:05.954530 ao3-cli-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2177 2022-02-06 13:33:57.000000 ao3-cli-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 15:27:05.918525 ao3-cli-0.1.6/ao3_cli/
+-rw-rw-rw-   0        0        0        0 2022-02-06 13:33:57.000000 ao3-cli-0.1.6/ao3_cli/__init__.py
+-rw-rw-rw-   0        0        0     3240 2023-06-16 15:22:18.000000 ao3-cli-0.1.6/ao3_cli/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:27:05.952526 ao3-cli-0.1.6/ao3_cli/utils/
+-rw-rw-rw-   0        0        0        0 2022-02-06 13:33:57.000000 ao3-cli-0.1.6/ao3_cli/utils/__init__.py
+-rw-rw-rw-   0        0        0     3835 2022-02-09 15:53:29.000000 ao3-cli-0.1.6/ao3_cli/utils/ao3.py
+-rw-rw-rw-   0        0        0    10285 2022-02-09 15:53:25.000000 ao3-cli-0.1.6/ao3_cli/utils/fetch_data.py
+-rw-rw-rw-   0        0        0     1352 2022-02-09 15:53:20.000000 ao3-cli-0.1.6/ao3_cli/utils/logging.py
+-rw-rw-rw-   0        0        0     3833 2023-06-16 15:18:59.000000 ao3-cli-0.1.6/ao3_cli/utils/processing.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:27:05.947523 ao3-cli-0.1.6/ao3_cli.egg-info/
+-rw-rw-rw-   0        0        0     2721 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      108 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 15:27:05.000000 ao3-cli-0.1.6/ao3_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2022-02-06 13:33:57.000000 ao3-cli-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      114 2023-06-16 15:27:05.962524 ao3-cli-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1038 2023-06-16 15:26:50.000000 ao3-cli-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:27:05.953526 ao3-cli-0.1.6/tests/
+-rw-rw-rw-   0        0        0     1332 2023-06-16 15:23:42.000000 ao3-cli-0.1.6/tests/test_cli.py
```

### Comparing `ao3-cli-0.1.5/PKG-INFO` & `ao3-cli-0.1.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ao3-cli
-Version: 0.1.5
-Summary: A CLI to download from archiveofourown.org
-Home-page: https://github.com/arzkar/ao3-cli/
-Author: Arbaaz Laskar
-Author-email: arzkar.dev@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <h1 align="center">ao3-cli</h1>
 
 A CLI to download from archiveofourown.org using their built-in download option.<br/><br/>
 To report issues for the CLI, open an issue at https://github.com/arzkar/ao3-cli/issues<br/>
 
 ### Features:
 
@@ -84,9 +69,7 @@
 
 ### Default Configuration
 
 - The fanfiction will be downloaded in epub format. To change it, use `-f` followed by the format.
 - The fanfiction will be downloaded in the current directory. To change it, use `-o` followed by the path to the directory.
 
 Check `ao3_cli --help` for more info.
-
-
```

### Comparing `ao3-cli-0.1.5/README.md` & `ao3-cli-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,89 @@
-<h1 align="center">ao3-cli</h1>
-
-A CLI to download from archiveofourown.org using their built-in download option.<br/><br/>
-To report issues for the CLI, open an issue at https://github.com/arzkar/ao3-cli/issues<br/>
-
-### Features:
-
-- Download works & series from archiveofourown.org
-- It also supports downloading all works or series from any archiveofourown.org page.<br/><br/>
-
-# Installation
-
-## Using pip (Recommended)
-
-```
-pip install -U ao3-cli
-```
-
-## From Source (Might have bugs, for development use)
-
-```
-pip install git+https://github.com/arzkar/ao3-cli@main
-```
-
-# Usage
-
-```
-> ao3_cli
-Usage: ao3_cli [OPTIONS]
-
-  A CLI to download from archiveofourown.org
-
-  To report issues for the CLI, open an issue at
-  https://github.com/arzkar/ao3-cli/issues
-
-Options:
-  -u, --url TEXT       The url of the fanfiction enclosed within quotes
-  -i, --infile TEXT    Give a filename to read URLs from
-  -l, --list-url TEXT  Enter a comma separated list of urls to download,enclosed within quotes
-  -o, --out-dir TEXT   Absolute path to the Output directory for files(default: Current Directory)
-  -f, --format TEXT    Download Format: EPUB (default), AZW3, MOBI, PDF or HTML
-  --force              Force overwrite of an existing file
-  --get-urls TEXT      Get all story urls found from a page
-  -d, --debug          Show the log in the console for debugging
-  --log                Save the logfile for debugging
-  -v, --version        Display version & quit.
-  --help               Show this message and exit.
-```
-
-## Example
-
-- To download using a URL
-
-```
-ao3_cli -u https://archiveofourown.org/works/10916730/chapters/24276864
-```
-
-- To download using a file containing URLs
-
-```
-ao3_cli -i urls.txt
-```
-
-- To download using a comma separated list of URLs
-
-```
-ao3_cli -l "https://archiveofourown.org/works/31923052/chapters/79053661,https://archiveofourown.org/works/31950595"
-```
-
-### Default Configuration
-
-- The fanfiction will be downloaded in epub format. To change it, use `-f` followed by the format.
-- The fanfiction will be downloaded in the current directory. To change it, use `-o` followed by the path to the directory.
-
-Check `ao3_cli --help` for more info.
+Metadata-Version: 2.1
+Name: ao3-cli
+Version: 0.1.6
+Summary: A CLI to download from archiveofourown.org
+Home-page: https://github.com/arzkar/ao3-cli/
+Author: Arbaaz Laskar
+Author-email: arzkar.dev@gmail.com
+License: Apache License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<h1 align="center">ao3-cli</h1>
+
+A CLI to download from archiveofourown.org using their built-in download option.<br/><br/>
+To report issues for the CLI, open an issue at https://github.com/arzkar/ao3-cli/issues<br/>
+
+### Features:
+
+- Download works & series from archiveofourown.org
+- It also supports downloading all works or series from any archiveofourown.org page.<br/><br/>
+
+# Installation
+
+## Using pip (Recommended)
+
+```
+pip install -U ao3-cli
+```
+
+## From Source (Might have bugs, for development use)
+
+```
+pip install git+https://github.com/arzkar/ao3-cli@main
+```
+
+# Usage
+
+```
+> ao3_cli
+Usage: ao3_cli [OPTIONS]
+
+  A CLI to download from archiveofourown.org
+
+  To report issues for the CLI, open an issue at
+  https://github.com/arzkar/ao3-cli/issues
+
+Options:
+  -u, --url TEXT       The url of the fanfiction enclosed within quotes
+  -i, --infile TEXT    Give a filename to read URLs from
+  -l, --list-url TEXT  Enter a comma separated list of urls to download,enclosed within quotes
+  -o, --out-dir TEXT   Absolute path to the Output directory for files(default: Current Directory)
+  -f, --format TEXT    Download Format: EPUB (default), AZW3, MOBI, PDF or HTML
+  --force              Force overwrite of an existing file
+  --get-urls TEXT      Get all story urls found from a page
+  -d, --debug          Show the log in the console for debugging
+  --log                Save the logfile for debugging
+  -v, --version        Display version & quit.
+  --help               Show this message and exit.
+```
+
+## Example
+
+- To download using a URL
+
+```
+ao3_cli -u https://archiveofourown.org/works/10916730/chapters/24276864
+```
+
+- To download using a file containing URLs
+
+```
+ao3_cli -i urls.txt
+```
+
+- To download using a comma separated list of URLs
+
+```
+ao3_cli -l "https://archiveofourown.org/works/31923052/chapters/79053661,https://archiveofourown.org/works/31950595"
+```
+
+### Default Configuration
+
+- The fanfiction will be downloaded in epub format. To change it, use `-f` followed by the format.
+- The fanfiction will be downloaded in the current directory. To change it, use `-o` followed by the path to the directory.
+
+Check `ao3_cli --help` for more info.
```

### Comparing `ao3-cli-0.1.5/ao3_cli/cli.py` & `ao3-cli-0.1.6/ao3_cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2021 Arbaaz Laskar
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import click
 import sys
 from loguru import logger
 from datetime import datetime
 from colorama import init, Fore
 
 from .utils.processing import get_format_type, show_urls_from_page
@@ -55,11 +69,11 @@
 
     elif get_urls:
         fic = FetchData(debug)
         fic.get_urls_from_page(get_urls)
         fic.exit_status = show_urls_from_page(fic)
 
     if version:
-        click.echo("Version: 0.1.5")
+        click.echo("Version: 0.1.6")
         sys.exit(0)
 
     sys.exit(fic.exit_status)
```

### Comparing `ao3-cli-0.1.5/ao3_cli/utils/ao3.py` & `ao3-cli-0.1.6/ao3_cli/utils/ao3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2021 Arbaaz Laskar
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import requests
 import re
 import time
 from loguru import logger
 from bs4 import BeautifulSoup
```

### Comparing `ao3-cli-0.1.5/ao3_cli/utils/fetch_data.py` & `ao3-cli-0.1.6/ao3_cli/utils/fetch_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2021 Arbaaz Laskar
+
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
+
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import re
 import requests
 from tqdm import tqdm
 from colorama import Fore, Style
 from loguru import logger
 from bs4 import BeautifulSoup
 from rich.console import Console
```

### Comparing `ao3-cli-0.1.5/ao3_cli.egg-info/PKG-INFO` & `ao3-cli-0.1.6/ao3_cli.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,89 @@
-Metadata-Version: 2.1
-Name: ao3-cli
-Version: 0.1.5
-Summary: A CLI to download from archiveofourown.org
-Home-page: https://github.com/arzkar/ao3-cli/
-Author: Arbaaz Laskar
-Author-email: arzkar.dev@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-<h1 align="center">ao3-cli</h1>
-
-A CLI to download from archiveofourown.org using their built-in download option.<br/><br/>
-To report issues for the CLI, open an issue at https://github.com/arzkar/ao3-cli/issues<br/>
-
-### Features:
-
-- Download works & series from archiveofourown.org
-- It also supports downloading all works or series from any archiveofourown.org page.<br/><br/>
-
-# Installation
-
-## Using pip (Recommended)
-
-```
-pip install -U ao3-cli
-```
-
-## From Source (Might have bugs, for development use)
-
-```
-pip install git+https://github.com/arzkar/ao3-cli@main
-```
-
-# Usage
-
-```
-> ao3_cli
-Usage: ao3_cli [OPTIONS]
-
-  A CLI to download from archiveofourown.org
-
-  To report issues for the CLI, open an issue at
-  https://github.com/arzkar/ao3-cli/issues
-
-Options:
-  -u, --url TEXT       The url of the fanfiction enclosed within quotes
-  -i, --infile TEXT    Give a filename to read URLs from
-  -l, --list-url TEXT  Enter a comma separated list of urls to download,enclosed within quotes
-  -o, --out-dir TEXT   Absolute path to the Output directory for files(default: Current Directory)
-  -f, --format TEXT    Download Format: EPUB (default), AZW3, MOBI, PDF or HTML
-  --force              Force overwrite of an existing file
-  --get-urls TEXT      Get all story urls found from a page
-  -d, --debug          Show the log in the console for debugging
-  --log                Save the logfile for debugging
-  -v, --version        Display version & quit.
-  --help               Show this message and exit.
-```
-
-## Example
-
-- To download using a URL
-
-```
-ao3_cli -u https://archiveofourown.org/works/10916730/chapters/24276864
-```
-
-- To download using a file containing URLs
-
-```
-ao3_cli -i urls.txt
-```
-
-- To download using a comma separated list of URLs
-
-```
-ao3_cli -l "https://archiveofourown.org/works/31923052/chapters/79053661,https://archiveofourown.org/works/31950595"
-```
-
-### Default Configuration
-
-- The fanfiction will be downloaded in epub format. To change it, use `-f` followed by the format.
-- The fanfiction will be downloaded in the current directory. To change it, use `-o` followed by the path to the directory.
-
-Check `ao3_cli --help` for more info.
-
-
+Metadata-Version: 2.1
+Name: ao3-cli
+Version: 0.1.6
+Summary: A CLI to download from archiveofourown.org
+Home-page: https://github.com/arzkar/ao3-cli/
+Author: Arbaaz Laskar
+Author-email: arzkar.dev@gmail.com
+License: Apache License
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+<h1 align="center">ao3-cli</h1>
+
+A CLI to download from archiveofourown.org using their built-in download option.<br/><br/>
+To report issues for the CLI, open an issue at https://github.com/arzkar/ao3-cli/issues<br/>
+
+### Features:
+
+- Download works & series from archiveofourown.org
+- It also supports downloading all works or series from any archiveofourown.org page.<br/><br/>
+
+# Installation
+
+## Using pip (Recommended)
+
+```
+pip install -U ao3-cli
+```
+
+## From Source (Might have bugs, for development use)
+
+```
+pip install git+https://github.com/arzkar/ao3-cli@main
+```
+
+# Usage
+
+```
+> ao3_cli
+Usage: ao3_cli [OPTIONS]
+
+  A CLI to download from archiveofourown.org
+
+  To report issues for the CLI, open an issue at
+  https://github.com/arzkar/ao3-cli/issues
+
+Options:
+  -u, --url TEXT       The url of the fanfiction enclosed within quotes
+  -i, --infile TEXT    Give a filename to read URLs from
+  -l, --list-url TEXT  Enter a comma separated list of urls to download,enclosed within quotes
+  -o, --out-dir TEXT   Absolute path to the Output directory for files(default: Current Directory)
+  -f, --format TEXT    Download Format: EPUB (default), AZW3, MOBI, PDF or HTML
+  --force              Force overwrite of an existing file
+  --get-urls TEXT      Get all story urls found from a page
+  -d, --debug          Show the log in the console for debugging
+  --log                Save the logfile for debugging
+  -v, --version        Display version & quit.
+  --help               Show this message and exit.
+```
+
+## Example
+
+- To download using a URL
+
+```
+ao3_cli -u https://archiveofourown.org/works/10916730/chapters/24276864
+```
+
+- To download using a file containing URLs
+
+```
+ao3_cli -i urls.txt
+```
+
+- To download using a comma separated list of URLs
+
+```
+ao3_cli -l "https://archiveofourown.org/works/31923052/chapters/79053661,https://archiveofourown.org/works/31950595"
+```
+
+### Default Configuration
+
+- The fanfiction will be downloaded in epub format. To change it, use `-f` followed by the format.
+- The fanfiction will be downloaded in the current directory. To change it, use `-o` followed by the path to the directory.
+
+Check `ao3_cli --help` for more info.
```

### Comparing `ao3-cli-0.1.5/setup.py` & `ao3-cli-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 setup(
     name='ao3-cli',
     author='Arbaaz Laskar',
     author_email="arzkar.dev@gmail.com",
     description="A CLI to download from archiveofourown.org",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.1.5',
-    license='MIT',
+    version='0.1.6',
+    license='Apache License',
     url="https://github.com/arzkar/ao3-cli/",
     packages=find_packages(include=['ao3_cli', 'ao3_cli.*']),
     include_package_data=True,
     install_requires=[
         'click>=7.1.2',
         'rich>=10.3.0',
         'requests>=2.25.1',
@@ -26,11 +26,11 @@
     ],
     entry_points='''
         [console_scripts]
         ao3_cli=ao3_cli.cli:run_cli
     ''',
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
 )
```

