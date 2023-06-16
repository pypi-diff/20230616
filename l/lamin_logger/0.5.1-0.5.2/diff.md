# Comparing `tmp/lamin_logger-0.5.1.tar.gz` & `tmp/lamin_logger-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.5.1.tar` & `lamin_logger-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.5.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.5.1/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.5.1/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.5.1/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.5.1/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.5.1/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.5.1/docs/api.md
--rw-r--r--   0        0        0     3170 2023-06-15 19:46:18.884967 lamin_logger-0.5.1/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.5.1/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.5.1/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.5.1/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-06-15 19:46:11.509161 lamin_logger-0.5.1/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.5.1/lamin_logger/_core.py
--rw-r--r--   0        0        0     7572 2023-06-15 19:45:48.150032 lamin_logger-0.5.1/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4157 2023-06-15 19:45:48.150302 lamin_logger-0.5.1/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     4107 2023-06-15 15:21:07.826610 lamin_logger-0.5.1/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.5.1/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     2758 2023-06-15 15:21:07.826983 lamin_logger-0.5.1/lamin_logger/_search.py
--rw-r--r--   0        0        0      334 2023-06-15 15:21:07.827322 lamin_logger-0.5.1/noxfile.py
--rw-r--r--   0        0        0      952 2023-06-15 19:45:48.151161 lamin_logger-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.5.1/tests/test_base.py
--rw-r--r--   0        0        0     1356 2023-06-14 17:38:57.247766 lamin_logger-0.5.1/tests/test_lookup.py
--rw-r--r--   0        0        0     2140 2023-06-15 15:21:07.827793 lamin_logger-0.5.1/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.5.1/tests/test_notebooks.py
--rw-r--r--   0        0        0     2101 2023-06-15 15:21:07.828218 lamin_logger-0.5.1/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:58:17.266637 lamin_logger-0.5.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 18:46:24.119961 lamin_logger-0.5.2/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 18:46:24.120069 lamin_logger-0.5.2/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 18:46:24.120174 lamin_logger-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 18:19:51.176749 lamin_logger-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-08-08 17:06:33.128130 lamin_logger-0.5.2/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-20 18:49:33.932419 lamin_logger-0.5.2/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 18:46:24.120507 lamin_logger-0.5.2/docs/api.md
+-rw-r--r--   0        0        0     3331 2023-06-16 10:33:14.536633 lamin_logger-0.5.2/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-23 18:45:50.337637 lamin_logger-0.5.2/docs/index.md
+-rw-r--r--   0        0        0     1360 2023-06-15 15:57:57.600362 lamin_logger-0.5.2/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 18:46:24.121862 lamin_logger-0.5.2/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-06-16 10:33:08.339442 lamin_logger-0.5.2/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 18:19:51.177212 lamin_logger-0.5.2/lamin_logger/_core.py
+-rw-r--r--   0        0        0     7600 2023-06-16 10:31:45.152421 lamin_logger-0.5.2/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4157 2023-06-15 22:43:54.438557 lamin_logger-0.5.2/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     4107 2023-06-15 15:58:17.267398 lamin_logger-0.5.2/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 18:19:51.177576 lamin_logger-0.5.2/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     2758 2023-06-15 15:58:17.267495 lamin_logger-0.5.2/lamin_logger/_search.py
+-rw-r--r--   0        0        0      334 2023-06-15 15:58:17.267619 lamin_logger-0.5.2/noxfile.py
+-rw-r--r--   0        0        0      952 2023-06-15 18:19:51.177764 lamin_logger-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 18:19:51.177888 lamin_logger-0.5.2/tests/test_base.py
+-rw-r--r--   0        0        0     1356 2023-06-15 15:58:17.267845 lamin_logger-0.5.2/tests/test_lookup.py
+-rw-r--r--   0        0        0     2140 2023-06-15 15:58:17.267943 lamin_logger-0.5.2/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:58:17.268069 lamin_logger-0.5.2/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2101 2023-06-15 15:58:17.268162 lamin_logger-0.5.2/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.5.2/PKG-INFO
```

### Comparing `lamin_logger-0.5.1/.github/workflows/build.yml` & `lamin_logger-0.5.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/.github/workflows/latest-changes.yml` & `lamin_logger-0.5.2/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/.gitignore` & `lamin_logger-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/.pre-commit-config.yaml` & `lamin_logger-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/LICENSE` & `lamin_logger-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/docs/changelog.md` & `lamin_logger-0.5.2/docs/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+💄 Log to stdout rather than stderr | [23](https://github.com/laminlabs/lamin-logger/pull/23) | [falexwolf](https://github.com/falexwolf) | 2023-06-16 | 0.5.2
 ✨ Lookup can also return sql records | [22](https://github.com/laminlabs/lamin-logger/pull/22) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.5.1
 ✨ Remove loguru and replace with standard (Scanpy-based) logger | [18](https://github.com/laminlabs/lamin-logger/pull/18) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.5.0
 🚚 Moved search and map_synonyms from bionty here | [21](https://github.com/laminlabs/lamin-logger/pull/21) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-15 | 0.4.0
 🚚 Temporarily added lookup | [20](https://github.com/laminlabs/lamin-logger/pull/20) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.3.4
 ✨ Added download level, changed info icon to 💬 | [19](https://github.com/laminlabs/lamin-logger/pull/19) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-27 | 0.3.2
 :sparkles: Add hint level | [17](https://github.com/laminlabs/lamin-logger/pull/17) | [falexwolf](https://github.com/falexwolf) | 2023-04-05 | 0.3.0
 🚸 Add all botocore subloggers | [16](https://github.com/laminlabs/lamin-logger/pull/16) | [falexwolf](https://github.com/falexwolf) | 2023-02-22 | 0.3rc1
```

### Comparing `lamin_logger-0.5.1/docs/quickstart.ipynb` & `lamin_logger-0.5.2/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/lamin_logger/_core.py` & `lamin_logger-0.5.2/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/lamin_logger/_logger.py` & `lamin_logger-0.5.2/lamin_logger/_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Logging and Profiling."""
 import logging
 import platform
+import sys
 from datetime import datetime, timedelta, timezone
 from logging import CRITICAL, DEBUG, ERROR, INFO, WARNING, getLevelName
 from typing import Optional
 
 HINT = 15
 DOWNLOAD = 21
 SUCCESS = 25
@@ -163,15 +164,15 @@
         return result
 
 
 logger = RootLogger()
 
 
 def set_handler(logger):
-    h = logging.StreamHandler()
+    h = logging.StreamHandler(stream=sys.stdout)
     h.setFormatter(_LogFormatter())
     h.setLevel(logger.level)
     if len(logger.handlers) == 1:
         logger.removeHandler(logger.handlers[0])
     elif len(logger.handlers) > 1:
         raise RuntimeError("Lamin's root logger somehow got more than one handler")
     logger.addHandler(h)
```

### Comparing `lamin_logger-0.5.1/lamin_logger/_lookup.py` & `lamin_logger-0.5.2/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/lamin_logger/_map_synonyms.py` & `lamin_logger-0.5.2/lamin_logger/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/lamin_logger/_python_version.py` & `lamin_logger-0.5.2/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/lamin_logger/_search.py` & `lamin_logger-0.5.2/lamin_logger/_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/pyproject.toml` & `lamin_logger-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/tests/test_lookup.py` & `lamin_logger-0.5.2/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/tests/test_map_synonyms.py` & `lamin_logger-0.5.2/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/tests/test_search.py` & `lamin_logger-0.5.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.5.1/PKG-INFO` & `lamin_logger-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.5.1
+Version: 0.5.2
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

