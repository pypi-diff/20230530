# Comparing `tmp/script_master-0.0.4.tar.gz` & `tmp/script_master-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "script_master-0.0.4.tar", max compression
+gzip compressed data, was "script_master-0.0.5.tar", max compression
```

## Comparing `script_master-0.0.4.tar` & `script_master-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0        0 2023-01-28 19:14:36.139208 script_master-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0    11507 2021-11-04 18:19:00.076000 script_master-0.0.4/LICENSE
--rw-r--r--   0        0        0     1111 2023-01-29 07:20:22.739591 script_master-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1061 2023-01-28 19:44:47.819376 script_master-0.0.4/README.md
--rw-r--r--   0        0        0       23 2023-01-29 07:20:22.728580 script_master-0.0.4/script_master/__init__.py
--rw-r--r--   0        0        0     2053 2023-01-28 19:26:17.553511 script_master-0.0.4/script_master/cli.py
--rw-r--r--   0        0        0      898 2023-01-28 19:44:47.819376 script_master-0.0.4/script_master/const.py
--rw-r--r--   0        0        0     4659 2023-01-28 09:59:41.379599 script_master-0.0.4/script_master/files.py
--rw-r--r--   0        0        0     1347 2023-01-28 10:10:21.388834 script_master-0.0.4/script_master/logger.py
--rw-r--r--   0        0        0       72 2023-01-28 10:57:27.246502 script_master-0.0.4/script_master/main.py
--rw-r--r--   0        0        0     5041 2023-01-28 18:40:20.128131 script_master-0.0.4/script_master/notebook/__init__.py
--rw-r--r--   0        0        0     6914 2023-01-28 09:59:41.410845 script_master-0.0.4/script_master/notebook/schemas.py
--rw-r--r--   0        0        0       92 2023-01-28 09:59:41.277798 script_master-0.0.4/script_master/notebook/service.py
--rw-r--r--   0        0        0     1530 2023-01-28 18:40:20.128131 script_master-0.0.4/script_master/notebook/tags.py
--rw-r--r--   0        0        0      630 2023-01-06 11:29:51.719393 script_master-0.0.4/script_master/resources.py
--rw-r--r--   0        0        0     4709 2023-01-28 18:40:20.143796 script_master-0.0.4/script_master/service.py
--rw-r--r--   0        0        0     2552 2023-01-28 10:52:16.736806 script_master-0.0.4/script_master/settings.py
--rw-r--r--   0        0        0     1145 2023-01-28 19:47:42.518113 script_master-0.0.4/script_master/template-settings.env
--rw-r--r--   0        0        0     1734 2023-01-28 09:59:41.348353 script_master-0.0.4/script_master/template.py
--rw-r--r--   0        0        0     2214 1970-01-01 00:00:00.000000 script_master-0.0.4/setup.py
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 script_master-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-01-28 19:14:36.139208 script_master-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0    11507 2021-11-04 18:19:00.076000 script_master-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1113 2023-05-30 15:45:43.454238 script_master-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1588 2023-05-30 15:44:17.764445 script_master-0.0.5/README.md
+-rw-r--r--   0        0        0       23 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/__init__.py
+-rw-r--r--   0        0        0     1360 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/cli.py
+-rw-r--r--   0        0        0     1144 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/const.py
+-rw-r--r--   0        0        0     4659 2023-05-30 15:32:09.002593 script_master-0.0.5/script_master/files.py
+-rw-r--r--   0        0        0     1347 2023-05-30 15:13:11.155039 script_master-0.0.5/script_master/logger.py
+-rw-r--r--   0        0        0     1319 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/main.py
+-rw-r--r--   0        0        0     5041 2023-05-30 15:32:18.324501 script_master-0.0.5/script_master/notebook/__init__.py
+-rw-r--r--   0        0        0     6914 2023-05-30 15:32:42.254774 script_master-0.0.5/script_master/notebook/schemas.py
+-rw-r--r--   0        0        0       92 2023-01-28 09:59:41.277798 script_master-0.0.5/script_master/notebook/service.py
+-rw-r--r--   0        0        0     1530 2023-01-28 18:40:20.128131 script_master-0.0.5/script_master/notebook/tags.py
+-rw-r--r--   0        0        0      463 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/resources.py
+-rw-r--r--   0        0        0     4709 2023-05-30 15:14:58.693832 script_master-0.0.5/script_master/service.py
+-rw-r--r--   0        0        0     2965 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/settings.py
+-rw-r--r--   0        0        0      958 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/template-settings.env
+-rw-r--r--   0        0        0     1734 2023-01-28 09:59:41.348353 script_master-0.0.5/script_master/template.py
+-rw-r--r--   0        0        0      142 2023-05-30 15:44:17.780068 script_master-0.0.5/script_master/utils.py
+-rw-r--r--   0        0        0     2725 1970-01-01 00:00:00.000000 script_master-0.0.5/setup.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 script_master-0.0.5/PKG-INFO
```

### Comparing `script_master-0.0.4/LICENSE` & `script_master-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/pyproject.toml` & `script_master-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "script-master"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Pavel Maksimov <vur21@ya.ru>"]
 license = "Apache-2.0"
 homepage = "https://github.com/pavelmaksimov/script-master"
 packages = [{include = "script_master"}]
 readme = "README.md"
 include = [
@@ -15,15 +15,15 @@
 keywords = []
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pendulum = "^2.1.2"
 PyYAML = "^6.0"
 pydantic = "^1.9.0"
-fastapi = "^0.88"
+fastapi = "^0.95.2"
 uvicorn = {extras = ["standart"], version = "^0.20.0"}
 aiopath = "^0.6.11"
 asyncio = "^3.4.3"
 better-exceptions = "^0.3.3"
 confz = "1.8.1"
 orjson = "^3.8.4"
 typer = "^0.7.0"
```

### Comparing `script_master-0.0.4/README.md` & `script_master-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-# Script-Master
-
-Сервис, который по конфигам (формат YAML), 
-создает задания запуска скриптов в сервисе [Process-Executor](https://github.com/pavelmaksimov/process-executor),
-согласно плану запусков полученных от сервиса [Work-Planner](https://github.com/pavelmaksimov/work-planner).
-
-## Install
-    poetry add script-master
-
-or
-
-    pip install script-master
-
-## Run
-    script-master --help
-    script-master init # Создаст конфиг в текущий директории
-    script-master run # Пользоваться командой, запускать всегда в директории, в которой выполнен init
-
-## Интерфейс
-Есть [интерфейс](https://github.com/pavelmaksimov/script-master-helper), он не обязателен. Для сервиса требуются только конфиги yaml, их иожно вручную создавать
+# Script-Master
+
+Сервис, который по конфигам (формат YAML), 
+создает задания запуска скриптов в сервисе [Process-Executor](https://github.com/pavelmaksimov/process-executor),
+согласно плану запусков полученных от сервиса [Work-Planner](https://github.com/pavelmaksimov/work-planner).
+
+Отлично подходит для запуска ETL скриптов по расписанию.
+
+Требует мало ресурсов, не требует БД, конфигурации скриптов 
+и их параметры запуска (расписание) создаются в YAML конфигах, 
+поэтому интерфейс не требуется, но он есть, дополнительно можно поставить.
+
+
+## Install
+    poetry add script-master
+
+or
+
+    pip install script-master
+
+## Run
+    script-master --help
+    script-master init # Создаст конфиг в текущий директории
+    script-master run # Запускать всегда в директории, в которой был выполнен init
+
+or 
+    
+    uvicorn script_master.main:app --port 8080 --reload
+
+
+## Интерфейс
+Есть [интерфейс](https://github.com/pavelmaksimov/script-master-helper), он не обязателен. Для сервиса требуются только конфиги yaml, их иожно вручную создавать
 Запускается отдельно/
```

### Comparing `script_master-0.0.4/script_master/files.py` & `script_master-0.0.5/script_master/files.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/logger.py` & `script_master-0.0.5/script_master/logger.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/notebook/__init__.py` & `script_master-0.0.5/script_master/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/notebook/schemas.py` & `script_master-0.0.5/script_master/notebook/schemas.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/notebook/tags.py` & `script_master-0.0.5/script_master/notebook/tags.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/service.py` & `script_master-0.0.5/script_master/service.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/script_master/template.py` & `script_master-0.0.5/script_master/template.py`

 * *Files identical despite different names*

### Comparing `script_master-0.0.4/setup.py` & `script_master-0.0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'aiopath>=0.6.11,<0.7.0',
  'asyncio>=3.4.3,<4.0.0',
  'better-exceptions>=0.3.3,<0.4.0',
  'confz==1.8.1',
- 'fastapi>=0.88,<0.89',
+ 'fastapi>=0.95.2,<0.96.0',
  'jinja2>=3.1.2,<4.0.0',
  'loguru>=0.6.0,<0.7.0',
  'orjson>=3.8.4,<4.0.0',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.9.0,<2.0.0',
  'script-master-helper>=0.0.2,<0.0.3',
  'typer>=0.7.0,<0.8.0',
  'uvicorn[standart]>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['script-master = script_master.cli:cli']}
 
 setup_kwargs = {
     'name': 'script-master',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': '',
-    'long_description': '# Script-Master\n\nСервис, который по конфигам (формат YAML), \nсоздает задания запуска скриптов в сервисе [Process-Executor](https://github.com/pavelmaksimov/process-executor),\nсогласно плану запусков полученных от сервиса [Work-Planner](https://github.com/pavelmaksimov/work-planner).\n\n## Install\n    poetry add script-master\n\nor\n\n    pip install script-master\n\n## Run\n    script-master --help\n    script-master init # Создаст конфиг в текущий директории\n    script-master run # Пользоваться командой, запускать всегда в директории, в которой выполнен init\n\n## Интерфейс\nЕсть [интерфейс](https://github.com/pavelmaksimov/script-master-helper), он не обязателен. Для сервиса требуются только конфиги yaml, их иожно вручную создавать\nЗапускается отдельно/',
+    'long_description': '# Script-Master\n\nСервис, который по конфигам (формат YAML), \nсоздает задания запуска скриптов в сервисе [Process-Executor](https://github.com/pavelmaksimov/process-executor),\nсогласно плану запусков полученных от сервиса [Work-Planner](https://github.com/pavelmaksimov/work-planner).\n\nОтлично подходит для запуска ETL скриптов по расписанию.\n\nТребует мало ресурсов, не требует БД, конфигурации скриптов \nи их параметры запуска (расписание) создаются в YAML конфигах, \nпоэтому интерфейс не требуется, но он есть, дополнительно можно поставить.\n\n\n## Install\n    poetry add script-master\n\nor\n\n    pip install script-master\n\n## Run\n    script-master --help\n    script-master init # Создаст конфиг в текущий директории\n    script-master run # Запускать всегда в директории, в которой был выполнен init\n\nor \n    \n    uvicorn script_master.main:app --port 8080 --reload\n\n\n## Интерфейс\nЕсть [интерфейс](https://github.com/pavelmaksimov/script-master-helper), он не обязателен. Для сервиса требуются только конфиги yaml, их иожно вручную создавать\nЗапускается отдельно/',
     'author': 'Pavel Maksimov',
     'author_email': 'vur21@ya.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pavelmaksimov/script-master',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `script_master-0.0.4/PKG-INFO` & `script_master-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: script-master
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Home-page: https://github.com/pavelmaksimov/script-master
 License: Apache-2.0
 Author: Pavel Maksimov
 Author-email: vur21@ya.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: aiopath (>=0.6.11,<0.7.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: better-exceptions (>=0.3.3,<0.4.0)
 Requires-Dist: confz (==1.8.1)
-Requires-Dist: fastapi (>=0.88,<0.89)
+Requires-Dist: fastapi (>=0.95.2,<0.96.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: orjson (>=3.8.4,<4.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: script-master-helper (>=0.0.2,<0.0.3)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
@@ -29,22 +29,34 @@
 
 # Script-Master
 
 Сервис, который по конфигам (формат YAML), 
 создает задания запуска скриптов в сервисе [Process-Executor](https://github.com/pavelmaksimov/process-executor),
 согласно плану запусков полученных от сервиса [Work-Planner](https://github.com/pavelmaksimov/work-planner).
 
+Отлично подходит для запуска ETL скриптов по расписанию.
+
+Требует мало ресурсов, не требует БД, конфигурации скриптов 
+и их параметры запуска (расписание) создаются в YAML конфигах, 
+поэтому интерфейс не требуется, но он есть, дополнительно можно поставить.
+
+
 ## Install
     poetry add script-master
 
 or
 
     pip install script-master
 
 ## Run
     script-master --help
     script-master init # Создаст конфиг в текущий директории
-    script-master run # Пользоваться командой, запускать всегда в директории, в которой выполнен init
+    script-master run # Запускать всегда в директории, в которой был выполнен init
+
+or 
+    
+    uvicorn script_master.main:app --port 8080 --reload
+
 
 ## Интерфейс
 Есть [интерфейс](https://github.com/pavelmaksimov/script-master-helper), он не обязателен. Для сервиса требуются только конфиги yaml, их иожно вручную создавать
 Запускается отдельно/
```

