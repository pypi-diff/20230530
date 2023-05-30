# Comparing `tmp/lavaplayer-1.0.8a0.tar.gz` & `tmp/lavaplayer-1.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavaplayer-1.0.8a0.tar", last modified: Sun Mar 27 13:40:25 2022, max compression
+gzip compressed data, was "lavaplayer-1.0.9a0.tar", last modified: Sun Jun 12 18:25:55 2022, max compression
```

## Comparing `lavaplayer-1.0.8a0.tar` & `lavaplayer-1.0.9a0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-03-27 13:40:25.774858 lavaplayer-1.0.8a0/
--rw-rw-rw-   0        0        0     1068 2021-12-23 20:00:48.000000 lavaplayer-1.0.8a0/LICENSE
--rw-rw-rw-   0        0        0     2803 2022-03-27 13:40:25.772859 lavaplayer-1.0.8a0/PKG-INFO
--rw-rw-rw-   0        0        0     1631 2022-02-18 11:09:11.000000 lavaplayer-1.0.8a0/README.md
-drwxrwxrwx   0        0        0        0 2022-03-27 13:40:25.719002 lavaplayer-1.0.8a0/lavaplayer/
--rw-rw-rw-   0        0        0      323 2022-02-19 20:17:17.000000 lavaplayer-1.0.8a0/lavaplayer/__init__.py
--rw-rw-rw-   0        0        0     1425 2022-01-26 05:05:21.000000 lavaplayer-1.0.8a0/lavaplayer/api.py
--rw-rw-rw-   0        0        0    20873 2022-03-27 13:19:00.000000 lavaplayer-1.0.8a0/lavaplayer/client.py
--rw-rw-rw-   0        0        0     2179 2022-01-26 05:05:21.000000 lavaplayer-1.0.8a0/lavaplayer/emitter.py
--rw-rw-rw-   0        0        0     2992 2022-02-19 19:37:44.000000 lavaplayer-1.0.8a0/lavaplayer/exceptions.py
--rw-rw-rw-   0        0        0     7405 2022-03-27 13:16:27.000000 lavaplayer-1.0.8a0/lavaplayer/objects.py
--rw-rw-rw-   0        0        0     6841 2022-03-27 13:19:03.000000 lavaplayer-1.0.8a0/lavaplayer/websocket.py
-drwxrwxrwx   0        0        0        0 2022-03-27 13:40:25.771863 lavaplayer-1.0.8a0/lavaplayer.egg-info/
--rw-rw-rw-   0        0        0     2803 2022-03-27 13:40:23.000000 lavaplayer-1.0.8a0/lavaplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2022-03-27 13:40:25.000000 lavaplayer-1.0.8a0/lavaplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-03-27 13:40:23.000000 lavaplayer-1.0.8a0/lavaplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-03-27 13:40:24.000000 lavaplayer-1.0.8a0/lavaplayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-03-27 13:40:25.000000 lavaplayer-1.0.8a0/lavaplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-03-27 13:40:25.775858 lavaplayer-1.0.8a0/setup.cfg
--rw-rw-rw-   0        0        0     1351 2022-03-27 13:39:28.000000 lavaplayer-1.0.8a0/setup.py
+drwxrwxrwx   0        0        0        0 2022-06-12 18:25:55.121458 lavaplayer-1.0.9a0/
+-rw-rw-rw-   0        0        0     1068 2021-12-23 20:00:48.000000 lavaplayer-1.0.9a0/LICENSE
+-rw-rw-rw-   0        0        0     2762 2022-06-12 18:25:55.118461 lavaplayer-1.0.9a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1631 2022-02-18 11:09:11.000000 lavaplayer-1.0.9a0/README.md
+drwxrwxrwx   0        0        0        0 2022-06-12 18:25:55.049457 lavaplayer-1.0.9a0/lavaplayer/
+-rw-rw-rw-   0        0        0      657 2022-06-07 21:33:05.000000 lavaplayer-1.0.9a0/lavaplayer/__init__.py
+-rw-rw-rw-   0        0        0     3408 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/api.py
+-rw-rw-rw-   0        0        0    20944 2022-06-07 21:33:05.000000 lavaplayer-1.0.9a0/lavaplayer/client.py
+-rw-rw-rw-   0        0        0     2390 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/emitter.py
+-rw-rw-rw-   0        0        0     2992 2022-02-19 19:37:44.000000 lavaplayer-1.0.9a0/lavaplayer/exceptions.py
+-rw-rw-rw-   0        0        0     7449 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/objects.py
+-rw-rw-rw-   0        0        0      272 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/routes.py
+-rw-rw-rw-   0        0        0     1260 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/utlits.py
+-rw-rw-rw-   0        0        0     8029 2022-06-07 21:13:10.000000 lavaplayer-1.0.9a0/lavaplayer/websocket.py
+drwxrwxrwx   0        0        0        0 2022-06-12 18:25:55.116464 lavaplayer-1.0.9a0/lavaplayer.egg-info/
+-rw-rw-rw-   0        0        0     2762 2022-06-12 18:25:52.000000 lavaplayer-1.0.9a0/lavaplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2022-06-12 18:25:54.000000 lavaplayer-1.0.9a0/lavaplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-06-12 18:25:52.000000 lavaplayer-1.0.9a0/lavaplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-06-12 18:25:54.000000 lavaplayer-1.0.9a0/lavaplayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-06-12 18:25:54.000000 lavaplayer-1.0.9a0/lavaplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-06-12 18:25:55.121458 lavaplayer-1.0.9a0/setup.cfg
+-rw-rw-rw-   0        0        0     1388 2022-06-07 09:22:52.000000 lavaplayer-1.0.9a0/setup.py
```

### Comparing `lavaplayer-1.0.8a0/LICENSE` & `lavaplayer-1.0.9a0/LICENSE`

 * *Files identical despite different names*

### Comparing `lavaplayer-1.0.8a0/PKG-INFO` & `lavaplayer-1.0.9a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: lavaplayer
-Version: 1.0.8a0
+Version: 1.0.9a0
 Summary: Its a lavalink nodes manger to make a music bots for discord with python.
 Home-page: https://github.com/HazemMeqdad/lavaplayer
 Author: HazemMeqdad
 Author-email: hazemmeqdad@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/HazemMeqdad/lavaplayer/issues
 Project-URL: Source, https://github.com/HazemMeqdad/lavaplayer/
 Project-URL: Documentation, https://lavaplayer.readthedocs.io/en/latest
 Keywords: lavalink,discord,discord-lavalink,lavaplayer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -99,9 +97,7 @@
 ```shell
 # Linux/OS X
 $ pip3 install -U lavaplayer
 
 # Windows
 $ pip install -U lavaplayer
 ```
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: lavaplayer Version: 1.0.8a0 Summary: Its a lavalink
+Metadata-Version: 2.1 Name: lavaplayer Version: 1.0.9a0 Summary: Its a lavalink
 nodes manger to make a music bots for discord with python. Home-page: https://
 github.com/HazemMeqdad/lavaplayer Author: HazemMeqdad Author-email:
-hazemmeqdad@gmail.com License: UNKNOWN Project-URL: Bug Reports, https://
-github.com/HazemMeqdad/lavaplayer/issues Project-URL: Source, https://
-github.com/HazemMeqdad/lavaplayer/ Project-URL: Documentation, https://
-lavaplayer.readthedocs.io/en/latest Keywords: lavalink,discord,discord-
-lavalink,lavaplayer Platform: UNKNOWN Classifier: Development Status :: 3 -
-Alpha Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
-License-File: LICENSE
+hazemmeqdad@gmail.com Project-URL: Bug Reports, https://github.com/HazemMeqdad/
+lavaplayer/issues Project-URL: Source, https://github.com/HazemMeqdad/
+lavaplayer/ Project-URL: Documentation, https://lavaplayer.readthedocs.io/en/
+latest Keywords: lavalink,discord,discord-lavalink,lavaplayer Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
+Type: text/markdown License-File: LICENSE
                            ****** Lavaplayer ******
                Support_Guild | Examples | Documentation | Source
 
 Its a lavalink nodes manger to make a music bots for discord with python. #
 About Lavaplayer is a nodes manager to connection with discord voice gateway,
 easy to create a music bot, you can use to anything async discord wrapper
 library # Usage example for create connecting with lavalink server using
```

### Comparing `lavaplayer-1.0.8a0/README.md` & `lavaplayer-1.0.9a0/README.md`

 * *Files identical despite different names*

### Comparing `lavaplayer-1.0.8a0/lavaplayer/api.py` & `lavaplayer-1.0.9a0/lavaplayer/api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import aiohttp
+from . import routes
+import logging
 
 
-class Api:
+_LOGGER = logging.getLogger(__name__)
+
+
+class LavalinkRest:
     """
-    The class make a request to the rest api for lavalink
+    The class make a request to the rest api for lavalink.
 
     Parameters
     ---------
     host: :class:`str`
-        ip address for lavalink server, default ip address for lavalink is ``127.0.0.1``
+        ip address for lavalink server, default ip address for lavalink is ``127.0.0.1`.
     port: :class:`int`
         The port to use for websocket and REST connections.
     password: :class:`str`
         The password used for authentication.
     is_ssl: :class:`bool`
-        Is server using ssl
+        Is server using ssl.
     """
     def __init__(self, *, host: str = "127.0.0.1", port: int, password: str, is_ssl: bool = False) -> None:
         self.rest_uri = f"{'https' if is_ssl else 'http'}://{host}:{port}"
         self.headers = {
             "Host": f"{host}:{port}",
             "Authorization": password
         }
@@ -34,8 +39,64 @@
         rout: :class:`str`
             rout from request like `/loadtracks`
         data: :class:`dict`
             data for request
         """
         async with aiohttp.ClientSession(headers=self.headers) as session:
             async with session.request(method, self.rest_uri + rout, data=data) as resp:
+                _LOGGER.debug(f"{method} {self.rest_uri + rout}")
                 return await resp.json()
+
+    async def load_tracks(self, query: str) -> list:
+        """
+        The REST api is used to resolve audio tracks for use with the play function :meth:`lavaplayer.Lavalink.play`.
+
+        Parameters
+        ---------
+        query: :class:`str`
+            query for request like `ytsearch:{query}`
+        """
+        return await self.request("GET", routes.LOADTRACKS.format(query=query))
+
+    async def decode_track(self, track: str) -> dict:
+        """
+        Decode a single track into its real info
+
+        Parameters
+        ---------
+        track: :class:`str`
+            track base64 encoded text for request like `ytsearch:`
+        """
+        return await self.request("GET", routes.DECODETRACK.format(track=track))
+
+    async def decode_tracks(self, tracks: list) -> list:
+        """
+        Decode a multiple track into their real info.
+
+        Parameters
+        ---------
+        tracks: :class:`list`
+            list of tracks base64 encoded text for request like `ytsearch:`
+        """
+        return await self.request("POST", routes.DECODETRACKS, data={"tracks": tracks})
+
+    async def route_planner_status(self) -> dict:
+        """
+        This function makes a request to the rest api for lavalink.
+        """
+        return await self.request("GET", routes.ROUTEPLANNER)
+    
+    async def route_planner_free_address(self, address: str) -> dict:
+        """
+        """
+        return await self.request("GET", routes.UNMARK_FAILED_ADDRESS.format(address=address))
+    
+    async def route_planner_free_all(self) -> dict:
+        """
+        """
+        return await self.request("GET", routes.UNMARK_ALL_FAILED_ADDRESS)
+    
+
+class Api(LavalinkRest):
+    """
+    Inherit from :class:`LavalinkRest`, ill remove it later.
+    """
```

### Comparing `lavaplayer-1.0.8a0/lavaplayer/client.py` & `lavaplayer-1.0.9a0/lavaplayer/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import asyncio
 import typing as t
+import random
 from lavaplayer.exceptions import NodeError, VolumeError, TrackLoadFailed
-from typing import Dict
-
 from .emitter import Emitter
 from .websocket import WS
-from .api import Api
-from .objects import Info, Track, Node, Filters, ConnectionInfo, Event, ErrorEvent, PlayList
-from lavaplayer import __version__
-import random
+from .api import LavalinkRest
+from .objects import Info, Track, Node, Filters, ConnectionInfo, Event, PlayList
+from . import __version__
+from .utlits import get_event_loop, prossing_tracks
 
 
-class LavalinkClient:
+class Lavalink:
     """
     Represents a Lavalink client used to manage nodes and connections.
 
     Parameters
     ---------
     host: :class:`str`
         ip address for lavalink server, default ip address for lavalink is ``127.0.0.1``
@@ -35,146 +34,111 @@
         *,
         host: t.Optional[str] = "127.0.0.1",
         port: int,
         password: str,
         user_id: int,
         num_shards: int = 1,
         is_ssl: bool = False,
+        loop: t.Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
-        try:
-            self._loop = asyncio.get_event_loop()
-        except RuntimeError:
-            self._loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(self._loop)
-        self._headers = {
-            "Authorization": password,
-            "User-Id": str(user_id),
-            "Client-Name": f"Lavaplayer/{__version__}",
-            "Num-Shards": str(num_shards)
-        }
-        self.event_manager = Emitter(self._loop)
-        self._ws = WS(self, host, port, is_ssl)
         self.info: Info = None
         self.host = host
         self.port = port
-        self.is_ssl = is_ssl
         self.password = password
         self.user_id = user_id
-        self._api = Api(host=self.host, port=self.port, password=self.password, is_ssl=self.is_ssl)
-        self._nodes: Dict[int, Node] = {}
-        self._voice_handlers: Dict[int, ConnectionInfo] = {}
-
-    def _prossing_tracks(self, tracks: list) -> t.List[Track]:
-        _tracks = []
-        for track in tracks:
-            info = track["info"]
-            _tracks.append(
-                Track(
-                    track=track["track"],
-                    identifier=info["identifier"],
-                    isSeekable=info["isSeekable"],
-                    author=info["author"],
-                    length=info["length"],
-                    isStream=info["isStream"],
-                    position=info["position"],
-                    sourceName=info.get("sourceName", None),
-                    title=info.get("title", None),
-                    uri=info["uri"]
-                )
-            )
-        return _tracks
+        self.num_shards = num_shards
+        self.is_ssl = is_ssl
+        
+        self.loop = loop or get_event_loop()
+        self.event_manager = Emitter(self.loop)
 
-    async def voice_update(self, guild_id: int, /, session_id: str, token: str, endpoint: str, channel_id: t.Optional[int]) -> None:
-        """
-        Update the voice connection for a guild.
+        self._ws = WS(
+            client=self, 
+            host=self.host, 
+            port=self.port, 
+            is_ssl=self.is_ssl, 
+            password=self.password, 
+            user_id=self.user_id, 
+            num_shards=self.num_shards
+        )
 
-        Parameters
-        ---------
-        guild_id: :class:`int`
-            guild id for server
-        session_id: :class:`str`
-            session id for connection
-        token: :class:`str`
-            token for connection
-        endpoint: :class:`str`
-            endpoint for connection
-        channel_id: :class:`int`
-            channel id for connection, if not give channel_id the connection will be closed
-        """
-        if not channel_id:
-            await self.destroy(guild_id)
-            return
-        await self._ws.send({
-            "op": "voiceUpdate",
-            "guildId": str(guild_id),
-            "sessionId": session_id,
-            "event": {
-                "token": token,
-                "guild_id": str(guild_id),
-                "endpoint": endpoint.replace("wss://", "")
-            }
-        })
-        await self.create_new_node(guild_id, is_connected=True)
-
-    async def create_new_node(self, guild_id: int, /, is_connected: bool = False) -> Node:
-        node = Node(guild_id, [], 100, is_connected=is_connected)
-        self._nodes[guild_id] = node
-        return node
+        # Unique identifier for the client.
+        self.rest = LavalinkRest(host=self.host, port=self.port, password=self.password, is_ssl=self.is_ssl)
+        self.info: Info = None
+        self._nodes: t.Dict[int, Node] = {}
+        self._voice_handlers: t.Dict[int, ConnectionInfo] = {}
+        self._task_loop: asyncio.Task = None
 
-    async def search_youtube(self, query: str) -> t.Union[t.Optional[t.List[Track]], t.Optional[PlayList]]:
+    async def search_youtube(self, query: str) -> t.Optional[t.Union[t.List[Track], TrackLoadFailed]]:
         """
         Search for tracks with youtube.
 
         Parameters
         ---------
         query: :class:`str`
             words for search with youtube. if not found result retrun empty :class:`list`
         
         Exceptions
         ----------
         :class:`lavaplayer.exceptions.TrackLoadFailed`
             If the track could not be loaded.
         """
-        result = await self._api.request("GET", "/loadtracks", data={"identifier": f"ytsearch:{query}"})
+        result = await self.rest.load_tracks(f"ytsearch:{query}")
         if result["loadType"] == "NO_MATCHES":
             return []
         if result["loadType"] == "LOAD_FAILED":
-            return None
-        return self._prossing_tracks(result["tracks"])
+            return TrackLoadFailed(result["exception"]["message"], result["exception"]["severity"])
+        return prossing_tracks(result["tracks"])
 
-    async def get_tracks(self, query: str) -> t.Union[t.Optional[t.List[Track]], t.Optional[PlayList]]:
+    async def get_tracks(self, query: str) -> t.Optional[t.Union[t.List[Track], PlayList, TrackLoadFailed]]:
         """
         Load tracks for unknow sits or youtube or soundcloud or radio.
 
         Parameters
         ---------
         query: :class:`str`
             track url, if not found result retrun empty :class:`list`
         
         Exceptions
         ----------
         :class:`lavaplayer.exceptions.TrackLoadFailed`
             If the track could not be loaded.
         """
-        result = await self._api.request("GET", "/loadtracks", data={"identifier": query})
+        result = await self.rest.load_tracks(query)
         if result["loadType"] == "NO_MATCHES":
             return []
         if result["loadType"] == "LOAD_FAILED":
             raise TrackLoadFailed(result["exception"]["message"], result["exception"]["severity"])
         if result["loadType"] == "PLAYLIST_LOADED":
-            return PlayList(result["playlistInfo"]["name"], result["playlistInfo"]["selectedTrack"], self._prossing_tracks(result["tracks"]))
-        return self._prossing_tracks(result["tracks"])
+            return PlayList(result["playlistInfo"]["name"], result["playlistInfo"]["selectedTrack"], prossing_tracks(result["tracks"]))
+        return prossing_tracks(result["tracks"])
 
-    async def _decodetrack(self, track: str) -> Track:
-        result = await self._api.request("GET", "/decodetrack", data={"track": track})
+    async def decodetrack(self, track: str) -> Track:
+        """
+        This method is used to decode a track from base64 only server can resolve, to info can anyone understanding it
+        
+        Parameters
+        ---------
+        track: :class:`str`
+            track result from base64
+        """
+        result = await self.rest.decode_track(track)
         return Track(track, **result)
 
-    async def _decodetracks(self, tracks: t.List[t.Dict]) -> t.List[Track]:
-        result = await self._api.request("POST", "/decodetrack", json=tracks)
-        return self._prossing_tracks(result)
+    async def decodetracks(self, tracks: t.List[t.Dict]) -> t.List[Track]:
+        """
+        This method is used to decode a tracks from base64 only server can resolve, to info can anyone understanding it
+
+        Parameters
+        ---------
+        tracks: :class:`list`
+            tracks result from base64
+        """
+        result = await self.rest.decode_tracks(tracks)
+        return prossing_tracks(result)
 
     async def auto_search_tracks(self, query: str) -> t.Union[t.Optional[t.List[Track]], t.Optional[PlayList]]:
         """
         Load tracks for youtube search or other urls.
 
         Parameters
         ---------
@@ -186,34 +150,18 @@
         :class:`lavaplayer.exceptions.TrackLoadFailed`
             If the track could not be loaded.
         """
         if "http" in query:
             return await self.get_tracks(query)
         return await self.search_youtube(query)
 
-    async def add_to_queue(self, guild_id: int, /, tracks: t.List[Track], requester: t.Optional[int] = None) -> None:
-        """
-        Add tracks to queue. use to load a playlist result.
-
-        >>> playlist = await lavaplayer.search_youtube("playlist url")
-        >>> await lavaplayer.add_to_queue(guild_id, playlist.tracks)
-
-        Parameters
-        ---------
-        guild_id: :class:`int`
-            guild id for server
-        tracks: :class:`list`
-            tracks to add to queue
-        """
-        node = await self.get_guild_node(guild_id)
-        if not node:
-            raise NodeError("Node not found", guild_id)
-
-        for track in tracks:
-            self._loop.create_task(self.play(guild_id, track, requester))
+    async def create_new_node(self, guild_id: int, /, is_connected: bool = False) -> Node:
+        node = Node(guild_id, [], 100, is_connected=is_connected)
+        self._nodes[guild_id] = node
+        return node
 
     async def get_guild_node(self, guild_id: int, /) -> t.Optional[Node]:
         """
         Get guild info from node cache memory.
 
         Parameters
         ---------
@@ -243,40 +191,34 @@
         ---------
         guild_id: :class:`int`
             guild id for server
         """
         await self.get_guild_node(guild_id)
         self._nodes[guild_id] = node
 
-    async def queue(self, guild_id: int, /) -> t.List[Track]:
-        """
-        Get guild queue list from node cache memory.
-
-        Parameters
-        ---------
-        guild_id: :class:`int`
-            guild id for server
+    async def add_to_queue(self, guild_id: int, /, tracks: t.List[Track], requester: t.Optional[int] = None) -> None:
         """
-        node = await self.get_guild_node(guild_id)
-        return node.queue
+        Add tracks to queue. use to load a playlist result.
 
-    async def repeat(self, guild_id: int, /, stats: bool) -> None:
-        """
-        Repeat the track for every.
+        >>> playlist = await lavaplayer.search_youtube("playlist url")
+        >>> await lavaplayer.add_to_queue(guild_id, playlist.tracks)
 
         Parameters
         ---------
         guild_id: :class:`int`
             guild id for server
-        stats: :class:`bool`
-            the stats for repeat track
+        tracks: :class:`list`
+            tracks to add to queue
         """
         node = await self.get_guild_node(guild_id)
-        node.repeat = stats
-        await self.set_guild_node(guild_id, node)
+        if not node:
+            raise NodeError("Node not found", guild_id)
+
+        for track in tracks:
+            self.loop.create_task(self.play(guild_id, track, requester))
 
     async def play(self, guild_id: int, /, track: Track, requester: t.Optional[int] = None, start: bool = False) -> None:
         """
         Play track or add to the queue list.
 
         Parameters
         ---------
@@ -308,15 +250,58 @@
         track.requester = requester
         node.queue.append(track)
         await self.set_guild_node(guild_id, node)
         if len(node.queue) != 1:
             return
         await self._ws.send(payload)
 
-    async def filters(self, guild_id: int, /, filters: Filters) -> None:
+    async def queue(self, guild_id: int, /) -> t.List[Track]:
+        """
+        Get guild queue list from node cache memory.
+
+        Parameters
+        ---------
+        guild_id: :class:`int`
+            guild id for server
+        """
+        node = await self.get_guild_node(guild_id)
+        return node.queue
+
+    async def repeat(self, guild_id: int, /, stats: bool) -> None:
+        """
+        Repeat the track for every.
+
+        Parameters
+        ---------
+        guild_id: :class:`int`
+            guild id for server
+        stats: :class:`bool`
+            the stats for repeat track
+        """
+        node = await self.get_guild_node(guild_id)
+        node.repeat = stats
+        await self.set_guild_node(guild_id, node)
+
+    async def queue_repeat(self, guild_id: int, /, stats: bool) -> None:
+        """
+        Repeat the queue for every.
+
+        Parameters
+        ---------
+        guild_id: :class:`int`
+            guild id for server
+        stats: :class:`bool`
+            the stats for repeat queue
+        """
+        node = await self.get_guild_node(guild_id)
+        node.queue_repeat = stats
+        node.repeat = False
+        await self.set_guild_node(guild_id, node)
+
+    async def filters(self, guild_id: int, /, filters: t.Optional[Filters]) -> None:
         """
         Repeat the track for every.
 
         Parameters
         ---------
         guild_id: :class:`int`
             guild id for server
@@ -327,14 +312,16 @@
         --------
         :exc:`.NodeError`
             If guild not found in nodes cache.
         """
         node = await self.get_guild_node(guild_id)
         if not node:
             raise NodeError("Node not found", guild_id)
+        if not filters:
+            filters = Filters()
         filters._payload["guildId"] = str(guild_id)
         await self._ws.send(filters._payload)
 
     async def stop(self, guild_id: int, /) -> None:
         """
         Stop the track.
 
@@ -514,14 +501,46 @@
         np = node.queue[0]
         node.queue.remove(np)
         node.queue = random.sample(node.queue, len(node.queue))
         node.queue.insert(0, np)
         await self.set_guild_node(guild_id, node)
         return node
 
+    async def voice_update(self, guild_id: int, /, session_id: str, token: str, endpoint: str, channel_id: t.Optional[int]) -> None:
+        """
+        Update the voice connection for a guild.
+
+        Parameters
+        ---------
+        guild_id: :class:`int`
+            guild id for server
+        session_id: :class:`str`
+            session id for connection
+        token: :class:`str`
+            token for connection
+        endpoint: :class:`str`
+            endpoint for connection
+        channel_id: :class:`int`
+            channel id for connection, if not give channel_id the connection will be closed
+        """
+        if not channel_id:
+            await self.destroy(guild_id)
+            return
+        await self._ws.send({
+            "op": "voiceUpdate",
+            "guildId": str(guild_id),
+            "sessionId": session_id,
+            "event": {
+                "token": token,
+                "guild_id": str(guild_id),
+                "endpoint": endpoint.replace("wss://", "")
+            }
+        })
+        await self.create_new_node(guild_id, is_connected=True)
+
     async def raw_voice_state_update(self, guild_id: int, /, user_id: int, session_id: str, channel_id: t.Optional[int]) -> None:
         """
         A voice state update has been received from Discord.
         
         Parameters
         ---------
         guild_id: :class:`int`
@@ -587,24 +606,14 @@
         """
         node = await self.get_guild_node(guild_id)
         if not node:
             raise NodeError("Node not found", guild_id)
         while (await self.get_guild_node(guild_id)):
             await asyncio.sleep(0.1)
 
-    def _raise_or_emit(self, exception: Exception, *args, **kwargs) -> None:
-        """
-        This function is used to raise or emit an exception. its not a complete becuse i need to save listener with asyncio.futures but not now.
-        """
-        listeners = self.event_manger.listeners
-        error_handler = [i for i in listeners if i["event"] == "ErrorEvent"]
-        if not error_handler:
-            raise exception(*args, **kwargs)
-        self.event_manger.emit(ErrorEvent, ErrorEvent(args[0], exception))
-
     def listen(self, event: t.Union[str, Event]) -> t.Callable[..., t.Awaitable]:
         """
         The register function for listener handler
 
         Parameters
         ---------
         event: :class:`Any` | :class:`str`
@@ -621,12 +630,23 @@
         """
         return self._ws.is_connect
 
     def connect(self):
         """
         Connect to the lavalink websocket
         """
-        self._loop.create_task(self._ws._connect())
+        self.loop.create_task(self._ws._connect())
+
+    async def close(self):
+        """
+        Disconnect from the lavalink websocket
+        """
+        await self._ws.ws.close()
 
     @property
     def nodes(self):
         return self._nodes
+
+class LavalinkClient(Lavalink):
+    """
+    Inherit from :class:`Lavalink`, ill remove it later..
+    """
```

### Comparing `lavaplayer-1.0.8a0/lavaplayer/emitter.py` & `lavaplayer-1.0.9a0/lavaplayer/emitter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import typing as t
 from collections import deque
 import logging
 from .objects import Event
 
+_LOGGER = logging.getLogger("lavaplayer.event_manger")
 
 class Emitter:
     """
     The class is a manger event from websocket.
 
     Parameters
     ---------
@@ -25,28 +26,30 @@
         Parameters
         ---------
         event: :class:`str` | :class:`Any`
             event name or class for event
         func: :class:`function`
             the function to callback event
         """
+        _LOGGER.debug(f"add listener {event}")
         event = event if isinstance(event, str) else event.__name__
         self.listeners.append({"event": event, "func": func})
 
     def remove_listener(self, event: t.Union[str, Event], func: t.Callable):
         """
         Remove listener for listeners list.
 
         Parameters
         ---------
         event: :class:`str` | :class:`Any`
             event name or class for event
         func: :class:`function`
             the function to callback event
         """
+        _LOGGER.debug(f"remove listener {event}")
         event = event if isinstance(event, str) else event.__name__
         self.listeners.remove([i for i in self.listeners if i["event"] == event and i["func"] == func])
 
     def emit(self, event: t.Union[str, t.Any], data: t.Any):
         """
         Emit for event dont use this.
 
@@ -56,11 +59,12 @@
             event name or class for event
         data: :class:`function`
             the data is revers to function callback
         """
         event = event if isinstance(event, str) else event.__name__
         events = [i for i in self.listeners if i["event"] == event]
         for event in events:
+            _LOGGER.debug(f"dispatch {event} for {len(events)} listeners")
             if asyncio.iscoroutinefunction(event["func"]):
                 self._loop.create_task(event["func"](data))
             else:
-                logging.error("events only async func, you can't use sync -_-")
+                _LOGGER.error("Events only async function")
```

### Comparing `lavaplayer-1.0.8a0/lavaplayer/exceptions.py` & `lavaplayer-1.0.9a0/lavaplayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `lavaplayer-1.0.8a0/lavaplayer/objects.py` & `lavaplayer-1.0.9a0/lavaplayer/objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from dataclasses import dataclass
 from lavaplayer.exceptions import FiltersError
 import typing as t
 
 
-class Event:
-    """
-    The class is a base event for websocket.
-    """
-
 
 @dataclass
 class Info:
     """
     Info websocket for connection
     """
     playing_players: int
@@ -42,14 +37,49 @@
     """
 
     def __repr__(self) -> str:
         return self.title
 
 
 @dataclass
+class Node:
+    """
+    The node is saved the queue guild list and volume and etc information.
+    """
+    guild_id: int
+    queue: t.List[Track]
+    volume: int
+    is_pause: bool = False
+    repeat: bool = False
+    queue_repeat: bool = False
+    is_connected: bool = False
+
+
+@dataclass
+class ConnectionInfo:
+    """
+    A info for Connection just use to save the connection information.
+    """
+    guild_id: int
+    session_id: str
+    channel_id: t.Optional[int]
+
+
+@dataclass
+class PlayList:
+    name: str
+    selected_track: int
+    tracks: t.List[Track]
+
+class Event:
+    """
+    The class is a base event for websocket.
+    """
+
+@dataclass
 class TrackStartEvent(Event):
     """
     Event on track start.
     """
     track: Track
     guild_id: int
 
@@ -68,17 +98,17 @@
 class TrackExceptionEvent(Event):
     """
     Event on track exception.
     """
     track: Track
     guild_id: int
     exception: str
-    message: str
-    severity: str
-    cause: str
+    message: t.Optional[str]
+    severity: t.Optional[str]
+    cause: t.Optional[str]
 
 
 @dataclass
 class TrackStuckEvent(Event):
     """
     Event on track stuck.
     """
@@ -88,15 +118,14 @@
 
 
 @dataclass
 class WebSocketClosedEvent(Event):
     """
     Event on websocket closed.
     """
-    track: Track
     guild_id: int
     code: int
     reason: str
     byRemote: bool
 
 
 @dataclass
@@ -115,44 +144,14 @@
     """
     Event on error.
     """
     guild_id: int
     exception: Exception
 
 
-@dataclass
-class Node:
-    """
-    The node is saved the queue guild list and volume and etc information.
-    """
-    guild_id: int
-    queue: t.List[Track]
-    volume: int
-    is_pause: bool = False
-    repeat: bool = False
-    is_connected: bool = False
-
-
-@dataclass
-class ConnectionInfo:
-    """
-    A info for Connection just use to save the connection information.
-    """
-    guild_id: int
-    session_id: str
-    channel_id: t.Optional[int]
-
-
-@dataclass
-class PlayList:
-    name: str
-    selected_track: int
-    tracks: t.List[Track]
-
-    
 @dataclass(init=True)
 class Filters:
     """
     All the filters are optional, and leaving them out of this message will disable them.
 
     Adding a filter can have adverse effects on performance. These filters force Lavaplayer to decode all audio to PCM, even if the input was already in the Opus format that Discord uses. This means decoding and encoding audio that would normally require very little processing. This is often the case with YouTube videos.
```

### Comparing `lavaplayer-1.0.8a0/lavaplayer/websocket.py` & `lavaplayer-1.0.9a0/lavaplayer/websocket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 import asyncio
 import aiohttp
 import logging
-from lavaplayer.exceptions import NodeError
+from lavaplayer.utlits import generate_resume_key
 from .objects import (
     Info,
     PlayerUpdateEvent,
     TrackStartEvent,
     TrackEndEvent,
     TrackExceptionEvent,
     TrackStuckEvent,
     WebSocketClosedEvent,
 )
 from .emitter import Emitter
 import typing as t
+from . import __version__
 
 if t.TYPE_CHECKING:
-    from .client import LavalinkClient
+    from .client import Lavalink
 
 
 _LOGGER = logging.getLogger("lavaplayer.ws")
 
 
 class WS:
     def __init__(
         self,
-        client: "LavalinkClient",
+        client: "Lavalink",
         host: str,
         port: int,
         is_ssl: bool = False,
+        password: str = None,
+        user_id: int = None,
+        num_shards: int = None,
+        resume_key: t.Optional[str] = None,
+        loop: t.Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
         self.ws = None
         self.ws_url = f"{'wss' if is_ssl else 'ws'}://{host}:{port}"
         self.client = client
-        self._headers = client._headers
-        self._loop = client._loop
+        self._headers = {
+            "Authorization": password,
+            "User-Id": str(user_id),
+            "Client-Name": f"Lavaplayer-py/{__version__}",
+            "Num-Shards": str(num_shards)
+        }
+        self._loop = loop or client.loop
         self.emitter: Emitter = client.event_manager
         self.is_connect: bool = False
+        self.resume_key = resume_key
     
     async def _connect(self):
+        if self.resume_key:
+            self._headers["Resume-Key"] = self.resume_key
         async with aiohttp.ClientSession(headers=self._headers, loop=self._loop) as session:
             self.session = session
             try:
                 self.ws = await self.session.ws_connect(self.ws_url)
                 if session is None:
                     await self.check_connection()
             except (aiohttp.ClientConnectorError, aiohttp.WSServerHandshakeError, aiohttp.ServerDisconnectedError) as error:
@@ -59,21 +73,28 @@
                     _LOGGER.warning("Please check your websocket port - closing websocket")
                 elif isinstance(error, aiohttp.ServerDisconnectedError):
                     _LOGGER.error(f"Could not connect to websocket: {error}")
                     _LOGGER.warning("Reconnecting to websocket after 10 seconds")
                     await asyncio.sleep(10)
                     await self._connect()
                     return
-
             _LOGGER.info("Connected to websocket")
             self.is_connect = True
+
+            self.resume_key = generate_resume_key()
+            await self.send({
+                "op": "configureResuming",
+                "key": self.resume_key,
+                "timeout": 60
+            })
+
             async for msg in self.ws:
                 if msg.type == aiohttp.WSMsgType.TEXT:
-                    await self.callback(msg.json())
-                elif msg.type == aiohttp.WSMsgType.CLOSED:
+                    self._loop.create_task(self.callback(msg.json()))
+                elif msg.type in (aiohttp.WSMsgType.CLOSE, aiohttp.WSMsgType.CLOSING, aiohttp.WSMsgType.CLOSED):
                     _LOGGER.error("Websocket closed")
                     break
                 elif msg.type == aiohttp.WSMsgType.ERROR:
                     _LOGGER.error(msg.data)
                     break
 
     async def check_connection(self):
@@ -94,70 +115,81 @@
                 uptime=payload["uptime"]
             )
 
         elif payload["op"] == "playerUpdate":
             guild_id = int(payload["guildId"])
             node = await self.client.get_guild_node(guild_id)
             position = payload["state"].get("position")
+            if node is None:
+                return
+            
             if node.queue:
                 node.queue[0].position = position / 1000
                 await self.client.set_guild_node(guild_id, node)
             data = PlayerUpdateEvent(
                 guild_id=guild_id,
                 time=payload["state"]["time"],
                 position=position / 1000 if isinstance(position, int) else None,
                 connected=payload["state"].get("connected", None),
             )
-            self.emitter.emit("playerUpdateEvent", data)
-
-        elif payload["op"] == "event":
+            self.emitter.emit("PlayerUpdateEvent", data)
 
-            if not payload.get("track"):
+        elif payload["op"] == "event" and payload.get("track") is not None:
+            await self.event_dispatch(payload)
+            
+    async def event_dispatch(self, payload: dict):
+        if payload.get("track"):
+            track = await self.client.decodetrack(payload["track"])
+        event = payload["type"]
+
+        guild_id = int(payload["guildId"])
+
+        node = await self.client.get_guild_node(guild_id)
+
+        if event == "TrackStartEvent":
+            self.emitter.emit("TrackStartEvent", TrackStartEvent(track, guild_id))
+
+        elif event == "TrackEndEvent":
+            self.emitter.emit("TrackEndEvent", TrackEndEvent(track, guild_id, payload["reason"]))
+            if not node or not node.queue:
                 return
-            track = await self.client._decodetrack(payload["track"])
-            guild_id = int(payload["guildId"])
-            try:
-                node = await self.client.get_guild_node(guild_id)
-            except NodeError:
-                node = None
-
-            if payload["type"] == "TrackStartEvent":
-                self.emitter.emit("TrackStartEvent", TrackStartEvent(track, guild_id))
-
-            elif payload["type"] == "TrackEndEvent":
-                self.emitter.emit("TrackEndEvent", TrackEndEvent(track, guild_id, payload["reason"]))
-                if not node:
-                    return
-                if not node.queue:
-                    return
-                if node.repeat:
-                    await self.client.play(guild_id, track, node.queue[0].requester, True)
-                    return
-                del node.queue[0]
+            if node.queue_repeat:
+                node.queue.append(node.queue.pop(0))
                 await self.client.set_guild_node(guild_id, node)
-                if len(node.queue) != 0:
-                    await self.client.play(guild_id, node.queue[0], node.queue[0].requester, True)
-
-            elif payload["type"] == "TrackExceptionEvent":
-                self.emitter.emit("TrackExceptionEvent", TrackExceptionEvent(track, guild_id, payload["exception"], payload["message"], payload["severity"], payload["cause"]))
-
-            elif payload["type"] == "TrackStuckEvent":
-                self.emitter.emit("TrackStuckEvent", TrackStuckEvent(track, guild_id, payload["thresholdMs"]))
-
-            elif payload["type"] == "WebSocketClosedEvent":
-                self.emitter.emit("WebSocketClosedEvent", WebSocketClosedEvent(track, guild_id, payload["code"], payload["reason"], payload["byRemote"]))
+                if len(node.queue) == 0:
+                    return
+                await self.client.play(guild_id, node.queue[0], node.queue[0].requester, True)
+                return
+            if node.repeat:
+                await self.client.play(guild_id, track, node.queue[0].requester, True)
+                return
+            del node.queue[0]
+            await self.client.set_guild_node(guild_id, node)
+            if len(node.queue) != 0:
+                await self.client.play(guild_id, node.queue[0], node.queue[0].requester, True)
+
+        elif event == "TrackExceptionEvent":
+            self.emitter.emit("TrackExceptionEvent", TrackExceptionEvent(track, guild_id, payload.get("exception"), payload.get("message"), payload.get("severity"), payload.get("cause")))
+
+        elif event == "TrackStuckEvent":
+            self.emitter.emit("TrackStuckEvent", TrackStuckEvent(track, guild_id, payload.get("thresholdMs")))
+
+        elif event == "WebSocketClosedEvent":
+            self.emitter.emit("WebSocketClosedEvent", WebSocketClosedEvent(guild_id, payload.get("code"), payload.get("reason"), payload.get("byRemote")))
+        
+        else:
+            _LOGGER.warning(f"Unknown event: {event}")
 
     @property
     def is_connected(self) -> bool:
         return self.is_connect and self.ws.closed is False
 
     async def send(self, payload):  # only dict
         if not self.is_connected:
             _LOGGER.error("Not connected to websocket")
-            await self.check_connection()
             return
         try:
             await self.ws.send_json(payload)
         except ConnectionResetError:
             _LOGGER.error("ConnectionResetError: Cannot write to closing transport")
             await self.check_connection()
             return
```

### Comparing `lavaplayer-1.0.8a0/lavaplayer.egg-info/PKG-INFO` & `lavaplayer-1.0.9a0/lavaplayer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: lavaplayer
-Version: 1.0.8a0
+Version: 1.0.9a0
 Summary: Its a lavalink nodes manger to make a music bots for discord with python.
 Home-page: https://github.com/HazemMeqdad/lavaplayer
 Author: HazemMeqdad
 Author-email: hazemmeqdad@gmail.com
-License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/HazemMeqdad/lavaplayer/issues
 Project-URL: Source, https://github.com/HazemMeqdad/lavaplayer/
 Project-URL: Documentation, https://lavaplayer.readthedocs.io/en/latest
 Keywords: lavalink,discord,discord-lavalink,lavaplayer
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -99,9 +97,7 @@
 ```shell
 # Linux/OS X
 $ pip3 install -U lavaplayer
 
 # Windows
 $ pip install -U lavaplayer
 ```
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.1 Name: lavaplayer Version: 1.0.8a0 Summary: Its a lavalink
+Metadata-Version: 2.1 Name: lavaplayer Version: 1.0.9a0 Summary: Its a lavalink
 nodes manger to make a music bots for discord with python. Home-page: https://
 github.com/HazemMeqdad/lavaplayer Author: HazemMeqdad Author-email:
-hazemmeqdad@gmail.com License: UNKNOWN Project-URL: Bug Reports, https://
-github.com/HazemMeqdad/lavaplayer/issues Project-URL: Source, https://
-github.com/HazemMeqdad/lavaplayer/ Project-URL: Documentation, https://
-lavaplayer.readthedocs.io/en/latest Keywords: lavalink,discord,discord-
-lavalink,lavaplayer Platform: UNKNOWN Classifier: Development Status :: 3 -
-Alpha Classifier: Intended Audience :: Developers Classifier: Topic :: Software
-Development :: Build Tools Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3 :: Only Description-Content-Type: text/markdown
-License-File: LICENSE
+hazemmeqdad@gmail.com Project-URL: Bug Reports, https://github.com/HazemMeqdad/
+lavaplayer/issues Project-URL: Source, https://github.com/HazemMeqdad/
+lavaplayer/ Project-URL: Documentation, https://lavaplayer.readthedocs.io/en/
+latest Keywords: lavalink,discord,discord-lavalink,lavaplayer Classifier:
+Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only Description-Content-
+Type: text/markdown License-File: LICENSE
                            ****** Lavaplayer ******
                Support_Guild | Examples | Documentation | Source
 
 Its a lavalink nodes manger to make a music bots for discord with python. #
 About Lavaplayer is a nodes manager to connection with discord voice gateway,
 easy to create a music bot, you can use to anything async discord wrapper
 library # Usage example for create connecting with lavalink server using
```

### Comparing `lavaplayer-1.0.8a0/setup.py` & `lavaplayer-1.0.9a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from setuptools import setup
-import pathlib
-
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / 'README.md').read_text(encoding='utf-8')
-
-
-setup(
-    name='lavaplayer',
-    version='1.0.8a',
-    description='Its a lavalink nodes manger to make a music bots for discord with python.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/HazemMeqdad/lavaplayer',
-    author='HazemMeqdad',
-    author_email='hazemmeqdad@gmail.com',
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        "Programming Language :: Python :: 3.10",
-        'Programming Language :: Python :: 3 :: Only',
-    ],
-    keywords='lavalink, discord, discord-lavalink, lavaplayer',
-    packages=["lavaplayer"],
-    install_requires=["aiohttp"],
-    project_urls={
-        'Bug Reports': 'https://github.com/HazemMeqdad/lavaplayer/issues',
-        'Source': 'https://github.com/HazemMeqdad/lavaplayer/',
-        'Documentation': 'https://lavaplayer.readthedocs.io/en/latest'
-    },
-)
+from setuptools import setup
+import pathlib
+
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / 'README.md').read_text(encoding='utf-8')
+
+
+setup(
+    name='lavaplayer',
+    version='1.0.9a',
+    description='Its a lavalink nodes manger to make a music bots for discord with python.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/HazemMeqdad/lavaplayer',
+    author='HazemMeqdad',
+    author_email='hazemmeqdad@gmail.com',
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Topic :: Software Development :: Build Tools',
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        "Programming Language :: Python :: 3.10",
+        'Programming Language :: Python :: 3 :: Only',
+    ],
+    keywords='lavalink, discord, discord-lavalink, lavaplayer',
+    packages=["lavaplayer"],
+    install_requires=["aiohttp"],
+    project_urls={
+        'Bug Reports': 'https://github.com/HazemMeqdad/lavaplayer/issues',
+        'Source': 'https://github.com/HazemMeqdad/lavaplayer/',
+        'Documentation': 'https://lavaplayer.readthedocs.io/en/latest'
+    },
+)
```

