# Comparing `tmp/Wavelink-2.5.0.tar.gz` & `tmp/Wavelink-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Wavelink-2.5.0.tar", last modified: Thu Jun 15 02:34:49 2023, max compression
+gzip compressed data, was "Wavelink-2.5.1.tar", last modified: Fri Jun 16 12:59:26 2023, max compression
```

## Comparing `Wavelink-2.5.0.tar` & `Wavelink-2.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.423637 Wavelink-2.5.0/
--rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     5772 2023-06-15 02:34:49.423637 Wavelink-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.5.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.407184 Wavelink-2.5.0/Wavelink.egg-info/
--rw-rw-rw-   0        0        0     5772 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-15 02:34:49.000000 Wavelink-2.5.0/Wavelink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1006 2023-06-15 00:30:25.000000 Wavelink-2.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.5.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 02:34:49.424137 Wavelink-2.5.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.418133 Wavelink-2.5.0/wavelink/
--rw-rw-rw-   0        0        0     1495 2023-06-15 00:30:25.000000 Wavelink-2.5.0/wavelink/__init__.py
--rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/backoff.py
--rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.5.0/wavelink/enums.py
--rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.5.0/wavelink/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.389981 Wavelink-2.5.0/wavelink/ext/
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.419134 Wavelink-2.5.0/wavelink/ext/spotify/
--rw-rw-rw-   0        0        0    17743 2023-06-15 00:16:21.000000 Wavelink-2.5.0/wavelink/ext/spotify/__init__.py
--rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/filters.py
--rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.5.0/wavelink/node.py
--rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.5.0/wavelink/payloads.py
--rw-rw-rw-   0        0        0    22017 2023-06-12 11:33:29.000000 Wavelink-2.5.0/wavelink/player.py
--rw-rw-rw-   0        0        0    12545 2023-06-15 00:04:14.000000 Wavelink-2.5.0/wavelink/queue.py
--rw-rw-rw-   0        0        0     9954 2023-06-15 00:00:10.000000 Wavelink-2.5.0/wavelink/tracks.py
-drwxrwxrwx   0        0        0        0 2023-06-15 02:34:49.422636 Wavelink-2.5.0/wavelink/types/
--rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/events.py
--rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/request.py
--rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/state.py
--rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.5.0/wavelink/types/track.py
--rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.5.0/wavelink/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.328668 Wavelink-2.5.1/
+-rw-rw-rw-   0        0        0     1108 2023-03-09 18:26:07.000000 Wavelink-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-06-16 12:59:26.328157 Wavelink-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4969 2023-03-09 18:33:50.000000 Wavelink-2.5.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.313156 Wavelink-2.5.1/Wavelink.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-16 12:59:26.000000 Wavelink-2.5.1/Wavelink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1006 2023-06-16 12:55:24.000000 Wavelink-2.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       49 2023-03-09 18:26:07.000000 Wavelink-2.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 12:59:26.328668 Wavelink-2.5.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.323151 Wavelink-2.5.1/wavelink/
+-rw-rw-rw-   0        0        0     1495 2023-06-16 12:55:24.000000 Wavelink-2.5.1/wavelink/__init__.py
+-rw-rw-rw-   0        0        0     2701 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/backoff.py
+-rw-rw-rw-   0        0        0     3689 2023-06-05 10:25:32.000000 Wavelink-2.5.1/wavelink/enums.py
+-rw-rw-rw-   0        0        0     3028 2023-06-05 09:44:43.000000 Wavelink-2.5.1/wavelink/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.295797 Wavelink-2.5.1/wavelink/ext/
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.323651 Wavelink-2.5.1/wavelink/ext/spotify/
+-rw-rw-rw-   0        0        0    17836 2023-06-16 12:50:04.000000 Wavelink-2.5.1/wavelink/ext/spotify/__init__.py
+-rw-rw-rw-   0        0        0    20203 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/filters.py
+-rw-rw-rw-   0        0        0    17836 2023-06-05 08:54:30.000000 Wavelink-2.5.1/wavelink/node.py
+-rw-rw-rw-   0        0        0     3461 2023-05-20 08:41:44.000000 Wavelink-2.5.1/wavelink/payloads.py
+-rw-rw-rw-   0        0        0    22017 2023-06-12 11:33:29.000000 Wavelink-2.5.1/wavelink/player.py
+-rw-rw-rw-   0        0        0    12545 2023-06-15 00:04:14.000000 Wavelink-2.5.1/wavelink/queue.py
+-rw-rw-rw-   0        0        0     9954 2023-06-15 00:00:10.000000 Wavelink-2.5.1/wavelink/tracks.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:59:26.327154 Wavelink-2.5.1/wavelink/types/
+-rw-rw-rw-   0        0        0      860 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/events.py
+-rw-rw-rw-   0        0        0      635 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/request.py
+-rw-rw-rw-   0        0        0      424 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/state.py
+-rw-rw-rw-   0        0        0      343 2023-03-09 18:26:07.000000 Wavelink-2.5.1/wavelink/types/track.py
+-rw-rw-rw-   0        0        0     9570 2023-05-20 08:53:53.000000 Wavelink-2.5.1/wavelink/websocket.py
```

### Comparing `Wavelink-2.5.0/LICENSE` & `Wavelink-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/PKG-INFO` & `Wavelink-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.5.0
+Version: 2.5.1
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.5.0/README.rst` & `Wavelink-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/Wavelink.egg-info/PKG-INFO` & `Wavelink-2.5.1/Wavelink.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Wavelink
-Version: 2.5.0
+Version: 2.5.1
 Summary: A robust and powerful Lavalink wrapper for discord.py
 Author-email: EvieePy <evieepy@gmail.com>
 Project-URL: Homepage, https://github.com/PythonistaGuild/Wavelink
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `Wavelink-2.5.0/Wavelink.egg-info/SOURCES.txt` & `Wavelink-2.5.1/Wavelink.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/pyproject.toml` & `Wavelink-2.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Wavelink"
-version = "2.5.0"
+version = "2.5.1"
 authors = [
   { name="EvieePy", email="evieepy@gmail.com" },
 ]
 dynamic = ["dependencies"]
 description = "A robust and powerful Lavalink wrapper for discord.py"
 readme = "README.rst"
 requires-python = ">=3.10"
```

### Comparing `Wavelink-2.5.0/wavelink/__init__.py` & `Wavelink-2.5.1/wavelink/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 __title__ = "WaveLink"
 __author__ = "PythonistaGuild, EvieePy"
 __license__ = "MIT"
 __copyright__ = "Copyright 2019-Present (c) PythonistaGuild, EvieePy"
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 
 from .enums import *
 from .exceptions import *
 from .node import *
 from .payloads import *
 from .player import Player as Player
 from .tracks import *
```

### Comparing `Wavelink-2.5.0/wavelink/backoff.py` & `Wavelink-2.5.1/wavelink/backoff.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/enums.py` & `Wavelink-2.5.1/wavelink/enums.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/exceptions.py` & `Wavelink-2.5.1/wavelink/exceptions.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/ext/spotify/__init__.py` & `Wavelink-2.5.1/wavelink/ext/spotify/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,28 +380,30 @@
         Parameters
         ----------
         player: :class:`wavelink.player.Player`
             If :attr:`wavelink.Player.autoplay` is enabled, this search will fill the AutoPlay Queue with more tracks.
         cls
             The class to convert this Spotify Track to.
         """
-        try:
-            tracks: list[cls] = await cls.search(f'"{self.isrc}"')
-        except wavelink.NoTracksError:
+        tracks: list[cls] = await cls.search(f'"{self.isrc}"')
+        if not tracks:
             tracks: list[cls] = await cls.search(f'{self.name} - {self.artists[0]}')
 
         if not player.autoplay or not populate:
             return tracks[0]
 
         node: Node = player.current_node
         sc: SpotifyClient | None = node._spotify
 
         if not sc:
             raise RuntimeError(f"There is no spotify client associated with <{node:!r}>")
 
+        if sc.is_token_expired():
+            await sc._get_bearer_token()
+
         if len(player._track_seeds) == 5:
             player._track_seeds.pop(0)
 
         player._track_seeds.append(self.id)
 
         url: str = RECURL.format(tracks=','.join(player._track_seeds))
         async with node._session.get(url=url, headers=sc.bearer_headers) as resp:
@@ -433,15 +435,15 @@
 
     def __init__(self, *, client_id: str, client_secret: str):
         self._client_id = client_id
         self._client_secret = client_secret
 
         self.session = aiohttp.ClientSession()
 
-        self._bearer_token: str = None  # type: ignore
+        self._bearer_token: str | None = None
         self._expiry: int = 0
 
     @property
     def grant_headers(self) -> dict:
         authbytes = f'{self._client_id}:{self._client_secret}'.encode()
         return {'Authorization': f'Basic {base64.b64encode(authbytes).decode()}',
                 'Content-Type': 'application/x-www-form-urlencoded'}
@@ -455,21 +457,24 @@
             if resp.status != 200:
                 raise SpotifyRequestError(resp.status, resp.reason)
 
             data = await resp.json()
             self._bearer_token = data['access_token']
             self._expiry = time.time() + (int(data['expires_in']) - 10)
 
+    def is_token_expired(self) -> bool:
+        return time.time() >= self._expiry
+
     async def _search(self,
                       query: str,
                       type: SpotifySearchType = SpotifySearchType.track,
                       iterator: bool = False,
                       ) -> list[SpotifyTrack]:
 
-        if not self._bearer_token or time.time() >= self._expiry:
+        if self.is_token_expired():
             await self._get_bearer_token()
 
         regex_result = URLREGEX.match(query)
 
         url = (
             BASEURL.format(
                 entity=regex_result['type'], identifier=regex_result['id']
```

### Comparing `Wavelink-2.5.0/wavelink/filters.py` & `Wavelink-2.5.1/wavelink/filters.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/node.py` & `Wavelink-2.5.1/wavelink/node.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/payloads.py` & `Wavelink-2.5.1/wavelink/payloads.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/player.py` & `Wavelink-2.5.1/wavelink/player.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/queue.py` & `Wavelink-2.5.1/wavelink/queue.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/tracks.py` & `Wavelink-2.5.1/wavelink/tracks.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/types/events.py` & `Wavelink-2.5.1/wavelink/types/events.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/types/request.py` & `Wavelink-2.5.1/wavelink/types/request.py`

 * *Files identical despite different names*

### Comparing `Wavelink-2.5.0/wavelink/websocket.py` & `Wavelink-2.5.1/wavelink/websocket.py`

 * *Files identical despite different names*

