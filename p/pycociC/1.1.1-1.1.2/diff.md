# Comparing `tmp/pycociC-1.1.1.tar.gz` & `tmp/pycociC-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycociC-1.1.1.tar", last modified: Sun Aug 21 10:24:11 2022, max compression
+gzip compressed data, was "pycociC-1.1.2.tar", last modified: Tue May 30 11:38:24 2023, max compression
```

## Comparing `pycociC-1.1.1.tar` & `pycociC-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-21 10:24:11.183866 pycociC-1.1.1/
--rw-rw-rw-   0        0        0     1096 2022-08-21 10:12:13.000000 pycociC-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     4355 2022-08-21 10:24:11.183866 pycociC-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-21 10:24:11.167855 pycociC-1.1.1/pycociC/
--rw-rw-rw-   0        0        0     4510 2022-08-21 10:06:25.000000 pycociC-1.1.1/pycociC/__init__.py
--rw-rw-rw-   0        0        0      844 2022-08-20 15:02:11.000000 pycociC-1.1.1/pycociC/__main__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 10:24:11.182862 pycociC-1.1.1/pycociC.egg-info/
--rw-rw-rw-   0        0        0     4355 2022-08-21 10:24:10.000000 pycociC-1.1.1/pycociC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2022-08-21 10:24:11.000000 pycociC-1.1.1/pycociC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-21 10:24:10.000000 pycociC-1.1.1/pycociC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-08-21 10:24:10.000000 pycociC-1.1.1/pycociC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-08-21 10:24:10.000000 pycociC-1.1.1/pycociC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-21 10:24:11.184854 pycociC-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1427 2022-08-21 10:13:02.000000 pycociC-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:38:24.713908 pycociC-1.1.2/
+-rw-rw-rw-   0        0        0     1096 2022-08-21 10:12:13.000000 pycociC-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3839 2023-05-30 11:38:24.713908 pycociC-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 11:38:24.711192 pycociC-1.1.2/pycociC/
+-rw-rw-rw-   0        0        0     3442 2023-05-30 11:36:03.000000 pycociC-1.1.2/pycociC/__init__.py
+-rw-rw-rw-   0        0        0      840 2023-05-26 06:38:49.000000 pycociC-1.1.2/pycociC/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:38:24.713908 pycociC-1.1.2/pycociC.egg-info/
+-rw-rw-rw-   0        0        0     3839 2023-05-30 11:38:24.000000 pycociC-1.1.2/pycociC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-30 11:38:24.000000 pycociC-1.1.2/pycociC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 11:38:24.000000 pycociC-1.1.2/pycociC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 11:38:24.000000 pycociC-1.1.2/pycociC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 11:38:24.000000 pycociC-1.1.2/pycociC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 11:38:24.713908 pycociC-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1427 2023-05-30 11:26:20.000000 pycociC-1.1.2/setup.py
```

### Comparing `pycociC-1.1.1/LICENSE` & `pycociC-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycociC-1.1.1/PKG-INFO` & `pycociC-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycociC
-Version: 1.1.1
+Version: 1.1.2
 Summary: Remove pycache (and numba cache) files
 Home-page: https://github.com/NIKDISSV-Forever/pycociC
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -46,44 +46,26 @@
 
 ```python
 # pycociC/__init__.py
 __all__ = ('FP_RE', 'bytes_to_pretty_view', 'eat_cache', 'dont_write_bytecode')
 FP_RE = re.compile(r'.*\.py([co]|.*\.nb[ci])', re.I)
 
 
-@_run_with_max_recursion
 def eat_cache(at_dirs: Iterable[AnyStr, os.PathLike[AnyStr]] = ('.',)):
     """Function removes files matching the regular expression (see FP_RE) from all "__pycache__" folders recursively."""
     ...
 
 
-def dont_write_bytecode() -> bool:
-    """
-    return True if env PYTHONDONTWRITEBYTECODE or -B arg passed else False
-
-    >>> import os
-    >>> os.environ['PYTHONDONTWRITEBYTECODE'] = 'x'
-    >>> dont_write_bytecode()
-    True
-    >>> del os.environ['PYTHONDONTWRITEBYTECODE']  # or os.environ['PYTHONDONTWRITEBYTECODE'] = ''
-    >>> dont_write_bytecode()
-    False
-    """
-    ...
-
-
-def bytes_to_pretty_view(bytes_size: int | float, *, skip_zero: bool = False) -> str:
+def bytes_to_pretty_view(bytes_size: int = 0) -> str:
     """
     Converts the number of bytes into a pretty SI prefix.
 
     >>> bytes_to_pretty_view(0)
     '0B'
-    >>> bytes_to_pretty_view(0, skip_zero=True)
-    ''
-    >>> bytes_to_pretty_view(1_000_000_24.)
+    >>> bytes_to_pretty_view(1_000_000_24)
     '100MB 24B'
     >>> bytes_to_pretty_view(0xFF_FF_FF_FF)
     '4GB 294MB 967kB 295B'
     """
     ...
 
 ```
```

### Comparing `pycociC-1.1.1/pycociC/__main__.py` & `pycociC-1.1.2/pycociC/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-from __future__ import annotations
-
+from sys import dont_write_bytecode
 from argparse import ArgumentParser
 from logging import warning
 
 from psutil import disk_partitions
 
-from pycociC import *
+from . import eat_cache
 
 
 def main():
-    if not dont_write_bytecode():
+    if not dont_write_bytecode:
         warning('pycociC doesn\'t remove bytecode files.\n'
                 '\tYou can use "-B" option of python or PYTHONDONTWRITEBYTECODE=x to do so.\n\n')
-
     disks = *(disk.device for disk in disk_partitions(all=True)),
-
     arg_parser = ArgumentParser('pycociC', description='pycociC - A tool to remove pycache (and numba cache) files')
     arg_parser.add_argument('-t', '-d', '--dirs', nargs='+',
-                            help=f'Directories to search for pycache files (default: {disks})')
-    args = arg_parser.parse_args()
-
-    eat_cache(args.dirs or disks)
+                            help=f"Directories to search for pycache files (default: {' '.join(map(str, disks))})")
+    eat_cache(arg_parser.parse_args().dirs or disks)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pycociC-1.1.1/pycociC.egg-info/PKG-INFO` & `pycociC-1.1.2/pycociC.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycociC
-Version: 1.1.1
+Version: 1.1.2
 Summary: Remove pycache (and numba cache) files
 Home-page: https://github.com/NIKDISSV-Forever/pycociC
 Author: Nikita (NIKDISSV)
 Author-email: nikdissv@proton.me
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -46,44 +46,26 @@
 
 ```python
 # pycociC/__init__.py
 __all__ = ('FP_RE', 'bytes_to_pretty_view', 'eat_cache', 'dont_write_bytecode')
 FP_RE = re.compile(r'.*\.py([co]|.*\.nb[ci])', re.I)
 
 
-@_run_with_max_recursion
 def eat_cache(at_dirs: Iterable[AnyStr, os.PathLike[AnyStr]] = ('.',)):
     """Function removes files matching the regular expression (see FP_RE) from all "__pycache__" folders recursively."""
     ...
 
 
-def dont_write_bytecode() -> bool:
-    """
-    return True if env PYTHONDONTWRITEBYTECODE or -B arg passed else False
-
-    >>> import os
-    >>> os.environ['PYTHONDONTWRITEBYTECODE'] = 'x'
-    >>> dont_write_bytecode()
-    True
-    >>> del os.environ['PYTHONDONTWRITEBYTECODE']  # or os.environ['PYTHONDONTWRITEBYTECODE'] = ''
-    >>> dont_write_bytecode()
-    False
-    """
-    ...
-
-
-def bytes_to_pretty_view(bytes_size: int | float, *, skip_zero: bool = False) -> str:
+def bytes_to_pretty_view(bytes_size: int = 0) -> str:
     """
     Converts the number of bytes into a pretty SI prefix.
 
     >>> bytes_to_pretty_view(0)
     '0B'
-    >>> bytes_to_pretty_view(0, skip_zero=True)
-    ''
-    >>> bytes_to_pretty_view(1_000_000_24.)
+    >>> bytes_to_pretty_view(1_000_000_24)
     '100MB 24B'
     >>> bytes_to_pretty_view(0xFF_FF_FF_FF)
     '4GB 294MB 967kB 295B'
     """
     ...
 
 ```
```

### Comparing `pycociC-1.1.1/setup.py` & `pycociC-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read().strip()
 with open('requirements.txt', encoding='UTF-8') as f:
     install_requires = f.read().splitlines()
 
 setuptools.setup(
     name="pycociC",
 
-    version="1.1.1",
+    version="1.1.2",
 
     author="Nikita (NIKDISSV)",
     author_email="nikdissv@proton.me",
 
     description="Remove pycache (and numba cache) files",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

