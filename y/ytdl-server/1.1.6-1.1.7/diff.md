# Comparing `tmp/ytdl-server-1.1.6.tar.gz` & `tmp/ytdl-server-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl-server-1.1.6.tar", last modified: Mon Feb 20 19:01:47 2023, max compression
+gzip compressed data, was "ytdl-server-1.1.7.tar", last modified: Tue May 30 06:45:27 2023, max compression
```

## Comparing `ytdl-server-1.1.6.tar` & `ytdl-server-1.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 19:01:47.728237 ytdl-server-1.1.6/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/COPYING
--rw-r--r--   0 root         (0) root         (0)     8771 2023-02-20 19:01:47.728237 ytdl-server-1.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7934 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-02-20 19:01:47.729236 ytdl-server-1.1.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 19:01:47.725236 ytdl-server-1.1.6/ytdl_server/
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2184 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/celery.py
--rw-rw-rw-   0 root         (0) root         (0)    10819 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/config.py
--rw-rw-rw-   0 root         (0) root         (0)    21681 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/config_option.py
--rw-rw-rw-   0 root         (0) root         (0)    20256 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/custom_opt.py
--rw-rw-rw-   0 root         (0) root         (0)     3940 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/database.py
--rw-rw-rw-   0 root         (0) root         (0)     7733 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/db_util.py
--rw-rw-rw-   0 root         (0) root         (0)      868 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/error.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/error_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2731 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/flask.py
--rw-rw-rw-   0 root         (0) root         (0)     2095 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/flask_config.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/health.py
--rw-rw-rw-   0 root         (0) root         (0)    10570 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/http_error.py
--rw-rw-rw-   0 root         (0) root         (0)    28953 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/job.py
--rw-rw-rw-   0 root         (0) root         (0)     3056 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/json.py
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/meta.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/run_celery.py
--rw-rw-rw-   0 root         (0) root         (0)     6968 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/type.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/util.py
--rw-rw-rw-   0 root         (0) root         (0)      502 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/version.py
--rw-rw-rw-   0 root         (0) root         (0)    10248 2023-02-20 19:01:13.000000 ytdl-server-1.1.6/ytdl_server/ytdl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 19:01:47.728237 ytdl-server-1.1.6/ytdl_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8771 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      773 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-20 19:01:47.000000 ytdl-server-1.1.6/ytdl_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:45:27.139426 ytdl-server-1.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/COPYING
+-rw-r--r--   0 root         (0) root         (0)     8771 2023-05-30 06:45:27.139426 ytdl-server-1.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7934 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-05-30 06:45:27.140426 ytdl-server-1.1.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:45:27.138426 ytdl-server-1.1.7/ytdl_server/
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2184 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/celery.py
+-rw-rw-rw-   0 root         (0) root         (0)    10819 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    21681 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/config_option.py
+-rw-rw-rw-   0 root         (0) root         (0)    20256 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/custom_opt.py
+-rw-rw-rw-   0 root         (0) root         (0)     3940 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     7733 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/db_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      868 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/error.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/error_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2731 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/flask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2095 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/flask_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      524 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/health.py
+-rw-rw-rw-   0 root         (0) root         (0)    10570 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/http_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    29353 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3056 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/run_celery.py
+-rw-rw-rw-   0 root         (0) root         (0)     6968 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/type.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/util.py
+-rw-rw-rw-   0 root         (0) root         (0)      502 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    10248 2023-05-30 06:45:02.000000 ytdl-server-1.1.7/ytdl_server/ytdl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 06:45:27.139426 ytdl-server-1.1.7/ytdl_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8771 2023-05-30 06:45:27.000000 ytdl-server-1.1.7/ytdl_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-05-30 06:45:27.000000 ytdl-server-1.1.7/ytdl_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 06:45:27.000000 ytdl-server-1.1.7/ytdl_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 06:45:26.000000 ytdl-server-1.1.7/ytdl_server.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-30 06:45:27.000000 ytdl-server-1.1.7/ytdl_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-30 06:45:27.000000 ytdl-server-1.1.7/ytdl_server.egg-info/top_level.txt
```

### Comparing `ytdl-server-1.1.6/COPYING` & `ytdl-server-1.1.7/COPYING`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/PKG-INFO` & `ytdl-server-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-server
-Version: 1.1.6
+Version: 1.1.7
 Summary: Download videos to a remote server using youtube-dl via a REST API
 Home-page: https://gitlab.com/adralioh/ytdl-server
 Author: Adralioh
 Project-URL: Documentation, https://adralioh.gitlab.io/ytdl-server
 Keywords: youtube-dl,yt-dlp,youtube,download,rest,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Celery
@@ -233,32 +233,32 @@
 ### REST API
 Images for the REST API are available at
 `registry.gitlab.com/adralioh/ytdl-server/api`.
 
 The images include [Gunicorn][gunicorn], which is used as the WSGI server.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
+- `latest`, `1`, `1.1`, `1.1.7`
 
 ### Celery worker
 Images for the Celery worker are available at
 `registry.gitlab.com/adralioh/ytdl-server/worker`.
 
 The *yt_dlp* tags use [yt-dlp](https://github.com/yt-dlp/yt-dlp) instead of
 youtube-dl. You also need to set the *YTDL_MODULE* env-var to `yt_dlp` on the
 REST API when using these.
 
 The *ffmpeg* tags include [FFmpeg](https://www.ffmpeg.org/), which is required
 for many of youtube-dl's post-processing options.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
-- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.6-yt_dlp`
-- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.6-ffmpeg`
-- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.6-yt_dlp-ffmpeg`
+- `latest`, `1`, `1.1`, `1.1.7`
+- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.7-yt_dlp`
+- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.7-ffmpeg`
+- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.7-yt_dlp-ffmpeg`
 
 ## Testing and development
 See [tests](tests)
 
 ## Frontends
 - [ytcl](https://gitlab.com/adralioh/ytcl) - Command-line interface with syntax
   similar to youtube-dl
```

### Comparing `ytdl-server-1.1.6/README.md` & `ytdl-server-1.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -211,32 +211,32 @@
 ### REST API
 Images for the REST API are available at
 `registry.gitlab.com/adralioh/ytdl-server/api`.
 
 The images include [Gunicorn][gunicorn], which is used as the WSGI server.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
+- `latest`, `1`, `1.1`, `1.1.7`
 
 ### Celery worker
 Images for the Celery worker are available at
 `registry.gitlab.com/adralioh/ytdl-server/worker`.
 
 The *yt_dlp* tags use [yt-dlp](https://github.com/yt-dlp/yt-dlp) instead of
 youtube-dl. You also need to set the *YTDL_MODULE* env-var to `yt_dlp` on the
 REST API when using these.
 
 The *ffmpeg* tags include [FFmpeg](https://www.ffmpeg.org/), which is required
 for many of youtube-dl's post-processing options.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
-- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.6-yt_dlp`
-- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.6-ffmpeg`
-- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.6-yt_dlp-ffmpeg`
+- `latest`, `1`, `1.1`, `1.1.7`
+- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.7-yt_dlp`
+- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.7-ffmpeg`
+- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.7-yt_dlp-ffmpeg`
 
 ## Testing and development
 See [tests](tests)
 
 ## Frontends
 - [ytcl](https://gitlab.com/adralioh/ytcl) - Command-line interface with syntax
   similar to youtube-dl
```

### Comparing `ytdl-server-1.1.6/setup.cfg` & `ytdl-server-1.1.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ytdl-server
-version = 1.1.6
+version = 1.1.7
 author = Adralioh
 description = Download videos to a remote server using youtube-dl via a REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/adralioh/ytdl-server
 project_urls = 
 	Documentation = https://adralioh.gitlab.io/ytdl-server
@@ -20,15 +20,15 @@
 	Topic :: System :: Archiving
 	Typing :: Typed
 
 [options]
 packages = ytdl_server
 python_requires = >=3.9
 zip_safe = False
-install_requires = Flask<2.2; Flask-SQLAlchemy; celery; billiard; SQLAlchemy<2; PyYAML
+install_requires = Flask<2.2; Flask-SQLAlchemy; Werkzeug<3; celery; billiard; SQLAlchemy<2; PyYAML
 
 [options.extras_require]
 dbapi = psycopg2
 
 [options.package_data]
 * = py.typed
```

### Comparing `ytdl-server-1.1.6/ytdl_server/celery.py` & `ytdl-server-1.1.7/ytdl_server/celery.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/config.py` & `ytdl-server-1.1.7/ytdl_server/config.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/config_option.py` & `ytdl-server-1.1.7/ytdl_server/config_option.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/custom_opt.py` & `ytdl-server-1.1.7/ytdl_server/custom_opt.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/database.py` & `ytdl-server-1.1.7/ytdl_server/database.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/db_util.py` & `ytdl-server-1.1.7/ytdl_server/db_util.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/error.py` & `ytdl-server-1.1.7/ytdl_server/error.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/flask.py` & `ytdl-server-1.1.7/ytdl_server/flask.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/flask_config.py` & `ytdl-server-1.1.7/ytdl_server/flask_config.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/health.py` & `ytdl-server-1.1.7/ytdl_server/health.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/http_error.py` & `ytdl-server-1.1.7/ytdl_server/http_error.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/job.py` & `ytdl-server-1.1.7/ytdl_server/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,20 @@
     """Verify that the user input received by `create_job()` is valid
 
     If the input is valid, it returns `None`
 
     If the input isn't valid, it raises `http_error.HTTPError`, which
     should be returned to the user as the response data.
     """
+    # Assert that the content type is JSON
+    if not flask.request.is_json:
+        raise http_error.DataBadType(
+            dict, description='Content-Type must be \'application/json\''
+        )
+
     # Assert that the request data is the right type
     if not isinstance(flask.request.json, dict):
         raise http_error.DataBadType(dict)
 
     # Assert that 'urls' exists in the request data
     if 'urls' not in flask.request.json:
         raise http_error.DataMissingKey('urls')
@@ -612,14 +618,20 @@
 
 def _cancel_job_check_input() -> None:
     """Verify that the user input received by `cancel_job()` is valid
 
     If the input isn't valid, it raises `http_error.HTTPError`, which
     should be returned to the user as the response data.
     """
+    # Assert that the content type is JSON
+    if not flask.request.is_json:
+        raise http_error.DataBadType(
+            dict, description='Content-Type must be \'application/json\''
+        )
+
     # Assert that the request data is the right type
     if not isinstance(flask.request.json, dict):
         raise http_error.DataBadType(dict)
 
     # Assert that 'status' exists in the request data
     if 'status' not in flask.request.json:
         raise http_error.DataMissingKey('status')
```

### Comparing `ytdl-server-1.1.6/ytdl_server/json.py` & `ytdl-server-1.1.7/ytdl_server/json.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/task.py` & `ytdl-server-1.1.7/ytdl_server/task.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/type.py` & `ytdl-server-1.1.7/ytdl_server/type.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/util.py` & `ytdl-server-1.1.7/ytdl_server/util.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server/ytdl.py` & `ytdl-server-1.1.7/ytdl_server/ytdl.py`

 * *Files identical despite different names*

### Comparing `ytdl-server-1.1.6/ytdl_server.egg-info/PKG-INFO` & `ytdl-server-1.1.7/ytdl_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-server
-Version: 1.1.6
+Version: 1.1.7
 Summary: Download videos to a remote server using youtube-dl via a REST API
 Home-page: https://gitlab.com/adralioh/ytdl-server
 Author: Adralioh
 Project-URL: Documentation, https://adralioh.gitlab.io/ytdl-server
 Keywords: youtube-dl,yt-dlp,youtube,download,rest,api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Celery
@@ -233,32 +233,32 @@
 ### REST API
 Images for the REST API are available at
 `registry.gitlab.com/adralioh/ytdl-server/api`.
 
 The images include [Gunicorn][gunicorn], which is used as the WSGI server.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
+- `latest`, `1`, `1.1`, `1.1.7`
 
 ### Celery worker
 Images for the Celery worker are available at
 `registry.gitlab.com/adralioh/ytdl-server/worker`.
 
 The *yt_dlp* tags use [yt-dlp](https://github.com/yt-dlp/yt-dlp) instead of
 youtube-dl. You also need to set the *YTDL_MODULE* env-var to `yt_dlp` on the
 REST API when using these.
 
 The *ffmpeg* tags include [FFmpeg](https://www.ffmpeg.org/), which is required
 for many of youtube-dl's post-processing options.
 
 Supported tags:
-- `latest`, `1`, `1.1`, `1.1.6`
-- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.6-yt_dlp`
-- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.6-ffmpeg`
-- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.6-yt_dlp-ffmpeg`
+- `latest`, `1`, `1.1`, `1.1.7`
+- `yt_dlp`, `1-yt_dlp`, `1.1-yt_dlp`, `1.1.7-yt_dlp`
+- `ffmpeg`, `1-ffmpeg`, `1.1-ffmpeg`, `1.1.7-ffmpeg`
+- `yt_dlp-ffmpeg`, `1-yt_dlp-ffmpeg`, `1.1-yt_dlp-ffmpeg`, `1.1.7-yt_dlp-ffmpeg`
 
 ## Testing and development
 See [tests](tests)
 
 ## Frontends
 - [ytcl](https://gitlab.com/adralioh/ytcl) - Command-line interface with syntax
   similar to youtube-dl
```

### Comparing `ytdl-server-1.1.6/ytdl_server.egg-info/SOURCES.txt` & `ytdl-server-1.1.7/ytdl_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

