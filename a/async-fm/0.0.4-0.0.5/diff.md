# Comparing `tmp/async_fm-0.0.4.tar.gz` & `tmp/async_fm-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_fm-0.0.4.tar", max compression
+gzip compressed data, was "async_fm-0.0.5.tar", max compression
```

## Comparing `async_fm-0.0.4.tar` & `async_fm-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-06-10 22:08:34.648947 async_fm-0.0.4/LICENSE
--rw-r--r--   0        0        0     1590 2023-06-10 22:08:34.648947 async_fm-0.0.4/README.md
--rw-r--r--   0        0        0      683 2023-06-10 22:08:34.648947 async_fm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      130 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/__init__.py
--rw-r--r--   0        0        0     1264 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/api/__init__.py
--rw-r--r--   0        0        0    14950 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/api/user.py
--rw-r--r--   0        0        0     2403 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/exceptions.py
--rw-r--r--   0        0        0     1437 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/types.py
--rw-r--r--   0        0        0      208 2023-06-10 22:08:34.648947 async_fm-0.0.4/src/asyncfm/utils.py
--rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-15 23:38:58.618624 async_fm-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1590 2023-06-15 23:38:58.618624 async_fm-0.0.5/README.md
+-rw-r--r--   0        0        0      683 2023-06-15 23:38:58.618624 async_fm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/__init__.py
+-rw-r--r--   0        0        0     1264 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/api/__init__.py
+-rw-r--r--   0        0        0    14965 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/api/user.py
+-rw-r--r--   0        0        0     2403 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/exceptions.py
+-rw-r--r--   0        0        0     1437 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/types.py
+-rw-r--r--   0        0        0      208 2023-06-15 23:38:58.618624 async_fm-0.0.5/src/asyncfm/utils.py
+-rw-r--r--   0        0        0     2273 1970-01-01 00:00:00.000000 async_fm-0.0.5/PKG-INFO
```

### Comparing `async_fm-0.0.4/LICENSE` & `async_fm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.4/README.md` & `async_fm-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.4/pyproject.toml` & `async_fm-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Async-FM"
-version = "0.0.4"
+version = "0.0.5"
 description = "Python library for interacting with the Last.fm API asynchronously."
 authors = ["NachABR <nachabr@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "asyncfm", from = "src"}]
 homepage = "https://github.com/NachABR/async-fm"
 repository = "https://github.com/NachABR/async-fm.git"
```

### Comparing `async_fm-0.0.4/src/asyncfm/api/__init__.py` & `async_fm-0.0.5/src/asyncfm/api/__init__.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.4/src/asyncfm/api/user.py` & `async_fm-0.0.5/src/asyncfm/api/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         if to_time is not None:
             params["to"] = to_time
 
         data = await self.api._make_request(params=params)
 
         if recent_tracks := data.get("recenttracks"):
             return Responses.Tracks(
-                data=list(
+                tracks=list(
                     map(
                         lambda track: Track(
                             artist=track["artist"]["#text"],
                             title=track["name"],
                             album=track["album"]["#text"],
                             images=get_images_(track.get("image")),
                             now_playing="@attr" in track
@@ -117,15 +117,15 @@
             "period": period,
             "limit": limit,
             "page": page,
         }
         data = await self.api._make_request(params=params)
         if artists := data.get("topartists"):
             return Responses.Artists(
-                data=list(
+                artists=list(
                     map(
                         lambda artist: Artist(
                             name=artist["name"],
                             images=get_images_(artist.get("image")),
                             playcount=artist["playcount"],
                             rank=artist["@attr"]["rank"],
                         ),
@@ -155,15 +155,15 @@
             "period": period,
             "limit": limit,
             "page": page,
         }
         data = await self.api._make_request(params=params)
         if albums := data.get("topalbums"):
             return Responses.Albums(
-                data=list(
+                albums=list(
                     map(
                         lambda album: Album(
                             artist=album["artist"]["name"],
                             title=album["name"],
                             images=get_images_(album.get("image")),
                             playcount=album["playcount"],
                             rank=album["@attr"]["rank"],
@@ -201,15 +201,15 @@
             "page": page,
         }
 
         data = await self.api._make_request(params=params)
 
         if top_tracks := data.get("toptracks"):
             return Responses.Tracks(
-                data=[
+                tracks=[
                     Track(
                         artist=track["artist"]["name"],
                         title=track["name"],
                         images=get_images_(track.get("image")),
                     )
                     for track in top_tracks["track"]
                 ],
@@ -240,15 +240,15 @@
             "page": page,
         }
 
         data = await self.api._make_request(params=params)
 
         if top_tags := data.get("toptags"):
             return Responses.Tags(
-                data=[Tag(**tag) for tag in top_tags["tag"]],
+                tags=[Tag(**tag) for tag in top_tags["tag"]],
                 total=len(top_tags["tag"]),
             )
 
     async def get_weekly_artist_chart(
         self,
         username: str,
         from_date: Optional[datetime] = None,
@@ -271,15 +271,15 @@
         if to_date is not None:
             params["to"] = to_date.strftime("%Y-%m-%d")
 
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklyartistchart"):
             return Responses.Tracks(
-                data=list(
+                tracks=list(
                     map(
                         lambda artist: Artist(
                             name=artist["name"],
                             playcount=artist["playcount"],
                             images=get_images_(images=images)
                             if (images := artist.get("image"))
                             else None,
@@ -316,15 +316,15 @@
         if to_date:
             params["to"] = to_date.strftime("%Y-%m-%d")
 
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklyalbumchart"):
             return Responses.Albums(
-                data=list(
+                albums=list(
                     map(
                         lambda album: Album(
                             artist=album["artist"]["#text"],
                             title=album["name"],
                             images=get_images_(images=images)
                             if (images := album.get("image"))
                             else None,
@@ -363,15 +363,15 @@
             params["from"] = from_date.strftime("%Y-%m-%d")
         if to_date is not None:
             params["to"] = to_date.strftime("%Y-%m-%d")
         data = await self.api._make_request(params=params)
 
         if weekly_chart := data.get("weeklytrackchart"):
             return Responses.Tracks(
-                data=list(
+                tracks=list(
                     map(
                         lambda track: Track(
                             artist=track["artist"]["#text"],
                             title=track["name"],
                             images=get_images_(track.get("image")),
                             rank=track["@attr"]["rank"],
                             playcount=track["playcount"],
```

### Comparing `async_fm-0.0.4/src/asyncfm/exceptions.py` & `async_fm-0.0.5/src/asyncfm/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.4/src/asyncfm/types.py` & `async_fm-0.0.5/src/asyncfm/types.py`

 * *Files identical despite different names*

### Comparing `async_fm-0.0.4/PKG-INFO` & `async_fm-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-fm
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for interacting with the Last.fm API asynchronously.
 Home-page: https://github.com/NachABR/async-fm
 License: MIT
 Keywords: python,lastfm,aiohttp,async
 Author: NachABR
 Author-email: nachabr@protonmail.com
 Requires-Python: >=3.10,<4.0
```

