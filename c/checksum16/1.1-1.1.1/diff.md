# Comparing `tmp/checksum16-1.1.tar.gz` & `tmp/checksum16-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checksum16-1.1.tar", last modified: Tue May 30 18:59:38 2023, max compression
+gzip compressed data, was "checksum16-1.1.1.tar", last modified: Tue May 30 19:02:53 2023, max compression
```

## Comparing `checksum16-1.1.tar` & `checksum16-1.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:59:38.870178 checksum16-1.1/
--rw-r--r--   0 root         (0) root         (0)      915 2023-05-30 18:59:38.870178 checksum16-1.1/PKG-INFO
--rw-r--r--   0 efiweiss  (1000) efiweiss  (1000)     1248 2023-05-30 18:42:44.670473 checksum16-1.1/checksum.c
--rw-r--r--   0 efiweiss  (1000) efiweiss  (1000)      883 2023-05-30 18:59:17.290184 checksum16-1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 19:02:53.830124 checksum16-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-30 19:02:53.830124 checksum16-1.1.1/PKG-INFO
+-rw-r--r--   0 efiweiss  (1000) efiweiss  (1000)     1248 2023-05-30 18:42:44.670473 checksum16-1.1.1/checksum.c
+-rw-r--r--   0 efiweiss  (1000) efiweiss  (1000)      885 2023-05-30 19:02:50.710125 checksum16-1.1.1/setup.py
```

### Comparing `checksum16-1.1/PKG-INFO` & `checksum16-1.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 1.0
 Name: checksum16
-Version: 1.1
+Version: 1.1.1
 Summary: Native checksum implementation for python
 Home-page: https://github.com/Valmarelox/checksum
 Author: Efi Weiss
 Author-email: valmarelox@gmail.com
 License: UNKNOWN
 Description: # Checksum only python native module
         I tried to find a quick python native implemenation of ip checksum to achieve a
-        better performance. Didn't find it, so I created my own module.
+        better performance - I Didn't find any, so I created my own module.
+        
+        
         Calculate IP checksum-16 (Host endianess for compatability with other pure
         python implementations:
-        How to use
+        
+        #### How to use
         ```python
         from checksum import checksum
         res = checksum(b'BEST DATA')
         ```
         The module also supports partial checksums:
         ```python
         from checksum import checksum
```

### Comparing `checksum16-1.1/checksum.c` & `checksum16-1.1.1/checksum.c`

 * *Files identical despite different names*

### Comparing `checksum16-1.1/setup.py` & `checksum16-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     checksum_module = Extension('checksum', 
             sources = ['checksum.c'],
             extra_compile_args=['-Wall', '-Wextra',
                 '-Wno-missing-field-initializers', '-Werror'],
             extra_link_args=['-Wl,--build-id=none', '-s'])
 
     setup(name='checksum16',
-            version='1.1',
+            version='1.1.1',
             description='Native checksum implementation for python',
             author='Efi Weiss',
             author_email='valmarelox@gmail.com',
             url='https://github.com/Valmarelox/checksum',
             python_requires='>=3',
             ext_modules = [checksum_module],
             long_description=long_description,
```

