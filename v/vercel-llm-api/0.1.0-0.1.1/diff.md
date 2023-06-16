# Comparing `tmp/vercel_llm_api-0.1.0-py3-none-any.whl.zip` & `tmp/vercel_llm_api-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 17949 bytes, number of entries: 6
--rw-r--r--  2.0 unx     4641 b- defN 23-May-29 09:51 vercel_ai.py
--rw-r--r--  2.0 unx    35148 b- defN 23-May-29 12:03 vercel_llm_api-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6596 b- defN 23-May-29 12:03 vercel_llm_api-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 12:03 vercel_llm_api-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-29 12:03 vercel_llm_api-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      491 b- defN 23-May-29 12:03 vercel_llm_api-0.1.0.dist-info/RECORD
-6 files, 46978 bytes uncompressed, 17059 bytes compressed:  63.7%
+Zip file size: 17943 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     4639 b- defN 23-Jun-16 18:58 vercel_ai.py
+-rw-r--r--  2.0 unx    35148 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6599 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      491 b- defN 23-Jun-16 18:59 vercel_llm_api-0.1.1.dist-info/RECORD
+6 files, 46979 bytes uncompressed, 17053 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: vercel_ai.py
 Comment: 
 
-Filename: vercel_llm_api-0.1.0.dist-info/LICENSE
+Filename: vercel_llm_api-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: vercel_llm_api-0.1.0.dist-info/METADATA
+Filename: vercel_llm_api-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: vercel_llm_api-0.1.0.dist-info/WHEEL
+Filename: vercel_llm_api-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: vercel_llm_api-0.1.0.dist-info/top_level.txt
+Filename: vercel_llm_api-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vercel_llm_api-0.1.0.dist-info/RECORD
+Filename: vercel_llm_api-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vercel_ai.py

```diff
@@ -10,15 +10,15 @@
 
 logging.basicConfig()
 logger = logging.getLogger()
 
 class Client:
   base_url = "https://play.vercel.ai"
   token_url = base_url + "/openai.jpeg" #nice try vercel
-  generate_url = base_url + "/api/generate"
+  generate_url = base_url + "/api/prompt"
 
   def __init__(self):
     self.session = requests.Session(impersonate="chrome110")
     self.headers = {
       "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110 Safari/537.36",
       "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
       "Accept-Encoding": "gzip, deflate, br",
```

## Comparing `vercel_llm_api-0.1.0.dist-info/LICENSE` & `vercel_llm_api-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vercel_llm_api-0.1.0.dist-info/METADATA` & `vercel_llm_api-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: vercel-llm-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: A reverse engineered API for the Vercel AI playground.
 Home-page: https://github.com/ading2210/vercel-llm-api
 Author: ading2210
 License: GPLv3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: curl-cffi
+License-File: LICENSE
 Requires-Dist: quickjs
+Requires-Dist: curl-cffi
 
 # Python Vercel LLM API
 
 [![PyPi Version](https://img.shields.io/pypi/v/vercel-llm-api.svg)](https://pypi.org/project/vercel-llm-api/)
 
 This is a reverse engineered API wrapper for the [Vercel AI Playground](https://play.vercel.ai/), which allows for free access to many LLMs, including OpenAI's ChatGPT, Cohere's Command Nightly, as well as some open source models.
 
@@ -190,8 +190,7 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ```
-
```

