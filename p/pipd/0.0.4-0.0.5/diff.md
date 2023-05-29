# Comparing `tmp/pipd-0.0.4.tar.gz` & `tmp/pipd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.0.4.tar", last modified: Mon May 29 13:19:32 2023, max compression
+gzip compressed data, was "pipd-0.0.5.tar", last modified: Mon May 29 23:43:07 2023, max compression
```

## Comparing `pipd-0.0.4.tar` & `pipd-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 13:19:32.677392 pipd-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-29 13:19:21.000000 pipd-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 13:19:21.000000 pipd-0.0.4/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-29 13:19:21.000000 pipd-0.0.4/pipd/pipd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:19:32.677392 pipd-0.0.4/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 13:19:32.000000 pipd-0.0.4/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:19:32.677392 pipd-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 13:19:21.000000 pipd-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:43:07.506709 pipd-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 23:43:07.506709 pipd-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-29 23:42:56.000000 pipd-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:43:07.506709 pipd-0.0.5/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 23:42:56.000000 pipd-0.0.5/pipd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-05-29 23:42:56.000000 pipd-0.0.5/pipd/pipd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:43:07.506709 pipd-0.0.5/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 23:43:07.000000 pipd-0.0.5/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 23:43:07.000000 pipd-0.0.5/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:43:07.000000 pipd-0.0.5/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 23:43:07.000000 pipd-0.0.5/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:43:07.506709 pipd-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-29 23:42:56.000000 pipd-0.0.5/setup.py
```

### Comparing `pipd-0.0.4/README.md` & `pipd-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pipd-0.0.4/pipd/pipd.py` & `pipd-0.0.5/pipd/pipd.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,26 @@
 from concurrent.futures import (
     FIRST_COMPLETED,
     ProcessPoolExecutor,
     ThreadPoolExecutor,
     wait,
 )
 from random import randint
-from typing import Callable, Dict, Iterable, Iterator, List, Optional, Sequence, TypeVar
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
 
 T = TypeVar("T")
 U = TypeVar("U")
 
 
 def log_and_continue(exception: Exception):
     print(repr(exception))
@@ -195,16 +206,17 @@
 
 
 shuffle = as_pipe(_shuffle)
 
 
 def _limit(items: Iterable[T], limit: int = 10**100) -> Iterator[T]:
     for count, item in enumerate(items):
-        if count < limit:
-            yield item
+        if count >= limit:
+            return
+        yield item
 
 
 limit = as_pipe(_limit)
 
 
 def _log(items: Iterable[T], fn: Callable[[T], None] = print) -> Iterator[T]:
     return _side(items, fn)
@@ -305,7 +317,48 @@
             if value not in cache:
                 cache.add(value)
                 file.write(value + "\n")
                 yield item
 
 
 filter_cached = as_pipe(_filter_cached)
+
+
+def _write_csv(
+    items: Iterable[Union[Dict[str, Any], Sequence[Any]]], filepath: str
+) -> Iterable[Union[Dict[str, Any], Sequence[Any]]]:
+    import csv
+
+    with open(filepath, "w", newline="") as f:
+        writer = csv.writer(f)
+
+        for i, item in enumerate(items):
+            if isinstance(item, dict):
+                if i == 0:  # Write headers only for the first dictionary item
+                    writer.writerow(item.keys())
+                item = item.values()  # type: ignore
+            writer.writerow(item)
+            yield item
+
+
+write_csv = as_pipe(_write_csv)
+
+
+def _read_csv(
+    _, filepath: str, header: Union[bool, Sequence[str]] = False
+) -> Iterable[Union[Dict[str, str], List[str]]]:
+    import csv
+
+    with open(filepath, "r") as f:
+        if header:
+            fieldnames = header if isinstance(header, Sequence) else None
+            yield from csv.DictReader(f, fieldnames=fieldnames)
+        else:
+            yield from csv.reader(f)
+
+
+read_csv = as_pipe(_read_csv)
+
+
+class ReadCSV(Pipe):
+    def __init__(self, *args, **kwargs):
+        super().__init__(read_csv(*args, **kwargs)())
```

