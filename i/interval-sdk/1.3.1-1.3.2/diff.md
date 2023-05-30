# Comparing `tmp/interval_sdk-1.3.1.tar.gz` & `tmp/interval_sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interval_sdk-1.3.1.tar", max compression
+gzip compressed data, was "interval_sdk-1.3.2.tar", max compression
```

## Comparing `interval_sdk-1.3.1.tar` & `interval_sdk-1.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     5078 2023-05-03 04:58:51.508173 interval_sdk-1.3.1/README.md
--rw-r--r--   0        0        0     1890 2023-05-30 12:58:52.179247 interval_sdk-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      331 2023-02-23 20:46:46.791505 interval_sdk-1.3.1/src/interval_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-01-18 22:41:09.625763 interval_sdk-1.3.1/src/interval_sdk/classes/__init__.py
--rw-r--r--   0        0        0      422 2023-01-18 22:41:09.625846 interval_sdk-1.3.1/src/interval_sdk/classes/action.py
--rw-r--r--   0        0        0     7151 2023-05-03 04:58:51.508556 interval_sdk-1.3.1/src/interval_sdk/classes/component.py
--rw-r--r--   0        0        0      931 2023-01-18 22:41:09.626005 interval_sdk-1.3.1/src/interval_sdk/classes/interval_file.py
--rw-r--r--   0        0        0    60224 2023-05-03 04:58:51.508764 interval_sdk-1.3.1/src/interval_sdk/classes/io.py
--rw-r--r--   0        0        0     8181 2023-05-30 12:34:33.787095 interval_sdk-1.3.1/src/interval_sdk/classes/io_client.py
--rw-r--r--   0        0        0      348 2023-01-18 22:41:09.626352 interval_sdk-1.3.1/src/interval_sdk/classes/io_error.py
--rw-r--r--   0        0        0    35098 2023-04-11 21:37:50.892013 interval_sdk-1.3.1/src/interval_sdk/classes/io_promise.py
--rw-r--r--   0        0        0     8059 2023-05-22 21:47:27.580443 interval_sdk-1.3.1/src/interval_sdk/classes/isocket.py
--rw-r--r--   0        0        0     1162 2023-05-03 04:58:51.509073 interval_sdk-1.3.1/src/interval_sdk/classes/layout.py
--rw-r--r--   0        0        0     3458 2023-01-21 01:17:31.463445 interval_sdk-1.3.1/src/interval_sdk/classes/logger.py
--rw-r--r--   0        0        0     2993 2023-01-18 22:41:09.626826 interval_sdk-1.3.1/src/interval_sdk/classes/page.py
--rw-r--r--   0        0        0     6155 2023-05-03 04:58:51.509176 interval_sdk-1.3.1/src/interval_sdk/classes/rpc.py
--rw-r--r--   0        0        0     2968 2023-04-04 21:38:44.984597 interval_sdk-1.3.1/src/interval_sdk/classes/transaction_loading_state.py
--rw-r--r--   0        0        0        0 2023-01-18 22:41:09.626993 interval_sdk-1.3.1/src/interval_sdk/components/__init__.py
--rw-r--r--   0        0        0     1704 2023-01-21 01:17:31.463657 interval_sdk-1.3.1/src/interval_sdk/components/grid.py
--rw-r--r--   0        0        0     6173 2023-05-03 04:58:51.509423 interval_sdk-1.3.1/src/interval_sdk/components/table.py
--rw-r--r--   0        0        0      810 2023-05-03 04:58:51.509517 interval_sdk-1.3.1/src/interval_sdk/handlers.py
--rw-r--r--   0        0        0    15318 2023-05-03 04:58:51.509645 interval_sdk-1.3.1/src/interval_sdk/internal_rpc_schema.py
--rw-r--r--   0        0        0    25838 2023-05-03 04:58:51.509791 interval_sdk-1.3.1/src/interval_sdk/io_schema.py
--rw-r--r--   0        0        0    65981 2023-05-30 12:29:17.877113 interval_sdk-1.3.1/src/interval_sdk/main.py
--rw-r--r--   0        0        0       41 2023-02-23 20:46:46.792747 interval_sdk-1.3.1/src/interval_sdk/superjson/__init__.py
--rw-r--r--   0        0        0     1081 2023-02-23 20:46:46.792808 interval_sdk-1.3.1/src/interval_sdk/superjson/main.py
--rw-r--r--   0        0        0     3810 2023-02-23 20:46:46.792871 interval_sdk-1.3.1/src/interval_sdk/superjson/plainer.py
--rw-r--r--   0        0        0        0 2023-02-23 20:46:46.792939 interval_sdk-1.3.1/src/interval_sdk/superjson/tests/__init__.py
--rw-r--r--   0        0        0      188 2023-02-23 20:46:46.793011 interval_sdk-1.3.1/src/interval_sdk/superjson/tests/node-only-types.js
--rw-r--r--   0        0        0      416 2023-02-23 20:46:46.793099 interval_sdk-1.3.1/src/interval_sdk/superjson/tests/round-trip-superjson.js
--rw-r--r--   0        0        0     3385 2023-02-23 20:46:46.793202 interval_sdk-1.3.1/src/interval_sdk/superjson/tests/test_superjson.py
--rw-r--r--   0        0        0     5935 2023-05-03 04:58:51.510227 interval_sdk-1.3.1/src/interval_sdk/superjson/transformer.py
--rw-r--r--   0        0        0     4550 2023-04-11 21:37:50.894844 interval_sdk-1.3.1/src/interval_sdk/types.py
--rw-r--r--   0        0        0     7342 2023-05-03 04:58:51.510323 interval_sdk-1.3.1/src/interval_sdk/util.py
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.3.1/setup.py
--rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     5078 2023-05-03 04:58:51.508173 interval_sdk-1.3.2/README.md
+-rw-r--r--   0        0        0     1890 2023-05-30 15:06:52.173903 interval_sdk-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-02-23 20:46:46.791505 interval_sdk-1.3.2/src/interval_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-18 22:41:09.625763 interval_sdk-1.3.2/src/interval_sdk/classes/__init__.py
+-rw-r--r--   0        0        0      422 2023-01-18 22:41:09.625846 interval_sdk-1.3.2/src/interval_sdk/classes/action.py
+-rw-r--r--   0        0        0     7151 2023-05-30 15:03:10.487013 interval_sdk-1.3.2/src/interval_sdk/classes/component.py
+-rw-r--r--   0        0        0      931 2023-01-18 22:41:09.626005 interval_sdk-1.3.2/src/interval_sdk/classes/interval_file.py
+-rw-r--r--   0        0        0    60224 2023-05-30 15:03:10.487590 interval_sdk-1.3.2/src/interval_sdk/classes/io.py
+-rw-r--r--   0        0        0     8181 2023-05-30 15:03:10.488044 interval_sdk-1.3.2/src/interval_sdk/classes/io_client.py
+-rw-r--r--   0        0        0      348 2023-05-30 15:03:10.488344 interval_sdk-1.3.2/src/interval_sdk/classes/io_error.py
+-rw-r--r--   0        0        0    35098 2023-04-11 21:37:50.892013 interval_sdk-1.3.2/src/interval_sdk/classes/io_promise.py
+-rw-r--r--   0        0        0     8059 2023-05-22 21:47:27.580443 interval_sdk-1.3.2/src/interval_sdk/classes/isocket.py
+-rw-r--r--   0        0        0     1162 2023-05-03 04:58:51.509073 interval_sdk-1.3.2/src/interval_sdk/classes/layout.py
+-rw-r--r--   0        0        0     3458 2023-05-30 15:03:10.488658 interval_sdk-1.3.2/src/interval_sdk/classes/logger.py
+-rw-r--r--   0        0        0     2993 2023-01-18 22:41:09.626826 interval_sdk-1.3.2/src/interval_sdk/classes/page.py
+-rw-r--r--   0        0        0     6155 2023-05-03 04:58:51.509176 interval_sdk-1.3.2/src/interval_sdk/classes/rpc.py
+-rw-r--r--   0        0        0     2968 2023-04-04 21:38:44.984597 interval_sdk-1.3.2/src/interval_sdk/classes/transaction_loading_state.py
+-rw-r--r--   0        0        0        0 2023-01-18 22:41:09.626993 interval_sdk-1.3.2/src/interval_sdk/components/__init__.py
+-rw-r--r--   0        0        0     1704 2023-01-21 01:17:31.463657 interval_sdk-1.3.2/src/interval_sdk/components/grid.py
+-rw-r--r--   0        0        0     6173 2023-05-03 04:58:51.509423 interval_sdk-1.3.2/src/interval_sdk/components/table.py
+-rw-r--r--   0        0        0      810 2023-05-03 04:58:51.509517 interval_sdk-1.3.2/src/interval_sdk/handlers.py
+-rw-r--r--   0        0        0    15318 2023-05-30 15:03:10.488832 interval_sdk-1.3.2/src/interval_sdk/internal_rpc_schema.py
+-rw-r--r--   0        0        0    25824 2023-05-30 15:05:10.040507 interval_sdk-1.3.2/src/interval_sdk/io_schema.py
+-rw-r--r--   0        0        0    65981 2023-05-30 15:03:10.489506 interval_sdk-1.3.2/src/interval_sdk/main.py
+-rw-r--r--   0        0        0       41 2023-02-23 20:46:46.792747 interval_sdk-1.3.2/src/interval_sdk/superjson/__init__.py
+-rw-r--r--   0        0        0     1081 2023-02-23 20:46:46.792808 interval_sdk-1.3.2/src/interval_sdk/superjson/main.py
+-rw-r--r--   0        0        0     3810 2023-02-23 20:46:46.792871 interval_sdk-1.3.2/src/interval_sdk/superjson/plainer.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:46:46.792939 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/__init__.py
+-rw-r--r--   0        0        0      188 2023-02-23 20:46:46.793011 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/node-only-types.js
+-rw-r--r--   0        0        0      416 2023-02-23 20:46:46.793099 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/round-trip-superjson.js
+-rw-r--r--   0        0        0     3385 2023-02-23 20:46:46.793202 interval_sdk-1.3.2/src/interval_sdk/superjson/tests/test_superjson.py
+-rw-r--r--   0        0        0     5935 2023-05-03 04:58:51.510227 interval_sdk-1.3.2/src/interval_sdk/superjson/transformer.py
+-rw-r--r--   0        0        0     4550 2023-04-11 21:37:50.894844 interval_sdk-1.3.2/src/interval_sdk/types.py
+-rw-r--r--   0        0        0     7342 2023-05-03 04:58:51.510323 interval_sdk-1.3.2/src/interval_sdk/util.py
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 interval_sdk-1.3.2/setup.py
+-rw-r--r--   0        0        0     6161 1970-01-01 00:00:00.000000 interval_sdk-1.3.2/PKG-INFO
```

### Comparing `interval_sdk-1.3.1/README.md` & `interval_sdk-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/pyproject.toml` & `interval_sdk-1.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "interval-sdk"
-version = "1.3.1"
+version = "1.3.2"
 description = "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more."
 authors = [
 	"Jacob Mischka <jacob@interval.com>",
 	"Ryan Coppolo <ryan@interval.com>",
 ]
 maintainers = [
 	"Jacob Mischka <jacob@interval.com>",
```

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/component.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/component.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/interval_file.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/interval_file.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/io.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/io.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/io_client.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/io_client.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/io_promise.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/io_promise.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/isocket.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/isocket.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/layout.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/layout.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/logger.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/logger.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/page.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/page.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/rpc.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/rpc.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/classes/transaction_loading_state.py` & `interval_sdk-1.3.2/src/interval_sdk/classes/transaction_loading_state.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/components/grid.py` & `interval_sdk-1.3.2/src/interval_sdk/components/grid.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/components/table.py` & `interval_sdk-1.3.2/src/interval_sdk/components/table.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/handlers.py` & `interval_sdk-1.3.2/src/interval_sdk/handlers.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/internal_rpc_schema.py` & `interval_sdk-1.3.2/src/interval_sdk/internal_rpc_schema.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/io_schema.py` & `interval_sdk-1.3.2/src/interval_sdk/io_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,15 +860,15 @@
         props=SelectMultipleProps,
         state=None,
         returns=list[LabelValueModel],
     ),
     "SEARCH": MethodDef(
         props=SearchProps,
         state=SearchState,
-        returns=SearchResultValue,
+        returns=str,
         supports_multiple=True,
     ),
     "UPLOAD_FILE": MethodDef(
         props=UploadFileProps,
         state=UploadFileState,
         returns=InnerFileModel,
     ),
```

### Comparing `interval_sdk-1.3.1/src/interval_sdk/main.py` & `interval_sdk-1.3.2/src/interval_sdk/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/superjson/main.py` & `interval_sdk-1.3.2/src/interval_sdk/superjson/main.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/superjson/plainer.py` & `interval_sdk-1.3.2/src/interval_sdk/superjson/plainer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/superjson/tests/test_superjson.py` & `interval_sdk-1.3.2/src/interval_sdk/superjson/tests/test_superjson.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/superjson/transformer.py` & `interval_sdk-1.3.2/src/interval_sdk/superjson/transformer.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/types.py` & `interval_sdk-1.3.2/src/interval_sdk/types.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/src/interval_sdk/util.py` & `interval_sdk-1.3.2/src/interval_sdk/util.py`

 * *Files identical despite different names*

### Comparing `interval_sdk-1.3.1/setup.py` & `interval_sdk-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ['aiohttp>=3.8.1,<4.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'typing-extensions>=4.4.0,<5.0.0',
  'websockets>=10.1,<11.0']
 
 setup_kwargs = {
     'name': 'interval-sdk',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': "The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.",
     'long_description': '<a href="https://interval.com">\n  <img alt="Interval" width="100" height="100" style="border-radius: 6px;" src="https://interval.com/img/readme-assets/interval-avatar.png">\n</a>\n\n# Interval Python SDK\n\n[![pypi version](https://img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/twitter/follow/useinterval.svg?color=%2338A1F3&label=twitter&style=flat)](https://twitter.com/useinterval) [![Discord](https://img.shields.io/badge/discord-join-blueviolet)](https://interval.com/discord)\n\n[Interval](https://interval.com) lets you quickly build internal web apps (think: customer support tools, admin panels, etc.) just by writing backend Python code.\n\nThis is our Python SDK which connects to the interval.com web app. If you don\'t have an Interval account, you can [create one here](https://interval.com/signup). All core features are free to use.\n\n## Why choose Interval?\n\n_"Python code > no-code"_\n\nInterval is an alternative to no-code/low-code UI builders. Modern frontend development is inherently complicated, and teams rightfully want to spend minimal engineering resources on internal dashboards. No-code tools attempt to solve this problem by allowing you to build UIs in a web browser without writing any frontend code.\n\nWe don\'t think this is the right solution. **Building UIs for mission-critical tools in your web browser** — often by non-technical teammates, outside of your codebase, without versioning or code review — **is an anti-pattern.** Apps built in this manner are brittle and break in unexpected ways.\n\nWith Interval, **all of the code for generating your web UIs lives within your app\'s codebase.** Tools built with Interval (we call these [actions](https://interval.com/docs/concepts/actions)) are just asynchronous functions that run in your backend. Because these are plain old functions, you can access the complete power of your Python app. You can loop, conditionally branch, access shared functions, and so on. When you need to request input or display output, `await` any of our [I/O methods](https://interval.com/docs/io-methods/) to present a form to the user and your script will pause execution until input is received.\n\nHere\'s a simple app with a single "Hello, world" action:\n\n```python\nfrom interval_sdk import Interval, IO\n\n# Initialize Interval\ninterval = Interval(api_key="<YOUR API KEY>")\n\n@interval.action\nasync def hello_world(io: IO):\n    name = await io.input.text("Your name")\n    return f"Hello, {name}"\n\n\n# Synchronously listen, blocking forever\ninterval.listen()\n```\n\nTo not block, interval can also be run asynchronously using\n`interval.listen_async()`. You must provide your own event loop.\n\nThe task will complete as soon as connection to Interval completes, so you\nlikely want to run forever or run alongside another permanent task.\n\n```python\nimport asyncio, signal\n\nloop = asyncio.get_event_loop()\ntask = loop.create_task(interval.listen_async())\ndef handle_done(task: asyncio.Task[None]):\n    try:\n        task.result()\n    except:\n        loop.stop()\n\ntask.add_done_callback(handle_done)\nfor sig in {signal.SIGINT, signal.SIGTERM}:\n    loop.add_signal_handler(sig, loop.stop)\nloop.run_forever()\n```\n\nInterval:\n\n- Makes creating full-stack apps as easy as writing CLI scripts.\n- Can scale from a handful of scripts to robust multi-user dashboards.\n- Lets you build faster than no-code, without leaving your codebase & IDE.\n\nWith Interval, you do not need to:\n\n- Write REST or GraphQL API endpoints to connect internal functionality to no-code tools.\n- Give Interval write access to your database (or give us _any_ of your credentials, for that matter).\n- Build web UIs with a drag-and-drop interface.\n\n## More about Interval\n\n- 📖 [Documentation](https://interval.com/docs)\n- 🌐 [Interval website](https://interval.com)\n- 💬 [Discord community](https://interval.com/discord)\n- 📰 [Product updates](https://interval.com/blog)\n\n## Contributing\n\nThis project uses [Poetry](https://python-poetry.org/) for dependency\nmanagement\n\n1. `poetry install` to install dependencies\n2. `poetry shell` to activate the virtual environment\n\nTasks are configured using [poethepoet](https://github.com/nat-n/poethepoet)\n(installed as a dev dependency).\n\n- `poe demo [demo_name]` to run a demo (`basic` by default if `demo_name` omitted)\n- `poe test` to run `pytest` (can also run `pytest` directly in virtual env)\n\nCode is formatted using [Black](https://github.com/psf/black). Please configure\nyour editor to format on save using Black, or run `poe format` to format the\ncode before committing changes.\n\n## Tests\n\n*Note:* Tests currently require a local instance of the Interval backend.\n\nTests use [pytest](https://docs.pytest.org/en/7.1.x/) and\n[playwright](https://playwright.dev/python/).\n\nCurrently assumes the `test-runner@interval.com` user exists already.\nRun `yarn test` in the `web` directory at least once to create it before\nrunning these.\n',
     'author': 'Jacob Mischka',
     'author_email': 'jacob@interval.com',
     'maintainer': 'Jacob Mischka',
     'maintainer_email': 'jacob@interval.com',
     'url': 'https://interval.com',
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['interval_sdk', 'interval_sdk.classes',
 'interval_sdk.components', 'interval_sdk.superjson',
 'interval_sdk.superjson.tests'] package_data = \ {'': ['*']} install_requires =
 \ ['aiohttp>=3.8.1,<4.0.0', 'pydantic>=1.9.0,<2.0.0', 'typing-
 extensions>=4.4.0,<5.0.0', 'websockets>=10.1,<11.0'] setup_kwargs = { 'name':
-'interval-sdk', 'version': '1.3.1', 'description': "The frontendless framework
+'interval-sdk', 'version': '1.3.2', 'description': "The frontendless framework
 for high growth companies. Interval automatically generates apps by inlining
 the UI in your backend code. It's a faster and more maintainable way to build
 internal tools, rapid prototypes, and more.", 'long_description': '\n_
 [Interval]\n\n\n# Interval Python SDK\n\n[![pypi version](https://
 img.shields.io/pypi/v/interval-sdk?style=flat)](https://pypi.org/project/
 interval-sdk) [![Documentation](https://img.shields.io/badge/documentation-
 informational)](https://interval.com/docs) [![Twitter](https://img.shields.io/
```

### Comparing `interval_sdk-1.3.1/PKG-INFO` & `interval_sdk-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interval-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: The frontendless framework for high growth companies. Interval automatically generates apps by inlining the UI in your backend code. It's a faster and more maintainable way to build internal tools, rapid prototypes, and more.
 Home-page: https://interval.com
 Keywords: internal tool,app,ui,ui builder
 Author: Jacob Mischka
 Author-email: jacob@interval.com
 Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: interval-sdk Version: 1.3.1 Summary: The
+Metadata-Version: 2.1 Name: interval-sdk Version: 1.3.2 Summary: The
 frontendless framework for high growth companies. Interval automatically
 generates apps by inlining the UI in your backend code. It's a faster and more
 maintainable way to build internal tools, rapid prototypes, and more. Home-
 page: https://interval.com Keywords: internal tool,app,ui,ui builder Author:
 Jacob Mischka Author-email: jacob@interval.com Maintainer: Jacob Mischka
 Maintainer-email: jacob@interval.com Requires-Python: >=3.9,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

