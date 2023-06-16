# Comparing `tmp/nhl_api_py-0.3.0.tar.gz` & `tmp/nhl_api_py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.3.0.tar", max compression
+gzip compressed data, was "nhl_api_py-0.4.1.tar", max compression
```

## Comparing `nhl_api_py-0.3.0.tar` & `nhl_api_py-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     3819 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/__init__.py
--rw-r--r--   0        0        0      315 2023-06-09 15:14:25.320047 nhl_api_py-0.3.0/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/core.py
--rw-r--r--   0        0        0     4171 2023-06-08 18:58:55.919296 nhl_api_py-0.3.0/nhlpy/api/games.py
--rw-r--r--   0        0        0     2856 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/nhlpy/api/helpers.py
--rw-r--r--   0        0        0     2016 2023-06-08 18:14:40.069269 nhl_api_py-0.3.0/nhlpy/api/players.py
--rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/standings.py
--rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.3.0/nhlpy/api/teams.py
--rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1277 2023-06-13 00:29:30.470493 nhl_api_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4871 1970-01-01 00:00:00.000000 nhl_api_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4792 2023-06-13 00:47:35.510504 nhl_api_py-0.4.1/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.4.1/nhlpy/__init__.py
+-rw-r--r--   0        0        0      315 2023-06-09 15:14:25.320047 nhl_api_py-0.4.1/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.4.1/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4213 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/games.py
+-rw-r--r--   0        0        0     6775 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/helpers.py
+-rw-r--r--   0        0        0     2035 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/players.py
+-rw-r--r--   0        0        0      910 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1967 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     2146 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      641 2023-06-13 00:29:30.470493 nhl_api_py-0.4.1/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1390 2023-06-16 18:35:41.424465 nhl_api_py-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5957 1970-01-01 00:00:00.000000 nhl_api_py-0.4.1/PKG-INFO
```

### Comparing `nhl_api_py-0.3.0/nhlpy/api/core.py` & `nhl_api_py-0.4.1/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.3.0/nhlpy/api/games.py` & `nhl_api_py-0.4.1/nhlpy/api/games.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 from typing import Union, List
 from nhlpy.api import BaseNHLAPIClient
 
+
 class Games(BaseNHLAPIClient):
     """
     This class is used to access the NHL API for game data.
     """
 
     def get_game_types(self) -> dict:
         """
@@ -54,25 +55,28 @@
             {GameType} are the following: 01=preseason, 02=regular season, 03=playoffs, 04=all-star.
 
             {GameNumber} is the game number in the season, starting at 0001.
         :return: dict
         """
         return self._get(resource=f"game/{game_id}/feed/live").json()
 
-    def get_game_live_feed_diff_after_timestamp(self, game_id: Union[str, int], timestamp: str) -> dict:
+    def get_game_live_feed_diff_after_timestamp(
+        self, game_id: Union[str, int], timestamp: str
+    ) -> dict:
         """
         Returns the difference in the live feed game data, from since the given timestamp: param.
         :param game_id:
         :param timestamp:
         :return:
         """
-        warnings.warn("This endpoint is still experimental and may not work as expected")
+        warnings.warn(
+            "This endpoint is still experimental and may not work as expected"
+        )
         return self._get(resource=f"game/{game_id}/feed/live/diffPath").json()
 
-
     def get_game_boxscore(self, game_id: Union[str, int]) -> List[dict]:
         """
         Less detail than get_game_live_feed() but still a large response, contains lots of information about
         the game.
 
         See documentation for get_game_live_feed() for more verbose explanation of game_id.
         :param game_id:
@@ -97,8 +101,8 @@
         headlines, description, etc.  A very large response payload.
 
         See documentation for get_game_live_feed() for more verbose explanation of game_id.
 
         :param game_id:
         :return:
         """
-        return self._get(resource=f"game/{game_id}/content").json()
+        return self._get(resource=f"game/{game_id}/content").json()
```

### Comparing `nhl_api_py-0.3.0/nhlpy/api/players.py` & `nhl_api_py-0.4.1/nhlpy/api/players.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Players(BaseNHLAPIClient):
     def get_player(self, person_id: str) -> dict:
         """
         Returns a player based on the person_id.
         :param person_id:
         :return:
         """
-        return self._get(resource=f"people/{person_id}").json()
+        return self._get(resource=f"people/{person_id}").json()["people"]
 
     def get_player_stats(
         self, person_id: str, season: str = None, stat_type: str = "statsSingleSeason"
     ) -> dict:
         """
         This returns a players statistics based on the param stat_type: and season:  An example of this
         may be client.players.get_player_stats(stat_type="yearByYear", season="20202021").  In some instances season:
@@ -28,15 +28,15 @@
             goalsByGameSituation, goalsByGameSituationPlayoffs, statsSingleSeason, statsSingleSeasonPlayoffs
 
         :return:
         """
         query = f"stats={stat_type}" if stat_type else ""
         return self._get(
             resource=f"people/{person_id}/stats?season={season}&{query}"
-        ).json()
+        ).json()["stats"]
 
     def get_player_stat_types(self) -> dict:
         """
         Returns the full list of stat(types) that can be used in get_player_stats()'s stat_type param
         :return:
         """
         return self._get(resource="statTypes").json()
```

### Comparing `nhl_api_py-0.3.0/nhlpy/api/standings.py` & `nhl_api_py-0.4.1/nhlpy/api/standings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 from nhlpy.api import BaseNHLAPIClient
 
 
 class Standings(BaseNHLAPIClient):
+    def get_standing_types(self) -> dict:
+        """
+        Returns a list of standing types that can be used in get_standings_by_standing_type()
+        :return: dict of standing types
+        """
+        return self._get(resource="standingsTypes").json()
+
     def get_standings(self, season: str = None, detailed_record: bool = False) -> dict:
         """
         Gets the standings for the season supplied via season: param.
         :param season:
         :param detailed_record: Detailed information for each team including
             home and away records, record in shootouts, last ten games, and split
             head-to-head records against divisions and conferences.
         :return: dict
         """
-        modifier = f"season={season}&" if season else ""
-        detailed = "expand=standings.record&" if detailed_record else ""
-        return self._get(resource=f"standings?{modifier}{detailed}").json()
+        modifier: str = f"season={season}&" if season else ""
+        detailed: str = "expand=standings.record&" if detailed_record else ""
 
-    def get_standing_types(self) -> dict:
-        """
-        Returns a list of standing types that can be used in get_standings_by_standing_type()
-        :return: dict of standing types
-        """
-        return self._get(resource="standingsTypes").json()
+        response: dict = self._get(resource=f"standings?{modifier}{detailed}").json()
+        return response["records"]
 
     def get_standings_by_standing_type(
         self, season: str, standing_type: str, detailed_records: bool = False
     ) -> dict:
         """
 
         :param detailed_records:  bool, indicates whether or not to return detailed records for each team
         :param season: str, Season in the format of 20202021
         :param standing_type: str, full list found in get_standing_types() with the following options:
             regularSeason, wildCard,divisionLeaders, wildCardWithLeaders, preseason,
             postseason, byDivision, byConference, byLeague
         :return: dict
         """
-        query = f"season={season}&"
-        detailed = "expand=standings.record&" if detailed_records else ""
-        return self._get(resource=f"standings/{standing_type}?{query}{detailed}").json()
+        query: str = f"season={season}&"
+        detailed: str = "expand=standings.record&" if detailed_records else ""
+        response: dict = self._get(
+            resource=f"standings/{standing_type}?{query}{detailed}"
+        ).json()
+        return response["records"]
```

### Comparing `nhl_api_py-0.3.0/nhlpy/api/teams.py` & `nhl_api_py-0.4.1/nhlpy/api/teams.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,64 +3,69 @@
 
 class Teams(BaseNHLAPIClient):
     def all(self) -> dict:
         """
         Returns a list of all teams.
         :return: dict
         """
-        return self._get(resource="/teams").json()
+        response: dict = self._get(resource="/teams").json()
+        return response["teams"]
 
     def get_by_id(
         self,
         id: int,
         roster: bool = False,
     ) -> dict:
         """
         Returns a team by id.
         :param id: int, NHL team id
         :param roster: bool, Should include the roster for the team
         :return: dict
         """
-        query = ""
+        query: str = ""
         if roster:
             query += "?expand=team.roster"
-        return self._get(resource=f"teams/{id}{query}").json()
+        return self._get(resource=f"teams/{id}{query}").json()["teams"]
 
     def get_team_next_game(self, id: int) -> dict:
         """
         Returns the next game for the team with the id supplied.
         :param id: int, NHL team id
         :return: dict
         """
-        return self._get(resource=f"teams/{id}?expand=team.schedule.next").json()
+        return self._get(resource=f"teams/{id}?expand=team.schedule.next").json()[
+            "teams"
+        ]
 
     def get_team_previous_game(self, id: int) -> dict:
         """
         Returns the previous game for the team with the id supplied.
         :param id: int, NHL team id
         :return: dict
         """
-        return self._get(resource=f"teams/{id}?expand=team.schedule.previous").json()
+        return self._get(resource=f"teams/{id}?expand=team.schedule.previous").json()[
+            "teams"
+        ]
 
     def get_team_with_stats(self, id: int) -> dict:
         """
         Returns the team with stats for the team with the id supplied.
         :param id: int, NHL team id
         :return: dict
         """
-        return self._get(resource=f"teams/{id}?expand=team.stats").json()
+        return self._get(resource=f"teams/{id}?expand=team.stats").json()["teams"]
 
     def get_team_roster(self, id: int) -> dict:
         """
         Returns the roster for the team with the id supplied.
         :param id: int, NHL team id
         :return: dict
         """
-        return self._get(resource=f"teams/{id}/roster").json()
+        return self._get(resource=f"teams/{id}/roster").json()["roster"]
 
     def get_team_stats(self, id: int) -> dict:
         """
         Returns the stats for the team with the id supplied.
         :param id:
         :return: dict
         """
-        return self._get(resource=f"teams/{id}/stats").json()
+        return self._get(resource=f"teams/{id}/stats").json()["stats"]
```

### Comparing `nhl_api_py-0.3.0/nhlpy/nhl_client.py` & `nhl_api_py-0.4.1/nhlpy/nhl_client.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.3.0/pyproject.toml` & `nhl_api_py-0.4.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.3.0"
-description = "NHL API Wrapper.  For standings, team stats, outcomes and player information."
+version = "0.4.1"
+description = "NHL API.  For standings, team stats, outcomes, player information.  Contains each individual API endpoint as well as convience methods for easy data loading in Pandas or any ML applications."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
 keywords = ["nhl", "api", "wrapper", "hockey", "sports"]
```

### Comparing `nhl_api_py-0.3.0/PKG-INFO` & `nhl_api_py-0.4.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: nhl-api-py
-Version: 0.3.0
-Summary: NHL API Wrapper.  For standings, team stats, outcomes and player information.
-Home-page: https://github.com/coreyjs/nhl-api-py
-License: GPL-3.0-or-later
-Keywords: nhl,api,wrapper,hockey,sports
-Author: Corey Schaf
-Author-email: cschaf@gmail.com
-Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: httpx
-Project-URL: Repository, https://github.com/coreyjs/nhl-api-py
-Description-Content-Type: text/markdown
-
 [![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
 ![nhl-api-py workflow](https://github.com/coreyjs/nhl-api-py/actions/workflows/python-app.yml/badge.svg?branch=main)
 
 # NHL-API-PY
 
 NHL-api-py is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
@@ -68,16 +44,41 @@
 client.standings.get_standing_types()
 
 # Player Stats
 client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
 client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="goalsByGameSituation")
 client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="yearByYear")
 
+# Schedule
+client.schedule.get_schedule(season="20222023")
+
+# Games
+client.games.get_game_types()
+client.games.get_game_play_types()
+client.games.get_game_status_codes()
+client.games.get_game_live_feed(game_id=2020020001)
+client.games.get_game_live_feed_diff_after_timestamp(game_id=2020020001, timestamp=1633070400)
+client.games.get_game_boxscore(game_id=2020020001)
+client.games.get_game_linescore(game_id=2020020001)
+client.games.get_game_content(game_id=2020020001)
+
+# Players
+client.players.get_player(person_id=8477949)
+client.players.get_player_stats(person_id=8477949, season="20222023", stat_type="statsSingleSeason")
+client.players.get_player_stat_types()
+
+# Helpers - Common use cases, data extraction, etc.  For easier dataframe .  These return data that has been parsed
+# out, with some additional calculations as well.
+standings_list = nhl_client.helpers.league_standings(season="20222023")
+standings_df = pd.DataFrame(standings_list)
+standings_df.head(20)
 ```
 
+
+
 - - - 
 
 As mentioned at the top, I created a notebook to go over some of the available methods in more detail.  Below is an export md of that notebook, with out cell executions.
 
 ```python
 pip install nhl-api-py
 ```
@@ -204,8 +205,7 @@
 
 - - - 
 
 
 ### Developers
 
 `poetry install --with dev`
-
```

