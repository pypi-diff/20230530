# Comparing `tmp/soccerdata-1.3.6.tar.gz` & `tmp/soccerdata-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.3.6.tar", max compression
+gzip compressed data, was "soccerdata-1.4.0.tar", max compression
```

## Comparing `soccerdata-1.3.6.tar` & `soccerdata-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1384 2023-04-28 15:50:52.938151 soccerdata-1.3.6/LICENSE.rst
--rw-r--r--   0        0        0     3130 2023-04-28 15:50:52.938151 soccerdata-1.3.6/README.rst
--rw-r--r--   0        0        0     2352 2023-04-28 15:51:06.062018 soccerdata-1.3.6/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-28 15:51:06.062018 soccerdata-1.3.6/soccerdata/__init__.py
--rw-r--r--   0        0        0    20428 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/_common.py
--rw-r--r--   0        0        0     5144 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/_config.py
--rw-r--r--   0        0        0     6218 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/clubelo.py
--rw-r--r--   0        0        0    12693 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/espn.py
--rw-r--r--   0        0        0    31315 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/fbref.py
--rw-r--r--   0        0        0     8584 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0     4547 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/match_history.py
--rw-r--r--   0        0        0     9831 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/sofifa.py
--rw-r--r--   0        0        0    32302 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/whoscored.py
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.3.6/setup.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1384 2023-05-30 09:46:00.237763 soccerdata-1.4.0/LICENSE.rst
+-rw-r--r--   0        0        0     3130 2023-05-30 09:46:00.237763 soccerdata-1.4.0/README.rst
+-rw-r--r--   0        0        0     2352 2023-05-30 09:46:16.973858 soccerdata-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-05-30 09:46:16.973858 soccerdata-1.4.0/soccerdata/__init__.py
+-rw-r--r--   0        0        0    20702 2023-05-30 09:46:00.245763 soccerdata-1.4.0/soccerdata/_common.py
+-rw-r--r--   0        0        0     5120 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/_config.py
+-rw-r--r--   0        0        0     6382 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    12890 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/espn.py
+-rw-r--r--   0        0        0    42225 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8536 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0     4547 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/match_history.py
+-rw-r--r--   0        0        0    16744 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    32302 2023-05-30 09:46:00.249763 soccerdata-1.4.0/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.4.0/setup.py
+-rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.4.0/PKG-INFO
```

### Comparing `soccerdata-1.3.6/LICENSE.rst` & `soccerdata-1.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.6/README.rst` & `soccerdata-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.6/pyproject.toml` & `soccerdata-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.3.6"
+version = "1.4.0"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
@@ -31,15 +31,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 mypy = "^1.0"
 pylint = "^2.15.5"
 pytest-deadfixtures = "^2.2.1"
 unify = "^0.5"
 black = "^23.0.0"
-Sphinx = "^6.0.0"
+Sphinx = "^7.0.0"
 sphinx-autobuild = "^2021.3.14"
 furo = "^2023.0.0"
 coverage = {version = "^7.0", extras = ["toml"]}
 pre-commit = "^3.0.0"
 flake8 = "^6.0.0"
 flake8-bugbear = "^23.0.0"
 flake8-docstrings = "^1.6.0"
```

### Comparing `soccerdata-1.3.6/soccerdata/_common.py` & `soccerdata-1.4.0/soccerdata/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,14 +512,21 @@
 
     def to_snake(name: str) -> str:
         name = re.sub("(.)([A-Z][a-z]+)", r"\1_\2", name)
         name = re.sub("__([A-Z])", r"_\1", name)
         name = re.sub("([a-z0-9])([A-Z])", r"\1_\2", name)
         return name.lower().replace("-", "_").replace(" ", "")
 
+    if df.columns.nlevels > 1 and cols is None:
+        # only standardize the first level
+        new_df = df.copy()
+        new_cols = [to_snake(c) for c in df.columns.levels[0]]
+        new_df.columns = new_df.columns.set_levels(new_cols, level=0)
+        return new_df
+
     if cols is None:
         cols = list(df.columns)
 
     return df.rename(columns={c: to_snake(c) for c in cols})
 
 
 def get_proxy() -> Dict[str, str]:
```

### Comparing `soccerdata-1.3.6/soccerdata/_config.py` & `soccerdata-1.4.0/soccerdata/_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -92,59 +92,59 @@
 LEAGUE_DICT = {
     "ENG-Premier League": {
         "ClubElo": "ENG_1",
         "MatchHistory": "E0",
         "FiveThirtyEight": "premier-league",
         "FBref": "Premier League",
         "ESPN": "eng.1",
-        "SoFIFA": "English Premier League (1)",
+        "SoFIFA": "[England] Premier League",
         "WhoScored": "England - Premier League",
         "season_start": "Aug",
         "season_end": "May",
     },
     "ESP-La Liga": {
         "ClubElo": "ESP_1",
         "MatchHistory": "SP1",
         "FiveThirtyEight": "la-liga",
         "FBref": "La Liga",
         "ESPN": "esp.1",
-        "SoFIFA": "Spain Primera Division (1)",
+        "SoFIFA": "[Spain] La Liga",
         "WhoScored": "Spain - LaLiga",
         "season_start": "Aug",
         "season_end": "May",
     },
     "ITA-Serie A": {
         "ClubElo": "ITA_1",
         "MatchHistory": "I1",
         "FiveThirtyEight": "serie-a",
         "FBref": "Serie A",
         "ESPN": "ita.1",
-        "SoFIFA": " Italian Serie A (1)",
+        "SoFIFA": "[Italy] Serie A",
         "WhoScored": "Italy - Serie A",
         "season_start": "Aug",
         "season_end": "May",
     },
     "GER-Bundesliga": {
         "ClubElo": "GER_1",
         "MatchHistory": "D1",
         "FiveThirtyEight": "bundesliga",
         "FBref": "Fußball-Bundesliga",
         "ESPN": "ger.1",
-        "SoFIFA": "German 1. Bundesliga (1)",
+        "SoFIFA": "[Germany] Bundesliga",
         "WhoScored": "Germany - Bundesliga",
         "season_start": "Aug",
         "season_end": "May",
     },
     "FRA-Ligue 1": {
         "ClubElo": "FRA_1",
         "MatchHistory": "F1",
         "FiveThirtyEight": "ligue-1",
         "FBref": "Ligue 1",
         "ESPN": "fra.1",
-        "SoFIFA": "French Ligue 1 (1)",
+        "SoFIFA": "[France] Ligue 1",
         "WhoScored": "France - Ligue 1",
         "season_start": "Aug",
         "season_end": "May",
     },
     "INT-World Cup": {
         "FBref": "FIFA World Cup",
         "WhoScored": "International - FIFA World Cup",
```

### Comparing `soccerdata-1.3.6/soccerdata/clubelo.py` & `soccerdata-1.4.0/soccerdata/clubelo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """Scraper for api.clubelo.com."""
 import re
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Callable, Dict, List, Optional, Union
+from typing import IO, Callable, Dict, List, Optional, Union
 
 import pandas as pd
 from unidecode import unidecode
 
 from ._common import BaseRequestsReader, standardize_colnames
 from ._config import DATA_DIR, NOCACHE, NOSTORE, TEAMNAME_REPLACEMENTS
 
 CLUB_ELO_DATADIR = DATA_DIR / "ClubElo"
 CLUB_ELO_API = "http://api.clubelo.com"
 
 
+def _parse_csv(data: IO[bytes]) -> pd.DataFrame:
+    return pd.read_csv(
+        data, parse_dates=["From", "To"], infer_datetime_format=True, dayfirst=False
+    )
+
+
 class ClubElo(BaseRequestsReader):
     """Provides pd.DataFrames from CSV API at http://api.clubelo.com.
 
     Data will be downloaded as necessary and cached locally in
     ``~/soccerdata/data/ClubElo``.
 
     Since the source does not provide league names, this class will not filter
@@ -58,49 +64,55 @@
             Union[str, Dict[str, str], List[Dict[str, str]], Callable[[], Dict[str, str]]]
         ] = None,
         no_cache: bool = NOCACHE,
         no_store: bool = NOSTORE,
         data_dir: Path = CLUB_ELO_DATADIR,
     ):
         """Initialize a new ClubElo reader."""
-        super().__init__(no_cache=no_cache, no_store=no_store, data_dir=data_dir)
+        super().__init__(proxy=proxy, no_cache=no_cache, no_store=no_store, data_dir=data_dir)
 
     def read_by_date(self, date: Optional[Union[str, datetime]] = None) -> pd.DataFrame:
         """Retrieve ELO scores for all teams at specified date.
 
         Elo scores are available as early as 1939. Values before 1960 should
         be considered provisional.
 
         Parameters
         ----------
         date : datetime object or string like 'YYYY-MM-DD'
             Date for which to retrieve ELO scores. If no date is specified,
             get today's scores.
 
+        Raises
+        ------
+        TypeError
+            If date is not a date string or datetime object.
+        ValueError
+            If data is an invalid date string.
+
         Returns
         -------
         pd.DataFrame
         """
         if not date:
             date = datetime.today()
         elif isinstance(date, str):
             date = datetime.strptime(date, "%Y-%m-%d")
-        else:
-            pass  # Assume datetime object
+
+        if not isinstance(date, datetime):
+            raise TypeError("'date' must be a datetime object or string like 'YYYY-MM-DD'")
 
         datestring = date.strftime("%Y-%m-%d")
         filepath = self.data_dir / f"{datestring}.csv"
         url = f"{CLUB_ELO_API}/{datestring}"
 
         data = self.get(url, filepath)
 
         df = (
-            pd.read_csv(
-                data, parse_dates=["From", "To"], infer_datetime_format=True, dayfirst=False
-            )
+            _parse_csv(data)
             .pipe(standardize_colnames)
             .rename(columns={"club": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .replace("None", float("nan"))
             .assign(rank=lambda x: x["rank"].astype("float"))
             .assign(league=lambda x: x["country"] + "_" + x["level"].astype(str))
             .pipe(self._translate_league)
@@ -110,24 +122,24 @@
         return df
 
     def read_team_history(
         self, team: str, max_age: Union[int, timedelta] = 1
     ) -> Optional[pd.DataFrame]:
         """Retrieve full ELO history for one club.
 
-        For the exact spelling of a club's name, check the result
-        of :func:`~soccerdata.ClubElo.read_by_date` or
-        `clubelo.com <http://clubelo.com/Ranking>`__. You can also use
-        alternative team names specified in `teamname_replacements.json`.
-        Values before 1960 should be considered provisional.
+        For the exact spelling of a club's name, check the result of
+        :func:`~soccerdata.ClubElo.read_by_date` or `clubelo.com
+        <http://clubelo.com/Ranking>`__. You can also use alternative team
+        names specified in `teamname_replacements.json`. Values before 1960
+        should be considered provisional.
 
         Parameters
         ----------
         team : str
-            The club's name
+            The club's name.
         max_age : int for age in days, or timedelta object
             The max. age of locally cached file before re-download.
 
         Raises
         ------
         TypeError
             If max_age is not an integer or timedelta object.
@@ -147,20 +159,15 @@
 
         for _team in teams_to_check:
             filepath = self.data_dir / f"{_team}.csv"
             url = f"{CLUB_ELO_API}/{_team}"
             data = self.get(url, filepath, max_age)
 
             df = (
-                pd.read_csv(
-                    data,
-                    parse_dates=["From", "To"],
-                    infer_datetime_format=True,
-                    dayfirst=False,
-                )
+                _parse_csv(data)
                 .pipe(standardize_colnames)
                 .rename(columns={"club": "team"})
                 .replace("None", float("nan"))
                 .assign(rank=lambda x: x["rank"].astype("float"))
                 .set_index("from")
                 .sort_index()
             )
```

### Comparing `soccerdata-1.3.6/soccerdata/espn.py` & `soccerdata-1.4.0/soccerdata/espn.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import itertools
 import json
 import re
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
-import requests
 
 from ._common import BaseRequestsReader, make_game_id, standardize_colnames
 from ._config import DATA_DIR, NOCACHE, NOSTORE, TEAMNAME_REPLACEMENTS, logger
 
 # http://site.api.espn.com/apis/site/v2/sports/soccer/eng.1/summary?event=513466
 # http://site.api.espn.com/apis/site/v2/sports/soccer/eng.1/scoreboard?dates=20180901
+# http://site.api.espn.com/apis/site/v2/sports/soccer/eng.1/news
+# http://site.api.espn.com/apis/site/v2/sports/soccer/eng.1/teams
 
 ESPN_DATADIR = DATA_DIR / "ESPN"
 ESPN_API = "http://site.api.espn.com/apis/site/v2/sports/soccer"
 
 
 class ESPN(BaseRequestsReader):
     """Provides pd.DataFrames from JSON api available at http://site.api.espn.com.
@@ -25,15 +26,14 @@
     Data will be downloaded as necessary and cached locally in
     ``~/soccerdata/data/ESPN``.
 
     Parameters
     ----------
     leagues : string or iterable, optional
         IDs of leagues to include.
-
     seasons : string, int or list, optional
         Seasons to include. Supports multiple formats.
         Examples: '16-17'; 2016; '2016-17'; [14, 15, 16]
     proxy : 'tor' or dict or list(dict) or callable, optional
         Use a proxy to hide your IP address. Valid options are:
             - "tor": Uses the Tor network. Tor should be running in
               the background on port 9050.
@@ -100,16 +100,17 @@
         for lkey, skey in itertools.product(self._selected_leagues.values(), self.seasons):
             if int(skey[:2]) > int(str(datetime.datetime.now().year + 1)[-2:]):
                 start_date = "".join(["19", skey[:2], "07", "01"])
             else:
                 start_date = "".join(["20", skey[:2], "07", "01"])
 
             url = urlmask.format(lkey, start_date)
-            resp = requests.get(url=url)
-            data = resp.json()
+            filepath = self.data_dir / filemask.format(lkey, start_date)
+            reader = self.get(url, filepath)
+            data = json.load(reader)
 
             match_dates = [
                 datetime.datetime.strptime(d, "%Y-%m-%dT%H:%MZ").strftime("%Y%m%d")
                 for d in data["leagues"][0]["calendar"]
             ]
             for date in match_dates:
                 url = urlmask.format(lkey, date)
```

### Comparing `soccerdata-1.3.6/soccerdata/fbref.py` & `soccerdata-1.4.0/soccerdata/fbref.py`

 * *Files 15% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         return df.loc[
             df.index.isin(itertools.product(self.leagues, self.seasons)), ["format", "url"]
         ]
 
     def read_team_season_stats(  # noqa: C901
         self, stat_type: str = "standard", opponent_stats: bool = False
     ) -> pd.DataFrame:
-        """Retrieve teams from the datasource for the selected leagues.
+        """Retrieve aggregated season stats for all teams in the selected leagues and seasons.
 
         The following stat types are available:
             * 'standard'
             * 'keeper'
             * 'keeper_adv'
             * 'shooting'
             * 'passing'
@@ -222,15 +222,15 @@
         stat_type: str
             Type of stats to retrieve.
         opponent_stats: bool
             If True, will retrieve opponent stats.
 
         Raises
         ------
-        TypeError
+        ValueError
             If ``stat_type`` is not valid.
 
         Returns
         -------
         pd.DataFrame
         """
         team_stats = [
@@ -246,15 +246,15 @@
             "playing_time",
             "misc",
         ]
 
         filemask = "teams_{}_{}_{}.html"
 
         if stat_type not in team_stats:
-            raise TypeError(f"Invalid argument: stat_type should be in {team_stats}")
+            raise ValueError(f"Invalid argument: stat_type should be in {team_stats}")
 
         if stat_type == "standard":
             page = "stats"
         elif stat_type == "keeper":
             page = "keepers"
         elif stat_type == "keeper_adv":
             page = "keepersadv"
@@ -311,23 +311,192 @@
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
                 df_table.drop("Rk", axis=1, level=1, inplace=True)
             teams.append(df_table)
 
         # return data frame
         df = (
             _concat(teams)
-            .rename(columns={"Squad": "team"})
+            .rename(columns={"Squad": "team", "# Pl": "players_used"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
+            # .pipe(standardize_colnames)
             .set_index(["league", "season", "team"])
             .sort_index()
         )
         return df
 
+    def read_team_match_stats(  # noqa: C901
+        self,
+        stat_type: str = "schedule",
+        opponent_stats: bool = False,
+        team: Optional[Union[str, List[str]]] = None,
+    ) -> pd.DataFrame:
+        """Retrieve the match logs for all teams in the selected leagues and seasons.
+
+        The following stat types are available:
+            * 'schedule'
+            * 'keeper'
+            * 'shooting'
+            * 'passing'
+            * 'passing_types'
+            * 'goal_shot_creation'
+            * 'defense'
+            * 'possession'
+            * 'misc'
+
+        Parameters
+        ----------
+        stat_type: str
+            Type of stats to retrieve.
+        opponent_stats: bool
+            If True, will retrieve opponent stats.
+        team: str or list of str, optional
+            Team(s) to retrieve. If None, will retrieve all teams.
+
+        Raises
+        ------
+        ValueError
+            If ``stat_type`` is not valid.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        team_stats = [
+            "schedule",
+            "shooting",
+            "keeper",
+            "passing",
+            "passing_types",
+            "goal_shot_creation",
+            "defense",
+            "possession",
+            "misc",
+        ]
+
+        filemask = "matchlogs_{}_{}_{}.html"
+
+        if stat_type not in team_stats:
+            raise ValueError(f"Invalid argument: stat_type should be in {team_stats}")
+
+        if stat_type == "goal_shot_creation":
+            stat_type = "gca"
+
+        if opponent_stats:
+            opp_type = "against"
+        else:
+            opp_type = "for"
+
+        # get list of teams
+        df_teams = self.read_team_season_stats()
+
+        if team is not None:
+            # get alternative names of the specified team(s)
+            teams = [team] if isinstance(team, str) else team
+            teams_to_check = []
+            for team in teams:
+                for alt_name, norm_name in TEAMNAME_REPLACEMENTS.items():
+                    if norm_name == team:
+                        teams_to_check.append(alt_name)
+            teams_to_check.append(team)
+
+            # select requested teams
+            iterator = df_teams.loc[df_teams.index.isin(teams_to_check, level=2), :]
+            if len(iterator) == 0:
+                raise ValueError("No data found for the given teams in the selected seasons.")
+        else:
+            iterator = df_teams
+
+        # collect match logs for each team
+        stats = []
+        for (lkey, skey, team), team_url in iterator.url.items():
+            # read html page
+            filepath = self.data_dir / filemask.format(team, skey, stat_type)
+            url = (
+                FBREF_API
+                + team_url.rsplit("/", 1)[0]
+                + "/matchlogs"
+                + "/all_comps"
+                + f"/{stat_type}"
+            )
+            reader = self.get(url, filepath)
+
+            # parse HTML and select table
+            tree = html.parse(reader)
+            (html_table,) = tree.xpath(f"//table[@id='matchlogs_{opp_type}']")
+            # remove icons
+            for elem in html_table.xpath("//span"):
+                elem.getparent().remove(elem)
+            # remove for / against header
+            for elem in html_table.xpath("//th[@data-stat='header_for_against']"):
+                elem.text = ""
+            # remove table sections
+            for elem in html_table.xpath("//tr[contains(@class, 'thead')]"):
+                elem.getparent().remove(elem)
+            # remove aggregate rows
+            for elem in html_table.xpath("//tfoot"):
+                elem.getparent().remove(elem)
+            # parse table
+            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table["league"] = lkey
+            df_table["season"] = skey
+            df_table["team"] = team
+            df_table["Time"] = html_table.xpath(".//td[@data-stat='start_time']/@csk")
+            df_table["Match Report"] = [
+                mlink.xpath("./a/@href")[0]
+                if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
+                else None
+                for mlink in html_table.xpath(".//td[@data-stat='match_report']")
+            ]
+            nb_levels = df_table.columns.nlevels
+            if nb_levels == 2:
+                df_table = df_table.drop("Comp", axis=1, level=1)
+                df_table = df_table.drop("Match Report", axis=1, level=1)
+                df_table = df_table.drop("Time", axis=1, level=1)
+            else:
+                del df_table["Comp"]
+            stats.append(df_table)
+
+        # return data frame
+        df = (
+            _concat(stats)
+            .replace(
+                {
+                    "Opponent": TEAMNAME_REPLACEMENTS,
+                }
+            )
+            .pipe(
+                standardize_colnames,
+                cols=[
+                    "Team",
+                    "Opponent",
+                    "Venue",
+                    "Date",
+                    "Time",
+                    "Round",
+                    "Day",
+                    "Result",
+                    "Match Report",
+                ],
+            )
+        )
+        df["date"] = pd.to_datetime(df["date"]).ffill()
+        # create match id column
+        df_tmp = df[["team", "opponent", "venue", "date"]].copy()
+        df_tmp.columns = ["team", "opponent", "venue", "date"]
+        df_tmp["home_team"] = df_tmp.apply(
+            lambda x: x["team"] if x["venue"] == "Home" else x["opponent"], axis=1
+        )
+        df_tmp["away_team"] = df_tmp.apply(
+            lambda x: x["team"] if x["venue"] == "Away" else x["opponent"], axis=1
+        )
+        df["game"] = df_tmp.apply(make_game_id, axis=1)
+        return df.set_index(["league", "season", "team", "game"]).sort_index().loc[self.leagues]
+
     def read_player_season_stats(self, stat_type: str = "standard") -> pd.DataFrame:  # noqa: C901
-        """Retrieve players from the datasource for the selected leagues.
+        """Retrieve players from the datasource for the selected leagues and seasons.
 
         The following stat types are available:
             * 'standard'
             * 'shooting'
             * 'passing'
             * 'passing_types'
             * 'goal_shot_creation'
@@ -413,47 +582,26 @@
                 df_table[("Unnamed: season", "season")] = skey
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
             else:
                 (el,) = tree.xpath(f"//comment()[contains(.,'div_stats_{stat_type}')]")
                 (df_table,) = pd.read_html(el.text, attrs={"id": f"stats_{stat_type}"})
                 df_table[("Unnamed: league", "league")] = lkey
                 df_table[("Unnamed: season", "season")] = skey
-
-            if not ("Unnamed: 2_level_0", "Nation") in df_table.columns:
-                df_table.loc[:, (slice(None), "Squad")] = (
-                    df_table.xs("Squad", axis=1, level=1)
-                    .squeeze()
-                    .apply(
-                        lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Squad" else None
-                    )
-                )
-                df_table.insert(
-                    2,
-                    ("Unnamed: nation", "Nation"),
-                    df_table.xs("Squad", axis=1, level=1).squeeze(),
-                )
-            else:
-                df_table.loc[:, (slice(None), "Nation")] = (
-                    df_table.xs("Nation", axis=1, level=1)
-                    .squeeze()
-                    .apply(
-                        lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Nation" else None
-                    )
-                )
-
+            df_table = _fix_nation_col(df_table)
             players.append(df_table)
 
         # return dataframe
         df = _concat(players)
         df = df[df.Player != "Player"]
         df = (
             df.drop("Matches", axis=1, level=0)
             .drop("Rk", axis=1, level=0)
-            .rename(columns={"Player": "player", "Squad": "team"})
+            .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
+            .pipe(standardize_colnames, cols=["Player", "Nation", "Pos", "Age", "Born"])
             .set_index(["league", "season", "team", "player"])
             .sort_index()
         )
 
         return df
 
     def read_schedule(self, force_cache: bool = False) -> pd.DataFrame:
@@ -541,14 +689,133 @@
         """
         team_nodes = tree.xpath("//div[@class='scorebox']//strong/a")[:2]
         teams = []
         for team in team_nodes:
             teams.append({"id": team.get("href").split("/")[3], "name": team.text.strip()})
         return teams
 
+    def read_player_match_stats(
+        self,
+        stat_type: str = "summary",
+        match_id: Optional[Union[str, List[str]]] = None,
+        force_cache: bool = False,
+    ) -> pd.DataFrame:
+        """Retrieve the match stats for the selected leagues and seasons.
+
+        The following stat types are available:
+            * 'summary'
+            * 'keepers'
+            * 'passing'
+            * 'passing_types'
+            * 'defense'
+            * 'possession'
+            * 'misc'
+
+        Parameters
+        ----------
+        stat_type : str
+            Type of stats to retrieve.
+        match_id : int or list of int, optional
+            Retrieve the event stream for a specific game.
+        force_cache : bool
+            By default no cached data is used to scrape the list of available
+            games for the current season. If True, will force the use of
+            cached data anyway.
+
+        Raises
+        ------
+        ValueError
+            If no games with the given IDs were found for the selected seasons and leagues.
+        TypeError
+            If ``stat_type`` is not valid.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
+        match_stats = [
+            "summary",
+            "keepers",
+            "passing",
+            "passing_types",
+            "defense",
+            "possession",
+            "misc",
+        ]
+
+        urlmask = FBREF_API + "/en/matches/{}"
+        filemask = "match_{}.html"
+
+        if stat_type not in match_stats:
+            raise TypeError(f"Invalid argument: stat_type should be in {match_stats}")
+
+        # Retrieve games for which a match report is available
+        df_schedule = self.read_schedule(force_cache).reset_index()
+        df_schedule = df_schedule[~df_schedule.game_id.isna() & ~df_schedule.match_report.isnull()]
+        # Selec requested games if available
+        if match_id is not None:
+            iterator = df_schedule[
+                df_schedule.game_id.isin([match_id] if isinstance(match_id, str) else match_id)
+            ]
+            if len(iterator) == 0:
+                raise ValueError("No games found with the given IDs in the selected seasons.")
+        else:
+            iterator = df_schedule
+
+        stats = []
+        for i, game in iterator.reset_index().iterrows():
+            url = urlmask.format(game["game_id"])
+            # get league and season
+            logger.info(
+                "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
+            )
+            filepath = self.data_dir / filemask.format(game["game_id"])
+            reader = self.get(url, filepath)
+            tree = html.parse(reader)
+            (home_team, away_team) = self._parse_teams(tree)
+            if stat_type == "keepers":
+                id_format = "keeper_stats_{}"
+            else:
+                id_format = "stats_{}_" + stat_type
+            html_table = tree.find("//table[@id='" + id_format.format(home_team["id"]) + "']")
+            if html_table is not None:
+                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table["team"] = home_team["name"]
+                df_table["game"] = game["game"]
+                df_table["league"] = game["league"]
+                df_table["season"] = game["season"]
+                df_table["game_id"] = game["game_id"]
+                df_table = _fix_nation_col(df_table)
+                stats.append(df_table)
+            else:
+                logger.warning("No stats found for home team for game with id=%s", game["game_id"])
+            html_table = tree.find("//table[@id='" + id_format.format(away_team["id"]) + "']")
+            if html_table is not None:
+                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table["team"] = away_team["name"]
+                df_table["game"] = game["game"]
+                df_table["league"] = game["league"]
+                df_table["season"] = game["season"]
+                df_table["game_id"] = game["game_id"]
+                df_table = _fix_nation_col(df_table)
+                stats.append(df_table)
+            else:
+                logger.warning("No stats found for away team for game with id=%s", game["game_id"])
+
+        df = _concat(stats)
+        df = df[~df.Player.str.contains(r"^\d+\sPlayers$")]
+        df = (
+            df.rename(columns={"#": "jersey_number"})
+            .replace({"team": TEAMNAME_REPLACEMENTS})
+            .pipe(standardize_colnames, cols=["Player", "Nation", "Pos", "Age", "Min"])
+            .set_index(["league", "season", "game", "team", "player"])
+            .sort_index()
+        )
+        return df
+
     def read_lineup(
         self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
     ) -> pd.DataFrame:
         """Retrieve lineups for the selected leagues and seasons.
 
         Parameters
         ----------
@@ -593,144 +860,128 @@
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
             html_tables = tree.xpath("//div[@class='lineup']")
             for i, html_table in enumerate(html_tables):
+                # parse lineup table
                 (df_table,) = pd.read_html(html.tostring(html_table))
                 df_table.columns = ["jersey_number", "player"]
                 df_table["team"] = teams[i]["name"]
                 if "Bench" in df_table.jersey_number.values:
                     bench_idx = df_table.index[df_table.jersey_number == "Bench"][0]
                     df_table.loc[:bench_idx, "is_starter"] = True
                     df_table.loc[bench_idx:, "is_starter"] = False
                     df_table["game"] = game["game"]
                     df_table["league"] = game["league"]
                     df_table["season"] = game["season"]
                     df_table["game"] = game["game"]
                     df_table.drop(bench_idx, inplace=True)
-                lineups.append(df_table)
-        df = pd.concat(lineups).set_index(["league", "season", "game", "team", "player"])
-        # TODO: sub in, sub out, position
+                # augment with stats
+                html_stats_table = tree.find(
+                    "//table[@id='" + "stats_{}_summary".format(teams[i]["id"]) + "']"
+                )
+                (df_stats_table,) = pd.read_html(html.tostring(html_stats_table))
+                df_stats_table = df_stats_table.droplevel(0, axis=1)[["Player", "Pos", "Min"]]
+                df_stats_table.columns = ["player", "position", "minutes_played"]
+                lineups.append(pd.merge(df_table, df_stats_table, on="player", how="left"))
+        df = pd.concat(lineups).set_index(["league", "season", "game"])
         return df
 
-    def read_player_match_stats(
-        self,
-        stat_type: str = "summary",
-        match_id: Optional[Union[str, List[str]]] = None,
-        force_cache: bool = False,
+    def read_events(
+        self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
     ) -> pd.DataFrame:
-        """Retrieve the match stats for the selected leagues and seasons.
+        """Retrieve match events for the selected seasons or selected matches.
 
-        The following stat types are available:
-            * 'summary'
-            * 'keepers'
-            * 'passing'
-            * 'passing_types'
-            * 'defense'
-            * 'possession'
-            * 'misc'
+        The data returned includes the timing of goals, cards and substitutions.
+        Also includes the players who are involved in the event.
 
         Parameters
         ----------
-        stat_type : str
-            Type of stats to retrieve.
         match_id : int or list of int, optional
-            Retrieve the event stream for a specific game.
+            Retrieve the events for a specific game.
         force_cache : bool
             By default no cached data is used to scrape the list of available
             games for the current season. If True, will force the use of
             cached data anyway.
 
         Raises
         ------
         ValueError
             If no games with the given IDs were found for the selected seasons and leagues.
-        TypeError
-            If ``stat_type`` is not valid.
 
         Returns
         -------
-        pd.DataFrame
+        pd.DataFrame.
         """
-        match_stats = [
-            "summary",
-            "keepers",
-            "passing",
-            "passing_types",
-            "defense",
-            "possession",
-            "misc",
-        ]
-
         urlmask = FBREF_API + "/en/matches/{}"
         filemask = "match_{}.html"
 
-        if stat_type not in match_stats:
-            raise TypeError(f"Invalid argument: stat_type should be in {match_stats}")
-
         # Retrieve games for which a match report is available
         df_schedule = self.read_schedule(force_cache).reset_index()
         df_schedule = df_schedule[~df_schedule.game_id.isna() & ~df_schedule.match_report.isnull()]
         # Selec requested games if available
         if match_id is not None:
             iterator = df_schedule[
                 df_schedule.game_id.isin([match_id] if isinstance(match_id, str) else match_id)
             ]
             if len(iterator) == 0:
                 raise ValueError("No games found with the given IDs in the selected seasons.")
         else:
             iterator = df_schedule
 
-        stats = []
+        events = []
         for i, game in iterator.reset_index().iterrows():
+            match_events = []
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
-            (home_team, away_team) = self._parse_teams(tree)
-            if stat_type == "keepers":
-                id_format = "keeper_stats_{}"
-            else:
-                id_format = "stats_{}_" + stat_type
-            html_table = tree.find("//table[@id='" + id_format.format(home_team["id"]) + "']")
-            if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table))
-                df_table["team"] = home_team["name"]
-                df_table["game"] = game["game"]
-                df_table["league"] = game["league"]
-                df_table["season"] = game["season"]
-                df_table["game_id"] = game["game_id"]
-                stats.append(df_table)
-            else:
-                logger.warning("No stats found for home team for game with id=%s", game["game_id"])
-            html_table = tree.find("//table[@id='" + id_format.format(away_team["id"]) + "']")
-            if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table))
-                df_table["team"] = away_team["name"]
-                df_table["game"] = game["game"]
-                df_table["league"] = game["league"]
-                df_table["season"] = game["season"]
-                df_table["game_id"] = game["game_id"]
-                stats.append(df_table)
-            else:
-                logger.warning("No stats found for away team for game with id=%s", game["game_id"])
+            teams = self._parse_teams(tree)
+            for team, tid in zip(teams, ["a", "b"]):
+                html_events = tree.xpath(f"////*[@id='events_wrap']/div/div[@class='event {tid}']")
+                for e in html_events:
+                    minute = e.xpath("./div[1]")[0].text.replace("&rsquor;", "").strip()
+                    score = e.xpath("./div[1]/small/span")[0].text
+                    player1 = e.xpath("./div[2]/div[2]/div/a")[0].text
+                    if e.xpath("./div[2]/div[2]/small"):
+                        player2 = e.xpath("./div[2]/div[2]/small/a")[0].text
+                    else:
+                        player2 = None
+                    event_type = e.xpath("./div[2]/div[1]/@class")[0].split(" ")[1]
+                    match_events.append(
+                        {
+                            "team": team["name"],
+                            "minute": minute,
+                            "score": score,
+                            "player1": player1,
+                            "player2": player2,
+                            "event_type": event_type,
+                        }
+                    )
+            df_match_events = pd.DataFrame(match_events).sort_values(by="minute")
+            df_match_events["game"] = game["game"]
+            df_match_events["league"] = game["league"]
+            df_match_events["season"] = game["season"]
+            events.append(df_match_events)
+
+        if len(events) == 0:
+            return pd.DataFrame()
 
-        df = _concat(stats)
-        df = df[~df.Player.str.contains(r"^\d+\sPlayers$")]
         df = (
-            df.rename(columns={"Player": "player"})
+            _concat(events)
             .replace({"team": TEAMNAME_REPLACEMENTS})
-            .set_index(["league", "season", "game", "team", "player"])
+            .set_index(["league", "season", "game"])
             .sort_index()
+            .dropna(how="all")
         )
         return df
 
     def read_shot_events(
         self, match_id: Optional[Union[str, List[str]]] = None, force_cache: bool = False
     ) -> pd.DataFrame:
         """Retrieve shooting data for the selected seasons or selected matches.
@@ -738,15 +989,15 @@
         The data returned includes who took the shot, when, with which body
         part and from how far away. Additionally, the player creating the
         chance and also the creation before this are included in the data.
 
         Parameters
         ----------
         match_id : int or list of int, optional
-            Retrieve the lineup for a specific game.
+            Retrieve the shots for a specific game.
         force_cache : bool
             By default no cached data is used to scrape the list of available
             games for the current season. If True, will force the use of
             cached data anyway.
 
         Raises
         ------
@@ -781,31 +1032,34 @@
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             html_table = tree.find("//table[@id='shots_all']")
             if html_table is not None:
-                (df_table,) = pd.read_html(html.tostring(html_table))
+                (df_table,) = pd.read_html(html.tostring(html_table), flavor="lxml")
                 df_table["league"] = game["league"]
                 df_table["season"] = game["season"]
                 df_table["game"] = game["game"]
                 shots.append(df_table)
             else:
                 logger.warning("No shot data found for game with id=%s", game["game_id"])
 
+        if len(shots) == 0:
+            return pd.DataFrame()
+
         df = (
             _concat(shots)
             .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(
                 standardize_colnames,
                 cols=["Outcome", "Minute", "Distance", "Player", "Body Part", "Notes", "Event"],
             )
-            .set_index(["league", "season", "game", "team", "player"])
+            .set_index(["league", "season", "game"])
             .sort_index()
             .dropna(how="all")
         )
         return df
 
 
 def _concat(dfs: List[pd.DataFrame]) -> pd.DataFrame:
@@ -825,25 +1079,62 @@
         Concatenated dataframe with uniform column names.
     """
     # Look for the most complete level 0 columns
     all_columns = []
     for df in dfs:
         columns = pd.DataFrame(df.columns.tolist())
         # Move missing columns to level 0
-        columns.replace({"": None}, inplace=True)
-        mask = pd.isnull(columns[1])
-        columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
+        if columns.shape[1] == 2:
+            columns.replace({"": None}, inplace=True)
+            mask = pd.isnull(columns[1])
+            columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
         # Rename unnamed columns
         mask = columns[0].str.startswith("Unnamed:").fillna(False)
         columns.loc[mask, 0] = None
         all_columns.append(columns)
     columns = reduce(lambda left, right: left.combine_first(right), all_columns)
 
     # Move the remaining missing columns back to level 1 and replace with empyt string
-    mask = pd.isnull(columns[0])
-    columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
-    columns.loc[mask, 1] = ""
+    if columns.shape[1] == 2:
+        mask = pd.isnull(columns[0])
+        columns.loc[mask, [0, 1]] = columns.loc[mask, [1, 0]].values
+        columns.loc[mask, 1] = ""
 
-    for df in dfs:
-        df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
+        for df in dfs:
+            df.columns = pd.MultiIndex.from_tuples(columns.to_records(index=False).tolist())
 
     return pd.concat(dfs)
+
+
+def _fix_nation_col(df_table: pd.DataFrame) -> pd.DataFrame:
+    """Fix the "Nation" column.
+
+    Removes the flag icon for domestic games and adds a 'nations' column for
+    international games based on the team's name.
+
+    Parameters
+    ----------
+    df_table : pd.DataFrame
+        Input dataframe.
+
+    Returns
+    -------
+    pd.DataFrame
+    """
+    if "Nation" not in df_table.columns.get_level_values(1):
+        df_table.loc[:, (slice(None), "Squad")] = (
+            df_table.xs("Squad", axis=1, level=1)
+            .squeeze()
+            .apply(lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Squad" else None)
+        )
+        df_table.insert(
+            2,
+            ("Unnamed: nation", "Nation"),
+            df_table.xs("Squad", axis=1, level=1).squeeze(),
+        )
+    else:
+        df_table.loc[:, (slice(None), "Nation")] = (
+            df_table.xs("Nation", axis=1, level=1)
+            .squeeze(axis=1)
+            .apply(lambda x: x.split(" ")[1] if isinstance(x, str) and x != "Nation" else None)
+        )
+    return df_table
```

### Comparing `soccerdata-1.3.6/soccerdata/fivethirtyeight.py` & `soccerdata-1.4.0/soccerdata/fivethirtyeight.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from ._config import DATA_DIR, NOCACHE, NOSTORE, TEAMNAME_REPLACEMENTS
 
 FIVETHIRTYEIGHT_DATA_DIR = DATA_DIR / "FiveThirtyEight"
 FIVETHIRTYEIGHT_API = "https://projects.fivethirtyeight.com/soccer-predictions"
 
 
 class FiveThirtyEight(BaseRequestsReader):
-    """Provides pd.DataFrames from fivethirtyeight's "Club Soccer Predictions" project.
+    """Provides pd.DataFrames from FiveThirtyEight's "Club Soccer Predictions" project.
 
     Data will be downloaded as necessary and cached locally in
     ``~/soccerdata/data/FiveThirtyEight``.
 
     Original project and background info:
     https://projects.fivethirtyeight.com/soccer-predictions/ and
     https://fivethirtyeight.com/features/how-our-club-soccer-projections-work/
 
 
     Parameters
     ----------
     leagues : string or iterable, optional
-        IDs of Leagues to include.
+        IDs of leagues to include.
     seasons : string, int or list, optional
         Seasons to include. Supports multiple formats.
         Examples: '16-17'; 2016; '2016-17'; [14, 15, 16]
     proxy : 'tor' or dict or list(dict) or callable, optional
         Use a proxy to hide your IP address. Valid options are:
             - "tor": Uses the Tor network. Tor should be running in
               the background on port 9050.
@@ -68,32 +68,29 @@
         data_dir: Path = FIVETHIRTYEIGHT_DATA_DIR,
     ):
         """Initialize a new FiveThirtyEight reader."""
         super().__init__(
             leagues=leagues, proxy=proxy, no_cache=no_cache, no_store=no_store, data_dir=data_dir
         )
         self.seasons = seasons  # type: ignore
-        self._data = {}
-
-        url = f"{FIVETHIRTYEIGHT_API}/data.json"
-        filepath = self.data_dir / "latest.json"
-        reader = self.get(url, filepath)
-
-        for k, v in json.load(reader).items():
-            self._data[k] = v
 
     def read_leagues(self) -> pd.DataFrame:
         """Retrieve the selected leagues from the datasource.
 
         Returns
         -------
         pd.DataFrame
         """
+        url = f"{FIVETHIRTYEIGHT_API}/data.json"
+        filepath = self.data_dir / "latest.json"
+        reader = self.get(url, filepath)
+        data = json.load(reader)
+
         df = (
-            pd.DataFrame.from_dict(self._data["leagues"])
+            pd.DataFrame.from_dict(data["leagues"])
             .rename(columns={"slug": "league", "id": "league_id"})
             .pipe(self._translate_league)
             .pipe(standardize_colnames)
             .drop(columns=["overview_column", "custom_template", "skip_cols"])
             .set_index("league")
             .loc[self._selected_leagues.keys()]
             .sort_index()
@@ -173,22 +170,22 @@
         data = []
         for lkey, skey in itertools.product(self._selected_leagues.values(), self.seasons):
             filepath = self.data_dir / filemask.format(lkey, skey)
             url = urlmask.format(skey[:2], lkey)
             reader = self.get(url, filepath)
 
             forecasts = json.load(reader)
-            for f in forecasts["forecasts"]:
-                for t in f["teams"]:
+            for forecast in forecasts["forecasts"]:
+                for team in forecast["teams"]:
                     data.append(
                         {
                             "league": lkey,
                             "season": skey,
-                            "last_updated": f["last_updated"],
-                            **t,
+                            "last_updated": forecast["last_updated"],
+                            **team,
                         }
                     )
         df = (
             pd.DataFrame.from_dict(data)
             .rename(columns={"name": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .replace("None", float("nan"))
```

### Comparing `soccerdata-1.3.6/soccerdata/match_history.py` & `soccerdata-1.4.0/soccerdata/match_history.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.6/soccerdata/whoscored.py` & `soccerdata-1.4.0/soccerdata/whoscored.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.6/setup.py` & `soccerdata-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'rich>=13.0.0,<14.0.0',
  'selenium>=4.0.0,<5.0.0',
  'undetected-chromedriver>=3.1.3,<4.0.0',
  'unicode>=2.7,<3.0']
 
 setup_kwargs = {
     'name': 'soccerdata',
-    'version': '1.3.6',
+    'version': '1.4.0',
     'description': 'A collection of wrappers over soccer data from various websites / APIs.',
     'long_description': ".. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png\n   :align: center\n   :alt: SoccerData\n   :width: 600px\n\n.. badges-begin\n\n|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/soccerdata.svg\n   :target: https://pypi.org/project/soccerdata/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/soccerdata\n   :target: https://pypi.org/project/soccerdata\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/soccerdata.svg\n   :target: https://opensource.org/licenses/Apache-2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/soccerdata/latest.svg?label=Read%20the%20Docs\n   :target: https://soccerdata.readthedocs.io/\n   :alt: Read the documentation at https://soccerdata.readthedocs.io/\n.. |Tests| image:: https://github.com/probberechts/soccerdata/workflows/CI/badge.svg\n   :target: https://github.com/probberechts/soccerdata/actions?workflow=CI\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/probberechts/soccerdata/branch/master/graph/badge.svg\n   :target: https://app.codecov.io/gh/probberechts/soccerdata\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\nSoccerData is a collection of wrappers over soccer data from `Club Elo`_,\n`ESPN`_, `FBref`_, `FiveThirtyEight`_, `Football-Data.co.uk`_, `SoFIFA`_ and\n`WhoScored`_. You get Pandas DataFrames with sensible, matching column names\nand identifiers across datasets. Data is downloaded when needed and cached\nlocally.\n\n.. code:: python\n\n   import soccerdata as sd\n\n   # Create scraper class instance for the Premier League\n   five38 = sd.FiveThirtyEight('ENG-Premier League', '1819')\n\n   # Fetch dataframes\n   games = five38.read_games()\n\nTo learn how to install, configure and use SoccerData, see the\n`Quickstart guide <https://soccerdata.readthedocs.io/en/latest/usage.html>`__. For documentation on each of the\nsupported data sources, see the `example notebooks <https://soccerdata.readthedocs.io/en/latest/datasources/>`__ and `API reference <https://soccerdata.readthedocs.io/en/latest/reference/>`__.\n\n.. _Club Elo: https://www.clubelo.com/\n.. _ESPN: https://www.espn.com/soccer/\n.. _FBref: https://www.fbref.com/en/\n.. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/\n.. _Football-Data.co.uk: https://www.football-data.co.uk/\n.. _SoFIFA: https://sofifa.com/\n.. _WhoScored: https://www.whoscored.com/\n\n**Disclaimer:** As soccerdata relies on web scraping, any changes to the\nscraped websites will break the package. Hence, do not expect that all code\nwill work all the time. If you spot any bugs, then please `fork it and start\na pull request <https://github.com/probberechts/soccerdata/blob/master/CONTRIBUTING.rst>`__.\n",
     'author': 'Pieter Robberechts',
     'author_email': 'pieter.robberechts@kuleuven.be',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/probberechts/soccerdata',
```

### Comparing `soccerdata-1.3.6/PKG-INFO` & `soccerdata-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.3.6
+Version: 1.4.0
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.8.1,<4.0.0
```

