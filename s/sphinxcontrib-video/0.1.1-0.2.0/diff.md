# Comparing `tmp/sphinxcontrib-video-0.1.1.tar.gz` & `tmp/sphinxcontrib-video-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-video-0.1.1.tar", last modified: Sun Mar 19 10:54:37 2023, max compression
+gzip compressed data, was "sphinxcontrib-video-0.2.0.tar", last modified: Tue May 30 19:03:01 2023, max compression
```

## Comparing `sphinxcontrib-video-0.1.1.tar` & `sphinxcontrib-video-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 10:54:37.484469 sphinxcontrib-video-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-19 10:54:37.484469 sphinxcontrib-video-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 10:54:37.484469 sphinxcontrib-video-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 10:54:37.480469 sphinxcontrib-video-0.1.1/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/sphinxcontrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/sphinxcontrib/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 10:54:37.484469 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-19 10:54:37.000000 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-19 10:54:37.000000 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 10:54:37.000000 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-19 10:54:37.000000 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-19 10:54:37.000000 sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 10:54:37.484469 sphinxcontrib-video-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-03-19 10:54:21.000000 sphinxcontrib-video-0.1.1/tests/test_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:03:01.935766 sphinxcontrib-video-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-30 19:03:01.935766 sphinxcontrib-video-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:03:01.935766 sphinxcontrib-video-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:03:01.931766 sphinxcontrib-video-0.2.0/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/sphinxcontrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/sphinxcontrib/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:03:01.935766 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-30 19:03:01.000000 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 19:03:01.000000 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:03:01.000000 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 19:03:01.000000 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 19:03:01.000000 sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:03:01.935766 sphinxcontrib-video-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-30 19:02:45.000000 sphinxcontrib-video-0.2.0/tests/test_build.py
```

### Comparing `sphinxcontrib-video-0.1.1/LICENSE` & `sphinxcontrib-video-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-video-0.1.1/PKG-INFO` & `sphinxcontrib-video-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-video
-Version: 0.1.1
+Version: 0.2.0
 Summary: Allows embedding of HTML5 videos in sphinx
 Author-email: Raphael Massabot <rmassabot@gmail.com>
 License: Apache Software License
 Project-URL: repository, https://github.com/sphinx-contrib/video
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
```

### Comparing `sphinxcontrib-video-0.1.1/README.rst` & `sphinxcontrib-video-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-video-0.1.1/pyproject.toml` & `sphinxcontrib-video-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sphinxcontrib-video"
-version = "0.1.1"
+version = "0.2.0"
 description = "Allows embedding of HTML5 videos in sphinx"
 requires-python = ">=3.6.9"
 dependencies = ["sphinx"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Sphinx :: Extension",
     "Intended Audience :: Developers",
@@ -74,13 +74,13 @@
 non_interactive = true
 warn_redundant_casts = true
 
 [tool.commitizen]
 changelog_incremental = false
 tag_format = "v$major.$minor.$patch$prerelease"
 update_changelog_on_bump = false
-version = "0.1.1"
+version = "0.2.0"
 version_files = [
     "pyproject.toml:version",
     "docs/conf.py:release",
     "sphinxcontrib/video.py:__version__"
 ]
```

### Comparing `sphinxcontrib-video-0.1.1/sphinxcontrib/video.py` & `sphinxcontrib-video-0.2.0/sphinxcontrib/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from docutils.parsers.rst import directives
 from sphinx.application import Sphinx
 from sphinx.environment import BuildEnvironment
 from sphinx.util import logging
 from sphinx.util.docutils import SphinxDirective, SphinxTranslator
 
 __author__ = "Raphael Massabot"
-__version__ = "0.1.1"
+__version__ = "0.2.0"
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_MIME_TYPES: Dict[str, str] = {
     ".mp4": "video/mp4",
     ".ogm": "video/ogg",
     ".ogv": "video/ogg",
@@ -84,14 +84,15 @@
         "nocontrols": directives.flag,
         "height": directives.unchanged,
         "loop": directives.flag,
         "muted": directives.flag,
         "poster": directives.unchanged,
         "preload": directives.unchanged,
         "width": directives.unchanged,
+        "class": directives.unchanged,
     }
 
     def run(self) -> List[video_node]:
         """Return the video node based on the set options."""
         env: BuildEnvironment = self.env
 
         # check options that need to be specific values
@@ -138,22 +139,25 @@
                 controls="nocontrols" not in self.options,
                 height=height,
                 loop="loop" in self.options,
                 muted="muted" in self.options,
                 poster=self.options.get("poster", ""),
                 preload=preload,
                 width=width,
+                klass=self.options.get("class", ""),
             )
         ]
 
 
 def visit_video_node_html(translator: SphinxTranslator, node: video_node) -> None:
     """Entry point of the html video node."""
     # start the video block
     attr: List[str] = [f'{k}="{node[k]}"' for k in SUPPORTED_OPTIONS if node[k]]
+    if node["klass"]:  # klass need to be special cased
+        attr += [f"class=\"{node['klass']}\""]
     html: str = f"<video {' '.join(attr)}>"
 
     # build the sources
     html_source = '<source src="{}" type="{}">'
     html += html_source.format(*node["primary_src"])
     if node["secondary_src"] is not None:
         html += html_source.format(*node["secondary_src"])
```

### Comparing `sphinxcontrib-video-0.1.1/sphinxcontrib_video.egg-info/PKG-INFO` & `sphinxcontrib-video-0.2.0/sphinxcontrib_video.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-video
-Version: 0.1.1
+Version: 0.2.0
 Summary: Allows embedding of HTML5 videos in sphinx
 Author-email: Raphael Massabot <rmassabot@gmail.com>
 License: Apache Software License
 Project-URL: repository, https://github.com/sphinx-contrib/video
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
```

### Comparing `sphinxcontrib-video-0.1.1/tests/test_build.py` & `sphinxcontrib-video-0.2.0/tests/test_build.py`

 * *Files identical despite different names*

