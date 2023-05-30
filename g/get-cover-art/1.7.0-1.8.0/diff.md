# Comparing `tmp/get_cover_art-1.7.0.tar.gz` & `tmp/get_cover_art-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_cover_art-1.7.0.tar", last modified: Thu Feb 16 04:20:54 2023, max compression
+gzip compressed data, was "get_cover_art-1.8.0.tar", last modified: Tue May 30 05:01:11 2023, max compression
```

## Comparing `get_cover_art-1.7.0.tar` & `get_cover_art-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-02-16 04:20:54.301085 get_cover_art-1.7.0/
--rw-r--r--   0 regosen    (501) staff       (20)     1065 2020-09-02 22:42:08.000000 get_cover_art-1.7.0/LICENSE
--rw-r--r--   0 regosen    (501) staff       (20)       66 2020-09-02 23:46:32.000000 get_cover_art-1.7.0/MANIFEST.in
--rw-r--r--   0 regosen    (501) staff       (20)     9249 2023-02-16 04:20:54.300194 get_cover_art-1.7.0/PKG-INFO
--rw-r--r--   0 regosen    (501) staff       (20)     8350 2023-02-15 00:30:26.000000 get_cover_art-1.7.0/README.md
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-02-16 04:20:54.279059 get_cover_art-1.7.0/get_cover_art/
--rw-r--r--   0 regosen    (501) staff       (20)       50 2021-11-02 19:50:11.000000 get_cover_art-1.7.0/get_cover_art/__init__.py
--rw-r--r--   0 regosen    (501) staff       (20)     4825 2022-09-21 16:41:17.000000 get_cover_art-1.7.0/get_cover_art/__main__.py
--rw-r--r--   0 regosen    (501) staff       (20)     4650 2022-05-30 19:59:34.000000 get_cover_art-1.7.0/get_cover_art/apple_downloader.py
--rw-r--r--   0 regosen    (501) staff       (20)     9864 2023-02-16 04:15:07.000000 get_cover_art-1.7.0/get_cover_art/cover_finder.py
--rw-r--r--   0 regosen    (501) staff       (20)      851 2021-06-08 05:31:32.000000 get_cover_art-1.7.0/get_cover_art/deromanizer.py
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-02-16 04:20:54.298848 get_cover_art-1.7.0/get_cover_art/meta/
--rw-r--r--   0 regosen    (501) staff       (20)      507 2023-02-15 00:25:46.000000 get_cover_art-1.7.0/get_cover_art/meta/__init__.py
--rw-r--r--   0 regosen    (501) staff       (20)     1249 2022-06-01 18:57:26.000000 get_cover_art-1.7.0/get_cover_art/meta/base_id3.py
--rw-r--r--   0 regosen    (501) staff       (20)     1381 2022-06-02 04:27:54.000000 get_cover_art-1.7.0/get_cover_art/meta/base_ogg.py
--rw-r--r--   0 regosen    (501) staff       (20)      988 2022-04-11 19:45:10.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_audio.py
--rw-r--r--   0 regosen    (501) staff       (20)      168 2022-06-01 19:00:02.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_dsf.py
--rw-r--r--   0 regosen    (501) staff       (20)     1070 2021-12-22 02:20:12.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_flac.py
--rw-r--r--   0 regosen    (501) staff       (20)      205 2022-06-01 18:59:46.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_mp3.py
--rw-r--r--   0 regosen    (501) staff       (20)     1054 2021-12-22 02:20:15.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_mp4.py
--rw-r--r--   0 regosen    (501) staff       (20)      181 2022-06-02 04:27:54.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_opus.py
--rw-r--r--   0 regosen    (501) staff       (20)      189 2022-06-02 04:27:54.000000 get_cover_art-1.7.0/get_cover_art/meta/meta_vorbis.py
--rw-r--r--   0 regosen    (501) staff       (20)     1378 2021-12-22 02:11:35.000000 get_cover_art-1.7.0/get_cover_art/normalizer.py
-drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-02-16 04:20:54.288159 get_cover_art-1.7.0/get_cover_art.egg-info/
--rw-r--r--   0 regosen    (501) staff       (20)     9249 2023-02-16 04:20:48.000000 get_cover_art-1.7.0/get_cover_art.egg-info/PKG-INFO
--rw-r--r--   0 regosen    (501) staff       (20)      743 2023-02-16 04:20:53.000000 get_cover_art-1.7.0/get_cover_art.egg-info/SOURCES.txt
--rw-r--r--   0 regosen    (501) staff       (20)        1 2023-02-16 04:20:48.000000 get_cover_art-1.7.0/get_cover_art.egg-info/dependency_links.txt
--rw-r--r--   0 regosen    (501) staff       (20)       62 2023-02-16 04:20:51.000000 get_cover_art-1.7.0/get_cover_art.egg-info/entry_points.txt
--rw-r--r--   0 regosen    (501) staff       (20)        8 2023-02-16 04:20:52.000000 get_cover_art-1.7.0/get_cover_art.egg-info/requires.txt
--rw-r--r--   0 regosen    (501) staff       (20)       14 2023-02-16 04:20:52.000000 get_cover_art-1.7.0/get_cover_art.egg-info/top_level.txt
--rw-r--r--   0 regosen    (501) staff       (20)       38 2023-02-16 04:20:54.302007 get_cover_art-1.7.0/setup.cfg
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-05-30 05:01:11.033908 get_cover_art-1.8.0/
+-rw-r--r--   0 regosen    (501) staff       (20)     1065 2020-09-02 22:42:08.000000 get_cover_art-1.8.0/LICENSE
+-rw-r--r--   0 regosen    (501) staff       (20)       66 2020-09-02 23:46:32.000000 get_cover_art-1.8.0/MANIFEST.in
+-rw-r--r--   0 regosen    (501) staff       (20)     9594 2023-05-30 05:01:11.033005 get_cover_art-1.8.0/PKG-INFO
+-rw-r--r--   0 regosen    (501) staff       (20)     8691 2023-05-30 04:39:56.000000 get_cover_art-1.8.0/README.md
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-05-30 05:01:11.016324 get_cover_art-1.8.0/get_cover_art/
+-rw-r--r--   0 regosen    (501) staff       (20)       50 2021-11-02 19:50:11.000000 get_cover_art-1.8.0/get_cover_art/__init__.py
+-rw-r--r--   0 regosen    (501) staff       (20)     4868 2023-05-30 04:32:39.000000 get_cover_art-1.8.0/get_cover_art/__main__.py
+-rw-r--r--   0 regosen    (501) staff       (20)     5232 2023-05-30 04:58:40.000000 get_cover_art-1.8.0/get_cover_art/apple_downloader.py
+-rw-r--r--   0 regosen    (501) staff       (20)    10018 2023-05-30 04:28:05.000000 get_cover_art-1.8.0/get_cover_art/cover_finder.py
+-rw-r--r--   0 regosen    (501) staff       (20)      851 2021-06-08 05:31:32.000000 get_cover_art-1.8.0/get_cover_art/deromanizer.py
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-05-30 05:01:11.031693 get_cover_art-1.8.0/get_cover_art/meta/
+-rw-r--r--   0 regosen    (501) staff       (20)      555 2023-05-23 05:00:22.000000 get_cover_art-1.8.0/get_cover_art/meta/__init__.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1229 2023-05-30 03:53:51.000000 get_cover_art-1.8.0/get_cover_art/meta/base_id3.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1384 2023-05-30 03:53:49.000000 get_cover_art-1.8.0/get_cover_art/meta/base_ogg.py
+-rw-r--r--   0 regosen    (501) staff       (20)      988 2022-04-11 19:45:10.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_audio.py
+-rw-r--r--   0 regosen    (501) staff       (20)      168 2022-06-01 19:00:02.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_dsf.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1063 2023-05-30 03:53:44.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_flac.py
+-rw-r--r--   0 regosen    (501) staff       (20)      205 2022-06-01 18:59:46.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_mp3.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1039 2023-05-30 03:53:21.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_mp4.py
+-rw-r--r--   0 regosen    (501) staff       (20)      181 2022-06-02 04:27:54.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_opus.py
+-rw-r--r--   0 regosen    (501) staff       (20)      189 2022-06-02 04:27:54.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_vorbis.py
+-rw-r--r--   0 regosen    (501) staff       (20)      171 2023-05-30 03:25:43.000000 get_cover_art-1.8.0/get_cover_art/meta/meta_wav.py
+-rw-r--r--   0 regosen    (501) staff       (20)     1394 2023-05-22 17:42:02.000000 get_cover_art-1.8.0/get_cover_art/normalizer.py
+drwxr-xr-x   0 regosen    (501) staff       (20)        0 2023-05-30 05:01:11.020939 get_cover_art-1.8.0/get_cover_art.egg-info/
+-rw-r--r--   0 regosen    (501) staff       (20)     9594 2023-05-30 05:01:09.000000 get_cover_art-1.8.0/get_cover_art.egg-info/PKG-INFO
+-rw-r--r--   0 regosen    (501) staff       (20)      774 2023-05-30 05:01:10.000000 get_cover_art-1.8.0/get_cover_art.egg-info/SOURCES.txt
+-rw-r--r--   0 regosen    (501) staff       (20)        1 2023-05-30 05:01:09.000000 get_cover_art-1.8.0/get_cover_art.egg-info/dependency_links.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       62 2023-05-30 05:01:10.000000 get_cover_art-1.8.0/get_cover_art.egg-info/entry_points.txt
+-rw-r--r--   0 regosen    (501) staff       (20)        8 2023-05-30 05:01:10.000000 get_cover_art-1.8.0/get_cover_art.egg-info/requires.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       14 2023-05-30 05:01:10.000000 get_cover_art-1.8.0/get_cover_art.egg-info/top_level.txt
+-rw-r--r--   0 regosen    (501) staff       (20)       38 2023-05-30 05:01:11.034167 get_cover_art-1.8.0/setup.cfg
```

### Comparing `get_cover_art-1.7.0/LICENSE` & `get_cover_art-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `get_cover_art-1.7.0/PKG-INFO` & `get_cover_art-1.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: get_cover_art
-Version: 1.7.0
+Version: 1.8.0
 Summary: Batch cover art downloader and embedder for audio files
 Home-page: https://github.com/regosen/get_cover_art
 Author: Rego Sen
 Author-email: regosen@gmail.com
 License: MIT
-Keywords: cover album art artwork embed itunes apple music mp3 id3 m4a m4b mp4 aac xmp flac dsf ogg vorbis opus songs
+Keywords: cover album art artwork embed itunes apple music mp3 id3 m4a m4b mp4 aac xmp flac dsf ogg vorbis opus wav songs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -41,14 +41,17 @@
 ## Supported formats (so far)
 - MP3
 - MP4 (.m4a, .m4b)
 - FLAC
 - DSF
 - Ogg Vorbis
 - Opus
+- WAV*
+
+(* NOTE: Apple Music and other players may not recognize ID3 tags on WAV files.)
 
 ## Setup
 
 ### Requirements
 - Python 3.5 or greater
 - Python packages: [mutagen](https://pypi.org/project/mutagen/)
   - automatically installed if you use `pip install` below
@@ -77,16 +80,17 @@
 artwork options:
   --art-size ART_SIZE   square dimensions of artwork (default: 500)
   --art-quality ART_QUALITY
                         jpeg compression quality (1-100, default: auto)
   --art-dest DEST       set artwork destination folder
   --art-dest-inline     set artwork destination folder to same folders as audio files
   --art-dest-filename ART_DEST_FILENAME
-                        set artwork destination filename format. Accepts {artist},
-                        {album}, and {title}. Default '{artist} - {album}.jpg'
+                        set artwork destination filename format. Accepts
+                        {artist}, {album}, {album_or_title}, {filename}, and
+                        {title}. Default is '{artist} - {album_or_title}.jpg'
   --external-art-mode {before,after,none}
                         Use images from local disk: "before" prevents
                         downloads, "after" downloads as a fallback. Default is none.
   --external-art-filename EXTERNAL_ART_FILENAME [EXTERNAL_ART_FILENAME ...]
                         Filename(s) of folder art to use. Accepts {artist},
                         {album}, and {title} for replacement: e.g. cover.jpg
                         or {album}-{artist}.jpg ; this does not affect the filename
@@ -161,17 +165,19 @@
 can also use bracket formatting with the artist, album, and title fields:
 for instance, --external-art-filename "{artist}-{album}-cover.jpg" would create
 filenames such as "The Beatles-Abbey Road-cover.jpg".
 
 The "--art-dest-filename" option allows you to specify the filename used to
 store downloaded files, for interoperability with other systems. You __must__
 be careful to avoid collisions between different albums: The default is
-"{artist} - {album}.jpg". If you know that all of the albums you're running
+"{artist} - {album_or_title}.jpg". If you know that all of the albums you're running
 against have their own directories _and_ you are using "--art-dest-inline", then you
-could use something more generic (such as "cover.jpg").
+could use something more generic (such as "cover.jpg").  A note about the format:
+- {album_or_title} falls back on the title tag if the album tag is blank
+- {filename} uses the filename of the source audio file (minus the extension)
 
 _Pro Tip:_ If you have a cover.jpg in each album directory, you can use:
 "--external-art-mode before --external-art-filename cover.jpg --art-dest-inline"
 and the local images will be used when present (avoiding network lookups).
 You could also specify "--art-dest-filename cover.jpg" if you want to store the
 newly downloaded covers in a similar location (again, this is only sane
 in combination with --art-dest-inline, in cases where each album is stored in
```

### Comparing `get_cover_art-1.7.0/README.md` & `get_cover_art-1.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 ## Supported formats (so far)
 - MP3
 - MP4 (.m4a, .m4b)
 - FLAC
 - DSF
 - Ogg Vorbis
 - Opus
+- WAV*
+
+(* NOTE: Apple Music and other players may not recognize ID3 tags on WAV files.)
 
 ## Setup
 
 ### Requirements
 - Python 3.5 or greater
 - Python packages: [mutagen](https://pypi.org/project/mutagen/)
   - automatically installed if you use `pip install` below
@@ -53,16 +56,17 @@
 artwork options:
   --art-size ART_SIZE   square dimensions of artwork (default: 500)
   --art-quality ART_QUALITY
                         jpeg compression quality (1-100, default: auto)
   --art-dest DEST       set artwork destination folder
   --art-dest-inline     set artwork destination folder to same folders as audio files
   --art-dest-filename ART_DEST_FILENAME
-                        set artwork destination filename format. Accepts {artist},
-                        {album}, and {title}. Default '{artist} - {album}.jpg'
+                        set artwork destination filename format. Accepts
+                        {artist}, {album}, {album_or_title}, {filename}, and
+                        {title}. Default is '{artist} - {album_or_title}.jpg'
   --external-art-mode {before,after,none}
                         Use images from local disk: "before" prevents
                         downloads, "after" downloads as a fallback. Default is none.
   --external-art-filename EXTERNAL_ART_FILENAME [EXTERNAL_ART_FILENAME ...]
                         Filename(s) of folder art to use. Accepts {artist},
                         {album}, and {title} for replacement: e.g. cover.jpg
                         or {album}-{artist}.jpg ; this does not affect the filename
@@ -137,17 +141,19 @@
 can also use bracket formatting with the artist, album, and title fields:
 for instance, --external-art-filename "{artist}-{album}-cover.jpg" would create
 filenames such as "The Beatles-Abbey Road-cover.jpg".
 
 The "--art-dest-filename" option allows you to specify the filename used to
 store downloaded files, for interoperability with other systems. You __must__
 be careful to avoid collisions between different albums: The default is
-"{artist} - {album}.jpg". If you know that all of the albums you're running
+"{artist} - {album_or_title}.jpg". If you know that all of the albums you're running
 against have their own directories _and_ you are using "--art-dest-inline", then you
-could use something more generic (such as "cover.jpg").
+could use something more generic (such as "cover.jpg").  A note about the format:
+- {album_or_title} falls back on the title tag if the album tag is blank
+- {filename} uses the filename of the source audio file (minus the extension)
 
 _Pro Tip:_ If you have a cover.jpg in each album directory, you can use:
 "--external-art-mode before --external-art-filename cover.jpg --art-dest-inline"
 and the local images will be used when present (avoiding network lookups).
 You could also specify "--art-dest-filename cover.jpg" if you want to store the
 newly downloaded covers in a similar location (again, this is only sane
 in combination with --art-dest-inline, in cases where each album is stored in
```

### Comparing `get_cover_art-1.7.0/get_cover_art/__main__.py` & `get_cover_art-1.8.0/get_cover_art/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     parser.add_argument('--path', help="audio file, or folder of audio files (recursive)", default=".")
 
     parser_art = parser.add_argument_group('artwork options')
     parser_art.add_argument('--art-size', type=check_art_size, help="square dimensions of artwork (default: 500)", default=DEFAULTS.get('art_size'))
     parser_art.add_argument('--art-quality', type=check_art_quality, help="jpeg compression quality (1-100, default: auto)", default=DEFAULTS.get('art_quality'))
     parser_art.add_argument('--art-dest', '--dest', help="set artwork destination folder", default=DEFAULTS.get('cover_art'))
     parser_art.add_argument('--art-dest-inline', '--inline', help="put artwork in same folders as audio files", action='store_true')
-    parser_art.add_argument('--art-dest-filename', default=DEFAULTS.get('art_dest_filename'), help="set artwork destination filename format. Accepts {artist}, {album}, and {title}. Default '{artist} - {album}.jpg")
+    parser_art.add_argument('--art-dest-filename', default=DEFAULTS.get('art_dest_filename'), help="set artwork destination filename format. Accepts {artist}, {album}, {album_or_title}, {filename}, and {title}. Default is '{artist} - {album_or_title}.jpg'")
     parser_art.add_argument('--external-art-mode', choices=['before', 'after', 'none'], default=DEFAULTS.get('external_art_mode'), help='Use image from local folder; "before" prevents downloads, "after" uses as a fallback.  Default is none.')
     parser_art.add_argument('--external-art-filename', default=DEFAULTS.get('external_art_filename'), help="Filename(s) of folder art to use for preexisting external art. Accepts {artist}, {album}, and {title} for replacement: e.g. cover.jpg or {album}-{artist}.jpg ; this does not affect the filename for art that must be fetched (use --art-dest-filename for that).", nargs="+")
 
     parser_behavior = parser.add_argument_group('behavior options')
     parser_behavior.add_argument('--test', '--no-embed', '--no_embed', help="scan and download only, don't embed artwork", action='store_true')
     parser_behavior.add_argument('--clear', help="clear artwork from audio file (regardless of finding art)", action='store_true')
     parser_behavior.add_argument('--cleanup', help="remove downloaded artwork files afterward", action='store_true')
```

### Comparing `get_cover_art-1.7.0/get_cover_art/apple_downloader.py` & `get_cover_art-1.8.0/get_cover_art/apple_downloader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from urllib.request import Request, urlopen, HTTPError
 from urllib.parse import urlparse, quote
 from .normalizer import ArtistNormalizer, AlbumNormalizer
 from .deromanizer import DeRomanizer
 
-QUERY_TEMPLATE = "https://itunes.apple.com/search?term=%s&media=music&entity=album"
+QUERY_TEMPLATE = "https://itunes.apple.com/search?term=%s&media=music&entity=%s"
 USER_AGENT = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.55 Safari/537.36"
 THROTTLED_HTTP_CODES = [403, 429]
 
 class AppleDownloader(object):
     def __init__(self, verbose, throttle, art_size, art_quality):
         quality_suffix = "bb" if art_quality == 0 else f"-{art_quality}"
         self.file_suffix = f"{art_size}x{art_size}{quality_suffix}"
@@ -49,57 +49,65 @@
         image_data = self._urlopen_safe(image_url)
         if self.verbose:
             print(f"Downloading from: {image_url}")
         with open(dest_path,'wb') as file:
             file.write(image_data)
         print(f"Downloaded cover art: {dest_path}")
 
-    def _query(self, artist, album):
-        query_term = f"{artist} {album}"
-        if album in artist:
+    def _query(self, artist, album, title):
+        token = album or title
+        entity = "album" if album else "musicTrack"
+        query_term = f"{artist} {token}"
+        if token in artist:
             query_term = artist
-        elif artist in album:
-            query_term = album
-        url = QUERY_TEMPLATE % quote(query_term)
+        elif artist in token:
+            query_term = token
+        url = QUERY_TEMPLATE % (quote(query_term), entity)
         json = self._urlopen_text(url)
         if json:
             try:
-                return eval(json)
+                safe_json = json.replace('true', 'True').replace('false', 'False')
+                return eval(safe_json)
             except Exception:
                 pass
         return {}
 
     def _get_data(self, meta):
         artist = self.artist_normalizer.normalize(meta.artist)
         album = self.album_normalizer.normalize(meta.album)
-        info = self._query(artist, album)
-        if not info or not info['resultCount']:
+        title = self.album_normalizer.normalize(meta.title)
+        info = self._query(artist, album, title)
+        if not info or not info.get('resultCount'):
             # no result found, try replacing any roman numerals
             artist = self.deromanizer.convert_all(artist)
             album = self.deromanizer.convert_all(album)
-            info = self._query(artist, album)
-        return (artist, album, info)
+            info = self._query(artist, album, title)
+        return (artist, album, info, len(album) == 0)
 
     def download(self, meta, art_path):
-        (meta_artist, meta_album, info) = self._get_data(meta)
+        (meta_artist, meta_album, info, title_only) = self._get_data(meta)
         if info:
             try:
                 art = ""
                 # go through albums, use exact match or first contains match if no exacts found
-                for album_info in reversed(info['results']):
-                    artist = self.artist_normalizer.normalize(album_info['artistName'])
-                    album = self.album_normalizer.normalize(album_info['collectionName'])
+                results = reversed(info.get('results'))
+                if title_only:
+                    # if no album name provided, use earliest matching release
+                    results = reversed(sorted(results, key=lambda x: x.get('releaseDate')))
+                for album_info in results:
+                    artist = self.artist_normalizer.normalize(album_info.get('artistName'))
+                    album = self.album_normalizer.normalize(album_info.get('collectionName'))
                     
                     if not meta_artist in artist:
                         continue
-                    if not meta_album in album:
+                    if not title_only and not meta_album in album:
                         continue
                     
-                    art = album_info['artworkUrl100'].replace('100x100bb', self.file_suffix)
-                    if meta_album == album:
+                    art = album_info.get('artworkUrl100').replace('100x100bb', self.file_suffix)
+                    if not title_only and meta_album == album:
                         break # exact match found
                 if art:
                     self._download_from_url(art, art_path)
                     return True
             except Exception as error:
                 print(f"ERROR encountered when downloading for artist ({meta_artist}) and album ({meta_album})")
                 print(error)
```

### Comparing `get_cover_art-1.7.0/get_cover_art/cover_finder.py` & `get_cover_art-1.8.0/get_cover_art/cover_finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "art_quality": "0", # falls back on default quality
     "cover_art": "_cover_art",
     "skip_artists": "./skip_artists.txt",
     "skip_albums": "./skip_albums.txt",
     "skip_artwork": "./skip_artwork.txt",
     "external_art_mode": "none",
     "external_art_filename": ['cover.jpg', '_albumcover.jpg', 'folder.jpg'],
-    "art_dest_filename": "{artist} - {album}.jpg",
+    "art_dest_filename": "{artist} - {album_or_title}.jpg",
     "throttle": 3,
 }
 
 # utility class to cache a set of values
 class ValueStore(object):
     def __init__(self, cache_file):
         self.filename = cache_file
@@ -148,15 +148,16 @@
                     if self.verbose: print(f"Deleted folder: {folder}")
 
     def scan_file(self, path, allow_cleanup = True):
         art_folder = self.art_folder_override or os.path.split(path)[0]
         try:
             meta = get_meta(path)
             if meta:
-                filename = self._slugify(self.art_dest_filename.format(artist=meta.artist, album=meta.album, title=meta.title))
+                filename_no_ext = os.path.splitext(os.path.basename(path))[0]
+                filename = self._slugify(self.art_dest_filename.format(artist=meta.artist, album=meta.album, title=meta.title, album_or_title=meta.album or meta.title, filename=filename_no_ext))
                 art_path = os.path.join(art_folder, filename)
                 if self._should_skip(meta, art_path, self.verbose):
                     self.files_skipped.append(path)
                     if self.cleanup:
                         if allow_cleanup:
                             self._cleanup([art_path])
                         else:
```

### Comparing `get_cover_art-1.7.0/get_cover_art/deromanizer.py` & `get_cover_art-1.8.0/get_cover_art/deromanizer.py`

 * *Files identical despite different names*

### Comparing `get_cover_art-1.7.0/get_cover_art/meta/base_id3.py` & `get_cover_art-1.8.0/get_cover_art/meta/base_id3.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from .meta_audio import MetaAudio
 from mutagen.id3 import APIC
 
 class MetaID3(MetaAudio):
+    def _get_tag(self, tag):
+        return self.audio.tags[tag].text[0] if tag in self.audio.tags else ""
+    
     def __init__(self, path, audio):
         self.audio_path = path
         self.audio = audio
-        try:
-            if 'TPE2' in self.audio.tags:
-                # use Album Artist first
-                self.artist = self.audio.tags['TPE2'].text[0]
-            else:
-                self.artist = self.audio.tags['TPE1'].text[0]
-            self.album = self.audio.tags['TALB'].text[0]
-            self.title = self.audio.tags['TIT2'].text[0]
-        except:
+        # prefer Album Artist
+        self.artist = self._get_tag('TPE2') or self._get_tag('TPE1') 
+        self.album = self._get_tag('TALB')
+        self.title = self._get_tag('TIT2')
+        if self.artist == "" or self.title == "":
             raise Exception("missing ID3 tags")
 
     def has_embedded_art(self):
         return self.audio.tags.getall("APIC") != []
 
     def detach_art(self):
         self.audio.tags.delall("APIC")
```

### Comparing `get_cover_art-1.7.0/get_cover_art/meta/base_ogg.py` & `get_cover_art-1.8.0/get_cover_art/meta/base_ogg.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,26 +4,25 @@
 # specifies that it uses the FLAC structure, base64-encoded.
 from mutagen.flac import Picture
 import base64
 
 ART_TAG = 'metadata_block_picture'
 
 class MetaOgg(MetaAudio):
+    def _get_tag(self, tag):
+        return self.audio[tag][0] if tag in self.audio else ""
+    
     def __init__(self, path, audio):
         self.audio_path = path
         self.audio = audio
-        try:
-            if 'albumartist' in self.audio:
-                # use Album Artist first
-                self.artist = self.audio['albumartist'][0]
-            else:
-                self.artist = self.audio['artist'][0]
-            self.album = self.audio['album'][0]
-            self.title = self.audio['title'][0]
-        except:
+        # prefer Album Artist
+        self.artist = self._get_tag('albumartist') or self._get_tag('artist') 
+        self.album = self._get_tag('album')
+        self.title = self._get_tag('title')
+        if self.artist == "" or self.title == "":
             raise Exception("missing VorbisComment tags (in ogg vorbis or opus file)")
     
     def has_embedded_art(self):
         return bool(self.audio.get(ART_TAG, None))
 
     def detach_art(self):
         self.audio.pop(ART_TAG)
```

### Comparing `get_cover_art-1.7.0/get_cover_art/meta/meta_audio.py` & `get_cover_art-1.8.0/get_cover_art/meta/meta_audio.py`

 * *Files identical despite different names*

### Comparing `get_cover_art-1.7.0/get_cover_art/meta/meta_flac.py` & `get_cover_art-1.8.0/get_cover_art/meta/meta_flac.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from .meta_audio import MetaAudio
 from mutagen.flac import Picture, FLAC
 
 class MetaFLAC(MetaAudio):
+    def _get_tag(self, tag):
+        return self.audio[tag][0] if tag in self.audio else ""
+    
     def __init__(self, path):
         self.audio_path = path
         self.audio = FLAC(path)
-        try:
-            if 'albumartist' in self.audio:
-                # use Album Artist first
-                self.artist = self.audio['albumartist'][0]
-            else:
-                self.artist = self.audio['artist'][0]
-            self.album = self.audio['album'][0]
-            self.title = self.audio['title'][0]
-        except Exception:
+        # prefer Album Artist
+        self.artist = self._get_tag('albumartist') or self._get_tag('artist') 
+        self.album = self._get_tag('album')
+        self.title = self._get_tag('title')
+        if self.artist == "" or self.title == "":
             raise Exception("missing FLAC tags")
     
     def has_embedded_art(self):
         return self.audio.pictures != []
 
     def detach_art(self):
         self.audio.clear_pictures()
```

### Comparing `get_cover_art-1.7.0/get_cover_art/meta/meta_mp4.py` & `get_cover_art-1.8.0/get_cover_art/meta/meta_mp4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from .meta_audio import MetaAudio
 from mutagen.mp4 import MP4
 from mutagen.m4a import M4ACover
 
 class MetaMP4(MetaAudio):
+    def _get_tag(self, tag):
+        return self.audio.tags[tag][0] if tag in self.audio.tags else ""
+    
     def __init__(self, path):
         self.audio_path = path
         self.audio = MP4(path)
-        try:
-            if 'aART' in self.audio.tags:
-                # use Album Artist first
-                self.artist = self.audio.tags['aART'][0]
-            else:
-                self.artist = self.audio.tags['©ART'][0]
-            self.album = self.audio.tags['©alb'][0]
-            self.title = self.audio.tags['©nam'][0]
-        except Exception:
+        # prefer Album Artist
+        self.artist = self._get_tag('aART') or self._get_tag('©ART') 
+        self.album = self._get_tag('©alb')
+        self.title = self._get_tag('©nam')
+        if self.artist == "" or self.title == "":
             raise Exception("missing XMP tags")
     
     def has_embedded_art(self):
         return 'covr' in self.audio.tags
 
     def detach_art(self):
         self.audio.tags['covr'] = []
```

### Comparing `get_cover_art-1.7.0/get_cover_art/normalizer.py` & `get_cover_art-1.8.0/get_cover_art/normalizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
         return ' '.join(field.split()).lower()
 
 
 class ArtistNormalizer(Normalizer):
     def normalize(self, artist):
         # If the artist name has a comma, strip it and swap the string segments.
         # e.g. "Beatles, The" -> "The Beatles", "Bowie, David" -> "David Bowie"
-        (last, _sep, first) = artist.partition(',')
+        (last, _sep, first) = (artist or '').partition(',')
         if first:
             artist = f"{first.strip()} {last.strip()}"
         return super().normalize(artist)
 
 
 class AlbumNormalizer(Normalizer):
     def normalize(self, album):
         # strip "(disc 1)", etc. from album names
-        album = re.sub(r" [\(\[{]disc [\d|I|V|X]+[}\)\]]", "", album, flags=re.IGNORECASE)
+        album = re.sub(r" [\(\[{]disc [\d|I|V|X]+[}\)\]]", "", (album or ''), flags=re.IGNORECASE)
         return super().normalize(album)
```

### Comparing `get_cover_art-1.7.0/get_cover_art.egg-info/PKG-INFO` & `get_cover_art-1.8.0/get_cover_art.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: get-cover-art
-Version: 1.7.0
+Version: 1.8.0
 Summary: Batch cover art downloader and embedder for audio files
 Home-page: https://github.com/regosen/get_cover_art
 Author: Rego Sen
 Author-email: regosen@gmail.com
 License: MIT
-Keywords: cover album art artwork embed itunes apple music mp3 id3 m4a m4b mp4 aac xmp flac dsf ogg vorbis opus songs
+Keywords: cover album art artwork embed itunes apple music mp3 id3 m4a m4b mp4 aac xmp flac dsf ogg vorbis opus wav songs
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -41,14 +41,17 @@
 ## Supported formats (so far)
 - MP3
 - MP4 (.m4a, .m4b)
 - FLAC
 - DSF
 - Ogg Vorbis
 - Opus
+- WAV*
+
+(* NOTE: Apple Music and other players may not recognize ID3 tags on WAV files.)
 
 ## Setup
 
 ### Requirements
 - Python 3.5 or greater
 - Python packages: [mutagen](https://pypi.org/project/mutagen/)
   - automatically installed if you use `pip install` below
@@ -77,16 +80,17 @@
 artwork options:
   --art-size ART_SIZE   square dimensions of artwork (default: 500)
   --art-quality ART_QUALITY
                         jpeg compression quality (1-100, default: auto)
   --art-dest DEST       set artwork destination folder
   --art-dest-inline     set artwork destination folder to same folders as audio files
   --art-dest-filename ART_DEST_FILENAME
-                        set artwork destination filename format. Accepts {artist},
-                        {album}, and {title}. Default '{artist} - {album}.jpg'
+                        set artwork destination filename format. Accepts
+                        {artist}, {album}, {album_or_title}, {filename}, and
+                        {title}. Default is '{artist} - {album_or_title}.jpg'
   --external-art-mode {before,after,none}
                         Use images from local disk: "before" prevents
                         downloads, "after" downloads as a fallback. Default is none.
   --external-art-filename EXTERNAL_ART_FILENAME [EXTERNAL_ART_FILENAME ...]
                         Filename(s) of folder art to use. Accepts {artist},
                         {album}, and {title} for replacement: e.g. cover.jpg
                         or {album}-{artist}.jpg ; this does not affect the filename
@@ -161,17 +165,19 @@
 can also use bracket formatting with the artist, album, and title fields:
 for instance, --external-art-filename "{artist}-{album}-cover.jpg" would create
 filenames such as "The Beatles-Abbey Road-cover.jpg".
 
 The "--art-dest-filename" option allows you to specify the filename used to
 store downloaded files, for interoperability with other systems. You __must__
 be careful to avoid collisions between different albums: The default is
-"{artist} - {album}.jpg". If you know that all of the albums you're running
+"{artist} - {album_or_title}.jpg". If you know that all of the albums you're running
 against have their own directories _and_ you are using "--art-dest-inline", then you
-could use something more generic (such as "cover.jpg").
+could use something more generic (such as "cover.jpg").  A note about the format:
+- {album_or_title} falls back on the title tag if the album tag is blank
+- {filename} uses the filename of the source audio file (minus the extension)
 
 _Pro Tip:_ If you have a cover.jpg in each album directory, you can use:
 "--external-art-mode before --external-art-filename cover.jpg --art-dest-inline"
 and the local images will be used when present (avoiding network lookups).
 You could also specify "--art-dest-filename cover.jpg" if you want to store the
 newly downloaded covers in a similar location (again, this is only sane
 in combination with --art-dest-inline, in cases where each album is stored in
```

### Comparing `get_cover_art-1.7.0/get_cover_art.egg-info/SOURCES.txt` & `get_cover_art-1.8.0/get_cover_art.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 get_cover_art/meta/base_ogg.py
 get_cover_art/meta/meta_audio.py
 get_cover_art/meta/meta_dsf.py
 get_cover_art/meta/meta_flac.py
 get_cover_art/meta/meta_mp3.py
 get_cover_art/meta/meta_mp4.py
 get_cover_art/meta/meta_opus.py
-get_cover_art/meta/meta_vorbis.py
+get_cover_art/meta/meta_vorbis.py
+get_cover_art/meta/meta_wav.py
```

