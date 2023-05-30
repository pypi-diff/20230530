# Comparing `tmp/meowerbot-2.5.5.tar.gz` & `tmp/meowerbot-2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meowerbot-2.5.5.tar", max compression
+gzip compressed data, was "meowerbot-2.5.7.tar", max compression
```

## Comparing `meowerbot-2.5.5.tar` & `meowerbot-2.5.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.5/LICENSE
--rw-r--r--   0        0        0      191 2023-05-25 01:57:18.056383 meowerbot-2.5.5/MeowerBot/__init__.py
--rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.5/MeowerBot/_Commands.py
--rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.5/MeowerBot/API.py
--rw-r--r--   0        0        0    14286 2023-05-25 02:29:49.057081 meowerbot-2.5.5/MeowerBot/Bot.py
--rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.5/MeowerBot/cloudlink/__init__.py
--rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.5/MeowerBot/cloudlink/cloudlink.py
--rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.5/MeowerBot/cog.py
--rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.5/MeowerBot/command.py
--rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.5/MeowerBot/context.py
--rw-r--r--   0        0        0      649 2023-05-25 02:34:23.921191 meowerbot-2.5.5/pyproject.toml
--rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.5/README.md
--rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 meowerbot-2.5.5/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 meowerbot-2.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-15 00:38:57.652815 meowerbot-2.5.7/LICENSE
+-rw-r--r--   0        0        0      191 2023-05-30 05:10:00.997418 meowerbot-2.5.7/MeowerBot/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-15 02:04:05.213537 meowerbot-2.5.7/MeowerBot/_Commands.py
+-rw-r--r--   0        0        0     1381 2023-05-24 23:08:36.965919 meowerbot-2.5.7/MeowerBot/API.py
+-rw-r--r--   0        0        0    14286 2023-05-30 05:08:19.515887 meowerbot-2.5.7/MeowerBot/Bot.py
+-rw-r--r--   0        0        0       26 2023-03-25 06:14:31.582953 meowerbot-2.5.7/MeowerBot/cloudlink/__init__.py
+-rw-r--r--   0        0        0     8309 2023-03-25 06:14:31.583953 meowerbot-2.5.7/MeowerBot/cloudlink/cloudlink.py
+-rw-r--r--   0        0        0      747 2023-04-14 01:23:14.205535 meowerbot-2.5.7/MeowerBot/cog.py
+-rw-r--r--   0        0        0     2443 2023-05-25 00:29:18.441297 meowerbot-2.5.7/MeowerBot/command.py
+-rw-r--r--   0        0        0     1507 2023-04-15 00:22:16.273775 meowerbot-2.5.7/MeowerBot/context.py
+-rw-r--r--   0        0        0      681 2023-05-30 05:09:48.150426 meowerbot-2.5.7/pyproject.toml
+-rw-r--r--   0        0        0      244 2023-04-14 22:42:08.188135 meowerbot-2.5.7/README.md
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 meowerbot-2.5.7/setup.py
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 meowerbot-2.5.7/PKG-INFO
```

### Comparing `meowerbot-2.5.5/LICENSE` & `meowerbot-2.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/API.py` & `meowerbot-2.5.7/MeowerBot/API.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/Bot.py` & `meowerbot-2.5.7/MeowerBot/Bot.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/cloudlink/cloudlink.py` & `meowerbot-2.5.7/MeowerBot/cloudlink/cloudlink.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/cog.py` & `meowerbot-2.5.7/MeowerBot/cog.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/command.py` & `meowerbot-2.5.7/MeowerBot/command.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/MeowerBot/context.py` & `meowerbot-2.5.7/MeowerBot/context.py`

 * *Files identical despite different names*

### Comparing `meowerbot-2.5.5/pyproject.toml` & `meowerbot-2.5.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "MeowerBot"
-version = "2.5.5"
+version = "2.5.7"
 description = "A meower bot lib for py"
 authors = ["showierdata9978 <68120127+showierdata9978@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "MeowerBot"}
 ]
 repository = "https://github.com/MeowerBots/MeowerBot.py"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.0"
 websocket-client = "*"
-
+backports-strenum = { version = "^1.2.4", python = "<3.11" }
 
 [tool.poetry.group.extras.dependencies]
-backports-strenum = "^1.2.4"
+
 
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `meowerbot-2.5.5/setup.py` & `meowerbot-2.5.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,25 +6,29 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['requests>=2.28.0,<3.0.0', 'websocket-client']
 
+extras_require = \
+{':python_version < "3.11"': ['backports-strenum>=1.2.4,<2.0.0']}
+
 setup_kwargs = {
     'name': 'meowerbot',
-    'version': '2.5.5',
+    'version': '2.5.7',
     'description': 'A meower bot lib for py',
     'long_description': '# MeowerBot.py\n\nA bot lib for Meower\n\n\n## License\n\nsee [LICENSE](./LICENSE)\n\n\n## docs\n\nThe Docs are located [here](https://meowerbot-py.showierdata.tech/)\n\n\n## Quick Example\n\nlook at the [tests directory](./tests) for examples ',
     'author': 'showierdata9978',
     'author_email': '68120127+showierdata9978@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/MeowerBots/MeowerBot.py',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `meowerbot-2.5.5/PKG-INFO` & `meowerbot-2.5.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: meowerbot
-Version: 2.5.5
+Version: 2.5.7
 Summary: A meower bot lib for py
 Home-page: https://github.com/MeowerBots/MeowerBot.py
 License: MIT
 Author: showierdata9978
 Author-email: 68120127+showierdata9978@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: backports-strenum (>=1.2.4,<2.0.0) ; python_version < "3.11"
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: websocket-client
 Project-URL: Repository, https://github.com/MeowerBots/MeowerBot.py
 Description-Content-Type: text/markdown
 
 # MeowerBot.py
```

