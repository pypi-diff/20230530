# Comparing `tmp/pybrook-0.1.5.tar.gz` & `tmp/pybrook-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrook-0.1.5.tar", max compression
+gzip compressed data, was "pybrook-0.1.6.tar", max compression
```

## Comparing `pybrook-0.1.5.tar` & `pybrook-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    34916 2023-05-09 13:38:36.699045 pybrook-0.1.5/LICENSE.md
--rw-r--r--   0        0        0     6563 2023-05-09 14:48:44.826974 pybrook-0.1.5/docs/index.md
--rw-r--r--   0        0        0      958 2023-05-09 13:38:36.706045 pybrook-0.1.5/pybrook/__init__.py
--rw-r--r--   0        0        0     6237 2023-05-09 13:38:36.706045 pybrook-0.1.5/pybrook/__main__.py
--rw-r--r--   0        0        0     1461 2023-05-09 13:38:36.706045 pybrook-0.1.5/pybrook/config.py
--rw-r--r--   0        0        0      701 2023-05-09 13:38:36.706045 pybrook-0.1.5/pybrook/consumers/__init__.py
--rw-r--r--   0        0        0    10592 2023-05-09 13:38:36.706045 pybrook-0.1.5/pybrook/consumers/base.py
--rw-r--r--   0        0        0     7310 2023-05-09 13:38:36.707045 pybrook-0.1.5/pybrook/consumers/dependency_resolver.py
--rw-r--r--   0        0        0     4541 2023-05-09 14:49:20.159821 pybrook-0.1.5/pybrook/consumers/field_generator.py
--rw-r--r--   0        0        0     5231 2023-05-09 13:38:36.707045 pybrook-0.1.5/pybrook/consumers/splitter.py
--rw-r--r--   0        0        0     6138 2023-05-09 13:38:36.707045 pybrook-0.1.5/pybrook/consumers/worker.py
--rw-r--r--   0        0        0     1720 2023-05-09 13:38:36.707045 pybrook-0.1.5/pybrook/encoding.py
--rw-r--r--   0        0        0      701 2023-05-09 13:38:36.707045 pybrook-0.1.5/pybrook/examples/__init__.py
--rw-r--r--   0        0        0     2571 2023-05-09 13:38:36.708045 pybrook-0.1.5/pybrook/examples/demo.py
--rw-r--r--   0        0        0     2469 2023-05-09 13:38:36.708045 pybrook-0.1.5/pybrook/examples/ztm.py
--rw-r--r--   0        0        0   697071 2023-05-09 13:38:36.712045 pybrook-0.1.5/pybrook/frontend/build/bundle.css
--rw-r--r--   0        0        0   263192 2023-05-09 13:38:36.715045 pybrook-0.1.5/pybrook/frontend/build/bundle.js
--rw-r--r--   0        0        0   875724 2023-05-09 13:38:36.724045 pybrook-0.1.5/pybrook/frontend/build/bundle.js.map
--rw-r--r--   0        0        0     3127 2023-05-09 13:38:36.724045 pybrook-0.1.5/pybrook/frontend/favicon.png
--rw-r--r--   0        0        0      890 2023-05-09 13:38:36.724045 pybrook-0.1.5/pybrook/frontend/global.css
--rw-r--r--   0        0        0      386 2023-05-09 13:38:36.724045 pybrook-0.1.5/pybrook/frontend/index.html
--rw-r--r--   0        0        0    32825 2023-05-09 13:38:36.724045 pybrook-0.1.5/pybrook/models.py
--rw-r--r--   0        0        0     2238 2023-05-09 13:38:36.725045 pybrook-0.1.5/pybrook/schemas.py
--rw-r--r--   0        0        0     1791 2023-05-09 15:07:25.347287 pybrook-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7996 1970-01-01 00:00:00.000000 pybrook-0.1.5/setup.py
--rw-r--r--   0        0        0     7848 1970-01-01 00:00:00.000000 pybrook-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-05-09 13:38:36.699045 pybrook-0.1.6/LICENSE.md
+-rw-r--r--   0        0        0     6981 2023-05-30 21:04:18.543186 pybrook-0.1.6/docs/index.md
+-rw-r--r--   0        0        0      958 2023-05-09 13:38:36.706045 pybrook-0.1.6/pybrook/__init__.py
+-rw-r--r--   0        0        0     6474 2023-05-30 20:39:17.318710 pybrook-0.1.6/pybrook/__main__.py
+-rw-r--r--   0        0        0     1461 2023-05-09 13:38:36.706045 pybrook-0.1.6/pybrook/config.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.706045 pybrook-0.1.6/pybrook/consumers/__init__.py
+-rw-r--r--   0        0        0    10592 2023-05-09 13:38:36.706045 pybrook-0.1.6/pybrook/consumers/base.py
+-rw-r--r--   0        0        0     7310 2023-05-09 13:38:36.707045 pybrook-0.1.6/pybrook/consumers/dependency_resolver.py
+-rw-r--r--   0        0        0     4541 2023-05-09 14:49:20.159821 pybrook-0.1.6/pybrook/consumers/field_generator.py
+-rw-r--r--   0        0        0     5231 2023-05-09 13:38:36.707045 pybrook-0.1.6/pybrook/consumers/splitter.py
+-rw-r--r--   0        0        0     6215 2023-05-30 20:28:38.884001 pybrook-0.1.6/pybrook/consumers/worker.py
+-rw-r--r--   0        0        0     1720 2023-05-09 13:38:36.707045 pybrook-0.1.6/pybrook/encoding.py
+-rw-r--r--   0        0        0      701 2023-05-09 13:38:36.707045 pybrook-0.1.6/pybrook/examples/__init__.py
+-rw-r--r--   0        0        0     2571 2023-05-30 20:49:24.074575 pybrook-0.1.6/pybrook/examples/demo.py
+-rw-r--r--   0        0        0     2469 2023-05-09 13:38:36.708045 pybrook-0.1.6/pybrook/examples/ztm.py
+-rw-r--r--   0        0        0   697071 2023-05-09 13:38:36.712045 pybrook-0.1.6/pybrook/frontend/build/bundle.css
+-rw-r--r--   0        0        0   263192 2023-05-09 13:38:36.715045 pybrook-0.1.6/pybrook/frontend/build/bundle.js
+-rw-r--r--   0        0        0   875724 2023-05-09 13:38:36.724045 pybrook-0.1.6/pybrook/frontend/build/bundle.js.map
+-rw-r--r--   0        0        0     3127 2023-05-09 13:38:36.724045 pybrook-0.1.6/pybrook/frontend/favicon.png
+-rw-r--r--   0        0        0      890 2023-05-09 13:38:36.724045 pybrook-0.1.6/pybrook/frontend/global.css
+-rw-r--r--   0        0        0      386 2023-05-09 13:38:36.724045 pybrook-0.1.6/pybrook/frontend/index.html
+-rw-r--r--   0        0        0    32880 2023-05-30 20:25:25.772694 pybrook-0.1.6/pybrook/models.py
+-rw-r--r--   0        0        0     2238 2023-05-09 13:38:36.725045 pybrook-0.1.6/pybrook/schemas.py
+-rw-r--r--   0        0        0     1732 2023-05-30 21:05:41.365054 pybrook-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     8368 1970-01-01 00:00:00.000000 pybrook-0.1.6/setup.py
+-rw-r--r--   0        0        0     8187 1970-01-01 00:00:00.000000 pybrook-0.1.6/PKG-INFO
```

### Comparing `pybrook-0.1.5/LICENSE.md` & `pybrook-0.1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/docs/index.md` & `pybrook-0.1.6/docs/index.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![PyPI](https://img.shields.io/pypi/v/pybrook?style=for-the-badge&color=purple)](https://pypi.org/project/pybrook/)
+[![docs](https://img.shields.io/badge/docs-mkdocs+mkdocstrings-lightblue?style=for-the-badge)](https://pybrook.github.io/pybrook/)
+![Python](https://img.shields.io/badge/python-3.7%2B-blue?style=for-the-badge)
+![Coverage](https://img.shields.io/badge/coverage-81%25-green?style=for-the-badge)
+
 # Introduction
 
 PyBrook - a real-time cloud computing framework for the Internet of Things.
 PyBrook enables users to define complex data processing models declaratively using the Python programming language.
 The framework also provides a generic web interface that presents the collected data in real-time.
 
 PyBrook aims to make the development of real-time data processing services as easy as possible by utilising powerful 
@@ -153,15 +158,15 @@
     image: pybrook:latest
     depends_on:
       - api
     ports:
       - 8089:8089
     command: locust -H http://api:8000
   redis:
-    image: redislabs/redisgears:latest
+    image: redislabs/redisgears:1.0.9
 ```
 
 Then run `docker-compose up --build` again, to start PyBrook - this time using your own model.
 
 ## Setup & Development
 
 You can install the PyBrook from PyPi using `pip`:
@@ -172,19 +177,19 @@
 
 ## Running all services manually, without Docker
 
 To run the `pybrook.examples.demo` model, you have to start all the required services manually:
 
 ```bash
 # Redis + Redis Gears
-docker run --net=host -d redislabs/redisgears
+docker run --net=host -d redislabs/redisgears:1.0.9
 # HTTP API based on pybrook.examples.demo - uvicorn
 uvicorn pybrook.examples.demo:app --reload  
 # PyBrook workers based on pybrook.examples.demo 
-pybrook pybrook.examples.demo:brook   
+pybrook pybrook.examples.demo:brook -rg 
 # Locust - load testing
 locust -H http://localhost:8000
 ```
 
 ## Contributing
 
 PyBrook uses [poetry](https://python-poetry.org) for dependency management.
```

### Comparing `pybrook-0.1.5/pybrook/__init__.py` & `pybrook-0.1.6/pybrook/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/__main__.py` & `pybrook-0.1.6/pybrook/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,19 +81,22 @@
         A dictionary of consumer configs filled with defaults. Consumer group names are used as keys.
 
     """
     workers_config = {}
     for c in consumers:
         if not isinstance(c, GearsStreamConsumer):
             consumer_config = ConsumerConfig()
-            parser.add_argument(
-                f'--{c.consumer_group_name}-workers',
-                type=int,
-                help='(default: %(default)s)',  # noqa: WPS323
-                default=consumer_config.workers)
+            try:
+                parser.add_argument(
+                    f'--{c.consumer_group_name}-workers',
+                    type=int,
+                    help='(default: %(default)s)',  # noqa: WPS323
+                    default=consumer_config.workers)
+            except argparse.ArgumentError:
+                ... # OK, this argument already exists
             workers_config[c.consumer_group_name] = consumer_config
     return workers_config
 
 
 def update_workers_config(args: argparse.Namespace,
                           workers_config: Dict[str, ConsumerConfig]):
     """
@@ -147,14 +150,15 @@
                                 (default: 4)
 
         ```
     """
 
     parser = argparse.ArgumentParser(add_help=False)
     parser.add_argument('-h', '--help', action='store_true')
+    parser.add_argument('-rg', '--enable-gears', action='store_true')
     parser.add_argument('APP', nargs=1)
     args: argparse.Namespace
     unknown: List[str]
     args, unknown = parser.parse_known_args()
     app_arg = args.APP[-1].split(':') if args.APP else None
     if not app_arg and args.help:
         parser.print_help()
@@ -172,15 +176,15 @@
             parser.print_help()
             return
         update_workers_config(args, workers_config)
         handler = ModelChangeEventHandler(brook)
         observer = Observer()
         observer.schedule(handler, model_module.__file__)  # noqa: WPS609
         observer.start()
-        brook.run(config=workers_config)
+        brook.run(config=workers_config, enable_gears=args.enable_gears)
         observer.stop()
         observer.join()
         reload(model_module)
         modified = handler.modified
 
 
 if __name__ == '__main__':
```

### Comparing `pybrook-0.1.5/pybrook/config.py` & `pybrook-0.1.6/pybrook/config.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/__init__.py` & `pybrook-0.1.6/pybrook/consumers/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/base.py` & `pybrook-0.1.6/pybrook/consumers/base.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/dependency_resolver.py` & `pybrook-0.1.6/pybrook/consumers/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/field_generator.py` & `pybrook-0.1.6/pybrook/consumers/field_generator.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/splitter.py` & `pybrook-0.1.6/pybrook/consumers/splitter.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/consumers/worker.py` & `pybrook-0.1.6/pybrook/consumers/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,24 +130,25 @@
 
         self.spawn_workers()
 
         for redis_url in self.redis_urls:
             redis_conn = redis.from_url(redis_url,
                                         decode_responses=True,
                                         encoding='utf-8')
-            self.acquire_gears_registration_lock(redis_conn)
-            ids = [
-                r[1]
-                for r in redis_conn.execute_command('RG.DUMPREGISTRATIONS')
-            ]
-            for i in ids:
-                redis_conn.execute_command('RG.UNREGISTER', i)
-            for consumer in self.gears_consumers:
-                consumer.register_builder(redis_conn)
-            redis_conn.delete('RG.REGISTERLOCK')
+            if self.gears_consumers:
+                self.acquire_gears_registration_lock(redis_conn)
+                ids = [
+                    r[1]
+                    for r in redis_conn.execute_command('RG.DUMPREGISTRATIONS')
+                ]
+                for i in ids:
+                    redis_conn.execute_command('RG.UNREGISTER', i)
+                for consumer in self.gears_consumers:
+                    consumer.register_builder(redis_conn)
+                redis_conn.delete('RG.REGISTERLOCK')
         for proc in self.processes:
             try:
                 proc.join()
             except KeyboardInterrupt:
                 ...
         self.processes = []
```

### Comparing `pybrook-0.1.5/pybrook/encoding.py` & `pybrook-0.1.6/pybrook/encoding.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/examples/__init__.py` & `pybrook-0.1.6/pybrook/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/examples/demo.py` & `pybrook-0.1.6/pybrook/examples/demo.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/examples/ztm.py` & `pybrook-0.1.6/pybrook/examples/ztm.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/frontend/build/bundle.css` & `pybrook-0.1.6/pybrook/frontend/build/bundle.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/frontend/build/bundle.js` & `pybrook-0.1.6/pybrook/frontend/build/bundle.js`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/frontend/build/bundle.js.map` & `pybrook-0.1.6/pybrook/frontend/build/bundle.js.map`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/frontend/favicon.png` & `pybrook-0.1.6/pybrook/frontend/favicon.png`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/frontend/global.css` & `pybrook-0.1.6/pybrook/frontend/global.css`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pybrook/models.py` & `pybrook-0.1.6/pybrook/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -778,25 +778,25 @@
                 self.visit(field)
 
     @property
     def app(self) -> fastapi.FastAPI:
         self.process_model()
         return self.api.fastapi
 
-    def run(self, config: Dict[str, ConsumerConfig] = None):
+    def run(self, config: Dict[str, ConsumerConfig] = None, enable_gears: bool = False):
         """
         Runs the workers.
 
         Args:
             config: Consumer config, can be skipped - defaults will be used. See [pybrook.__main__][pybrook.__main__] for details.
         """
 
         config = config or {}
         self.process_model()
-        self.manager = WorkerManager(self.consumers, config=config)
+        self.manager = WorkerManager(self.consumers, config=config, enable_gears=enable_gears)
         self.manager.run()
 
     def terminate(self):
         """Terminates all worker processes gracefully."""
         if not self.manager:
             raise RuntimeError('PyBrook is not running!')
         self.manager.terminate()
```

### Comparing `pybrook-0.1.5/pybrook/schemas.py` & `pybrook-0.1.6/pybrook/schemas.py`

 * *Files identical despite different names*

### Comparing `pybrook-0.1.5/pyproject.toml` & `pybrook-0.1.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 [tool.poetry]
 name = "pybrook"
-version = "0.1.5"
+version = "0.1.6"
 description = "PyBrook - a real-time cloud computing framework for the Internet of Things."
 repository = "https://github.com/pybrook/pybrook"
 authors = ["Michał Rokita <mrokita@mrokita.pl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [tool.poetry.scripts]
 pybrook = "pybrook.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-fastapi = "^0.87.0"
-uvicorn = {extras = ["standard"], version = "^0.20.0"}
-pytest = "^6.2.5"
-redis = {extras = ["asyncio"], version = "^4.5.1"}
-loguru = "^0.5.3"
+fastapi = "^0.95.2"
+uvicorn = {extras = ["standard"], version = "^0.22.0"}
+redis = {extras = ["asyncio"], version = "^4.5.5"}
+loguru = "^0.7.0"
 gunicorn = "^20.1.0"
-httpx = "^0.21.1"
-watchdog = "^2.1.6"
+watchdog = "^3.0.0"
 uvloop = "^0.17.0"
-orjson = "^3.6.5"
+orjson = "^3.8.7"
 locust = "^2.6.1"
-pydantic = "^1.10.6"
+pydantic = "^1.10.8"
 
 
 [tool.poetry.group.dev.dependencies]
 # docs
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.3"
@@ -36,27 +34,26 @@
 
 # formatting
 yapf = "^0.31.0"
 isort = "^5.5.1"
 
 # linting
 darglint = "^1.5.8"
-flake8-bandit = "^2.1.2"
 flake8-bugbear = "^21.4.3"
 flake8-builtins = "^1.5.3"
 flake8-comprehensions = "^3.3.1"
 flake8-pytest-style = "^1.3.0"
 flake8-string-format = "^0.3.0"
 flake8-tidy-imports = "^4.2.1"
 flake8-variables-names = "^0.0.4"
 pep8-naming = "^0.12.1"
 mypy = "^0.910"
 
 # tests
-pytest = "^6.2"
+pytest = "^7.3.1"
 pytest-cov = "^3.0.0"
 pytest-sugar = "^0.9.4"
 
 # misc
 ptpython = "^3.0.7"
 pytest-asyncio = "^0.15.1"
 types-redis = "^3.5.15"
```

### Comparing `pybrook-0.1.5/setup.py` & `pybrook-0.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 packages = \
 ['pybrook', 'pybrook.consumers', 'pybrook.examples']
 
 package_data = \
 {'': ['*'], 'pybrook': ['frontend/*', 'frontend/build/*']}
 
 install_requires = \
-['fastapi>=0.87.0,<0.88.0',
+['fastapi>=0.95.2,<0.96.0',
  'gunicorn>=20.1.0,<21.0.0',
- 'httpx>=0.21.1,<0.22.0',
  'locust>=2.6.1,<3.0.0',
- 'loguru>=0.5.3,<0.6.0',
- 'orjson>=3.6.5,<4.0.0',
- 'pydantic>=1.10.6,<2.0.0',
- 'pytest>=6.2.5,<7.0.0',
- 'redis[asyncio]>=4.5.1,<5.0.0',
- 'uvicorn[standard]>=0.20.0,<0.21.0',
+ 'loguru>=0.7.0,<0.8.0',
+ 'orjson>=3.8.7,<4.0.0',
+ 'pydantic>=1.10.8,<2.0.0',
+ 'redis[asyncio]>=4.5.5,<5.0.0',
+ 'uvicorn[standard]>=0.22.0,<0.23.0',
  'uvloop>=0.17.0,<0.18.0',
- 'watchdog>=2.1.6,<3.0.0']
+ 'watchdog>=3.0.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['pybrook = pybrook.__main__:main']}
 
 setup_kwargs = {
     'name': 'pybrook',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'PyBrook - a real-time cloud computing framework for the Internet of Things.',
-    'long_description': '# Introduction\n\nPyBrook - a real-time cloud computing framework for the Internet of Things.\nPyBrook enables users to define complex data processing models declaratively using the Python programming language.\nThe framework also provides a generic web interface that presents the collected data in real-time.\n\nPyBrook aims to make the development of real-time data processing services as easy as possible by utilising powerful \nmechanisms of the Python programming language and modern concepts like hot-reloading or deploying software in Linux Containers.\n\nA simple `docker-compose up` is enough to start playing with the framework.\n\n## Run demo with Docker\n\nIt is recommended to use `docker-compose` for learning (you can use the `docker-compose.yml` from the [project repository](https://github.com/pybrook/pybrook/blob/master/docker-compose.yml):\n\n```bash\ndocker-compose up\n```\n\nThis command will start all the services, including Redis with Redis Gears enabled.\n\nThe following services will be available:\n\n- OpenAPI docs (ReDoc): <http://localhost:8000/redoc> \n- OpenAPI docs (Swagger UI): <http://localhost:8000/docs> \n- PyBrook frontend: <http://localhost:8000/panel> \n- Locust panel for load testing: <http://localhost:8089>\n\nYou should probably visit the Locust panel first and start sending some reports.\n\n### Using your own model\n\nThe configured model is `pybrook.examples.demo`, but replacing it with your own is very easy.  \nFirst, you have to save your custom model somewhere. \nFor now, you can just copy the source of `pybrook.examples.demo` (attached below) and save it as `mymodel.py` in your working directory.\n\n??? example "Source of `pybrook.examples.demo`"\n\n    ```python linenums="1"\n    from datetime import datetime\n    from math import atan2, degrees\n    from typing import Optional, Sequence\n    \n    from pybrook.models import (\n        InReport,\n        OutReport,\n        PyBrook,\n        ReportField,\n        dependency,\n        historical_dependency,\n    )\n    \n    brook = PyBrook(\'redis://localhost\')\n    app = brook.app\n    \n    \n    @brook.input(\'ztm-report\', id_field=\'vehicle_number\')\n    class ZTMReport(InReport):\n        vehicle_number: int\n        time: datetime\n        lat: float\n        lon: float\n        brigade: str\n        line: str\n    \n    \n    @brook.output(\'location-report\')\n    class LocationReport(OutReport):\n        vehicle_number = ReportField(ZTMReport.vehicle_number)\n        lat = ReportField(ZTMReport.lat)\n        lon = ReportField(ZTMReport.lon)\n        line = ReportField(ZTMReport.line)\n        time = ReportField(ZTMReport.time)\n        brigade = ReportField(ZTMReport.brigade)\n    \n    \n    @brook.artificial_field()\n    def direction(lat_history: Sequence[float] = historical_dependency(\n        ZTMReport.lat, history_length=1),\n                        lon_history: Sequence[float] = historical_dependency(\n                            ZTMReport.lon, history_length=1),\n                        lat: float = dependency(ZTMReport.lat),\n                        lon: float = dependency(ZTMReport.lon)) -> Optional[float]:\n        prev_lat, = lat_history\n        prev_lon, = lon_history\n        if prev_lat and prev_lon:\n            return degrees(atan2(lon - prev_lon, lat - prev_lat))\n        else:\n            return None\n    \n    \n    @brook.output(\'direction-report\')\n    class DirectionReport(OutReport):\n        direction = ReportField(direction)\n    \n    \n    @brook.artificial_field()\n    async def counter(prev_values: Sequence[int] = historical_dependency(\n        \'counter\', history_length=1),\n                      time: datetime = dependency(ZTMReport.time)) -> int:\n        prev_value, = prev_values\n        if prev_value is None:\n            prev_value = -1\n        prev_value += 1\n        return prev_value\n    \n    \n    @brook.output(\'counter-report\')\n    class CounterReport(OutReport):\n        counter = ReportField(counter)\n    \n    \n    brook.set_meta(latitude_field=LocationReport.lat,\n                   longitude_field=LocationReport.lon,\n                   time_field=LocationReport.time,\n                   group_field=LocationReport.line,\n                   direction_field=DirectionReport.direction)\n    \n    if __name__ == \'__main__\':\n        brook.run()\n    ```\n\nAfter creating `mymodel.py`, you should add it to the `api` and `worker` containers, using a Docker volume.\nTo make PyBrook use `mymodel` instead of `pybrook.examples.demo`, you should also alter the arguments passed to `gunicorn` and `pybrook`. \nYou can simply add it to the default `docker-compose.yml`:\n\n```yaml hl_lines="20 21 10 11 12 13 14 24" linenums="1"\nservices:\n  api:\n    image: pybrook:latest\n    build:\n      context: .\n    environment:\n      REDIS_URL: redis://redis\n    ports:\n      - 8000:8000\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: gunicorn mymodel:app \n          -w 4 -k uvicorn.workers.UvicornWorker \n          -b 0.0.0.0:8000\n  worker:\n    image: pybrook:latest\n    depends_on:\n      - api\n    environment:\n      REDIS_URL: redis://redis\n      DEFAULT_WORKERS: 8\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: pybrook mymodel:brook\n  locust:\n    image: pybrook:latest\n    depends_on:\n      - api\n    ports:\n      - 8089:8089\n    command: locust -H http://api:8000\n  redis:\n    image: redislabs/redisgears:latest\n```\n\nThen run `docker-compose up --build` again, to start PyBrook - this time using your own model.\n\n## Setup & Development\n\nYou can install the PyBrook from PyPi using `pip`:\n\n```bash\npip install pybrook\n```\n\n## Running all services manually, without Docker\n\nTo run the `pybrook.examples.demo` model, you have to start all the required services manually:\n\n```bash\n# Redis + Redis Gears\ndocker run --net=host -d redislabs/redisgears\n# HTTP API based on pybrook.examples.demo - uvicorn\nuvicorn pybrook.examples.demo:app --reload  \n# PyBrook workers based on pybrook.examples.demo \npybrook pybrook.examples.demo:brook   \n# Locust - load testing\nlocust -H http://localhost:8000\n```\n\n## Contributing\n\nPyBrook uses [poetry](https://python-poetry.org) for dependency management.\nTo install all its development dependencies, simply run this command:\n\n```bash\npoetry install\n```\n\n### Tests\n\n```bash\nmake test\n```\n\n### Code quality\n\nThe source code of PyBrook is formatted using yapf and isort.  \nTo run them with the correct settings, use the following command:\n\n```bash\nmake format\n```\n\nPyBrook uses `mypy` for type checking and `flake8` for linting.\nUse the following command to run them with the appropriate settings:\n\n```bash\nmake lint\n```',
+    'long_description': '[![PyPI](https://img.shields.io/pypi/v/pybrook?style=for-the-badge&color=purple)](https://pypi.org/project/pybrook/)\n[![docs](https://img.shields.io/badge/docs-mkdocs+mkdocstrings-lightblue?style=for-the-badge)](https://pybrook.github.io/pybrook/)\n![Python](https://img.shields.io/badge/python-3.7%2B-blue?style=for-the-badge)\n![Coverage](https://img.shields.io/badge/coverage-81%25-green?style=for-the-badge)\n\n# Introduction\n\nPyBrook - a real-time cloud computing framework for the Internet of Things.\nPyBrook enables users to define complex data processing models declaratively using the Python programming language.\nThe framework also provides a generic web interface that presents the collected data in real-time.\n\nPyBrook aims to make the development of real-time data processing services as easy as possible by utilising powerful \nmechanisms of the Python programming language and modern concepts like hot-reloading or deploying software in Linux Containers.\n\nA simple `docker-compose up` is enough to start playing with the framework.\n\n## Run demo with Docker\n\nIt is recommended to use `docker-compose` for learning (you can use the `docker-compose.yml` from the [project repository](https://github.com/pybrook/pybrook/blob/master/docker-compose.yml):\n\n```bash\ndocker-compose up\n```\n\nThis command will start all the services, including Redis with Redis Gears enabled.\n\nThe following services will be available:\n\n- OpenAPI docs (ReDoc): <http://localhost:8000/redoc> \n- OpenAPI docs (Swagger UI): <http://localhost:8000/docs> \n- PyBrook frontend: <http://localhost:8000/panel> \n- Locust panel for load testing: <http://localhost:8089>\n\nYou should probably visit the Locust panel first and start sending some reports.\n\n### Using your own model\n\nThe configured model is `pybrook.examples.demo`, but replacing it with your own is very easy.  \nFirst, you have to save your custom model somewhere. \nFor now, you can just copy the source of `pybrook.examples.demo` (attached below) and save it as `mymodel.py` in your working directory.\n\n??? example "Source of `pybrook.examples.demo`"\n\n    ```python linenums="1"\n    from datetime import datetime\n    from math import atan2, degrees\n    from typing import Optional, Sequence\n    \n    from pybrook.models import (\n        InReport,\n        OutReport,\n        PyBrook,\n        ReportField,\n        dependency,\n        historical_dependency,\n    )\n    \n    brook = PyBrook(\'redis://localhost\')\n    app = brook.app\n    \n    \n    @brook.input(\'ztm-report\', id_field=\'vehicle_number\')\n    class ZTMReport(InReport):\n        vehicle_number: int\n        time: datetime\n        lat: float\n        lon: float\n        brigade: str\n        line: str\n    \n    \n    @brook.output(\'location-report\')\n    class LocationReport(OutReport):\n        vehicle_number = ReportField(ZTMReport.vehicle_number)\n        lat = ReportField(ZTMReport.lat)\n        lon = ReportField(ZTMReport.lon)\n        line = ReportField(ZTMReport.line)\n        time = ReportField(ZTMReport.time)\n        brigade = ReportField(ZTMReport.brigade)\n    \n    \n    @brook.artificial_field()\n    def direction(lat_history: Sequence[float] = historical_dependency(\n        ZTMReport.lat, history_length=1),\n                        lon_history: Sequence[float] = historical_dependency(\n                            ZTMReport.lon, history_length=1),\n                        lat: float = dependency(ZTMReport.lat),\n                        lon: float = dependency(ZTMReport.lon)) -> Optional[float]:\n        prev_lat, = lat_history\n        prev_lon, = lon_history\n        if prev_lat and prev_lon:\n            return degrees(atan2(lon - prev_lon, lat - prev_lat))\n        else:\n            return None\n    \n    \n    @brook.output(\'direction-report\')\n    class DirectionReport(OutReport):\n        direction = ReportField(direction)\n    \n    \n    @brook.artificial_field()\n    async def counter(prev_values: Sequence[int] = historical_dependency(\n        \'counter\', history_length=1),\n                      time: datetime = dependency(ZTMReport.time)) -> int:\n        prev_value, = prev_values\n        if prev_value is None:\n            prev_value = -1\n        prev_value += 1\n        return prev_value\n    \n    \n    @brook.output(\'counter-report\')\n    class CounterReport(OutReport):\n        counter = ReportField(counter)\n    \n    \n    brook.set_meta(latitude_field=LocationReport.lat,\n                   longitude_field=LocationReport.lon,\n                   time_field=LocationReport.time,\n                   group_field=LocationReport.line,\n                   direction_field=DirectionReport.direction)\n    \n    if __name__ == \'__main__\':\n        brook.run()\n    ```\n\nAfter creating `mymodel.py`, you should add it to the `api` and `worker` containers, using a Docker volume.\nTo make PyBrook use `mymodel` instead of `pybrook.examples.demo`, you should also alter the arguments passed to `gunicorn` and `pybrook`. \nYou can simply add it to the default `docker-compose.yml`:\n\n```yaml hl_lines="20 21 10 11 12 13 14 24" linenums="1"\nservices:\n  api:\n    image: pybrook:latest\n    build:\n      context: .\n    environment:\n      REDIS_URL: redis://redis\n    ports:\n      - 8000:8000\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: gunicorn mymodel:app \n          -w 4 -k uvicorn.workers.UvicornWorker \n          -b 0.0.0.0:8000\n  worker:\n    image: pybrook:latest\n    depends_on:\n      - api\n    environment:\n      REDIS_URL: redis://redis\n      DEFAULT_WORKERS: 8\n    volumes:\n      - ./mymodel.py:/src/mymodel.py\n    command: pybrook mymodel:brook\n  locust:\n    image: pybrook:latest\n    depends_on:\n      - api\n    ports:\n      - 8089:8089\n    command: locust -H http://api:8000\n  redis:\n    image: redislabs/redisgears:1.0.9\n```\n\nThen run `docker-compose up --build` again, to start PyBrook - this time using your own model.\n\n## Setup & Development\n\nYou can install the PyBrook from PyPi using `pip`:\n\n```bash\npip install pybrook\n```\n\n## Running all services manually, without Docker\n\nTo run the `pybrook.examples.demo` model, you have to start all the required services manually:\n\n```bash\n# Redis + Redis Gears\ndocker run --net=host -d redislabs/redisgears:1.0.9\n# HTTP API based on pybrook.examples.demo - uvicorn\nuvicorn pybrook.examples.demo:app --reload  \n# PyBrook workers based on pybrook.examples.demo \npybrook pybrook.examples.demo:brook -rg \n# Locust - load testing\nlocust -H http://localhost:8000\n```\n\n## Contributing\n\nPyBrook uses [poetry](https://python-poetry.org) for dependency management.\nTo install all its development dependencies, simply run this command:\n\n```bash\npoetry install\n```\n\n### Tests\n\n```bash\nmake test\n```\n\n### Code quality\n\nThe source code of PyBrook is formatted using yapf and isort.  \nTo run them with the correct settings, use the following command:\n\n```bash\nmake format\n```\n\nPyBrook uses `mypy` for type checking and `flake8` for linting.\nUse the following command to run them with the appropriate settings:\n\n```bash\nmake lint\n```',
     'author': 'Michał Rokita',
     'author_email': 'mrokita@mrokita.pl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pybrook/pybrook',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pybrook-0.1.5/PKG-INFO` & `pybrook-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: pybrook
-Version: 0.1.5
+Version: 0.1.6
 Summary: PyBrook - a real-time cloud computing framework for the Internet of Things.
 Home-page: https://github.com/pybrook/pybrook
 License: GPL-3.0-or-later
 Author: Michał Rokita
 Author-email: mrokita@mrokita.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fastapi (>=0.87.0,<0.88.0)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: gunicorn (>=20.1.0,<21.0.0)
-Requires-Dist: httpx (>=0.21.1,<0.22.0)
 Requires-Dist: locust (>=2.6.1,<3.0.0)
-Requires-Dist: loguru (>=0.5.3,<0.6.0)
-Requires-Dist: orjson (>=3.6.5,<4.0.0)
-Requires-Dist: pydantic (>=1.10.6,<2.0.0)
-Requires-Dist: pytest (>=6.2.5,<7.0.0)
-Requires-Dist: redis[asyncio] (>=4.5.1,<5.0.0)
-Requires-Dist: uvicorn[standard] (>=0.20.0,<0.21.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: orjson (>=3.8.7,<4.0.0)
+Requires-Dist: pydantic (>=1.10.8,<2.0.0)
+Requires-Dist: redis[asyncio] (>=4.5.5,<5.0.0)
+Requires-Dist: uvicorn[standard] (>=0.22.0,<0.23.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
-Requires-Dist: watchdog (>=2.1.6,<3.0.0)
+Requires-Dist: watchdog (>=3.0.0,<4.0.0)
 Project-URL: Repository, https://github.com/pybrook/pybrook
 Description-Content-Type: text/markdown
 
+[![PyPI](https://img.shields.io/pypi/v/pybrook?style=for-the-badge&color=purple)](https://pypi.org/project/pybrook/)
+[![docs](https://img.shields.io/badge/docs-mkdocs+mkdocstrings-lightblue?style=for-the-badge)](https://pybrook.github.io/pybrook/)
+![Python](https://img.shields.io/badge/python-3.7%2B-blue?style=for-the-badge)
+![Coverage](https://img.shields.io/badge/coverage-81%25-green?style=for-the-badge)
+
 # Introduction
 
 PyBrook - a real-time cloud computing framework for the Internet of Things.
 PyBrook enables users to define complex data processing models declaratively using the Python programming language.
 The framework also provides a generic web interface that presents the collected data in real-time.
 
 PyBrook aims to make the development of real-time data processing services as easy as possible by utilising powerful 
@@ -184,15 +187,15 @@
     image: pybrook:latest
     depends_on:
       - api
     ports:
       - 8089:8089
     command: locust -H http://api:8000
   redis:
-    image: redislabs/redisgears:latest
+    image: redislabs/redisgears:1.0.9
 ```
 
 Then run `docker-compose up --build` again, to start PyBrook - this time using your own model.
 
 ## Setup & Development
 
 You can install the PyBrook from PyPi using `pip`:
@@ -203,19 +206,19 @@
 
 ## Running all services manually, without Docker
 
 To run the `pybrook.examples.demo` model, you have to start all the required services manually:
 
 ```bash
 # Redis + Redis Gears
-docker run --net=host -d redislabs/redisgears
+docker run --net=host -d redislabs/redisgears:1.0.9
 # HTTP API based on pybrook.examples.demo - uvicorn
 uvicorn pybrook.examples.demo:app --reload  
 # PyBrook workers based on pybrook.examples.demo 
-pybrook pybrook.examples.demo:brook   
+pybrook pybrook.examples.demo:brook -rg 
 # Locust - load testing
 locust -H http://localhost:8000
 ```
 
 ## Contributing
 
 PyBrook uses [poetry](https://python-poetry.org) for dependency management.
```

