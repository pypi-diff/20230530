# Comparing `tmp/namer-1.9.7.tar.gz` & `tmp/namer-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namer-1.9.7.tar", max compression
+gzip compressed data, was "namer-1.9.8.tar", max compression
```

## Comparing `namer-1.9.7.tar` & `namer-1.9.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0        0 2022-10-15 02:26:32.652258 namer-1.9.7/namer/__init__.py
--rw-r--r--   0        0        0     2433 2022-10-15 02:26:32.652258 namer-1.9.7/namer/__main__.py
--rw-r--r--   0        0        0    15683 2022-10-15 02:26:32.652258 namer-1.9.7/namer/command.py
--rw-r--r--   0        0        0     8912 2022-10-15 02:26:32.652258 namer-1.9.7/namer/comparison_results.py
--rw-r--r--   0        0        0    15676 2022-10-15 02:26:32.652258 namer-1.9.7/namer/configuration.py
--rw-r--r--   0        0        0    10518 2022-10-15 02:26:32.652258 namer-1.9.7/namer/configuration_utils.py
--rw-r--r--   0        0        0     8162 2022-10-15 02:26:32.652258 namer-1.9.7/namer/database.py
--rw-r--r--   0        0        0     9614 2022-10-15 02:26:32.652258 namer-1.9.7/namer/ffmpeg.py
--rw-r--r--   0        0        0     5551 2022-10-15 02:26:32.652258 namer-1.9.7/namer/filenameparts.py
--rw-r--r--   0        0        0     1261 2022-10-15 02:26:32.652258 namer-1.9.7/namer/http.py
--rw-r--r--   0        0        0    16806 2022-10-15 02:26:32.652258 namer-1.9.7/namer/metadataapi.py
--rw-r--r--   0        0        0     5273 2022-10-15 02:26:32.652258 namer-1.9.7/namer/moviexml.py
--rw-r--r--   0        0        0     5141 2022-10-15 02:26:32.652258 namer-1.9.7/namer/mutagen.py
--rw-r--r--   0        0        0     2154 2022-10-15 02:26:32.652258 namer-1.9.7/namer/name_formatter.py
--rwxr-xr-x   0        0        0    14337 2022-10-15 02:26:32.652258 namer-1.9.7/namer/namer.py
--rw-r--r--   0        0        0     5025 2022-10-15 02:26:32.652258 namer-1.9.7/namer/videophash.py
--rw-r--r--   0        0        0     9775 2022-10-15 02:26:32.652258 namer-1.9.7/namer/watchdog.py
--rw-r--r--   0        0        0     5633 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/actions.py
--rw-r--r--   0        0        0   284546 2022-10-15 02:27:09.528489 namer-1.9.7/namer/web/public/assets/bundle.min.css
--rw-r--r--   0        0        0  1252498 2022-10-15 02:27:09.528489 namer-1.9.7/namer/web/public/assets/bundle.min.js
--rw-r--r--   0        0        0   150592 2022-10-15 02:27:09.528489 namer-1.9.7/namer/web/public/assets/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   112440 2022-10-15 02:27:09.528489 namer-1.9.7/namer/web/public/assets/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0     3764 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/public/favicon.png
--rw-r--r--   0        0        0        0 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/routes/__init__.py
--rw-r--r--   0        0        0     3519 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/routes/api.py
--rw-r--r--   0        0        0     1730 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/routes/web.py
--rw-r--r--   0        0        0     4813 2022-10-15 02:26:32.652258 namer-1.9.7/namer/web/server.py
--rw-r--r--   0        0        0      891 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/components/card.html
--rw-r--r--   0        0        0     1118 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/components/cardLog.html
--rw-r--r--   0        0        0      492 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/components/navigations.html
--rw-r--r--   0        0        0     1064 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/components/performersBadges.html
--rw-r--r--   0        0        0     3880 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/pages/failed.html
--rw-r--r--   0        0        0      260 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/pages/index.html
--rw-r--r--   0        0        0      472 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/pages/queue.html
--rw-r--r--   0        0        0      328 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/pages/settings.html
--rw-r--r--   0        0        0      764 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/partials/base.html
--rw-r--r--   0        0        0     1174 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/failedFiles.html
--rw-r--r--   0        0        0      733 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/fileActions.html
--rw-r--r--   0        0        0      831 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/logDetails.html
--rw-r--r--   0        0        0      367 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/logFile.html
--rw-r--r--   0        0        0      247 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/performerBadge.html
--rw-r--r--   0        0        0      292 2022-10-15 02:27:09.536489 namer-1.9.7/namer/web/templates/render/searchResults.html
--rw-r--r--   0        0        0     1356 2022-10-15 02:26:32.656258 namer-1.9.7/pyproject.toml
--rw-r--r--   0        0        0    13312 2022-10-15 02:26:32.656258 namer-1.9.7/readme.rst
--rw-r--r--   0        0        0    14978 1970-01-01 00:00:00.000000 namer-1.9.7/setup.py
--rw-r--r--   0        0        0    14497 1970-01-01 00:00:00.000000 namer-1.9.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-06 21:17:30.083132 namer-1.9.8/namer/__init__.py
+-rw-r--r--   0        0        0     2433 2022-11-06 21:17:30.083132 namer-1.9.8/namer/__main__.py
+-rw-r--r--   0        0        0    15683 2022-11-06 21:17:30.083132 namer-1.9.8/namer/command.py
+-rw-r--r--   0        0        0     8912 2022-11-06 21:17:30.083132 namer-1.9.8/namer/comparison_results.py
+-rw-r--r--   0        0        0    15676 2022-11-06 21:17:30.083132 namer-1.9.8/namer/configuration.py
+-rw-r--r--   0        0        0    10518 2022-11-06 21:17:30.083132 namer-1.9.8/namer/configuration_utils.py
+-rw-r--r--   0        0        0     8162 2022-11-06 21:17:30.083132 namer-1.9.8/namer/database.py
+-rw-r--r--   0        0        0     9614 2022-11-06 21:17:30.083132 namer-1.9.8/namer/ffmpeg.py
+-rw-r--r--   0        0        0     5551 2022-11-06 21:17:30.083132 namer-1.9.8/namer/filenameparts.py
+-rw-r--r--   0        0        0     1261 2022-11-06 21:17:30.083132 namer-1.9.8/namer/http.py
+-rw-r--r--   0        0        0    16806 2022-11-06 21:17:30.083132 namer-1.9.8/namer/metadataapi.py
+-rw-r--r--   0        0        0     5773 2022-11-06 21:17:30.083132 namer-1.9.8/namer/moviexml.py
+-rw-r--r--   0        0        0     5141 2022-11-06 21:17:30.083132 namer-1.9.8/namer/mutagen.py
+-rw-r--r--   0        0        0     2154 2022-11-06 21:17:30.083132 namer-1.9.8/namer/name_formatter.py
+-rwxr-xr-x   0        0        0    14337 2022-11-06 21:17:30.083132 namer-1.9.8/namer/namer.py
+-rw-r--r--   0        0        0     5025 2022-11-06 21:17:30.083132 namer-1.9.8/namer/videophash.py
+-rw-r--r--   0        0        0     9775 2022-11-06 21:17:30.083132 namer-1.9.8/namer/watchdog.py
+-rw-r--r--   0        0        0     5633 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/actions.py
+-rw-r--r--   0        0        0   284546 2022-11-06 21:18:07.367305 namer-1.9.8/namer/web/public/assets/bundle.min.css
+-rw-r--r--   0        0        0  1252498 2022-11-06 21:18:07.367305 namer-1.9.8/namer/web/public/assets/bundle.min.js
+-rw-r--r--   0        0        0   150592 2022-11-06 21:18:07.367305 namer-1.9.8/namer/web/public/assets/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   112440 2022-11-06 21:18:07.367305 namer-1.9.8/namer/web/public/assets/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0     3764 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/public/favicon.png
+-rw-r--r--   0        0        0        0 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/routes/__init__.py
+-rw-r--r--   0        0        0     3519 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/routes/api.py
+-rw-r--r--   0        0        0     1730 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/routes/web.py
+-rw-r--r--   0        0        0     4813 2022-11-06 21:17:30.083132 namer-1.9.8/namer/web/server.py
+-rw-r--r--   0        0        0      891 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/components/card.html
+-rw-r--r--   0        0        0     1118 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/components/cardLog.html
+-rw-r--r--   0        0        0      492 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/components/navigations.html
+-rw-r--r--   0        0        0     1064 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/components/performersBadges.html
+-rw-r--r--   0        0        0     3880 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/pages/failed.html
+-rw-r--r--   0        0        0      260 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/pages/index.html
+-rw-r--r--   0        0        0      472 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/pages/queue.html
+-rw-r--r--   0        0        0      328 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/pages/settings.html
+-rw-r--r--   0        0        0      764 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/partials/base.html
+-rw-r--r--   0        0        0     1174 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/failedFiles.html
+-rw-r--r--   0        0        0      733 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/fileActions.html
+-rw-r--r--   0        0        0      831 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/logDetails.html
+-rw-r--r--   0        0        0      367 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/logFile.html
+-rw-r--r--   0        0        0      247 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/performerBadge.html
+-rw-r--r--   0        0        0      292 2022-11-06 21:18:07.371305 namer-1.9.8/namer/web/templates/render/searchResults.html
+-rw-r--r--   0        0        0     1385 2022-11-06 21:17:30.087132 namer-1.9.8/pyproject.toml
+-rw-r--r--   0        0        0    13312 2022-11-06 21:17:30.087132 namer-1.9.8/readme.rst
+-rw-r--r--   0        0        0    14987 1970-01-01 00:00:00.000000 namer-1.9.8/setup.py
+-rw-r--r--   0        0        0    14557 1970-01-01 00:00:00.000000 namer-1.9.8/PKG-INFO
```

### Comparing `namer-1.9.7/namer/__main__.py` & `namer-1.9.8/namer/__main__.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/command.py` & `namer-1.9.8/namer/command.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/comparison_results.py` & `namer-1.9.8/namer/comparison_results.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/configuration.py` & `namer-1.9.8/namer/configuration.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/configuration_utils.py` & `namer-1.9.8/namer/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/database.py` & `namer-1.9.8/namer/database.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/ffmpeg.py` & `namer-1.9.8/namer/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/filenameparts.py` & `namer-1.9.8/namer/filenameparts.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/http.py` & `namer-1.9.8/namer/http.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/metadataapi.py` & `namer-1.9.8/namer/metadataapi.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/mutagen.py` & `namer-1.9.8/namer/mutagen.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/name_formatter.py` & `namer-1.9.8/namer/name_formatter.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/namer.py` & `namer-1.9.8/namer/namer.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/videophash.py` & `namer-1.9.8/namer/videophash.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/watchdog.py` & `namer-1.9.8/namer/watchdog.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/actions.py` & `namer-1.9.8/namer/web/actions.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/public/assets/bundle.min.css` & `namer-1.9.8/namer/web/public/assets/bundle.min.css`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/public/assets/bundle.min.js` & `namer-1.9.8/namer/web/public/assets/bundle.min.js`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/public/assets/fonts/bootstrap-icons.woff` & `namer-1.9.8/namer/web/public/assets/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/public/assets/fonts/bootstrap-icons.woff2` & `namer-1.9.8/namer/web/public/assets/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/public/favicon.png` & `namer-1.9.8/namer/web/public/favicon.png`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/routes/api.py` & `namer-1.9.8/namer/web/routes/api.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/routes/web.py` & `namer-1.9.8/namer/web/routes/web.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/server.py` & `namer-1.9.8/namer/web/server.py`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/components/card.html` & `namer-1.9.8/namer/web/templates/components/card.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/components/cardLog.html` & `namer-1.9.8/namer/web/templates/components/cardLog.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/components/performersBadges.html` & `namer-1.9.8/namer/web/templates/components/performersBadges.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/pages/failed.html` & `namer-1.9.8/namer/web/templates/pages/failed.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/partials/base.html` & `namer-1.9.8/namer/web/templates/partials/base.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/render/failedFiles.html` & `namer-1.9.8/namer/web/templates/render/failedFiles.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/render/fileActions.html` & `namer-1.9.8/namer/web/templates/render/fileActions.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/namer/web/templates/render/logDetails.html` & `namer-1.9.8/namer/web/templates/render/logDetails.html`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/pyproject.toml` & `namer-1.9.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 [tool.poetry]
 name = "namer"
-version = "1.9.7"
+version = "1.9.8"
 description = "A namer of video files based on metadata from the porndb."
 readme = "readme.rst"
 authors = ["4c0d3r <4c0d3r@protonmail.com>"]
 include = ["**/web/public/assets/**/*", "**/web/templates/**/*"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 rapidfuzz = "^2.0.5"
 watchdog = "^2.1.6"
 pathvalidate = "^2.5.0"
 requests = "^2.27.1"
 mutagen = "^1.45.1"
-lxml = "^4.8.0"
 schedule = "^1.1.0"
 loguru = "^0.6.0"
 Unidecode = "^1.3.4"
 flask = "^2.2.0"
 jinja2 = "^3.1.2"
 waitress = "^2.1.1"
 Flask-Compress = "^1.12"
 Pillow = "^9.1.1"
 requests-cache = "^0.9.4"
 ffmpeg-python = "^0.2.0"
 ImageHash = "^4.2.1"
 jsonpickle = "^2.2.0"
+ConfigUpdater = "^3.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
 coverage = "^6.3.2"
 flakeheaven = "^3.0.0"
 selenium = "^4.2.0"
 webdriver-manager = "^3.7.0"
 assertpy = "^1.1"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+
 [tool.flakeheaven]
 exclude = [".git", "__pycache__", "docs/source/conf.py", "old", "build", "dist", "*migrations*", "init"]
 format = "colored"
 show_source = false
 max_line_length = 150
 
 [tool.flakeheaven.plugins]
 mccabe = ["+*"]
 pycodestyle = ["+*", "-E501", "-E722"]
 pyflakes = ["+*"]
 pylint = ["+*", "-C0301", "-I1101"]
 
 [tool.pylint.'MASTER']
-extension-pkg-allow-list = ["lxml"]
 max-line-length = 150
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `namer-1.9.7/readme.rst` & `namer-1.9.8/readme.rst`

 * *Files identical despite different names*

### Comparing `namer-1.9.7/setup.py` & `namer-1.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,44 +11,44 @@
                'public/assets/fonts/*',
                'templates/components/*',
                'templates/pages/*',
                'templates/partials/*',
                'templates/render/*']}
 
 install_requires = \
-['Flask-Compress>=1.12,<2.0',
+['ConfigUpdater>=3.1.1,<4.0.0',
+ 'Flask-Compress>=1.12,<2.0',
  'ImageHash>=4.2.1,<5.0.0',
  'Pillow>=9.1.1,<10.0.0',
  'Unidecode>=1.3.4,<2.0.0',
  'ffmpeg-python>=0.2.0,<0.3.0',
  'flask>=2.2.0,<3.0.0',
  'jinja2>=3.1.2,<4.0.0',
  'jsonpickle>=2.2.0,<3.0.0',
  'loguru>=0.6.0,<0.7.0',
- 'lxml>=4.8.0,<5.0.0',
  'mutagen>=1.45.1,<2.0.0',
  'pathvalidate>=2.5.0,<3.0.0',
  'rapidfuzz>=2.0.5,<3.0.0',
  'requests-cache>=0.9.4,<0.10.0',
  'requests>=2.27.1,<3.0.0',
  'schedule>=1.1.0,<2.0.0',
  'waitress>=2.1.1,<3.0.0',
  'watchdog>=2.1.6,<3.0.0']
 
 setup_kwargs = {
     'name': 'namer',
-    'version': '1.9.7',
+    'version': '1.9.8',
     'description': 'A namer of video files based on metadata from the porndb.',
     'long_description': '.. |logo| image:: ./logo/namer.png\n  :width: 80\n  :class: display: inline flow; align: left\n\n##############\n|logo| Namer\n##############\n\n.. image:: https://github.com/ThePornDatabase/namer/actions/workflows/ci.yml/badge.svg?\n  :target: https://github.com/ThePornDatabase/namer/actions/workflows/ci.yml/\n.. image:: https://codecov.io/gh/ThePornDatabase/namer/branch/main/graph/badge.svg?token=4MQEN2NUKZ\n  :target: https://codecov.io/gh/ThePornDatabase/namer\n.. image:: https://badge.fury.io/py/namer.svg?\n  :target: https://badge.fury.io/py/namer\n.. image:: https://img.shields.io/pypi/dm/namer?logo=pypi&logoColor=fff\n  :target: https://pypi.org/project/namer\n.. image:: https://static.pepy.tech/personalized-badge/namer?period=total&units=international_system&left_color=grey&right_color=yellowgreen&left_text=Downloads\n  :target: https://pepy.tech/project/namer  \n.. image:: https://static.pepy.tech/personalized-badge/namer?period=month&units=international_system&left_color=grey&right_color=yellowgreen&left_text=Downloads/Month\n  :target: https://pepy.tech/project/namer\n\nNamer is a powerful command line tool and web app for renaming and tagging mp4 video files in a way that helps plex/jellyfin/emby and related plugins extract that data or lookup data with the PornDB_\'s plugins for plex or jellyfin/emby.\nNamer is easily installed as a python pip and can:\n\n* can be used to name and embed tags in individual files with metadata from porndb:\n\n  ``python -m namer rename -f /path/to/file/Site.[YY]YY.MM.DD.MessOfText.XXX.2160.mp4 [-v]`` \n\n* can be used to name and tag files with metadata from a jellyfin/emby/kodi .nfo file (should be named the same as the file except for extension).\n\n  ``python -m namer rename -f /path/to/file/Site.[YY]YY.MM.DD.MessOfText.XXX.2160.mp4 -i [-v]``\n\n* can be used to rename a tag a file based on the directory name, so if you have a file like ``/Site.[YY]YY.MM.DD.MessOfText.XXX.2160/abc.mp4`` \n\n  ``python -m namer rename -d /path/to/dir/Site.[YY]YY.MM.DD.MessOfText.XXX.2160/``\n\n* can be used to rename a tag a whole mess of dirs and files in a directory (using -m, meaning "many").\n\n  ``python -m namer rename -m -d /path/to/dir/``\n  \n* can be used to just suggest a possible name.  The file doesn\'t need to exist but should have an extension.\n\n  ``python -m namer suggest -f Site.[YY]YY.MM.DD.MessOfText.XXX.2160.mp4``\n\n* can be run watching a directory for new files to name, tag and move to an output location, possible setting file permissions, writing .nfo files with downloaded images, attempting to grab trailers, and retrying failed files nightly.\n\n  ``python -m namer watchdog``  \n\n* while running watchdog, will also have a webui that can be used to manually match and rename any failed files.  You can set the webroot, port, bound ip, enable/disable in the namer.cfg file.\n\n  ``http:\\\\<ip>:6980\\``\n\nFor all of the above it\'s recommended to have a config file in your home directory (copied from namer.cfg.sample in this git repo)\n\nAlso provided is a docker file if you prefer.\n\nIt is possible to ignore and not need to parse dates for studios added to a list in the configuration file.  This is mostly used for studios that do not list dates on videos.\n\nWhy should I use this?\n----------------------\n\n1.  You have partially well structured file names (say from an rss feed, etc) and you never want to have to manually match files in plex/jellyfin/emby with the PornDB_\'s plugin.\n2.  You don\'t want your recent videos to be added to your library until they are matchable in the PornDB_.\n3.  You want to store the metadata about a file in mp4 files, in a way that can be read by Apple TV app, including information like: Studio, date created, name, performers, original url, proper HD tags, ratings, and movie poster.   All of this data is readable by Plex, and most by Jellyfin/Emby in case you want to standard Apple video players or your library\'s metadata storage is ever damaged.\n\nHow successful at matching videos is this tool?\n------------------------------------------------\n\nFor data pulled from the internet with rss feeds (which are often in the file format listed below) .... perfect.  The author and others have only experienced one mismatch, and that type of failure can never occur again.\n\nIf running in a background watchdog mode, files that were failed to match are retried every 24 hours, letting the PornDB_ scrapers catch up with any metadata they may be missing.\n\nOptionally, a log file can be enabled to show the original file name parts, what options were evaluated, and which match was used to name the file, it will be written next to your video file with the same name as the file (with a _namer.log) suffix rather than an mp4/mkv/avi/mov/flv extension.   This is very useful for sanity checking matches, and if ever a mismatch does occur the original file name is available in the log.\n\n\nFor the curious, how is a match made?\n------------------------------------------------\n\nIt assumes that file names exist as in a format like ```sitename-[YY]YY-MM-DD-Scene.and.or.performer.name.mp4.```.  A powerful regex tries to determine the various parts of a file\'s name.   Note that the separating dashes and dots above are interchangeable, and spaces may also be used as separators (or any number of any combo of the three.)   This regex is overridable, but you really need to know what you\'re doing and if you don\'t have all the match groups for the regex, the match from the the PornDB_ will likely not be any where near as robust as it is with a site, a date, and a scene/perform name section.\nYou\'ll have to read the code to figure out how to set this.   You really shouldn\'t do it.\n\nWhen determining a possible queried match from the PornDB_:\n\nSitename my not need be the full name of the site, as long as a the looked up sitename starts with file\'s sitename it could be a valid match.\n\nThe date may have a four digit or two digit year.  If two digit, "20" is assumed as the default century, not "19".  A potential match must be with one day plus/minus the file\'s date to be considered a match.\n\nFinally the looked up scene name and all performers first and last names are combined in to what is called a powerset (every combo of including or not including each artist and/or scene name), and that is compared against the file\'s \'Scene.and.or.performer.name\' section with a tool called rapidfuzz.   A name must be 90% similar to a member of the powerset to be considered a match, though all potential matches are evaluated and sorted before selecting the best match.   Information about all potential matches are stored in the local log file if it is enabled.\n\nI\'m sold how do I install it!\n--------------------------------------------------\n\nYou have two choices.   Do you use docker?  Pull the docker image, here\'s docker-compose snippet to help you out.\n\n\n.. code-block:: yaml\n\n  version: "3"\n  services:  \n    namer:\n      container_name: namer\n      image: ghcr.io/theporndatabase/namer:latest\n      environment:\n        - PUID=1001\n        - PGID=1000\n        - TZ=America/Los_Angeles\n        - NAMER_CONFIG=/config/namer.cfg\n      volumes:\n        - /apps/namer/:/config <- this will store the namer.cfg file.\n        - /media:/data <- this will have the four folders namer needs to work, referenced in the config file.\n      restart: always\n\nCopy namer.cfg to your config location (a path mapped to /config/namer.cfg above), and set values for your setup.   \nThe config is well commented and you should only need to add a token for the porndb and change file locations.\n\nRunning a service will occur automatically once you call ``docker-compose up``.  Now check out the configuration section below.\n\n\nPip/Python usage\n--------------------\n\nWhat if you don\'t want to use docker and/or containers?  Do you have python 3 and pip (sometimes pip3) and the command line tool ``ffmpeg`` installed locally?  If so,  ``pip install namer`` gets the job done.  If\nyou don\'t have python (3), pip and ``ffmpeg`` installed Homebrew_ can help you on Mac, and Chocolatey_ can help you on windows\n\n\n.. code-block:: sh\n\n  # install namer\n  pip3 install namer\n\n  #optionallly, set your configuration location, the below is the default:\n  export NAMER_CONFIG=${HOME}/.namer.cfg  \n\n  # Run the watchdog service:\n  python3 -m namer watchdog\n\n  # Or manually rename a file, dir, or all sub-dirs/sub-files of a dir:\n  # This calls the help method so that you can see the options.\n  python3 -m namer rename -h\n\n\nConfiguration:\n---------------------------\n\nThere is a well documented template of namer.cfg in this git repo, which is broken up in to three sections.\nOne section is related to command line renaming, the `namer section`_, one related to tagging mp4s `metadata section`_, \nand finally one related to the watchdog process `watchdog section`_.\nPlease note that the `namer section`_ section and the `watchdog section`_ \nsection both have a field to describe the new name of a file based on looked up metadata from the PornDB_.   \nThey differ because when run from the command line namer will keep the file "in place".  \nIf namer is passed a dir on the command line as input it can operate in one of two modes,\nthe default mode is to look for the largest mp4 file, or other configured movie file extension if no mp4 exists,\nand rename and move that file to the root of the folder (if it\'s in a sub-folder).\nIn this case, by default the assumption is the name of the folder should be parsed to look for information to\nsearch the PornDB_ for matching rather than the file name.   Meaning,\nif you pass a file to namer on the commandline it will be renamed but stay in the same directory.\n\n\nTypical Watchdog Behavior:\n----------------------------\n\nThe watchdog process will watch a single folder, configured with watch_dir_ in the ``namer.cfg`` file.   Any new files and directories that appear in the watch_dir_\nwill be processed once an mp4/mkv/avi/mov/flv file has been fully copied in to it.  \n\nThe first step in processing is to more the newly appearing directory or file in to the work_dir_.\n\nOnce moved the processing is highly dependant on the namer.cfg file, but in general, the name of video file or the directory file (configured with ``prefer_dir_name_if_available`` flag)\nis parsed and matched with a scene from the PornDB_.   See `For the curious, how is a match made?`_.  If a match cannot be made the general assumption is that the PornDB_ doesn\'t have metadata for that file yet.\nThe file is move to the failed dir fail_dir_ to be retried once a day at a time configured with retry_time_,\nwhich by default will be a random selected minute in the 3am hour of your timezone.   If enabled_tagging_ flag is set to true then\nthe metadata (including cover art if enable_poster_ is set) will be embedded in the mp4 file.  Please read the comments in the namer.cfg to find out about genres, tags, performers, etc.\n\nFinally, the file is moved to a location defined by dest_dir_ and new_relative_path_name_.\n\n\nDevelopment\n------------------------------\n\n.. code-block:: sh\n\n  # Building:\n  # install yarn deps\n  yarn intall   \n\n  # build css/js/copy templates\n  yarn run build\n\n  # install poetry dependencies\n  poetry install\n\n  # build python package in dist dir\n  poetry build\n\n  # Linting:\n  poetry run flakeheaven lint\n\n  # Testing:\n  poetry run pytest\n\n  # Formatting, maybe....:\n  poetry run autopep8 --in-place namer/*.py test/*.py\n\n  # Code Coverage:\n  poetry run pytest --cov\n\n  # Html Coverage report:\n  poetry run coverage html\n\n  # Local python install\n  pip install ./dist/namer-<version>.tar.gz\n\n  # Publishing:\n  # First make sure you have set gotten a token from pypi and set it on your machine.\n  poetry config pypi-token.pypi <token>\n\n  # Perhaps update the version number?\n\n  # Publishing a release to pypi.org:\n  poetry publish\n\n  # build docker file with:\n  ./docker_build.sh\n\nPull Requests Are Welcome!\n---------------------------\n\nJust be sure to pay attention to the tests and any failing pylint results.   If you want to vet a pr will be accepted before building code, file an new feature request issue, and 4c0d3r will comment on it and set you up for success.   Tests are must.\n\n.. _PornDB: http://metadataapi.net/\n.. _namer section: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L1\n.. _metadata section: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L59\n.. _watchdog section: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L89\n.. _watch_dir: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L100\n.. _work_dir: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L104\n.. _fail_dir: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L109\n.. _dest_dir: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L112\n.. _retry_time: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L115\n.. _new_relative_path_name: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L97\n.. _enabled_tagging: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L67\n.. _enable_poster: https://github.com/ThePornDatabase/namer/blob/main/namer.cfg.sample#L72\n.. _Homebrew: https://docs.brew.sh/Installation\n.. _Chocolatey: https://chocolatey.org/install\n',
     'author': '4c0d3r',
     'author_email': '4c0d3r@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `namer-1.9.7/PKG-INFO` & `namer-1.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: namer
-Version: 1.9.7
+Version: 1.9.8
 Summary: A namer of video files based on metadata from the porndb.
 Author: 4c0d3r
 Author-email: 4c0d3r@protonmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ConfigUpdater (>=3.1.1,<4.0.0)
 Requires-Dist: Flask-Compress (>=1.12,<2.0)
 Requires-Dist: ImageHash (>=4.2.1,<5.0.0)
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
 Requires-Dist: Unidecode (>=1.3.4,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: flask (>=2.2.0,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonpickle (>=2.2.0,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: mutagen (>=1.45.1,<2.0.0)
 Requires-Dist: pathvalidate (>=2.5.0,<3.0.0)
 Requires-Dist: rapidfuzz (>=2.0.5,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.4,<0.10.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: waitress (>=2.1.1,<3.0.0)
```

