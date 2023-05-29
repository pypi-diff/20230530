# Comparing `tmp/shared-0.0.8.tar.gz` & `tmp/shared-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shared-0.0.8.tar", last modified: Tue Nov 16 20:30:28 2021, max compression
+gzip compressed data, was "dist/shared-0.0.9.tar", last modified: Tue Jan 18 22:03:47 2022, max compression
```

## Comparing `shared-0.0.8.tar` & `shared-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,23 @@
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.119935 shared-0.0.8/
--rw-r-----   0 alex      (1002) alex      (1003)     1075 2021-02-02 12:38:23.000000 shared-0.0.8/LICENSE
--rw-rw-r--   0 alex      (1002) alex      (1003)       69 2021-05-28 16:59:21.000000 shared-0.0.8/MANIFEST.in
--rw-rw-r--   0 alex      (1002) alex      (1003)     9444 2021-11-16 20:30:28.119935 shared-0.0.8/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)     8801 2021-09-17 05:59:13.000000 shared-0.0.8/README.md
--rw-rw-r--   0 alex      (1002) alex      (1003)        5 2021-11-16 19:12:50.000000 shared-0.0.8/VERSION
--rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-02-14 09:34:02.000000 shared-0.0.8/pyproject.toml
--rw-rw-r--   0 alex      (1002) alex      (1003)      855 2021-11-16 20:30:28.123935 shared-0.0.8/setup.cfg
--rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-02-14 09:31:37.000000 shared-0.0.8/setup.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:27.999935 shared-0.0.8/shared/
--rw-rw-r--   0 alex      (1002) alex      (1003)    11882 2021-09-17 06:04:22.000000 shared-0.0.8/shared/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)     5856 2021-09-01 21:02:27.000000 shared-0.0.8/shared/__main__.py
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:27.979935 shared-0.0.8/shared/pyrustic_data/
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:27.979935 shared-0.0.8/shared/pyrustic_data/backstage/
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.063935 shared-0.0.8/shared/pyrustic_data/backstage/config/
--rw-rw-r--   0 alex      (1002) alex      (1003)      109 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/backstage/config/build.json
--rw-rw-r--   0 alex      (1002) alex      (1003)       39 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/backstage/config/init.json
--rw-rw-r--   0 alex      (1002) alex      (1003)      133 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/backstage/config/release.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.063935 shared-0.0.8/shared/pyrustic_data/backstage/data/
--rw-rw-r--   0 alex      (1002) alex      (1003)      165 2021-11-16 19:12:46.000000 shared-0.0.8/shared/pyrustic_data/backstage/data/build_report.json
--rw-rw-r--   0 alex      (1002) alex      (1003)      422 2021-09-29 19:55:01.000000 shared-0.0.8/shared/pyrustic_data/backstage/data/github_release_form.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.095935 shared-0.0.8/shared/pyrustic_data/backstage/hooking/
--rw-rw-r--   0 alex      (1002) alex      (1003)       75 2021-11-16 19:12:35.000000 shared-0.0.8/shared/pyrustic_data/backstage/hooking/build.json
--rw-rw-r--   0 alex      (1002) alex      (1003)       39 2021-11-16 19:12:35.000000 shared-0.0.8/shared/pyrustic_data/backstage/hooking/init.json
--rw-rw-r--   0 alex      (1002) alex      (1003)        2 2021-11-16 19:12:35.000000 shared-0.0.8/shared/pyrustic_data/backstage/hooking/release.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.115935 shared-0.0.8/shared/pyrustic_data/backstage/report/
--rw-rw-r--   0 alex      (1002) alex      (1003)      320 2021-09-29 19:55:24.000000 shared-0.0.8/shared/pyrustic_data/backstage/report/build_report.json
--rw-rw-r--   0 alex      (1002) alex      (1003)        2 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/backstage/report/release_report.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.119935 shared-0.0.8/shared/pyrustic_data/hubstore/
--rw-rw-r--   0 alex      (1002) alex      (1003)       48 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/hubstore/img.json
--rw-rw-r--   0 alex      (1002) alex      (1003)        2 2021-09-01 19:30:28.000000 shared-0.0.8/shared/pyrustic_data/hubstore/promotion.json
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.039935 shared-0.0.8/shared.egg-info/
--rw-rw-r--   0 alex      (1002) alex      (1003)     9444 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1002) alex      (1003)      968 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       49 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/entry_points.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-05-31 21:57:25.000000 shared-0.0.8/shared.egg-info/not-zip-safe
--rw-rw-r--   0 alex      (1002) alex      (1003)        7 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/requires.txt
--rw-rw-r--   0 alex      (1002) alex      (1003)       13 2021-11-16 20:30:27.000000 shared-0.0.8/shared.egg-info/top_level.txt
-drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2021-11-16 20:30:28.119935 shared-0.0.8/tests/
--rw-r-----   0 alex      (1002) alex      (1003)        0 2020-05-31 07:38:19.000000 shared-0.0.8/tests/__init__.py
--rw-rw-r--   0 alex      (1002) alex      (1003)      365 2021-11-16 19:12:35.000000 shared-0.0.8/tests/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 22:03:47.047977 shared-0.0.9/
+-rw-r-----   0 alex      (1002) alex      (1003)     1082 2022-01-16 17:56:58.000000 shared-0.0.9/LICENSE
+-rw-rw-r--   0 alex      (1002) alex      (1003)       69 2021-05-28 16:59:21.000000 shared-0.0.9/MANIFEST.in
+-rw-rw-r--   0 alex      (1002) alex      (1003)    11697 2022-01-18 22:03:47.047977 shared-0.0.9/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)    11060 2022-01-17 18:51:23.000000 shared-0.0.9/README.md
+-rw-rw-r--   0 alex      (1002) alex      (1003)        5 2021-11-16 20:30:30.000000 shared-0.0.9/VERSION
+-rw-rw-r--   0 alex      (1002) alex      (1003)      100 2021-02-14 09:34:02.000000 shared-0.0.9/pyproject.toml
+-rw-rw-r--   0 alex      (1002) alex      (1003)      849 2022-01-18 22:03:47.051977 shared-0.0.9/setup.cfg
+-rw-rw-r--   0 alex      (1002) alex      (1003)       70 2021-02-14 09:31:37.000000 shared-0.0.9/setup.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 22:03:47.003977 shared-0.0.9/shared/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    14038 2021-12-28 12:10:13.000000 shared-0.0.9/shared/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)     5885 2021-12-28 11:26:45.000000 shared-0.0.9/shared/__main__.py
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 22:03:47.039977 shared-0.0.9/shared.egg-info/
+-rw-rw-r--   0 alex      (1002) alex      (1003)    11697 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1002) alex      (1003)      356 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       49 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/entry_points.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)        1 2021-05-31 21:57:25.000000 shared-0.0.9/shared.egg-info/not-zip-safe
+-rw-rw-r--   0 alex      (1002) alex      (1003)        7 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1002) alex      (1003)       13 2022-01-18 22:03:46.000000 shared-0.0.9/shared.egg-info/top_level.txt
+drwxrwxr-x   0 alex      (1002) alex      (1003)        0 2022-01-18 22:03:47.039977 shared-0.0.9/tests/
+-rw-r-----   0 alex      (1002) alex      (1003)        0 2020-05-31 07:38:19.000000 shared-0.0.9/tests/__init__.py
+-rw-rw-r--   0 alex      (1002) alex      (1003)      365 2021-11-16 19:12:35.000000 shared-0.0.9/tests/__main__.py
```

### Comparing `shared-0.0.8/LICENSE` & `shared-0.0.9/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 Pyrustic Evangelist
+Copyright (c) 2021, 2022 Pyrustic Evangelist
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `shared-0.0.8/PKG-INFO` & `shared-0.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,192 @@
 Metadata-Version: 2.1
 Name: shared
-Version: 0.0.8
+Version: 0.0.9
 Summary: Shared data for Python
 Home-page: https://github.com/pyrustic/shared
 Author: Pyrustic Evangelist
-Author-email: pyrustic@protonmail.com
+Author-email: rusticalex@yahoo.com
 Maintainer: Pyrustic Evangelist
-Maintainer-email: pyrustic@protonmail.com
+Maintainer-email: rusticalex@yahoo.com
 License: MIT
 Keywords: library,json,data,shared,binary,database,configuration,collections,persistence,pyrustic,lightweight
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# Shared
+**Smooth way to store, share, and edit data (collections and binary).**
 
-## Shared
+This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
+> [Installation](#installation) . [Latest](https://github.com/pyrustic/shared/tags) . [Modules Documentation](https://github.com/pyrustic/shared/tree/master/docs/modules#readme)
 
-`Shared` is the Python library to store, expose, read, and edit collections of data.
- It's part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
+## Table of contents
+- [Overview](#overview) 
+- [Jason](#jason) 
+- [Store](#store)
+- [Shared collections](shared-collections)
+- [Installation](#installation) 
+
+# Overview
+**Shared** contains two main classes: `Jason` and `Store`.
+
+| Class  | Description | Relevance |
+|--------|-------------|-----------|
+| `Jason` | allows individual access to `JSON` files that are likely to be **manually edited by a human** | relevant for managing configuration files |
+| `Store` | allows you to store collections of data **without worrying about how they are actually saved** | relevant for application data storage and persistent data caching |
 
-[Installation](#installation) | [Reference](https://github.com/pyrustic/shared/tree/master/docs/reference#readme)
+**Shared** is included in [Gaspium](https://github.com/pyrustic/gaspium), the high-productivity framework to build Python apps.
 
+# Jason
+Under the hood, **Jason** uses the [JSON](https://en.wikipedia.org/wiki/JSON) format to store data.
 
-## Overview
-Shared contains two main classes: `Jason` and `Store`.
+```python
+from shared import Jason
 
-`Jason` allows individual access to `json` files that are likely to be manually edited by a human user. `Jason` is relevant for managing configuration files.
 
-`Store` allows you to store collections of data without worrying about how they are actually saved. `Store` is relevant for application data storage and persistent data caching.
+# Create a new jason instance that will be tied to the file 'my-data.json'.
+# If this file doesn't exist yet, it will be automatically created
+jason = Jason("my-data.json")
+
+# From now, we can use jason to read and write the contents of 'my-data.json' !
+# ...
+```
 
-### Jason
+## Initialization
+It's as easy as testing a boolean to see if your JSON file is newly created or not:
 
-Let's play with `Jason`:
 ```python
 from shared import Jason
 
 
 # access 'my-data.json'
 jason = Jason("my-data.json")
-# let's initialize the content of 'my-data'
+
+# let's initialize the content of 'my-data.json'
 if jason.new:
     jason.data = {"name": "alex", "job": "angelist"}
+    # oops I have been distracted by the woman in red !
+    jason.data["job"] = "evangelist"
+    # now let's save the contents of jason.data to the underlying JSON file
+    jason.save()  # persisted !
+```
 
-jason.data["job"] = "evangelist"
 
-jason.save()  # persisted !
-```
+## Default data
+**Jason** comes with a feature to automatically initialize a file with default data:
 
-The same stuff with two twists:
 ```python
 from shared import Jason
 
-# default data to init my 'my-data.json'
-DEFAULT_DATA = {"name": "alex", "job": "angelist"}
+# default data to init the file 'my-data.json'
+DEFAULT_DATA = {"name": "alex", "job": "evangelist"}
 
 # access 'my-data.json'
 jason = Jason("my-data.json", default=DEFAULT_DATA)
 
-# jason.data is either an instance of
-# shared.SharedDict or shared.SharedList
-data = jason.data
-
-data["job"] = "evangelist"
-
-# yes, you can call the .save method directly
-# from the data returned by the jason.data property
-data.save()  # persisted !
+# Done !
 
 ```
-By default, the `json` files are saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
+
+## Data location
+By default, the `JSON` files are saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
 
 ```python
 from shared import Jason
 
-LOCATION = "/home/alex/app-data"
+LOCATION = "/home/alex/private"
 
 # access 'my-data.json'
-jason = Jason("my-data.json", location=LOCATION, readonly=True)
-
-# when you set readonly to True, you can't anymore edit the content !
+jason = Jason("my-data.json", location=LOCATION)
 
 ```
-Two more tips:
+
+## Autosave
+Thanks to [probed](https://github.com/pyrustic/probed) collections, you can tell **Jason** to autosave when the contents of a collection change:
+
 ```python
 from shared import Jason
 
 
 # access 'my-config.json'
 jason = Jason("my-config.json", autosave=True, default=[])
 
 # when you set autosave to True, you don't anymore need
 # to call the method .save() !
 
 jason.data.append("batman")  # persisted ! yeah yeah !
+```
+
+`shared.SharedList`, `shared.SharedDict`, and `shared.SharedSet` are based on `probed.ProbedList`, `probed.ProbedDict`, and `probed.ProbedSet` respectively. If you want to have full control over your collections in your projects, such as being notified when their contents change or filtering what is added to them, check [probed](https://github.com/pyrustic/probed) !
+
+## Readonly
+Sometimes you need to access a JSON file with the guarantee that its contents will not be modified by your own code:
 
-# you can delete the jason file (assuming that readonly is False)
+```python
+from shared import Jason
+
+
+# access 'my-data.json'
+jason = Jason("my-data.json", readonly=True)
+
+# when you set readonly to True, you can't anymore edit the content !
+# shared.ReadonlyError will be raised if you try to mess with a readonly jason
+
+```
+
+## Clear data
+You can delete a JSON file (assuming that the file isn't accessed in readonly mode):
+```python
+from shared import Jason
+
+
+# access 'my-data.json'
+jason = Jason("my-data.json")
+
+# delete "my-data.json"
 jason.delete()
 
 print(jason.deleted)  # output: True
-```
 
-Now let's discover the class `shared.Store` !
+```
 
+# Store
+Under the hood, **Store** uses the [JSON](https://en.wikipedia.org/wiki/JSON) and binary files.
 
-### Store
-Store data:
+Let's create data in **script_1.py**:
 
 ```python
+# script_1.py
 from shared import Store
 
 # data
 people = {"Jack": "male", "Jane": "female"}  # dict
 planets = ["Mars", "Venus", "Jupiter"]  # list
 colors = {"red", "green", "blue"}  # set
 
 # let's persist the data in the store 'my-store'
 store = Store("my-store")
 store.set("people", people)  # set the entry 'people'
 store.set("planets", planets)  # set the entry 'planets'
 store.set("colors", colors)  # set the entry 'colors'
 
-# Done !
+# Done ! The data is persisted !
 ```
 
-Read data from another script:
-
+From **script_2.py** let's access the data created by **script_1.py**:
 ```python
+# script_2.py
 from shared import Store
 
 # let's open the shared store in readonly mode
-store = Store("my-store", readonly=True)
+store = Store("my-store")
 
 # get data from the shared store 'my-store'
 people = store.get("people") # get the entry 'people'
 planets = store.get("planets") # get the entry 'planets'
 colors = store.get("colors") # get the entry 'colors'
 
 print(people)
@@ -147,222 +196,210 @@
 # output: ['Mars', 'Venus', 'Jupiter']
 
 print(colors)
 # output: {'red', 'green', 'blue'}
 
 ```
 
-Since we're all consenting adults here, you can edit the data from another script:
-
+## Data location
+By default, the data is saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
 ```python
 from shared import Store
 
-store = Store("my-store")
-planets = store.get("planets")
-
-# the object 'planets' is a SharedList
-print(type(planets))
-# output: <class 'shared.SharedList'>
-
-# you can update its content like a standard list
-planets.append("Earth")
-
-# then you can save the updated collection
-planets.save()
+LOCATION = "/home/alex/private/stores"
 
+# access 'my-store'
+store = Store("my-store", location=LOCATION)
 ```
 
-Maybe you need your collection to be automatically saved when its content changes:
+## Autosave
+Thanks to [probed](https://github.com/pyrustic/probed) collections, you can tell **Store** to autosave when the contents of a collection change:
 
 ```python
 from shared import Store
 
-# the 'autosave' feature will save your collections
-# whenever their content change
+# access 'my-store' with autosave set to True
+# so shared collections will be automatically persisted
 store = Store("my-store", autosave=True)
-planets = store.get("planets")
 
-planets.append("Saturn")  # done ! collection updated and saved !
+# get the entry 'people' previously stored as {'Jack': 'male', 'Jane': 'female'}
+people = store.get("people")  # the value returned is a 'shared.SharedDict'
 
-```
+# update the contents of people
+people["Janet"] = "female"  # persisted !
 
-`Shared` comes with an easy-to-use command line interface:
+# set a new entry
+new_entry = store.set("new_entry", ["alpha", 42, True])  # the value returned is a 'shared.SharedList
 
-```bash
-$ shared store "my-store" "planets"
-['Mars', 'Venus', 'Jupiter', 'Earth', 'Saturn']
+# update the contents of new_entry
+new_entry.append(3.14)  # persisted !
 
-$ shared store "my-store" "colors"
-{'red', 'green', 'blue'}
-
-$ shared store "my-store" "people"
-{'Jack': 'male', 'Jane': 'female'}
 ```
 
-Type `help` in the command line interface to display a short manual.
-
-Now you are wondering where `Shared` stores collections and in what file format.
-
-Well, the file format is [JSON](https://en.wikipedia.org/wiki/JSON), and the default location is in the [home directory](https://en.wikipedia.org/wiki/Home_directory). More precisely, the default directory to keep stores is: `$HOME/PyrusticData/shared`.
-
-```bash
-$ shared store "my-store"
-/home/alex/PyrusticData/shared
-- colors (set)
-- people (dict)
-- planets (list)
-```
-
-You can change the default location:
-
+## Readonly
+Sometimes you need to access a store with the guarantee that its contents will not be modified by your own code:
 ```python
 from shared import Store
 
-PRIVATE_DATA_DIRECTORY = "/home/alex/private"
-store = Store("secret-store-42", location=PRIVATE_DATA_DIRECTORY)
 
-# the store 'secret-store-42' will be created inside
-# the directory '/home/alex/private'
-
-```
-
-Private stores are still accessible through the command line interface. You will just need to change the current working directory:
+# access 'my-store'
+store = Store("my-store", readonly=True)
 
-```bash
-$ cd "/home/alex/private"
+# when you set readonly to True, you can't anymore edit the contents !
+# you can only use the 'get' method of the store, not anymore the 'set' method, nor autosave.
+# shared.ReadonlyError will be raised if you try to mess with a readonly jason
 
-$ shared store "secret-store-42"
-- Empty store -
 ```
 
-As you can see, `Shared` is great for sharing collections with other software, or just used as private data storage. The command line interface makes things more wonderful.
-
-Wait... can you store binary data with `Shared` ?
-
-Yes, you can:
+## Binary data
+You can store binary data with in your store :
 
 ```python
+# script_1.py
 from shared import Store
 
 store = Store("my-store")
 
 with open("/home/alex/selfie.png", "rb") as file:
     data = file.read()
     store.set("selfie", data)  # set the entry 'selfie'
 
+# the method 'set' returns the path to the binary file that stores the binary entry
 ```
 
-From the command line, you can copy this binary data into an arbitrary file:
-
-```bash
-$ shared store "my-store" "selfie" > "/home/alex/new.png"
-
-```
-
-Or you can do the same thing but in reverse, i.e. store the binary data from the command line:
-
-```bash
-$ shared store "my-store" "selfie" bin "/home/alex/selfie.png"
-Successfully updated the entry 'selfie' !
-```
-
-Then programmatically copy this binary data to an arbitrary file:
-
+You can retrieve your binary data from another script:
 ```python
+# script_2.py
 from shared import Store
 from shutil import copyfile
 
 store = Store("my-store")
 source_path = store.get("selfie")  # get the bin entry 'selfie'
 destination_path = "/home/alex/new.png"
 
 # copy the content from source to destination
 copyfile(source_path, destination_path)
 
 ```
 
-Do you care about the space available on your hard drive ?
-
-Well you can easily delete any entry. Programmatically:
+## Clear data
+You can decide to delete a store:
 
 ```python
 from shared import Store
 
 store = Store("my-store")
-# delete the entry 'selfie'
-store.delete("selfie")
-
+store.delete()  # data collections, binary data, and meta data are gone
 ```
 
-or from the command line interface:
+
+## Command line interface
+**Shared** comes with an easy-to-use command line interface for the class **Store**. Type `help` in the command line interface to display a short manual.
+
+Let assume that we got a store named `my-store` which contains data:
 
 ```bash
-$ shared del "my-store" "selfie"
-Successfully deleted !
+$ shared store "my-store" "planets"
+['Mars', 'Venus', 'Jupiter', 'Earth', 'Saturn']
+
+$ shared store "my-store" "colors"
+{'red', 'green', 'blue'}
+
+$ shared store "my-store" "people"
+{'Jack': 'male', 'Jane': 'female'}
+```
+
+You can check the contents of a store:
+```bash
+$ shared store "my-store"
+/home/alex/PyrusticData/shared
+- colors (set)
+- people (dict)
+- planets (list)
 ```
 
-You can decide to be a badass and delete the store. Programmatically:
+By default, the command line interface looks for the requested store in the default location `$HOME/PyrusticData/shared`. Private stores are still accessible through the command line interface. You will just need to change the current working directory:
 
-```python
-from shared import Store
+```bash
+$ cd "/home/alex/private"
 
-store = Store("my-store")
-store.delete()  # data collections, binary data, and meta data are gone
+$ shared store "secret-store-42"
+- Empty store -
 ```
 
-or from the command line interface:
+You can store binary data as an entry from the command line:
 
 ```bash
-$ shared del "my-store"
-Successfully deleted !
+$ shared store "my-store" "selfie" bin "/home/alex/selfie.png"
+Successfully updated the entry 'selfie' !
+```
+
+You can copy a binary entry into an arbitrary file from the command line:
+
+```bash
+$ shared store "my-store" "selfie" > "/home/alex/new.png"
 
 ```
 
-Between us, do you trust the `delete` feature ? Here is a snippet of the code which shows that the directory to be deleted must have a particular signature, otherwise it will not be deleted:
+You can delete an entry from the command line:
 
-```python
+```bash
+$ shared del "my-store" "selfie"
+Successfully deleted !
+```
 
-def delete(self, *names):
-    
-    ...
-    
-    if self._readonly:
-        raise ReadonlyError
-    # the directory to delete is checked
-    # to be sure that it has the store signature
-    if not valid_store(self._store_path):
-        return False
-    if not names:  # delete store
-        shutil.rmtree(self._store_path)
-    
-    ...
+You can delete a store from the command line:
 
+```bash
+$ shared del "my-store"
+Successfully deleted !
 ```
 
-Are you wondering how the `autosave` feature works ? Under the hood, `Shared` uses the awesome library `probed`.
 
-`Probed` collections let you know when their content change (with 1 more twist !).
+# Shared collections
+**Jason** and **Store** works with shared collections that are based on [probed](https://github.com/pyrustic/probed) collections. If the boolean `readonly` isn't set to True, you can use the method `save` of the shared collections returned by **Jason** and **Store**.
 
-Discover [Probed](https://github.com/pyrustic/probed) !
+There is an intuitive mapping between Python collections, Shared collections, and Probed collections:
 
+| Python collections | Shared collections | Probed collections |
+|--------------------|--------------------|--------------------|
+| dict               | shared.SharedDict  | probed.ProbedDict  |
+| list               | shared.SharedList  | probed.ProbedList  |
+| set                | shared.SharedSet   | probed.ProbedSet   |
 
-## Installation
-Do you like `Shared` ? Guess what, it's available on [PyPI](https://pypi.org):
+
+
+# Installation
+**Shared** is **cross platform** and versions under **1.0.0** will be considered **Beta** at best. It is built on [Ubuntu](https://ubuntu.com/download/desktop) with [Python 3.8](https://www.python.org/downloads/) and should work on **Python 3.5** or **newer**.
+
+## For the first time
 
 ```bash
 $ pip install shared
 ```
 
-## Related projects
-Both `Shared` and `Probed` are part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
+## Upgrade
+```bash
+$ pip install shared --upgrade --upgrade-strategy eager
 
-Looking for an awesome theme for your desktop application ? Check [Cyberpunk Theme](https://github.com/pyrustic/cyberpunk-theme) !
+```
+
+## Make your project packageable
+**Backstage** is an extensible command line tool for managing software projects. By default, it supports Python, so you can run the `init` command to make your Python project [packageable](https://packaging.python.org/en/latest/tutorials/packaging-projects/):
+
+```bash
+$ cd /path/to/project
+$ backstage init
+Project successfully initialized !
+```
 
-Do you want to create a popular theme for Python desktop apps ? Check [TkStyle](https://github.com/pyrustic/tkstyle) !
+You can also create a distribution package of your project with the `build` command, then publish it to [PyPI](https://pypi.org/) with the `release` command, et cetera.
 
-Do you dream to add the autocomplete feature to your desktop app ? Check [Suggestion](https://github.com/pyrustic/suggestion) !
+**Discover [Backstage](https://github.com/pyrustic/backstage) !**
 
-Struggling with GUI+multithreading ? Check [Threadom](https://github.com/pyrustic/threadom) !
 
-Do you like the project(s) and want to help ? Tell your friends about the project(s) !
+<br>
+<br>
+<br>
 
+[Back to top](#readme)
```

### Comparing `shared-0.0.8/README.md` & `shared-0.0.9/shared.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,124 +1,192 @@
+Metadata-Version: 2.1
+Name: shared
+Version: 0.0.9
+Summary: Shared data for Python
+Home-page: https://github.com/pyrustic/shared
+Author: Pyrustic Evangelist
+Author-email: rusticalex@yahoo.com
+Maintainer: Pyrustic Evangelist
+Maintainer-email: rusticalex@yahoo.com
+License: MIT
+Keywords: library,json,data,shared,binary,database,configuration,collections,persistence,pyrustic,lightweight
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Shared
+**Smooth way to store, share, and edit data (collections and binary).**
+
+This project is part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
+> [Installation](#installation) . [Latest](https://github.com/pyrustic/shared/tags) . [Modules Documentation](https://github.com/pyrustic/shared/tree/master/docs/modules#readme)
+
+## Table of contents
+- [Overview](#overview) 
+- [Jason](#jason) 
+- [Store](#store)
+- [Shared collections](shared-collections)
+- [Installation](#installation) 
+
+# Overview
+**Shared** contains two main classes: `Jason` and `Store`.
+
+| Class  | Description | Relevance |
+|--------|-------------|-----------|
+| `Jason` | allows individual access to `JSON` files that are likely to be **manually edited by a human** | relevant for managing configuration files |
+| `Store` | allows you to store collections of data **without worrying about how they are actually saved** | relevant for application data storage and persistent data caching |
 
-## Shared
+**Shared** is included in [Gaspium](https://github.com/pyrustic/gaspium), the high-productivity framework to build Python apps.
 
-`Shared` is the Python library to store, expose, read, and edit collections of data.
- It's part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
-
-[Installation](#installation) | [Reference](https://github.com/pyrustic/shared/tree/master/docs/reference#readme)
+# Jason
+Under the hood, **Jason** uses the [JSON](https://en.wikipedia.org/wiki/JSON) format to store data.
 
+```python
+from shared import Jason
 
-## Overview
-Shared contains two main classes: `Jason` and `Store`.
 
-`Jason` allows individual access to `json` files that are likely to be manually edited by a human user. `Jason` is relevant for managing configuration files.
+# Create a new jason instance that will be tied to the file 'my-data.json'.
+# If this file doesn't exist yet, it will be automatically created
+jason = Jason("my-data.json")
 
-`Store` allows you to store collections of data without worrying about how they are actually saved. `Store` is relevant for application data storage and persistent data caching.
+# From now, we can use jason to read and write the contents of 'my-data.json' !
+# ...
+```
 
-### Jason
+## Initialization
+It's as easy as testing a boolean to see if your JSON file is newly created or not:
 
-Let's play with `Jason`:
 ```python
 from shared import Jason
 
 
 # access 'my-data.json'
 jason = Jason("my-data.json")
-# let's initialize the content of 'my-data'
+
+# let's initialize the content of 'my-data.json'
 if jason.new:
     jason.data = {"name": "alex", "job": "angelist"}
+    # oops I have been distracted by the woman in red !
+    jason.data["job"] = "evangelist"
+    # now let's save the contents of jason.data to the underlying JSON file
+    jason.save()  # persisted !
+```
 
-jason.data["job"] = "evangelist"
 
-jason.save()  # persisted !
-```
+## Default data
+**Jason** comes with a feature to automatically initialize a file with default data:
 
-The same stuff with two twists:
 ```python
 from shared import Jason
 
-# default data to init my 'my-data.json'
-DEFAULT_DATA = {"name": "alex", "job": "angelist"}
+# default data to init the file 'my-data.json'
+DEFAULT_DATA = {"name": "alex", "job": "evangelist"}
 
 # access 'my-data.json'
 jason = Jason("my-data.json", default=DEFAULT_DATA)
 
-# jason.data is either an instance of
-# shared.SharedDict or shared.SharedList
-data = jason.data
-
-data["job"] = "evangelist"
-
-# yes, you can call the .save method directly
-# from the data returned by the jason.data property
-data.save()  # persisted !
+# Done !
 
 ```
-By default, the `json` files are saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
+
+## Data location
+By default, the `JSON` files are saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
 
 ```python
 from shared import Jason
 
-LOCATION = "/home/alex/app-data"
+LOCATION = "/home/alex/private"
 
 # access 'my-data.json'
-jason = Jason("my-data.json", location=LOCATION, readonly=True)
-
-# when you set readonly to True, you can't anymore edit the content !
+jason = Jason("my-data.json", location=LOCATION)
 
 ```
-Two more tips:
+
+## Autosave
+Thanks to [probed](https://github.com/pyrustic/probed) collections, you can tell **Jason** to autosave when the contents of a collection change:
+
 ```python
 from shared import Jason
 
 
 # access 'my-config.json'
 jason = Jason("my-config.json", autosave=True, default=[])
 
 # when you set autosave to True, you don't anymore need
 # to call the method .save() !
 
 jason.data.append("batman")  # persisted ! yeah yeah !
+```
+
+`shared.SharedList`, `shared.SharedDict`, and `shared.SharedSet` are based on `probed.ProbedList`, `probed.ProbedDict`, and `probed.ProbedSet` respectively. If you want to have full control over your collections in your projects, such as being notified when their contents change or filtering what is added to them, check [probed](https://github.com/pyrustic/probed) !
+
+## Readonly
+Sometimes you need to access a JSON file with the guarantee that its contents will not be modified by your own code:
 
-# you can delete the jason file (assuming that readonly is False)
+```python
+from shared import Jason
+
+
+# access 'my-data.json'
+jason = Jason("my-data.json", readonly=True)
+
+# when you set readonly to True, you can't anymore edit the content !
+# shared.ReadonlyError will be raised if you try to mess with a readonly jason
+
+```
+
+## Clear data
+You can delete a JSON file (assuming that the file isn't accessed in readonly mode):
+```python
+from shared import Jason
+
+
+# access 'my-data.json'
+jason = Jason("my-data.json")
+
+# delete "my-data.json"
 jason.delete()
 
 print(jason.deleted)  # output: True
-```
 
-Now let's discover the class `shared.Store` !
+```
 
+# Store
+Under the hood, **Store** uses the [JSON](https://en.wikipedia.org/wiki/JSON) and binary files.
 
-### Store
-Store data:
+Let's create data in **script_1.py**:
 
 ```python
+# script_1.py
 from shared import Store
 
 # data
 people = {"Jack": "male", "Jane": "female"}  # dict
 planets = ["Mars", "Venus", "Jupiter"]  # list
 colors = {"red", "green", "blue"}  # set
 
 # let's persist the data in the store 'my-store'
 store = Store("my-store")
 store.set("people", people)  # set the entry 'people'
 store.set("planets", planets)  # set the entry 'planets'
 store.set("colors", colors)  # set the entry 'colors'
 
-# Done !
+# Done ! The data is persisted !
 ```
 
-Read data from another script:
-
+From **script_2.py** let's access the data created by **script_1.py**:
 ```python
+# script_2.py
 from shared import Store
 
 # let's open the shared store in readonly mode
-store = Store("my-store", readonly=True)
+store = Store("my-store")
 
 # get data from the shared store 'my-store'
 people = store.get("people") # get the entry 'people'
 planets = store.get("planets") # get the entry 'planets'
 colors = store.get("colors") # get the entry 'colors'
 
 print(people)
@@ -128,220 +196,210 @@
 # output: ['Mars', 'Venus', 'Jupiter']
 
 print(colors)
 # output: {'red', 'green', 'blue'}
 
 ```
 
-Since we're all consenting adults here, you can edit the data from another script:
-
+## Data location
+By default, the data is saved in `$HOME/PyrusticData/shared`. You can change the location to fit your needs:
 ```python
 from shared import Store
 
-store = Store("my-store")
-planets = store.get("planets")
-
-# the object 'planets' is a SharedList
-print(type(planets))
-# output: <class 'shared.SharedList'>
-
-# you can update its content like a standard list
-planets.append("Earth")
-
-# then you can save the updated collection
-planets.save()
+LOCATION = "/home/alex/private/stores"
 
+# access 'my-store'
+store = Store("my-store", location=LOCATION)
 ```
 
-Maybe you need your collection to be automatically saved when its content changes:
+## Autosave
+Thanks to [probed](https://github.com/pyrustic/probed) collections, you can tell **Store** to autosave when the contents of a collection change:
 
 ```python
 from shared import Store
 
-# the 'autosave' feature will save your collections
-# whenever their content change
+# access 'my-store' with autosave set to True
+# so shared collections will be automatically persisted
 store = Store("my-store", autosave=True)
-planets = store.get("planets")
 
-planets.append("Saturn")  # done ! collection updated and saved !
+# get the entry 'people' previously stored as {'Jack': 'male', 'Jane': 'female'}
+people = store.get("people")  # the value returned is a 'shared.SharedDict'
 
-```
+# update the contents of people
+people["Janet"] = "female"  # persisted !
 
-`Shared` comes with an easy-to-use command line interface:
+# set a new entry
+new_entry = store.set("new_entry", ["alpha", 42, True])  # the value returned is a 'shared.SharedList
 
-```bash
-$ shared store "my-store" "planets"
-['Mars', 'Venus', 'Jupiter', 'Earth', 'Saturn']
+# update the contents of new_entry
+new_entry.append(3.14)  # persisted !
 
-$ shared store "my-store" "colors"
-{'red', 'green', 'blue'}
-
-$ shared store "my-store" "people"
-{'Jack': 'male', 'Jane': 'female'}
 ```
 
-Type `help` in the command line interface to display a short manual.
-
-Now you are wondering where `Shared` stores collections and in what file format.
-
-Well, the file format is [JSON](https://en.wikipedia.org/wiki/JSON), and the default location is in the [home directory](https://en.wikipedia.org/wiki/Home_directory). More precisely, the default directory to keep stores is: `$HOME/PyrusticData/shared`.
-
-```bash
-$ shared store "my-store"
-/home/alex/PyrusticData/shared
-- colors (set)
-- people (dict)
-- planets (list)
-```
-
-You can change the default location:
-
+## Readonly
+Sometimes you need to access a store with the guarantee that its contents will not be modified by your own code:
 ```python
 from shared import Store
 
-PRIVATE_DATA_DIRECTORY = "/home/alex/private"
-store = Store("secret-store-42", location=PRIVATE_DATA_DIRECTORY)
-
-# the store 'secret-store-42' will be created inside
-# the directory '/home/alex/private'
-
-```
 
-Private stores are still accessible through the command line interface. You will just need to change the current working directory:
+# access 'my-store'
+store = Store("my-store", readonly=True)
 
-```bash
-$ cd "/home/alex/private"
+# when you set readonly to True, you can't anymore edit the contents !
+# you can only use the 'get' method of the store, not anymore the 'set' method, nor autosave.
+# shared.ReadonlyError will be raised if you try to mess with a readonly jason
 
-$ shared store "secret-store-42"
-- Empty store -
 ```
 
-As you can see, `Shared` is great for sharing collections with other software, or just used as private data storage. The command line interface makes things more wonderful.
-
-Wait... can you store binary data with `Shared` ?
-
-Yes, you can:
+## Binary data
+You can store binary data with in your store :
 
 ```python
+# script_1.py
 from shared import Store
 
 store = Store("my-store")
 
 with open("/home/alex/selfie.png", "rb") as file:
     data = file.read()
     store.set("selfie", data)  # set the entry 'selfie'
 
+# the method 'set' returns the path to the binary file that stores the binary entry
 ```
 
-From the command line, you can copy this binary data into an arbitrary file:
-
-```bash
-$ shared store "my-store" "selfie" > "/home/alex/new.png"
-
-```
-
-Or you can do the same thing but in reverse, i.e. store the binary data from the command line:
-
-```bash
-$ shared store "my-store" "selfie" bin "/home/alex/selfie.png"
-Successfully updated the entry 'selfie' !
-```
-
-Then programmatically copy this binary data to an arbitrary file:
-
+You can retrieve your binary data from another script:
 ```python
+# script_2.py
 from shared import Store
 from shutil import copyfile
 
 store = Store("my-store")
 source_path = store.get("selfie")  # get the bin entry 'selfie'
 destination_path = "/home/alex/new.png"
 
 # copy the content from source to destination
 copyfile(source_path, destination_path)
 
 ```
 
-Do you care about the space available on your hard drive ?
-
-Well you can easily delete any entry. Programmatically:
+## Clear data
+You can decide to delete a store:
 
 ```python
 from shared import Store
 
 store = Store("my-store")
-# delete the entry 'selfie'
-store.delete("selfie")
-
+store.delete()  # data collections, binary data, and meta data are gone
 ```
 
-or from the command line interface:
+
+## Command line interface
+**Shared** comes with an easy-to-use command line interface for the class **Store**. Type `help` in the command line interface to display a short manual.
+
+Let assume that we got a store named `my-store` which contains data:
 
 ```bash
-$ shared del "my-store" "selfie"
-Successfully deleted !
+$ shared store "my-store" "planets"
+['Mars', 'Venus', 'Jupiter', 'Earth', 'Saturn']
+
+$ shared store "my-store" "colors"
+{'red', 'green', 'blue'}
+
+$ shared store "my-store" "people"
+{'Jack': 'male', 'Jane': 'female'}
 ```
 
-You can decide to be a badass and delete the store. Programmatically:
+You can check the contents of a store:
+```bash
+$ shared store "my-store"
+/home/alex/PyrusticData/shared
+- colors (set)
+- people (dict)
+- planets (list)
+```
 
-```python
-from shared import Store
+By default, the command line interface looks for the requested store in the default location `$HOME/PyrusticData/shared`. Private stores are still accessible through the command line interface. You will just need to change the current working directory:
 
-store = Store("my-store")
-store.delete()  # data collections, binary data, and meta data are gone
+```bash
+$ cd "/home/alex/private"
+
+$ shared store "secret-store-42"
+- Empty store -
 ```
 
-or from the command line interface:
+You can store binary data as an entry from the command line:
 
 ```bash
-$ shared del "my-store"
-Successfully deleted !
+$ shared store "my-store" "selfie" bin "/home/alex/selfie.png"
+Successfully updated the entry 'selfie' !
+```
+
+You can copy a binary entry into an arbitrary file from the command line:
+
+```bash
+$ shared store "my-store" "selfie" > "/home/alex/new.png"
 
 ```
 
-Between us, do you trust the `delete` feature ? Here is a snippet of the code which shows that the directory to be deleted must have a particular signature, otherwise it will not be deleted:
+You can delete an entry from the command line:
 
-```python
+```bash
+$ shared del "my-store" "selfie"
+Successfully deleted !
+```
 
-def delete(self, *names):
-    
-    ...
-    
-    if self._readonly:
-        raise ReadonlyError
-    # the directory to delete is checked
-    # to be sure that it has the store signature
-    if not valid_store(self._store_path):
-        return False
-    if not names:  # delete store
-        shutil.rmtree(self._store_path)
-    
-    ...
+You can delete a store from the command line:
 
+```bash
+$ shared del "my-store"
+Successfully deleted !
 ```
 
-Are you wondering how the `autosave` feature works ? Under the hood, `Shared` uses the awesome library `probed`.
 
-`Probed` collections let you know when their content change (with 1 more twist !).
+# Shared collections
+**Jason** and **Store** works with shared collections that are based on [probed](https://github.com/pyrustic/probed) collections. If the boolean `readonly` isn't set to True, you can use the method `save` of the shared collections returned by **Jason** and **Store**.
+
+There is an intuitive mapping between Python collections, Shared collections, and Probed collections:
+
+| Python collections | Shared collections | Probed collections |
+|--------------------|--------------------|--------------------|
+| dict               | shared.SharedDict  | probed.ProbedDict  |
+| list               | shared.SharedList  | probed.ProbedList  |
+| set                | shared.SharedSet   | probed.ProbedSet   |
 
-Discover [Probed](https://github.com/pyrustic/probed) !
 
 
-## Installation
-Do you like `Shared` ? Guess what, it's available on [PyPI](https://pypi.org):
+# Installation
+**Shared** is **cross platform** and versions under **1.0.0** will be considered **Beta** at best. It is built on [Ubuntu](https://ubuntu.com/download/desktop) with [Python 3.8](https://www.python.org/downloads/) and should work on **Python 3.5** or **newer**.
+
+## For the first time
 
 ```bash
 $ pip install shared
 ```
 
-## Related projects
-Both `Shared` and `Probed` are part of the [Pyrustic Open Ecosystem](https://pyrustic.github.io).
+## Upgrade
+```bash
+$ pip install shared --upgrade --upgrade-strategy eager
+
+```
+
+## Make your project packageable
+**Backstage** is an extensible command line tool for managing software projects. By default, it supports Python, so you can run the `init` command to make your Python project [packageable](https://packaging.python.org/en/latest/tutorials/packaging-projects/):
+
+```bash
+$ cd /path/to/project
+$ backstage init
+Project successfully initialized !
+```
+
+You can also create a distribution package of your project with the `build` command, then publish it to [PyPI](https://pypi.org/) with the `release` command, et cetera.
 
-Looking for an awesome theme for your desktop application ? Check [Cyberpunk Theme](https://github.com/pyrustic/cyberpunk-theme) !
+**Discover [Backstage](https://github.com/pyrustic/backstage) !**
 
-Do you want to create a popular theme for Python desktop apps ? Check [TkStyle](https://github.com/pyrustic/tkstyle) !
 
-Do you dream to add the autocomplete feature to your desktop app ? Check [Suggestion](https://github.com/pyrustic/suggestion) !
+<br>
+<br>
+<br>
 
-Struggling with GUI+multithreading ? Check [Threadom](https://github.com/pyrustic/threadom) !
+[Back to top](#readme)
 
-Do you like the project(s) and want to help ? Tell your friends about the project(s) !
```

### Comparing `shared-0.0.8/setup.cfg` & `shared-0.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = shared
 version = file: VERSION
 url = https://github.com/pyrustic/shared
 author = Pyrustic Evangelist
-author_email = pyrustic@protonmail.com
+author_email = rusticalex@yahoo.com
 maintainer = Pyrustic Evangelist
-maintainer_email = pyrustic@protonmail.com
+maintainer_email = rusticalex@yahoo.com
 description = Shared data for Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 keywords = 
 	library
 	json
```

### Comparing `shared-0.0.8/shared/__init__.py` & `shared-0.0.9/shared/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,139 @@
+"""Main module where are defined the classes Jason and Store"""
 import os
 import os.path
 import time
 import json
 import shutil
 from probed import ProbedDict, ProbedList, ProbedSet
 
 
 DEFAULT_LOCATION = os.path.join(os.path.expanduser("~"),
                                 "PyrusticData", "shared")
 
 
 class Jason:
+    """
+    Definition of the class Jason
+    """
     def __init__(self, name, *, readonly=False,
                  autosave=False, default=None,
                  location=DEFAULT_LOCATION):
+        """
+        Init.
+
+        [parameters]
+        - name: string, the name of the JSON file. Example: "data.json"
+        - readonly: boolean to say if you want to open this JSON file in readonly mode or not
+        - autosave: boolean to say if you want to activate the autosave feature or not
+        - default: default value for this JSON file. It can be None, a dict or a list.
+        If the JSON file is newly created, the default value will populate it.
+        - location: the directory where you want to store the JSON file.
+        By default, the directory is "$HOME/PyrusticData/shared"
+
+        """
         self._name = name
         self._readonly = readonly
         self._autosave = autosave
         self._default = default
         self._location = location
         self._new = False
         self._deleted = False
         self._filename = None
         self._data = None
         self._setup()
 
     @property
     def name(self):
+        """
+        Return the name of the JSON file
+        """
         return self._name
 
     @property
     def data(self):
+        """
+        Return the contents of the JSON file
+        """
         return self._data
 
     @data.setter
     def data(self, val):
+        """
+        Set the contents of the JSON file
+        """
         if self._deleted:
             raise JasonDeletedError
         if self._readonly:
             raise ReadonlyError
         self._data = self._convert_collection(val)
         self._bind_save_method()
 
     @property
     def readonly(self):
+        """
+        Return the readonly boolean state
+        """
         return self._readonly
 
     @property
     def autosave(self):
+        """
+        Return the autosave boolean state
+        """
         return self._autosave
 
     @property
     def location(self):
+        """
+        Return the value of the location variable
+        """
         return self._location
 
     @property
     def new(self):
-        """ Returns True if this json file is newly created, else return False """
+        """
+        Returns True if this JSON file is newly created, else return False
+        """
         return self._new
 
     @property
     def deleted(self):
+        """
+        Return True if this JSON file is deleted else return False
+        """
         return self._deleted
 
+    def save(self):
+        """
+        Write the contents of the property 'data' in the JSON file
+        """
+        if self._deleted:
+            raise JasonDeletedError
+        if self._readonly:
+            raise ReadonlyError
+        json_dump(self._filename, self._data, pretty=True)
+
+    def delete(self):
+        """
+        This method delete the Jason file.
+        Returns a boolean or raise ReadonlyError
+        """
+        if self._deleted:
+            raise JasonDeletedError
+        if self._readonly:
+            raise ReadonlyError
+        if not valid_jason(self._filename):
+            return False
+        os.remove(self._filename)
+        self._deleted = True
+        return True
+
     def _setup(self):
+        # TODO: if location is None, so self._name is path to file
         try:
             os.makedirs(self._location)
         except FileExistsError:
             pass
         self._filename = os.path.join(self._location,
                                       self._name)
         if os.path.isfile(self._filename):
@@ -90,45 +156,30 @@
     def _bind_save_method(self):
         if self._data is None:
             return
         self._data.save = lambda self=self: self.save()
         if self._autosave:
             self._data.on_change = (lambda info: info.collection.save())
 
-    def save(self):
-        if self._deleted:
-            raise JasonDeletedError
-        if self._readonly:
-            raise ReadonlyError
-        json_dump(self._filename, self._data, pretty=True)
-
-    def delete(self):
-        """
-        This method delete the Jason file.
-        Returns a boolean or raise ReadonlyError
-        """
-        if self._deleted:
-            raise JasonDeletedError
-        if self._readonly:
-            raise ReadonlyError
-        if not valid_jason(self._filename):
-            return False
-        os.remove(self._filename)
-        self._deleted = True
-        return True
-
 
 class Store:
+    """
+    Definition of the class Store
+    """
     def __init__(self, name, *, readonly=False,
                  autosave=False, location=DEFAULT_LOCATION):
         """
+        Init.
+
+        [parameters]
         - name: str, the name of the store
         - readonly: bool, readonly mode
         - autosave: bool, auto-save mode
-        - location: str, the directory where stores will be created
+        - location: str, the directory where stores will be created.
+        By default, this directory is '$HOME/PyrusticData/shared'
         """
         self._name = name
         self._readonly = readonly
         self._autosave = autosave
         self._location = location
         self._store_path = None
         self._meta_filename = None
@@ -136,26 +187,38 @@
         self._cache = dict()
         self._deleted = False
         self._new = False
         self._setup()
 
     @property
     def name(self):
+        """
+        Return the name of the store
+        """
         return self._name
 
     @property
     def readonly(self):
+        """
+        Return the state of the readonly boolean
+        """
         return self._readonly
 
     @property
     def autosave(self):
+        """
+        Return the state of the autosave boolean
+        """
         return self._autosave
 
     @property
     def location(self):
+        """
+        Return the location of the store
+        """
         return self._location
 
     @property
     def info(self):
         """
         Returns a dictionary of entries and their container types
         Example: {"entry_1": "dict", "entry_2": "bin", "entry_3": "set"}
@@ -165,41 +228,57 @@
         for name, info in self._meta.items():
             container, _ = info
             cache[name] = container
         return cache
 
     @property
     def new(self):
-        """ Returns True if this store is newly created, else return False """
+        """
+        Returns True if this store is newly created, else return False
+        """
         return self._new
 
     @property
     def deleted(self):
-        """ Returns True if this store has been deleted through this object """
+        """
+        Returns True if this store has been deleted through this object
+        """
         return self._deleted
 
     def set(self, name, data):
         """
         Set an entry.
-        Data should be a dict, a list, a set or a binary data.
+
+        [parameters]
+        - name: str, the name of the entry
+        - data: a dict, a list, a set or binary data.
+
+        [return value]
         This method will return a path if the entry is a binary data.
         SharedDict, SharedList, SharedSet are returned respectively if the entry
-        requested is a dict, a list or a set.
+        is a dict, a list or a set.
         You can call the method "save" on the instances of SharedDict, SharedList,
         or SharedSet.
         """
         if self._deleted:
             raise StoreDeletedError
         if self._readonly:
             raise ReadonlyError
         container = self._get_container(data)
         return self._save(name, container, data)
 
     def get(self, name, default=None):
         """
+        Get an entry.
+
+        [parameters]
+        - name: the name of the entry.
+        - default: a dict, a list, a set or binary data to return if the entry doesn't exist.
+
+        [return value]
         This method returns None if the entry isn't in the store.
         A path is returned if the entry requested exists and is a binary data.
         SharedDict, SharedList, SharedSet are returned respectively if the entry
         requested is a dict, a list or a set
         """
         if self._deleted:
             raise StoreDeletedError
@@ -216,16 +295,18 @@
         data = json_load(filename)
         collection = self._convert_collection(container, data)
         self._bind_save_method(name, collection)
         return collection
 
     def delete(self, *names):
         """
-        This method delete the store if there isn't any argument.
+        This method deletes the store if there isn't any argument.
         Else, the arguments are the entries to delete.
+
+        [return value]
         Returns a boolean or raise ReadonlyError
         """
         if self._deleted:
             raise StoreDeletedError
         if self._readonly:
             raise ReadonlyError
         if not valid_store(self._store_path):
```

### Comparing `shared-0.0.8/shared/__main__.py` & `shared-0.0.9/shared/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Command line interface"""
 import sys
 import os
 import os.path
 import pprint
 from shared import Store, DEFAULT_LOCATION, valid_store, json_load
```

