# Comparing `tmp/lektor-git-timestamp-1.0.0b1.tar.gz` & `tmp/lektor_git_timestamp-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lektor-git-timestamp-1.0.0b1.tar", last modified: Tue Apr 11 19:52:55 2023, max compression
+gzip compressed data, was "lektor_git_timestamp-1.0.0b2.tar", last modified: Thu Jun 15 22:29:33 2023, max compression
```

## Comparing `lektor-git-timestamp-1.0.0b1.tar` & `lektor_git_timestamp-1.0.0b2.tar`

### file list

```diff
@@ -1,27 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-11 19:52:55.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/Test Site.lektorproject
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/content/contents.lr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 19:52:55.894060 lektor-git-timestamp-1.0.0b1/tests/test-site/models/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test-site/models/page.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-11 19:52:47.000000 lektor-git-timestamp-1.0.0b1/tox.ini
+-rw-r--r--   0        0        0     1456 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/CHANGES.md
+-rw-r--r--   0        0        0     1074 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     7436 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/README.md
+-rw-r--r--   0        0        0     7080 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/lektor_git_timestamp.py
+-rw-r--r--   0        0        0      753 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/pdm_build.py
+-rw-r--r--   0        0        0    11383 2023-06-15 22:29:33.928881 lektor_git_timestamp-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3186 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/conftest.py
+-rw-r--r--   0        0        0       27 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/test-site/Test Site.lektorproject
+-rw-r--r--   0        0        0        0 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/test-site/content/contents.lr
+-rw-r--r--   0        0        0      317 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/test-site/models/page.ini
+-rw-r--r--   0        0        0     4881 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/test_functional.py
+-rw-r--r--   0        0        0    11401 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tests/test_plugin.py
+-rw-r--r--   0        0        0     1156 2023-06-15 22:29:17.964671 lektor_git_timestamp-1.0.0b2/tox.ini
+-rw-r--r--   0        0        0    11159 1970-01-01 00:00:00.000000 lektor_git_timestamp-1.0.0b2/PKG-INFO
```

### Comparing `lektor-git-timestamp-1.0.0b1/LICENSE` & `lektor_git_timestamp-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `lektor-git-timestamp-1.0.0b1/PKG-INFO` & `lektor_git_timestamp-1.0.0b2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: lektor-git-timestamp
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: Lektor type to deduce page modification time from git
-Author-email: Jeff Dairiki <dairiki@dairiki.org>
+Keywords: Lektor plugin
+Author-Email: Jeff Dairiki <dairiki@dairiki.org>
 License: Copyright © 2020, 2021, 2023 Geoffrey T. Dairiki
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
         without limitation the rights to use, copy, modify, merge, publish,
         distribute, sublicense, and/or sell copies of the Software, and to
@@ -19,41 +20,40 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
         EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
         MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
         NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
         LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Home, https://github.com/dairiki/lektor-git-timestamp
-Keywords: Lektor plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Lektor
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Version Control :: Git
 Classifier: Topic :: Text Processing
+Project-URL: Home, https://github.com/dairiki/lektor-git-timestamp
 Requires-Python: >=3.7
+Requires-Dist: lektorlib>=1.2.1
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Lektor-Git-Timestamp
 
 [![PyPI version](https://img.shields.io/pypi/v/lektor-git-timestamp.svg)](https://pypi.org/project/lektor-git-timestamp/)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektor-git-timestamp.svg)](https://pypi.python.org/pypi/lektor-git-timestamp/)
 [![GitHub license](https://img.shields.io/github/license/dairiki/lektor-git-timestamp)](https://github.com/dairiki/lektor-git-timestamp/blob/master/LICENSE)
 [![GitHub Actions (Tests)](https://github.com/dairiki/lektor-git-timestamp/workflows/Tests/badge.svg)](https://github.com/dairiki/lektor-git-timestamp)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhat85618pg4zbl1nilh)](https://trackgit.com)
 
 This Lektor plugin implements a new datetime-like type,
 `gittimestamp`, which gets it's default value from git timestamps.
 This can be used to implement auto-updating `pub_date` and `last_mod`
 fields in Lektor datamodels.
 
 ## Description
@@ -70,15 +70,15 @@
 the source file is dirty with respect to git’s HEAD, or if the file is
 not checked into the git tree, the file’s mtime is prepended to that
 list of timestamps.  That list of timestamps is filtered based on the
 `ignore_commits` and `skip_first_commit` options (see below); then,
 finally, a timestamp is selected from those that remain based on the
 setting of the `strategy` option.
 
-### Options
+### Field Options
 
 The `gittimestamp` type supports the following options.
 
 #### `ignore_commits`
 
 This can be set to a string, which is interpreted as a regular
 expression.  Any git commits whose commit message matches this pattern
@@ -110,14 +110,49 @@
     may not be monotonically increasing, in which case this option causes the
     greatest (most recent) timestamp remaining after any filtering to be selected.
 
 - `earliest`: The earliest timestamp is used.  Normally this produces the same
     result at `first`, but if the timestamps in the git log are not monotonic,
     this will select the minimum of all the timestamps remaining after any filtering.
 
+### Global Configuration
+
+The following global configuration options are supported.
+These values are specified by way of the plugins' [configuration file]:
+`configs/git-timestamp.ini` under the project site directory.
+
+By default, the [`--follow`][git-log-follow] option is passed to `git log` when
+computing timestamps.  This behavior may be adjusted on a global basis by way of the plugins' [configuration file] (`configs/git-timestamp.ini` under the project site directory) via the following settings:
+
+#### `follow_renames`
+
+This is a boolean setting that specifies whether the
+[`--follow`][git-log-follow] option should be passed to `git log` when
+querying git for timestamps.  This options causes `git` to attempt to
+follow file renames.
+
+Currently, if unspecified, `follow_renames` defaults to _true_.
+(This may change in the future.)
+
+> **Note** Since we currently run `git log` on a per-source-file basis, when `--follow`
+> is specified, _copied_ files will be detected as “renamed”. This may not be ideal.
+
+
+#### `follow_rename_threshold`
+
+Set the _similarity index threshold_ (passed to `git log` via its
+[`-M` option][git-log-M]) used when detecting renames. This should be
+specified as a (floating point) number between 0 and 100,
+inclusive. Setting `follow_rename_threshold = 100` will limit
+detection to exact renames only. The default value is 50.
+
+[git-log-M]: https://git-scm.com/docs/git-log#Documentation/git-log.txt--Mltngt
+[git-log-follow]: https://git-scm.com/docs/git-log#Documentation/git-log.txt---follow
+[configuration file]: https://www.getlektor.com/docs/plugins/howto/#configure-plugins
+
 ## Examples
 
 Here is a simple example excerpt from a datamodel file:
 
 ```ini
 <...>
 
@@ -185,14 +220,38 @@
 
 ## Author
 
 Jeff Dairiki <dairiki@dairiki.org>
 
 ## Changelog
 
+### Release 1.0.0b2 (2023-06-15)
+
+- Added type annotations.
+- Convert packaging to PDM.
+
+#### Code Style
+
+- Style: Run [black] and [reorder-python-imports] on code. Configure
+  [pre-commit] to keep all up-to-date.
+
+#### Tests
+
+- Disuse the deprecated module `pkg_resources`.
+
+#### Buglets
+
+- Do not strip trailing whitespace from `git log` output. (This was
+  erroneously removing trailing newlines from the final commit
+  message.)
+
+[black]: https://github.com/psf/black
+[pre-commit]: https://pre-commit.com/
+[reorder-python-imports]: https://github.com/asottile/reorder-python-imports
+
 ### Release 1.0.0b1 (2023-04-11)
 
 - Drop support for python 2.7 and 3.6. ([#2])
 
 #### Testing
 
 - Test under python 3.10 and 3.11. ([#2])
@@ -224,8 +283,7 @@
 
 Fixed attrocious typo which prevented the use of anything other than the
 default `strategy=last` for picking timestamps.
 
 ### Release 0.1a1 (2020-06-16)
 
 Initial release.
-
```

### Comparing `lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.egg-info/PKG-INFO` & `lektor_git_timestamp-1.0.0b2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,14 @@
-Metadata-Version: 2.1
-Name: lektor-git-timestamp
-Version: 1.0.0b1
-Summary: Lektor type to deduce page modification time from git
-Author-email: Jeff Dairiki <dairiki@dairiki.org>
-License: Copyright © 2020, 2021, 2023 Geoffrey T. Dairiki
-        
-        Permission is hereby granted, free of charge, to any person obtaining
-        a copy of this software and associated documentation files (the
-        "Software"), to deal in the Software without restriction, including
-        without limitation the rights to use, copy, modify, merge, publish,
-        distribute, sublicense, and/or sell copies of the Software, and to
-        permit persons to whom the Software is furnished to do so, subject to
-        the following conditions:
-        
-        The above copyright notice and this permission notice shall be
-        included in all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-        EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-        NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-        LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-        OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-        WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: Home, https://github.com/dairiki/lektor-git-timestamp
-Keywords: Lektor plugin
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Plugins
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Lektor
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Version Control :: Git
-Classifier: Topic :: Text Processing
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Lektor-Git-Timestamp
 
 [![PyPI version](https://img.shields.io/pypi/v/lektor-git-timestamp.svg)](https://pypi.org/project/lektor-git-timestamp/)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/lektor-git-timestamp.svg)](https://pypi.python.org/pypi/lektor-git-timestamp/)
 [![GitHub license](https://img.shields.io/github/license/dairiki/lektor-git-timestamp)](https://github.com/dairiki/lektor-git-timestamp/blob/master/LICENSE)
 [![GitHub Actions (Tests)](https://github.com/dairiki/lektor-git-timestamp/workflows/Tests/badge.svg)](https://github.com/dairiki/lektor-git-timestamp)
+[![Trackgit Views](https://us-central1-trackgit-analytics.cloudfunctions.net/token/ping/lhat85618pg4zbl1nilh)](https://trackgit.com)
 
 This Lektor plugin implements a new datetime-like type,
 `gittimestamp`, which gets it's default value from git timestamps.
 This can be used to implement auto-updating `pub_date` and `last_mod`
 fields in Lektor datamodels.
 
 ## Description
@@ -70,15 +25,15 @@
 the source file is dirty with respect to git’s HEAD, or if the file is
 not checked into the git tree, the file’s mtime is prepended to that
 list of timestamps.  That list of timestamps is filtered based on the
 `ignore_commits` and `skip_first_commit` options (see below); then,
 finally, a timestamp is selected from those that remain based on the
 setting of the `strategy` option.
 
-### Options
+### Field Options
 
 The `gittimestamp` type supports the following options.
 
 #### `ignore_commits`
 
 This can be set to a string, which is interpreted as a regular
 expression.  Any git commits whose commit message matches this pattern
@@ -110,14 +65,49 @@
     may not be monotonically increasing, in which case this option causes the
     greatest (most recent) timestamp remaining after any filtering to be selected.
 
 - `earliest`: The earliest timestamp is used.  Normally this produces the same
     result at `first`, but if the timestamps in the git log are not monotonic,
     this will select the minimum of all the timestamps remaining after any filtering.
 
+### Global Configuration
+
+The following global configuration options are supported.
+These values are specified by way of the plugins' [configuration file]:
+`configs/git-timestamp.ini` under the project site directory.
+
+By default, the [`--follow`][git-log-follow] option is passed to `git log` when
+computing timestamps.  This behavior may be adjusted on a global basis by way of the plugins' [configuration file] (`configs/git-timestamp.ini` under the project site directory) via the following settings:
+
+#### `follow_renames`
+
+This is a boolean setting that specifies whether the
+[`--follow`][git-log-follow] option should be passed to `git log` when
+querying git for timestamps.  This options causes `git` to attempt to
+follow file renames.
+
+Currently, if unspecified, `follow_renames` defaults to _true_.
+(This may change in the future.)
+
+> **Note** Since we currently run `git log` on a per-source-file basis, when `--follow`
+> is specified, _copied_ files will be detected as “renamed”. This may not be ideal.
+
+
+#### `follow_rename_threshold`
+
+Set the _similarity index threshold_ (passed to `git log` via its
+[`-M` option][git-log-M]) used when detecting renames. This should be
+specified as a (floating point) number between 0 and 100,
+inclusive. Setting `follow_rename_threshold = 100` will limit
+detection to exact renames only. The default value is 50.
+
+[git-log-M]: https://git-scm.com/docs/git-log#Documentation/git-log.txt--Mltngt
+[git-log-follow]: https://git-scm.com/docs/git-log#Documentation/git-log.txt---follow
+[configuration file]: https://www.getlektor.com/docs/plugins/howto/#configure-plugins
+
 ## Examples
 
 Here is a simple example excerpt from a datamodel file:
 
 ```ini
 <...>
 
@@ -182,50 +172,7 @@
 [#789](https://github.com/lektor/lektor/pull/789) which was merged to
 the master branch on February 6, 2021, but didn't make it into a release
 until Lektor 3.3, released on December 13 2021.
 
 ## Author
 
 Jeff Dairiki <dairiki@dairiki.org>
-
-## Changelog
-
-### Release 1.0.0b1 (2023-04-11)
-
-- Drop support for python 2.7 and 3.6. ([#2])
-
-#### Testing
-
-- Test under python 3.10 and 3.11. ([#2])
-
-- Test that `lektor.db.Record.get_sort_key` works with
-  descriptor-valued fields. (This requires `lektor>=3.3`.)
-
-[#2]: https://github.com/dairiki/lektor-git-timestamp/pull/2
-
-
-### Release 0.1.0.post1 (2021-08-12)
-
-No code changes.
-
-Add warning to README about `lektor > 3.2` (not yet released) being
-required in order to be able to sort records by `gittimestamp` fields.
-
-### Release 0.1 (2021-02-05)
-
-No code changes.
-
-Update development status classifier to "stable".
-
-Add functional tests.
-
-### Release 0.1a2 (2021-02-03)
-
-#### Bugs Fixed
-
-Fixed attrocious typo which prevented the use of anything other than the
-default `strategy=last` for picking timestamps.
-
-### Release 0.1a1 (2020-06-16)
-
-Initial release.
-
```

### Comparing `lektor-git-timestamp-1.0.0b1/lektor_git_timestamp.py` & `lektor_git_timestamp-1.0.0b2/lektor_git_timestamp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,238 @@
-from collections import namedtuple
+from __future__ import annotations
+
 import datetime
+import enum
 import hashlib
-from operator import attrgetter
 import os
 import pickle
 import re
 import subprocess
+from contextlib import suppress
+from dataclasses import dataclass
+from typing import Any
+from typing import Iterable
+from typing import Iterator
+from typing import Mapping
+from typing import NamedTuple
+from typing import overload
+from typing import Sequence
+from typing import TYPE_CHECKING
 
 import jinja2
 from lektor.context import get_ctx
+from lektor.pluginsystem import get_plugin
 from lektor.pluginsystem import Plugin
 from lektor.reporter import reporter
 from lektor.sourceobj import VirtualSourceObject
 from lektor.types import DateTimeType
 from lektor.utils import bool_from_string
+from lektorlib.recordcache import get_or_create_virtual
 from werkzeug.utils import cached_property
 
-from lektorlib.recordcache import get_or_create_virtual
+if TYPE_CHECKING:
+    from _typeshed import StrPath
+    from lektor.builder import PathCache
+    from lektor.db import Record
+    from lektor.types.base import RawValue
+
 
-VIRTUAL_PATH_PREFIX = 'git-timestamp'
+VIRTUAL_PATH_PREFIX = "git-timestamp"
 
 
-def run_git(*args):
-    cmd = ('git', *args)
+def run_git(*args: str | StrPath) -> str:
+    cmd = ("git", *args)
     proc = subprocess.run(cmd, capture_output=True, text=True, check=True)
-    return proc.stdout.rstrip()
+    return proc.stdout
 
 
-def _fs_mtime(filename):
+def _fs_mtime(filename: StrPath) -> int | None:
     try:
         st = os.stat(filename)
     except OSError as exc:
         reporter.report_generic(f"{filename}: {exc!s}")
         return None
     else:
         # (truncate to one second resolution)
         return int(st.st_mtime)
 
 
-def _is_dirty(filename):
-    status = run_git('status', '-z', '--', filename)
-    return status != ''
-
-
-timestamp = namedtuple('timestamp', ['ts', 'commit_message'])
-
-
-def _iter_timestamps(filename):
-    output = run_git('log', '--pretty=format:%at %B', '-z',
-                     '--follow', '--remove-empty',
-                     '--', filename)
+def _is_dirty(filename: StrPath) -> bool:
+    status = run_git("status", "-z", "--", filename)
+    return status != ""
+
+
+class Timestamp(NamedTuple):
+    ts: int
+    commit_message: str | None
+
+
+def _iter_timestamps(
+    filename: StrPath, config: Mapping[str, str]
+) -> Iterator[Timestamp]:
+    options = ["--remove-empty"]
+    follow_renames = bool_from_string(config.get("follow_renames", "true"))
+    if follow_renames:
+        options.append("--follow")
+        with suppress(LookupError, ValueError):
+            threshold = float(config["follow_rename_threshold"])
+            if 0 < threshold < 100:
+                options.append(f"-M{threshold:.4f}%")
+
+    output = run_git(
+        "log",
+        "--pretty=format:%at %B",
+        "-z",
+        *options,
+        "--",
+        filename,
+    )
     if not output or _is_dirty(filename):
         ts = _fs_mtime(filename)
         if ts is not None:
-            yield timestamp(ts, None)
+            yield Timestamp(ts, None)
     if output:
-        for line in output.split('\0'):
-            ts, _, commit_message = line.partition(' ')
-            yield timestamp(int(ts), commit_message)
-
-
-def get_mtime(timestamps,
-              ignore_commits=None,
-              strategy='last',
-              skip_first_commit=False):
-    def is_not_ignored(timestamp):
+        for line in output.split("\0"):
+            tstamp, _, commit_message = line.partition(" ")
+            yield Timestamp(int(tstamp), commit_message)
+
+
+class Strategy(enum.Enum):
+    FIRST = "first"
+    EARLIEST = "earliest"
+    LATEST = "latest"
+    LAST = "last"
+
+
+def get_mtime(
+    timestamps: Iterable[Timestamp],
+    ignore_commits: str | re.Pattern[str] | None = None,
+    strategy: Strategy = Strategy.LAST,
+    skip_first_commit: bool = False,
+) -> int | None:
+    def is_not_ignored(timestamp: Timestamp) -> bool:
         if ignore_commits is None:
             return True
         message = timestamp.commit_message
         if message is None:
             return True
         return re.search(ignore_commits, message) is None
 
     filtered = list(filter(is_not_ignored, timestamps))
     if skip_first_commit:
         filtered = filtered[:-1]
 
     if len(filtered) == 0:
         return None
-    elif strategy == 'first':
+    if strategy is Strategy.FIRST:
         return filtered[-1].ts
-    elif strategy == 'earliest':
-        return min(map(attrgetter('ts'), filtered))
-    elif strategy == 'latest':
-        return max(map(attrgetter('ts'), filtered))
-    else:                       # strategy == 'last'
-        return filtered[0].ts
+    if strategy is Strategy.EARLIEST:
+        return min(timestamp.ts for timestamp in filtered)
+    if strategy is Strategy.LATEST:
+        return max(timestamp.ts for timestamp in filtered)
+    assert strategy is Strategy.LAST
+    return filtered[0].ts
 
 
-def _compute_checksum(data):
+def _compute_checksum(data: tuple[Timestamp, ...]) -> str:
     return hashlib.sha1(pickle.dumps(data, protocol=0)).hexdigest()
 
 
-class GitTimestampSource(VirtualSourceObject):
+class GitTimestampSource(VirtualSourceObject):  # type: ignore[misc]
     @classmethod
-    def get(cls, record):
-        def creator():
+    def get(cls, record: Record) -> GitTimestampSource:
+        def creator() -> GitTimestampSource:
             return cls(record)
+
         return get_or_create_virtual(record, VIRTUAL_PATH_PREFIX, creator)
 
     @property
-    def path(self):
+    def path(self) -> str:
         return f"{self.record.path}@{VIRTUAL_PATH_PREFIX}"
 
-    def get_checksum(self, path_cache):
+    def get_checksum(self, path_cache: PathCache) -> str:
         return _compute_checksum(self.timestamps)
 
     @cached_property
-    def timestamps(self):
-        return tuple(_iter_timestamps(self.source_filename))
+    def timestamps(self) -> tuple[Timestamp, ...]:
+        plugin_config: Mapping[str, str] = {}
+        with suppress(LookupError):
+            plugin_config = get_plugin(GitTimestampPlugin, self.pad.env).get_config()
 
+        return tuple(_iter_timestamps(self.source_filename, plugin_config))
 
-class GitTimestampDescriptor:
-    def __init__(self, raw,
-                 ignore_commits=None,
-                 strategy='last',
-                 skip_first_commit=False):
-        self.raw = raw
-        self.kwargs = {
-            'ignore_commits': ignore_commits,
-            'strategy': strategy,
-            'skip_first_commit': skip_first_commit,
-            }
 
-    def __get__(self, obj, type_=None):
+@dataclass
+class GitTimestampDescriptor:
+    raw: RawValue
+    ignore_commits: str | re.Pattern[str] | None = None
+    strategy: Strategy = Strategy.LAST
+    skip_first_commit: bool = False
+
+    @overload
+    def __get__(self, obj: None) -> GitTimestampDescriptor:
+        ...
+
+    @overload
+    def __get__(self, obj: Record) -> datetime.datetime | jinja2.Undefined:
+        ...
+
+    def __get__(
+        self, obj: Record | None, type_: object = None
+    ) -> GitTimestampDescriptor | datetime.datetime | jinja2.Undefined:
         if obj is None:
             return self
         ctx = get_ctx()
         src = GitTimestampSource.get(obj)
         if ctx:
             ctx.record_virtual_dependency(src)
-        mtime = get_mtime(src.timestamps, **self.kwargs)
+        mtime = get_mtime(
+            src.timestamps,
+            ignore_commits=self.ignore_commits,
+            strategy=self.strategy,
+            skip_first_commit=self.skip_first_commit,
+        )
         if mtime is None:
-            return self.raw.missing_value("no suitable git timestamp exists")
+            return self.raw.missing_value(  # type: ignore[no-any-return]
+                "no suitable git timestamp exists"
+            )
         return datetime.datetime.fromtimestamp(mtime)
 
 
-class GitTimestampType(DateTimeType):
-    def value_from_raw(self, raw):
+class GitTimestampType(DateTimeType):  # type: ignore[misc]
+    def value_from_raw(
+        self, raw: RawValue
+    ) -> GitTimestampDescriptor | datetime.datetime:
         value = super().value_from_raw(raw)
-        if jinja2.is_undefined(value):
-            options = self.options
-            value = GitTimestampDescriptor(
-                raw,
-                ignore_commits=options.get('ignore_commits'),
-                strategy=options.get('strategy', 'last'),
-                skip_first_commit=bool_from_string(
-                    options.get('skip_first_commit', False)),
-                )
-        return value
-
-
-class GitTimestampPlugin(Plugin):
-    name = 'git-timestamp'
-    description = 'Lektor type to deduce page modification time from git'
+        if not jinja2.is_undefined(value):
+            assert isinstance(value, datetime.datetime)
+            return value
+
+        options = self.options
+        try:
+            strategy = Strategy(options["strategy"])
+        except (KeyError, ValueError):
+            strategy = Strategy.LAST
+        return GitTimestampDescriptor(
+            raw,
+            ignore_commits=options.get("ignore_commits"),
+            strategy=strategy,
+            skip_first_commit=bool_from_string(options.get("skip_first_commit", False)),
+        )
+
+
+class GitTimestampPlugin(Plugin):  # type: ignore[misc]
+    name = "git-timestamp"
+    description = "Lektor type to deduce page modification time from git"
 
-    def on_setup_env(self, **extra):
+    def on_setup_env(self, **extra: Any) -> None:
         env = self.env
         env.add_type(GitTimestampType)
         env.virtualpathresolver(VIRTUAL_PATH_PREFIX)(self.resolve_virtual_path)
 
     @staticmethod
-    def resolve_virtual_path(record, pieces):
+    def resolve_virtual_path(
+        record: Record, pieces: Sequence[str]
+    ) -> GitTimestampSource | None:
         if len(pieces) == 0:
             return GitTimestampSource.get(record)
+        return None
```

### Comparing `lektor-git-timestamp-1.0.0b1/tox.ini` & `lektor_git_timestamp-1.0.0b2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     3.10: py310
     3.11: py311, lint
 
 [testenv]
 deps =
     pytest
     pytest-cov
+    importlib_metadata; python_version<'3.8'
+    packaging
     !lektor33: lektor>=3.4.0a0
     lektor33: lektor<3.4.0
 setenv =
     # Prevent parallel pytest-cov runs from clobbering each others .coverage file
     COVERAGE_FILE = {envtmpdir}/.coverage
 passenv =
     # Needed by git (to find global config settings user.email, user.name)
@@ -38,14 +40,15 @@
     twine
 commands =
     python -m build --sdist --outdir {envtmpdir}/dist {toxinidir}
     twine check {envtmpdir}/dist/*
     flake8
 
 [flake8]
+max-line-length = 88
 exclude =
     .tox,
     .git,
     __pycache__,
     .eggs,
     # excludes other virtualenv lib and bin directories
     python*.*, bin
```

