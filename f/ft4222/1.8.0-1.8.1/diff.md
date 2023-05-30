# Comparing `tmp/ft4222-1.8.0.tar.gz` & `tmp/ft4222-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/msrelectronics/python-ft4222/dist/.tmp-p7bu3a1_/ft4222-1.8.0.tar", last modified: Wed Feb  1 08:05:52 2023, max compression
+gzip compressed data, was "/builds/msrelectronics/python-ft4222/dist/.tmp-iwfe9xj0/ft4222-1.8.1.tar", last modified: Tue May 30 08:11:30 2023, max compression
```

## Comparing `ft4222-1.8.0.tar` & `ft4222-1.8.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-02-01 08:05:38.000000 ft4222-1.8.0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-02-01 08:05:38.000000 ft4222-1.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4225 2023-02-01 08:05:52.000000 ft4222-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3264 2023-02-01 08:05:38.000000 ft4222-1.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/GPIO/
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/GPIO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/GPIO/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/I2CMaster/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/I2CMaster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/I2CMaster/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/SPI/
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPI/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPI/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/SPIMaster/
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPIMaster/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPIMaster/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/SPISlave/
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPISlave/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/SPISlave/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2856 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/cftd2xx.pxd
--rw-rw-rw-   0 root         (0) root         (0)     8561 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/clibft4222.pxd
--rw-r--r--   0 root         (0) root         (0)   967064 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222/ft4222.c
--rw-rw-rw-   0 root         (0) root         (0)     4422 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/ft4222.pyi
--rw-rw-rw-   0 root         (0) root         (0)    32411 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/ft4222.pyx
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-01 08:05:38.000000 ft4222-1.8.0/ft4222/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4225 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1342 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-02-01 08:05:52.000000 ft4222-1.8.0/ft4222.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/
--rwxrwxrwx   0 root         (0) root         (0)     5321 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/WinTypes.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/build-arm-v6-hf/
--rwxrwxrwx   0 root         (0) root         (0)   531536 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v6-hf/libft4222.so
--rwxrwxrwx   0 root         (0) root         (0)   531536 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v6-hf/libft4222.so.1.4.4.170
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/build-arm-v7-hf/
--rwxrwxrwx   0 root         (0) root         (0)   422768 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v7-hf/libft4222.so
--rwxrwxrwx   0 root         (0) root         (0)   422768 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v7-hf/libft4222.so.1.4.4.170
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/build-arm-v8/
--rwxrwxrwx   0 root         (0) root         (0)   548720 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v8/libft4222.so
--rwxrwxrwx   0 root         (0) root         (0)   548720 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-arm-v8/libft4222.so.1.4.4.170
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/build-i386/
--rwxrwxrwx   0 root         (0) root         (0)   456473 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-i386/libft4222.so
--rwxrwxrwx   0 root         (0) root         (0)   456473 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-i386/libft4222.so.1.4.4.44
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/linux/build-x86_64/
--rwxrwxrwx   0 root         (0) root         (0)   561736 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-x86_64/libft4222.so
--rwxrwxrwx   0 root         (0) root         (0)   561736 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/build-x86_64/libft4222.so.1.4.4.170
--rwxrwxrwx   0 root         (0) root         (0)   144504 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/ftd2xx.h
--rwxrwxrwx   0 root         (0) root         (0)    13864 2023-02-01 08:05:38.000000 ft4222-1.8.0/linux/libft4222.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/osx/
--rwxrwxrwx   0 root         (0) root         (0)     5321 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/WinTypes.h
--rwxrwxrwx   0 root         (0) root         (0)   144504 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/ftd2xx.h
--rwxrwxrwx   0 root         (0) root         (0)  1096720 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/libft4222.1.4.4.170.dylib
--rwxrwxrwx   0 root         (0) root         (0)  1096720 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/libft4222.dylib
--rw-rw-rw-   0 root         (0) root         (0)    13864 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/libft4222.h
--rwxrwxrwx   0 root         (0) root         (0)  1051440 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/libftd2xx.dylib
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-02-01 08:05:38.000000 ft4222-1.8.0/osx/readme.md
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-02-01 08:05:38.000000 ft4222-1.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-01 08:05:52.000000 ft4222-1.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4308 2023-02-01 08:05:38.000000 ft4222-1.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/win/
--rw-rw-rw-   0 root         (0) root         (0)    14155 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/LibFT4222.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/win/amd64/
--rw-rw-rw-   0 root         (0) root         (0)   278392 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/amd64/LibFT4222-64.dll
--rw-rw-rw-   0 root         (0) root         (0)    14238 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/amd64/LibFT4222-64.lib
--rw-rw-rw-   0 root         (0) root         (0)   647616 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/amd64/ftd2xx.dll
--rw-rw-rw-   0 root         (0) root         (0)    20260 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/amd64/ftd2xx.lib
--rw-rw-rw-   0 root         (0) root         (0)    51546 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/ftd2xx.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-01 08:05:52.000000 ft4222-1.8.0/win/i386/
--rw-rw-rw-   0 root         (0) root         (0)   231800 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/i386/LibFT4222.dll
--rw-rw-rw-   0 root         (0) root         (0)    14220 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/i386/LibFT4222.lib
--rw-rw-rw-   0 root         (0) root         (0)   392128 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/i386/ftd2xx.dll
--rw-rw-rw-   0 root         (0) root         (0)    22190 2023-02-01 08:05:38.000000 ft4222-1.8.0/win/i386/ftd2xx.lib
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-05-30 08:11:21.000000 ft4222-1.8.1/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-05-30 08:11:21.000000 ft4222-1.8.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-05-30 08:11:30.000000 ft4222-1.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3264 2023-05-30 08:11:21.000000 ft4222-1.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/GPIO/
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/GPIO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/GPIO/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/I2CMaster/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/I2CMaster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/I2CMaster/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/SPI/
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPI/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPI/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/SPIMaster/
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPIMaster/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPIMaster/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/SPISlave/
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPISlave/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/SPISlave/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/cftd2xx.pxd
+-rw-rw-rw-   0 root         (0) root         (0)     8561 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/clibft4222.pxd
+-rw-r--r--   0 root         (0) root         (0)   970975 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222/ft4222.c
+-rw-rw-rw-   0 root         (0) root         (0)     4422 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/ft4222.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    32642 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/ft4222.pyx
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:11:21.000000 ft4222-1.8.1/ft4222/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4225 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-30 08:11:30.000000 ft4222-1.8.1/ft4222.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/
+-rwxrwxrwx   0 root         (0) root         (0)     5321 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/WinTypes.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/build-arm-v6-hf/
+-rwxrwxrwx   0 root         (0) root         (0)   531536 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v6-hf/libft4222.so
+-rwxrwxrwx   0 root         (0) root         (0)   531536 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v6-hf/libft4222.so.1.4.4.170
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/build-arm-v7-hf/
+-rwxrwxrwx   0 root         (0) root         (0)   422768 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v7-hf/libft4222.so
+-rwxrwxrwx   0 root         (0) root         (0)   422768 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v7-hf/libft4222.so.1.4.4.170
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/build-arm-v8/
+-rwxrwxrwx   0 root         (0) root         (0)   548720 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v8/libft4222.so
+-rwxrwxrwx   0 root         (0) root         (0)   548720 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-arm-v8/libft4222.so.1.4.4.170
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/build-i386/
+-rwxrwxrwx   0 root         (0) root         (0)   456473 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-i386/libft4222.so
+-rwxrwxrwx   0 root         (0) root         (0)   456473 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-i386/libft4222.so.1.4.4.44
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/linux/build-x86_64/
+-rwxrwxrwx   0 root         (0) root         (0)   561736 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-x86_64/libft4222.so
+-rwxrwxrwx   0 root         (0) root         (0)   561736 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/build-x86_64/libft4222.so.1.4.4.170
+-rwxrwxrwx   0 root         (0) root         (0)   144504 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/ftd2xx.h
+-rwxrwxrwx   0 root         (0) root         (0)    13864 2023-05-30 08:11:21.000000 ft4222-1.8.1/linux/libft4222.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/osx/
+-rwxrwxrwx   0 root         (0) root         (0)     5321 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/WinTypes.h
+-rwxrwxrwx   0 root         (0) root         (0)   144504 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/ftd2xx.h
+-rwxrwxrwx   0 root         (0) root         (0)  1096720 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/libft4222.1.4.4.170.dylib
+-rwxrwxrwx   0 root         (0) root         (0)  1096720 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/libft4222.dylib
+-rw-rw-rw-   0 root         (0) root         (0)    13864 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/libft4222.h
+-rwxrwxrwx   0 root         (0) root         (0)  1051440 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/libftd2xx.dylib
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-05-30 08:11:21.000000 ft4222-1.8.1/osx/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-30 08:11:21.000000 ft4222-1.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 08:11:30.000000 ft4222-1.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4308 2023-05-30 08:11:21.000000 ft4222-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/win/
+-rw-rw-rw-   0 root         (0) root         (0)    14155 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/LibFT4222.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/win/amd64/
+-rw-rw-rw-   0 root         (0) root         (0)   278392 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/amd64/LibFT4222-64.dll
+-rw-rw-rw-   0 root         (0) root         (0)    14238 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/amd64/LibFT4222-64.lib
+-rw-rw-rw-   0 root         (0) root         (0)   647616 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/amd64/ftd2xx.dll
+-rw-rw-rw-   0 root         (0) root         (0)    20260 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/amd64/ftd2xx.lib
+-rw-rw-rw-   0 root         (0) root         (0)    51546 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/ftd2xx.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:11:30.000000 ft4222-1.8.1/win/i386/
+-rw-rw-rw-   0 root         (0) root         (0)   231800 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/i386/LibFT4222.dll
+-rw-rw-rw-   0 root         (0) root         (0)    14220 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/i386/LibFT4222.lib
+-rw-rw-rw-   0 root         (0) root         (0)   392128 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/i386/ftd2xx.dll
+-rw-rw-rw-   0 root         (0) root         (0)    22190 2023-05-30 08:11:21.000000 ft4222-1.8.1/win/i386/ftd2xx.lib
```

### Comparing `ft4222-1.8.0/LICENSE.txt` & `ft4222-1.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/PKG-INFO` & `ft4222-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft4222
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python wrapper around libFT4222.
 Home-page: https://gitlab.com/msrelectronics/python-ft4222
 Author: Bearsh
 Author-email: me@bearsh.org
 License: MIT
 Keywords: ftdi ft4222
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ft4222-1.8.0/README.md` & `ft4222-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/GPIO/__init__.py` & `ft4222-1.8.1/ft4222/GPIO/__init__.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/I2CMaster/__init__.py` & `ft4222-1.8.1/ft4222/I2CMaster/__init__.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/SPI/__init__.py` & `ft4222-1.8.1/ft4222/SPI/__init__.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/SPIMaster/__init__.py` & `ft4222-1.8.1/ft4222/SPIMaster/__init__.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/SPISlave/__init__.py` & `ft4222-1.8.1/ft4222/SPISlave/__init__.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/__init__.py` & `ft4222-1.8.1/ft4222/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from .ft4222 import *
 from .GPIO import *
 from .I2CMaster import *
 from .SPI import *
 from .SPIMaster import *
 from .SPISlave import *
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 __all__ = [
     'FT2XXDeviceError',
     'FT4222DeviceError',
     'SysClock',
     'createDeviceInfoList',
     'getDeviceInfoDetail',
```

### Comparing `ft4222-1.8.0/ft4222/cftd2xx.pxd` & `ft4222-1.8.1/ft4222/cftd2xx.pxd`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/clibft4222.pxd` & `ft4222-1.8.1/ft4222/clibft4222.pxd`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/ft4222.c` & `ft4222-1.8.1/ft4222/ft4222.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "linux/ftd2xx.h",
             "linux/libft4222.h"
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,16 +102,20 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
@@ -227,15 +231,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +270,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1030,29 +1034,29 @@
 #ifndef _ARRAYARRAY_H
 struct arrayobject;
 typedef struct arrayobject arrayobject;
 #endif
 struct __pyx_obj_6ft4222_6ft4222__closer;
 struct __pyx_obj_6ft4222_6ft4222_FT4222;
 
-/* "ft4222/ft4222.pyx":169
+/* "ft4222/ft4222.pyx":182
  * 
  * 
  * cdef class _closer:             # <<<<<<<<<<<<<<
  *     """Wrap a hid_device *ptr and a provide a way to call hid_close() on it.
  *     Used internally for weakref.finalize, which only accepts Python objects.
  */
 struct __pyx_obj_6ft4222_6ft4222__closer {
   PyObject_HEAD
   struct __pyx_vtabstruct_6ft4222_6ft4222__closer *__pyx_vtab;
   FT_HANDLE _handle;
 };
 
 
-/* "ft4222/ft4222.pyx":187
+/* "ft4222/ft4222.pyx":200
  * 
  * 
  * cdef class FT4222:             # <<<<<<<<<<<<<<
  *     cdef FT_HANDLE _handle
  *     cdef DWORD _chip_version
  */
 struct __pyx_obj_6ft4222_6ft4222_FT4222 {
@@ -1063,29 +1067,29 @@
   DWORD _dll_version;
   PyObject *__weakref__;
   PyObject *_close;
 };
 
 
 
-/* "ft4222/ft4222.pyx":169
+/* "ft4222/ft4222.pyx":182
  * 
  * 
  * cdef class _closer:             # <<<<<<<<<<<<<<
  *     """Wrap a hid_device *ptr and a provide a way to call hid_close() on it.
  *     Used internally for weakref.finalize, which only accepts Python objects.
  */
 
 struct __pyx_vtabstruct_6ft4222_6ft4222__closer {
   PyObject *(*wrap)(FT_HANDLE);
 };
 static struct __pyx_vtabstruct_6ft4222_6ft4222__closer *__pyx_vtabptr_6ft4222_6ft4222__closer;
 
 
-/* "ft4222/ft4222.pyx":187
+/* "ft4222/ft4222.pyx":200
  * 
  * 
  * cdef class FT4222:             # <<<<<<<<<<<<<<
  *     cdef FT_HANDLE _handle
  *     cdef DWORD _chip_version
  */
 
@@ -1473,22 +1477,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
+#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_35 {
+   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -3186,21 +3198,21 @@
   return __pyx_r;
 }
 
 /* "ft4222/ft4222.pyx":117
  *     raise FT2XXDeviceError, status
  * 
  * def openBySerial(serial):             # <<<<<<<<<<<<<<
- *     """Open a handle to a usb device by serial number"""
- *     cdef FT_HANDLE handle
+ *     """Open a handle to a usb device by serial number
+ * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_6ft4222_6ft4222_5openBySerial(PyObject *__pyx_self, PyObject *__pyx_v_serial); /*proto*/
-static char __pyx_doc_6ft4222_6ft4222_4openBySerial[] = "Open a handle to a usb device by serial number";
+static char __pyx_doc_6ft4222_6ft4222_4openBySerial[] = "Open a handle to a usb device by serial number\n\n    Args:\n        serial (bytes, str): Serial number\n\n    Returns:\n        :obj:`FT4222`: Opened device\n\n    Raises:\n        FT2XXDeviceError: on error\n\n    ";
 static PyMethodDef __pyx_mdef_6ft4222_6ft4222_5openBySerial = {"openBySerial", (PyCFunction)__pyx_pw_6ft4222_6ft4222_5openBySerial, METH_O, __pyx_doc_6ft4222_6ft4222_4openBySerial};
 static PyObject *__pyx_pw_6ft4222_6ft4222_5openBySerial(PyObject *__pyx_self, PyObject *__pyx_v_serial) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("openBySerial (wrapper)", 0);
   __pyx_r = __pyx_pf_6ft4222_6ft4222_4openBySerial(__pyx_self, ((PyObject *)__pyx_v_serial));
 
@@ -3211,126 +3223,176 @@
 
 static PyObject *__pyx_pf_6ft4222_6ft4222_4openBySerial(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_serial) {
   FT_HANDLE __pyx_v_handle;
   char *__pyx_v_cserial;
   FT_STATUS __pyx_v_status;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  char *__pyx_t_1;
+  int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
+  char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("openBySerial", 0);
+  __Pyx_INCREF(__pyx_v_serial);
+
+  /* "ft4222/ft4222.pyx":130
+ * 
+ *     """
+ *     if isinstance(serial, str):             # <<<<<<<<<<<<<<
+ *         serial = serial.encode('utf-8')
+ *     cdef FT_HANDLE handle
+ */
+  __pyx_t_1 = PyUnicode_Check(__pyx_v_serial); 
+  __pyx_t_2 = (__pyx_t_1 != 0);
+  if (__pyx_t_2) {
 
-  /* "ft4222/ft4222.pyx":120
- *     """Open a handle to a usb device by serial number"""
+    /* "ft4222/ft4222.pyx":131
+ *     """
+ *     if isinstance(serial, str):
+ *         serial = serial.encode('utf-8')             # <<<<<<<<<<<<<<
+ *     cdef FT_HANDLE handle
+ *     cdef char* cserial = serial
+ */
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_serial, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_4, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF_SET(__pyx_v_serial, __pyx_t_3);
+    __pyx_t_3 = 0;
+
+    /* "ft4222/ft4222.pyx":130
+ * 
+ *     """
+ *     if isinstance(serial, str):             # <<<<<<<<<<<<<<
+ *         serial = serial.encode('utf-8')
+ *     cdef FT_HANDLE handle
+ */
+  }
+
+  /* "ft4222/ft4222.pyx":133
+ *         serial = serial.encode('utf-8')
  *     cdef FT_HANDLE handle
  *     cdef char* cserial = serial             # <<<<<<<<<<<<<<
  *     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)
  *     if status == FT_OK:
  */
-  __pyx_t_1 = __Pyx_PyObject_AsWritableString(__pyx_v_serial); if (unlikely((!__pyx_t_1) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
-  __pyx_v_cserial = __pyx_t_1;
+  __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_serial); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L1_error)
+  __pyx_v_cserial = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":121
+  /* "ft4222/ft4222.pyx":134
  *     cdef FT_HANDLE handle
  *     cdef char* cserial = serial
  *     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)             # <<<<<<<<<<<<<<
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)
  */
   __pyx_v_status = FT_OpenEx(((PVOID)__pyx_v_cserial), FT_OPEN_BY_SERIAL_NUMBER, (&__pyx_v_handle));
 
-  /* "ft4222/ft4222.pyx":122
+  /* "ft4222/ft4222.pyx":135
  *     cdef char* cserial = serial
  *     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status
  */
   __pyx_t_2 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":123
+    /* "ft4222/ft4222.pyx":136
  *     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)             # <<<<<<<<<<<<<<
  *     raise FT2XXDeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 123, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 136, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":122
+    /* "ft4222/ft4222.pyx":135
  *     cdef char* cserial = serial
  *     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":124
+  /* "ft4222/ft4222.pyx":137
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  * def openByDescription(desc):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 124, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_5, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 124, __pyx_L1_error)
+  __PYX_ERR(0, 137, __pyx_L1_error)
 
   /* "ft4222/ft4222.pyx":117
  *     raise FT2XXDeviceError, status
  * 
  * def openBySerial(serial):             # <<<<<<<<<<<<<<
- *     """Open a handle to a usb device by serial number"""
- *     cdef FT_HANDLE handle
+ *     """Open a handle to a usb device by serial number
+ * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_AddTraceback("ft4222.ft4222.openBySerial", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_serial);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":126
+/* "ft4222/ft4222.pyx":139
  *     raise FT2XXDeviceError, status
  * 
  * def openByDescription(desc):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by description
  * 
  */
 
@@ -3363,142 +3425,142 @@
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("openByDescription", 0);
   __Pyx_INCREF(__pyx_v_desc);
 
-  /* "ft4222/ft4222.pyx":139
+  /* "ft4222/ft4222.pyx":152
  * 
  *     """
  *     if isinstance(desc, str):             # <<<<<<<<<<<<<<
  *         desc = desc.encode('utf-8')
  *     cdef FT_HANDLE handle
  */
   __pyx_t_1 = PyUnicode_Check(__pyx_v_desc); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":140
+    /* "ft4222/ft4222.pyx":153
  *     """
  *     if isinstance(desc, str):
  *         desc = desc.encode('utf-8')             # <<<<<<<<<<<<<<
  *     cdef FT_HANDLE handle
  *     cdef char* cdesc = desc
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_desc, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_desc, __pyx_n_s_encode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_utf_8);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 140, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_desc, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "ft4222/ft4222.pyx":139
+    /* "ft4222/ft4222.pyx":152
  * 
  *     """
  *     if isinstance(desc, str):             # <<<<<<<<<<<<<<
  *         desc = desc.encode('utf-8')
  *     cdef FT_HANDLE handle
  */
   }
 
-  /* "ft4222/ft4222.pyx":142
+  /* "ft4222/ft4222.pyx":155
  *         desc = desc.encode('utf-8')
  *     cdef FT_HANDLE handle
  *     cdef char* cdesc = desc             # <<<<<<<<<<<<<<
  *     status = FT_OpenEx(<PVOID>cdesc, FT_OPEN_BY_DESCRIPTION, &handle)
  *     if status == FT_OK:
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_desc); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableString(__pyx_v_desc); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 155, __pyx_L1_error)
   __pyx_v_cdesc = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":143
+  /* "ft4222/ft4222.pyx":156
  *     cdef FT_HANDLE handle
  *     cdef char* cdesc = desc
  *     status = FT_OpenEx(<PVOID>cdesc, FT_OPEN_BY_DESCRIPTION, &handle)             # <<<<<<<<<<<<<<
  *     if status == FT_OK:
  *         #printf("handle: %d\n", handle)
  */
   __pyx_v_status = FT_OpenEx(((PVOID)__pyx_v_cdesc), FT_OPEN_BY_DESCRIPTION, (&__pyx_v_handle));
 
-  /* "ft4222/ft4222.pyx":144
+  /* "ft4222/ft4222.pyx":157
  *     cdef char* cdesc = desc
  *     status = FT_OpenEx(<PVOID>cdesc, FT_OPEN_BY_DESCRIPTION, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         #printf("handle: %d\n", handle)
  *         return FT4222(<uintptr_t>handle, update=False)
  */
   __pyx_t_2 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":146
+    /* "ft4222/ft4222.pyx":159
  *     if status == FT_OK:
  *         #printf("handle: %d\n", handle)
  *         return FT4222(<uintptr_t>handle, update=False)             # <<<<<<<<<<<<<<
  *     raise FT2XXDeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 146, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 146, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":144
+    /* "ft4222/ft4222.pyx":157
  *     cdef char* cdesc = desc
  *     status = FT_OpenEx(<PVOID>cdesc, FT_OPEN_BY_DESCRIPTION, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         #printf("handle: %d\n", handle)
  *         return FT4222(<uintptr_t>handle, update=False)
  */
   }
 
-  /* "ft4222/ft4222.pyx":147
+  /* "ft4222/ft4222.pyx":160
  *         #printf("handle: %d\n", handle)
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  * def openByLocation(locId):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_5, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 147, __pyx_L1_error)
+  __PYX_ERR(0, 160, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":126
+  /* "ft4222/ft4222.pyx":139
  *     raise FT2XXDeviceError, status
  * 
  * def openByDescription(desc):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by description
  * 
  */
 
@@ -3512,15 +3574,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_desc);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":149
+/* "ft4222/ft4222.pyx":162
  *     raise FT2XXDeviceError, status
  * 
  * def openByLocation(locId):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by location
  * 
  */
 
@@ -3550,86 +3612,86 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("openByLocation", 0);
 
-  /* "ft4222/ft4222.pyx":163
+  /* "ft4222/ft4222.pyx":176
  *     """
  *     cdef FT_HANDLE handle
  *     status = FT_OpenEx(<PVOID><uintptr_t>locId, FT_OPEN_BY_LOCATION, &handle)             # <<<<<<<<<<<<<<
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)
  */
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_locId); if (unlikely((__pyx_t_1 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_locId); if (unlikely((__pyx_t_1 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
   __pyx_v_status = FT_OpenEx(((PVOID)((uintptr_t)__pyx_t_1)), FT_OPEN_BY_LOCATION, (&__pyx_v_handle));
 
-  /* "ft4222/ft4222.pyx":164
+  /* "ft4222/ft4222.pyx":177
  *     cdef FT_HANDLE handle
  *     status = FT_OpenEx(<PVOID><uintptr_t>locId, FT_OPEN_BY_LOCATION, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status
  */
   __pyx_t_2 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":165
+    /* "ft4222/ft4222.pyx":178
  *     status = FT_OpenEx(<PVOID><uintptr_t>locId, FT_OPEN_BY_LOCATION, &handle)
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)             # <<<<<<<<<<<<<<
  *     raise FT2XXDeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_FromSize_t(((uintptr_t)__pyx_v_handle)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 165, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 165, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_update, Py_False) < 0) __PYX_ERR(0, 178, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_6ft4222_6ft4222_FT4222), __pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 178, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_5;
     __pyx_t_5 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":164
+    /* "ft4222/ft4222.pyx":177
  *     cdef FT_HANDLE handle
  *     status = FT_OpenEx(<PVOID><uintptr_t>locId, FT_OPEN_BY_LOCATION, &handle)
  *     if status == FT_OK:             # <<<<<<<<<<<<<<
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":166
+  /* "ft4222/ft4222.pyx":179
  *     if status == FT_OK:
  *         return FT4222(<uintptr_t>handle, update=False)
  *     raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_5, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 166, __pyx_L1_error)
+  __PYX_ERR(0, 179, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":149
+  /* "ft4222/ft4222.pyx":162
  *     raise FT2XXDeviceError, status
  * 
  * def openByLocation(locId):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by location
  * 
  */
 
@@ -3642,15 +3704,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":177
+/* "ft4222/ft4222.pyx":190
  * 
  *     @staticmethod
  *     cdef wrap(FT_HANDLE h):             # <<<<<<<<<<<<<<
  *         cdef _closer closer = _closer()
  *         closer._handle = h
  */
 
@@ -3660,48 +3722,48 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap", 0);
 
-  /* "ft4222/ft4222.pyx":178
+  /* "ft4222/ft4222.pyx":191
  *     @staticmethod
  *     cdef wrap(FT_HANDLE h):
  *         cdef _closer closer = _closer()             # <<<<<<<<<<<<<<
  *         closer._handle = h
  *         return closer
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6ft4222_6ft4222__closer)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_6ft4222_6ft4222__closer)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_closer = ((struct __pyx_obj_6ft4222_6ft4222__closer *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":179
+  /* "ft4222/ft4222.pyx":192
  *     cdef wrap(FT_HANDLE h):
  *         cdef _closer closer = _closer()
  *         closer._handle = h             # <<<<<<<<<<<<<<
  *         return closer
  * 
  */
   __pyx_v_closer->_handle = __pyx_v_h;
 
-  /* "ft4222/ft4222.pyx":180
+  /* "ft4222/ft4222.pyx":193
  *         cdef _closer closer = _closer()
  *         closer._handle = h
  *         return closer             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_closer));
   __pyx_r = ((PyObject *)__pyx_v_closer);
   goto __pyx_L0;
 
-  /* "ft4222/ft4222.pyx":177
+  /* "ft4222/ft4222.pyx":190
  * 
  *     @staticmethod
  *     cdef wrap(FT_HANDLE h):             # <<<<<<<<<<<<<<
  *         cdef _closer closer = _closer()
  *         closer._handle = h
  */
 
@@ -3713,15 +3775,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_closer);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":182
+/* "ft4222/ft4222.pyx":195
  *         return closer
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         FT4222_UnInitialize(self._handle)
  *         FT_Close(self._handle)
  */
 
@@ -3739,33 +3801,33 @@
 }
 
 static PyObject *__pyx_pf_6ft4222_6ft4222_7_closer_close(struct __pyx_obj_6ft4222_6ft4222__closer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "ft4222/ft4222.pyx":183
+  /* "ft4222/ft4222.pyx":196
  * 
  *     def close(self):
  *         FT4222_UnInitialize(self._handle)             # <<<<<<<<<<<<<<
  *         FT_Close(self._handle)
  * 
  */
   (void)(FT4222_UnInitialize(__pyx_v_self->_handle));
 
-  /* "ft4222/ft4222.pyx":184
+  /* "ft4222/ft4222.pyx":197
  *     def close(self):
  *         FT4222_UnInitialize(self._handle)
  *         FT_Close(self._handle)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   (void)(FT_Close(__pyx_v_self->_handle));
 
-  /* "ft4222/ft4222.pyx":182
+  /* "ft4222/ft4222.pyx":195
  *         return closer
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         FT4222_UnInitialize(self._handle)
  *         FT_Close(self._handle)
  */
 
@@ -3885,15 +3947,15 @@
   __Pyx_AddTraceback("ft4222.ft4222._closer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":194
+/* "ft4222/ft4222.pyx":207
  *     cdef object _close
  * 
  *     def __init__(self, handle, update=True):             # <<<<<<<<<<<<<<
  *         self._handle = <FT_HANDLE><uintptr_t>handle
  *         self._chip_version = 0
  */
 
@@ -3932,15 +3994,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_update);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 194, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 207, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -3948,15 +4010,15 @@
       }
     }
     __pyx_v_handle = values[0];
     __pyx_v_update = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 194, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 207, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222___init__(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_handle, __pyx_v_update);
 
@@ -3976,65 +4038,65 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "ft4222/ft4222.pyx":195
+  /* "ft4222/ft4222.pyx":208
  * 
  *     def __init__(self, handle, update=True):
  *         self._handle = <FT_HANDLE><uintptr_t>handle             # <<<<<<<<<<<<<<
  *         self._chip_version = 0
  *         self._dll_version = 0
  */
-  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_handle); if (unlikely((__pyx_t_1 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_size_t(__pyx_v_handle); if (unlikely((__pyx_t_1 == ((uintptr_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
   __pyx_v_self->_handle = ((FT_HANDLE)((uintptr_t)__pyx_t_1));
 
-  /* "ft4222/ft4222.pyx":196
+  /* "ft4222/ft4222.pyx":209
  *     def __init__(self, handle, update=True):
  *         self._handle = <FT_HANDLE><uintptr_t>handle
  *         self._chip_version = 0             # <<<<<<<<<<<<<<
  *         self._dll_version = 0
  *         self._get_version()
  */
   __pyx_v_self->_chip_version = 0;
 
-  /* "ft4222/ft4222.pyx":197
+  /* "ft4222/ft4222.pyx":210
  *         self._handle = <FT_HANDLE><uintptr_t>handle
  *         self._chip_version = 0
  *         self._dll_version = 0             # <<<<<<<<<<<<<<
  *         self._get_version()
  *         self._close = weakref_finalize(self, _closer.wrap(self._handle).close)
  */
   __pyx_v_self->_dll_version = 0;
 
-  /* "ft4222/ft4222.pyx":198
+  /* "ft4222/ft4222.pyx":211
  *         self._chip_version = 0
  *         self._dll_version = 0
  *         self._get_version()             # <<<<<<<<<<<<<<
  *         self._close = weakref_finalize(self, _closer.wrap(self._handle).close)
  * 
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_6ft4222_6ft4222_FT4222 *)__pyx_v_self->__pyx_vtab)->_get_version(__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_6ft4222_6ft4222_FT4222 *)__pyx_v_self->__pyx_vtab)->_get_version(__pyx_v_self); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "ft4222/ft4222.pyx":199
+  /* "ft4222/ft4222.pyx":212
  *         self._dll_version = 0
  *         self._get_version()
  *         self._close = weakref_finalize(self, _closer.wrap(self._handle).close)             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_weakref_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_weakref_finalize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __pyx_f_6ft4222_6ft4222_7_closer_wrap(__pyx_v_self->_handle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_4 = __pyx_f_6ft4222_6ft4222_7_closer_wrap(__pyx_v_self->_handle); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_close); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
@@ -4044,53 +4106,53 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, ((PyObject *)__pyx_v_self), __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, ((PyObject *)__pyx_v_self), __pyx_t_5};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, ((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_close);
   __Pyx_DECREF(__pyx_v_self->_close);
   __pyx_v_self->_close = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "ft4222/ft4222.pyx":194
+  /* "ft4222/ft4222.pyx":207
  *     cdef object _close
  * 
  *     def __init__(self, handle, update=True):             # <<<<<<<<<<<<<<
  *         self._handle = <FT_HANDLE><uintptr_t>handle
  *         self._chip_version = 0
  */
 
@@ -4106,15 +4168,15 @@
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":201
+/* "ft4222/ft4222.pyx":214
  *         self._close = weakref_finalize(self, _closer.wrap(self._handle).close)
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Closes the device."""
  *         FT4222_UnInitialize(self._handle)
  */
 
@@ -4140,77 +4202,77 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "ft4222/ft4222.pyx":203
+  /* "ft4222/ft4222.pyx":216
  *     def close(self):
  *         """Closes the device."""
  *         FT4222_UnInitialize(self._handle)             # <<<<<<<<<<<<<<
  *         status = FT_Close(self._handle)
  *         if status != FT4222_OK:
  */
   (void)(FT4222_UnInitialize(__pyx_v_self->_handle));
 
-  /* "ft4222/ft4222.pyx":204
+  /* "ft4222/ft4222.pyx":217
  *         """Closes the device."""
  *         FT4222_UnInitialize(self._handle)
  *         status = FT_Close(self._handle)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
   __pyx_v_status = FT_Close(__pyx_v_self->_handle);
 
-  /* "ft4222/ft4222.pyx":205
+  /* "ft4222/ft4222.pyx":218
  *         FT4222_UnInitialize(self._handle)
  *         status = FT_Close(self._handle)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  *         self._handle = NULL
  */
   __pyx_t_1 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":206
+    /* "ft4222/ft4222.pyx":219
  *         status = FT_Close(self._handle)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  *         self._handle = NULL
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 206, __pyx_L1_error)
+    __PYX_ERR(0, 219, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":205
+    /* "ft4222/ft4222.pyx":218
  *         FT4222_UnInitialize(self._handle)
  *         status = FT_Close(self._handle)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  *         self._handle = NULL
  */
   }
 
-  /* "ft4222/ft4222.pyx":207
+  /* "ft4222/ft4222.pyx":220
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  *         self._handle = NULL             # <<<<<<<<<<<<<<
  * 
  *     cdef _get_version(self):
  */
   __pyx_v_self->_handle = NULL;
 
-  /* "ft4222/ft4222.pyx":201
+  /* "ft4222/ft4222.pyx":214
  *         self._close = weakref_finalize(self, _closer.wrap(self._handle).close)
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         """Closes the device."""
  *         FT4222_UnInitialize(self._handle)
  */
 
@@ -4224,15 +4286,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":209
+/* "ft4222/ft4222.pyx":222
  *         self._handle = NULL
  * 
  *     cdef _get_version(self):             # <<<<<<<<<<<<<<
  *         cdef FT4222_Version ver
  *         status = FT4222_GetVersion(self._handle, &ver)
  */
 
@@ -4241,78 +4303,78 @@
   FT4222_STATUS __pyx_v_status;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   DWORD __pyx_t_2;
   __Pyx_RefNannySetupContext("_get_version", 0);
 
-  /* "ft4222/ft4222.pyx":211
+  /* "ft4222/ft4222.pyx":224
  *     cdef _get_version(self):
  *         cdef FT4222_Version ver
  *         status = FT4222_GetVersion(self._handle, &ver)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             self._chip_version = ver.chipVersion
  */
   __pyx_v_status = FT4222_GetVersion(__pyx_v_self->_handle, (&__pyx_v_ver));
 
-  /* "ft4222/ft4222.pyx":212
+  /* "ft4222/ft4222.pyx":225
  *         cdef FT4222_Version ver
  *         status = FT4222_GetVersion(self._handle, &ver)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             self._chip_version = ver.chipVersion
  *             self._dll_version = ver.dllVersion
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":213
+    /* "ft4222/ft4222.pyx":226
  *         status = FT4222_GetVersion(self._handle, &ver)
  *         if status == FT4222_OK:
  *             self._chip_version = ver.chipVersion             # <<<<<<<<<<<<<<
  *             self._dll_version = ver.dllVersion
  * 
  */
     __pyx_t_2 = __pyx_v_ver.chipVersion;
     __pyx_v_self->_chip_version = __pyx_t_2;
 
-    /* "ft4222/ft4222.pyx":214
+    /* "ft4222/ft4222.pyx":227
  *         if status == FT4222_OK:
  *             self._chip_version = ver.chipVersion
  *             self._dll_version = ver.dllVersion             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __pyx_t_2 = __pyx_v_ver.dllVersion;
     __pyx_v_self->_dll_version = __pyx_t_2;
 
-    /* "ft4222/ft4222.pyx":212
+    /* "ft4222/ft4222.pyx":225
  *         cdef FT4222_Version ver
  *         status = FT4222_GetVersion(self._handle, &ver)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             self._chip_version = ver.chipVersion
  *             self._dll_version = ver.dllVersion
  */
   }
 
-  /* "ft4222/ft4222.pyx":209
+  /* "ft4222/ft4222.pyx":222
  *         self._handle = NULL
  * 
  *     cdef _get_version(self):             # <<<<<<<<<<<<<<
  *         cdef FT4222_Version ver
  *         status = FT4222_GetVersion(self._handle, &ver)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":217
+/* "ft4222/ft4222.pyx":230
  * 
  *     @property
  *     def chipVersion(self) -> int:             # <<<<<<<<<<<<<<
  *         """Chip version as number"""
  *         return self._chip_version
  */
 
@@ -4334,29 +4396,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "ft4222/ft4222.pyx":219
+  /* "ft4222/ft4222.pyx":232
  *     def chipVersion(self) -> int:
  *         """Chip version as number"""
  *         return self._chip_version             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_chip_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_chip_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "ft4222/ft4222.pyx":217
+  /* "ft4222/ft4222.pyx":230
  * 
  *     @property
  *     def chipVersion(self) -> int:             # <<<<<<<<<<<<<<
  *         """Chip version as number"""
  *         return self._chip_version
  */
 
@@ -4367,15 +4429,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":222
+/* "ft4222/ft4222.pyx":235
  * 
  *     @property
  *     def libVersion(self) -> int:             # <<<<<<<<<<<<<<
  *         """Library version as number"""
  *         return self._dll_version
  */
 
@@ -4397,29 +4459,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "ft4222/ft4222.pyx":224
+  /* "ft4222/ft4222.pyx":237
  *     def libVersion(self) -> int:
  *         """Library version as number"""
  *         return self._dll_version             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_dll_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_dll_version); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "ft4222/ft4222.pyx":222
+  /* "ft4222/ft4222.pyx":235
  * 
  *     @property
  *     def libVersion(self) -> int:             # <<<<<<<<<<<<<<
  *         """Library version as number"""
  *         return self._dll_version
  */
 
@@ -4430,15 +4492,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":227
+/* "ft4222/ft4222.pyx":240
  * 
  *     @property
  *     def chipRevision(self) -> str:             # <<<<<<<<<<<<<<
  *         """The revision of the chip in human readable format"""
  *         try:
  */
 
@@ -4466,15 +4528,15 @@
   int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "ft4222/ft4222.pyx":229
+  /* "ft4222/ft4222.pyx":242
  *     def chipRevision(self) -> str:
  *         """The revision of the chip in human readable format"""
  *         try:             # <<<<<<<<<<<<<<
  *             return __chip_rev_map[self._chip_version]
  *         except KeyError:
  */
   {
@@ -4482,59 +4544,59 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "ft4222/ft4222.pyx":230
+      /* "ft4222/ft4222.pyx":243
  *         """The revision of the chip in human readable format"""
  *         try:
  *             return __chip_rev_map[self._chip_version]             # <<<<<<<<<<<<<<
  *         except KeyError:
  *             return "Rev. unknown"
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_chip_rev_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_chip_rev_map); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 243, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, __pyx_v_self->_chip_version, DWORD, 0, __Pyx_PyInt_From_DWORD, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_4, __pyx_v_self->_chip_version, DWORD, 0, __Pyx_PyInt_From_DWORD, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 243, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_r = __pyx_t_5;
       __pyx_t_5 = 0;
       goto __pyx_L7_try_return;
 
-      /* "ft4222/ft4222.pyx":229
+      /* "ft4222/ft4222.pyx":242
  *     def chipRevision(self) -> str:
  *         """The revision of the chip in human readable format"""
  *         try:             # <<<<<<<<<<<<<<
  *             return __chip_rev_map[self._chip_version]
  *         except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-    /* "ft4222/ft4222.pyx":231
+    /* "ft4222/ft4222.pyx":244
  *         try:
  *             return __chip_rev_map[self._chip_version]
  *         except KeyError:             # <<<<<<<<<<<<<<
  *             return "Rev. unknown"
  * 
  */
     __pyx_t_6 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_6) {
       __Pyx_AddTraceback("ft4222.ft4222.FT4222.chipRevision.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 231, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_4, &__pyx_t_7) < 0) __PYX_ERR(0, 244, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "ft4222/ft4222.pyx":232
+      /* "ft4222/ft4222.pyx":245
  *             return __chip_rev_map[self._chip_version]
  *         except KeyError:
  *             return "Rev. unknown"             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -4544,15 +4606,15 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "ft4222/ft4222.pyx":229
+    /* "ft4222/ft4222.pyx":242
  *     def chipRevision(self) -> str:
  *         """The revision of the chip in human readable format"""
  *         try:             # <<<<<<<<<<<<<<
  *             return __chip_rev_map[self._chip_version]
  *         except KeyError:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -4570,15 +4632,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "ft4222/ft4222.pyx":227
+  /* "ft4222/ft4222.pyx":240
  * 
  *     @property
  *     def chipRevision(self) -> str:             # <<<<<<<<<<<<<<
  *         """The revision of the chip in human readable format"""
  *         try:
  */
 
@@ -4591,15 +4653,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":234
+/* "ft4222/ft4222.pyx":247
  *             return "Rev. unknown"
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "FT4222: chipVersion: 0x{:x} ({:s}), libVersion: 0x{:x}".format(self._chip_version, self.chipRevision, self._dll_version)
  * 
  */
 
@@ -4628,29 +4690,29 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "ft4222/ft4222.pyx":235
+  /* "ft4222/ft4222.pyx":248
  * 
  *     def __repr__(self):
  *         return "FT4222: chipVersion: 0x{:x} ({:s}), libVersion: 0x{:x}".format(self._chip_version, self.chipRevision, self._dll_version)             # <<<<<<<<<<<<<<
  * 
  *     def setTimeouts(self, read_timeout, write_timeout):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_FT4222_chipVersion_0x_x_s_libVer, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_FT4222_chipVersion_0x_x_s_libVer, __pyx_n_s_format); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_chip_version); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_chip_version); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_chipRevision); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_chipRevision); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_dll_version); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_DWORD(__pyx_v_self->_dll_version); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_6 = NULL;
   __pyx_t_7 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -4659,58 +4721,58 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_7 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_t_5};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_t_3, __pyx_t_4, __pyx_t_5};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     if (__pyx_t_6) {
       __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_t_5);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_8, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 248, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "ft4222/ft4222.pyx":234
+  /* "ft4222/ft4222.pyx":247
  *             return "Rev. unknown"
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "FT4222: chipVersion: 0x{:x} ({:s}), libVersion: 0x{:x}".format(self._chip_version, self.chipRevision, self._dll_version)
  * 
  */
 
@@ -4727,15 +4789,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":237
+/* "ft4222/ft4222.pyx":250
  *         return "FT4222: chipVersion: 0x{:x} ({:s}), libVersion: 0x{:x}".format(self._chip_version, self.chipRevision, self._dll_version)
  * 
  *     def setTimeouts(self, read_timeout, write_timeout):             # <<<<<<<<<<<<<<
  *         """Set the read and write timeouts
  * 
  */
 
@@ -4770,32 +4832,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_read_timeout)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_write_timeout)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("setTimeouts", 1, 2, 2, 1); __PYX_ERR(0, 237, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("setTimeouts", 1, 2, 2, 1); __PYX_ERR(0, 250, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "setTimeouts") < 0)) __PYX_ERR(0, 237, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "setTimeouts") < 0)) __PYX_ERR(0, 250, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_read_timeout = values[0];
     __pyx_v_write_timeout = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("setTimeouts", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 237, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("setTimeouts", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 250, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.setTimeouts", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_6setTimeouts(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_read_timeout, __pyx_v_write_timeout);
 
@@ -4814,61 +4876,61 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setTimeouts", 0);
 
-  /* "ft4222/ft4222.pyx":248
+  /* "ft4222/ft4222.pyx":261
  * 
  *         """
  *         status = FT_SetTimeouts(self._handle, read_timeout, write_timeout)             # <<<<<<<<<<<<<<
  *         if status != FT_OK:
  *             raise FT2XXDeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_ULONG(__pyx_v_read_timeout); if (unlikely((__pyx_t_1 == ((ULONG)-1)) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_ULONG(__pyx_v_write_timeout); if (unlikely((__pyx_t_2 == ((ULONG)-1)) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_ULONG(__pyx_v_read_timeout); if (unlikely((__pyx_t_1 == ((ULONG)-1)) && PyErr_Occurred())) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_ULONG(__pyx_v_write_timeout); if (unlikely((__pyx_t_2 == ((ULONG)-1)) && PyErr_Occurred())) __PYX_ERR(0, 261, __pyx_L1_error)
   __pyx_v_status = FT_SetTimeouts(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2);
 
-  /* "ft4222/ft4222.pyx":249
+  /* "ft4222/ft4222.pyx":262
  *         """
  *         status = FT_SetTimeouts(self._handle, read_timeout, write_timeout)
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT2XXDeviceError, status
  * 
  */
   __pyx_t_3 = ((__pyx_v_status != FT_OK) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "ft4222/ft4222.pyx":250
+    /* "ft4222/ft4222.pyx":263
  *         status = FT_SetTimeouts(self._handle, read_timeout, write_timeout)
  *         if status != FT_OK:
  *             raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def setClock(self, clk):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 250, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_4, __pyx_t_5, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 250, __pyx_L1_error)
+    __PYX_ERR(0, 263, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":249
+    /* "ft4222/ft4222.pyx":262
  *         """
  *         status = FT_SetTimeouts(self._handle, read_timeout, write_timeout)
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT2XXDeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":237
+  /* "ft4222/ft4222.pyx":250
  *         return "FT4222: chipVersion: 0x{:x} ({:s}), libVersion: 0x{:x}".format(self._chip_version, self.chipRevision, self._dll_version)
  * 
  *     def setTimeouts(self, read_timeout, write_timeout):             # <<<<<<<<<<<<<<
  *         """Set the read and write timeouts
  * 
  */
 
@@ -4882,15 +4944,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":252
+/* "ft4222/ft4222.pyx":265
  *             raise FT2XXDeviceError, status
  * 
  *     def setClock(self, clk):             # <<<<<<<<<<<<<<
  *         """Set the system clock
  * 
  */
 
@@ -4917,60 +4979,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setClock", 0);
 
-  /* "ft4222/ft4222.pyx":262
+  /* "ft4222/ft4222.pyx":275
  * 
  *         """
  *         status = FT4222_SetClock(self._handle, clk)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((FT4222_ClockRate)__Pyx_PyInt_As_FT4222_ClockRate(__pyx_v_clk)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 262, __pyx_L1_error)
+  __pyx_t_1 = ((FT4222_ClockRate)__Pyx_PyInt_As_FT4222_ClockRate(__pyx_v_clk)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 275, __pyx_L1_error)
   __pyx_v_status = FT4222_SetClock(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":263
+  /* "ft4222/ft4222.pyx":276
  *         """
  *         status = FT4222_SetClock(self._handle, clk)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":264
+    /* "ft4222/ft4222.pyx":277
  *         status = FT4222_SetClock(self._handle, clk)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def getClock(self):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 264, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 277, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 264, __pyx_L1_error)
+    __PYX_ERR(0, 277, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":263
+    /* "ft4222/ft4222.pyx":276
  *         """
  *         status = FT4222_SetClock(self._handle, clk)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":252
+  /* "ft4222/ft4222.pyx":265
  *             raise FT2XXDeviceError, status
  * 
  *     def setClock(self, clk):             # <<<<<<<<<<<<<<
  *         """Set the system clock
  * 
  */
 
@@ -4984,15 +5046,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":266
+/* "ft4222/ft4222.pyx":279
  *             raise FT4222DeviceError, status
  * 
  *     def getClock(self):             # <<<<<<<<<<<<<<
  *         """Get the system clock
  * 
  */
 
@@ -5021,91 +5083,91 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getClock", 0);
 
-  /* "ft4222/ft4222.pyx":277
+  /* "ft4222/ft4222.pyx":290
  *         """
  *         cdef FT4222_ClockRate clk
  *         status = FT4222_GetClock(self._handle, &clk)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return SysClock(clk)
  */
   __pyx_v_status = FT4222_GetClock(__pyx_v_self->_handle, (&__pyx_v_clk));
 
-  /* "ft4222/ft4222.pyx":278
+  /* "ft4222/ft4222.pyx":291
  *         cdef FT4222_ClockRate clk
  *         status = FT4222_GetClock(self._handle, &clk)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return SysClock(clk)
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":279
+    /* "ft4222/ft4222.pyx":292
  *         status = FT4222_GetClock(self._handle, &clk)
  *         if status == FT4222_OK:
  *             return SysClock(clk)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SysClock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_SysClock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_ClockRate(__pyx_v_clk); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_ClockRate(__pyx_v_clk); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 279, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":278
+    /* "ft4222/ft4222.pyx":291
  *         cdef FT4222_ClockRate clk
  *         status = FT4222_GetClock(self._handle, &clk)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return SysClock(clk)
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":280
+  /* "ft4222/ft4222.pyx":293
  *         if status == FT4222_OK:
  *             return SysClock(clk)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def setSuspendOut(self, enable):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 280, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 280, __pyx_L1_error)
+  __PYX_ERR(0, 293, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":266
+  /* "ft4222/ft4222.pyx":279
  *             raise FT4222DeviceError, status
  * 
  *     def getClock(self):             # <<<<<<<<<<<<<<
  *         """Get the system clock
  * 
  */
 
@@ -5119,15 +5181,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":282
+/* "ft4222/ft4222.pyx":295
  *         raise FT4222DeviceError, status
  * 
  *     def setSuspendOut(self, enable):             # <<<<<<<<<<<<<<
  *         """Enable or disable, suspend out, which will emit a signal when FT4222H enters suspend mode.
  * 
  */
 
@@ -5154,60 +5216,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setSuspendOut", 0);
 
-  /* "ft4222/ft4222.pyx":292
+  /* "ft4222/ft4222.pyx":305
  * 
  *         """
  *         status = FT4222_SetSuspendOut(self._handle, enable)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_BOOL(__pyx_v_enable); if (unlikely((__pyx_t_1 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_BOOL(__pyx_v_enable); if (unlikely((__pyx_t_1 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 305, __pyx_L1_error)
   __pyx_v_status = FT4222_SetSuspendOut(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":293
+  /* "ft4222/ft4222.pyx":306
  *         """
  *         status = FT4222_SetSuspendOut(self._handle, enable)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":294
+    /* "ft4222/ft4222.pyx":307
  *         status = FT4222_SetSuspendOut(self._handle, enable)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def setWakeUpInterrupt(self, enable):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 294, __pyx_L1_error)
+    __PYX_ERR(0, 307, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":293
+    /* "ft4222/ft4222.pyx":306
  *         """
  *         status = FT4222_SetSuspendOut(self._handle, enable)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":282
+  /* "ft4222/ft4222.pyx":295
  *         raise FT4222DeviceError, status
  * 
  *     def setSuspendOut(self, enable):             # <<<<<<<<<<<<<<
  *         """Enable or disable, suspend out, which will emit a signal when FT4222H enters suspend mode.
  * 
  */
 
@@ -5221,15 +5283,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":296
+/* "ft4222/ft4222.pyx":309
  *             raise FT4222DeviceError, status
  * 
  *     def setWakeUpInterrupt(self, enable):             # <<<<<<<<<<<<<<
  *         """Enable or disable the wakeup/interrupt
  * 
  */
 
@@ -5256,60 +5318,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setWakeUpInterrupt", 0);
 
-  /* "ft4222/ft4222.pyx":306
+  /* "ft4222/ft4222.pyx":319
  * 
  *         """
  *         status = FT4222_SetWakeUpInterrupt(self._handle, enable)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_BOOL(__pyx_v_enable); if (unlikely((__pyx_t_1 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_BOOL(__pyx_v_enable); if (unlikely((__pyx_t_1 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 319, __pyx_L1_error)
   __pyx_v_status = FT4222_SetWakeUpInterrupt(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":307
+  /* "ft4222/ft4222.pyx":320
  *         """
  *         status = FT4222_SetWakeUpInterrupt(self._handle, enable)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":308
+    /* "ft4222/ft4222.pyx":321
  *         status = FT4222_SetWakeUpInterrupt(self._handle, enable)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def getMaxTransferSize(self):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 308, __pyx_L1_error)
+    __PYX_ERR(0, 321, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":307
+    /* "ft4222/ft4222.pyx":320
  *         """
  *         status = FT4222_SetWakeUpInterrupt(self._handle, enable)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":296
+  /* "ft4222/ft4222.pyx":309
  *             raise FT4222DeviceError, status
  * 
  *     def setWakeUpInterrupt(self, enable):             # <<<<<<<<<<<<<<
  *         """Enable or disable the wakeup/interrupt
  * 
  */
 
@@ -5323,15 +5385,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":310
+/* "ft4222/ft4222.pyx":323
  *             raise FT4222DeviceError, status
  * 
  *     def getMaxTransferSize(self):             # <<<<<<<<<<<<<<
  *         """Get the maximum transfer size for the currently configured operating mode
  * 
  */
 
@@ -5358,82 +5420,82 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getMaxTransferSize", 0);
 
-  /* "ft4222/ft4222.pyx":319
+  /* "ft4222/ft4222.pyx":332
  *             FT4222DeviceError: on error
  *         """
  *         cdef uint16 maxTransferSize = 0             # <<<<<<<<<<<<<<
  *         status = FT4222_GetMaxTransferSize(self._handle, &maxTransferSize)
  *         if status == FT4222_OK:
  */
   __pyx_v_maxTransferSize = 0;
 
-  /* "ft4222/ft4222.pyx":320
+  /* "ft4222/ft4222.pyx":333
  *         """
  *         cdef uint16 maxTransferSize = 0
  *         status = FT4222_GetMaxTransferSize(self._handle, &maxTransferSize)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return maxTransferSize
  */
   __pyx_v_status = FT4222_GetMaxTransferSize(__pyx_v_self->_handle, (&__pyx_v_maxTransferSize));
 
-  /* "ft4222/ft4222.pyx":321
+  /* "ft4222/ft4222.pyx":334
  *         cdef uint16 maxTransferSize = 0
  *         status = FT4222_GetMaxTransferSize(self._handle, &maxTransferSize)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return maxTransferSize
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":322
+    /* "ft4222/ft4222.pyx":335
  *         status = FT4222_GetMaxTransferSize(self._handle, &maxTransferSize)
  *         if status == FT4222_OK:
  *             return maxTransferSize             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_maxTransferSize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_maxTransferSize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":321
+    /* "ft4222/ft4222.pyx":334
  *         cdef uint16 maxTransferSize = 0
  *         status = FT4222_GetMaxTransferSize(self._handle, &maxTransferSize)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return maxTransferSize
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":323
+  /* "ft4222/ft4222.pyx":336
  *         if status == FT4222_OK:
  *             return maxTransferSize
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def vendorCmdGet(self, req, bytesToRead):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 336, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 323, __pyx_L1_error)
+  __PYX_ERR(0, 336, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":310
+  /* "ft4222/ft4222.pyx":323
  *             raise FT4222DeviceError, status
  * 
  *     def getMaxTransferSize(self):             # <<<<<<<<<<<<<<
  *         """Get the maximum transfer size for the currently configured operating mode
  * 
  */
 
@@ -5445,15 +5507,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":325
+/* "ft4222/ft4222.pyx":338
  *         raise FT4222DeviceError, status
  * 
  *     def vendorCmdGet(self, req, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Vendor get command"""
  *         cdef:
  */
 
@@ -5488,32 +5550,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_req)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytesToRead)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("vendorCmdGet", 1, 2, 2, 1); __PYX_ERR(0, 325, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vendorCmdGet", 1, 2, 2, 1); __PYX_ERR(0, 338, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "vendorCmdGet") < 0)) __PYX_ERR(0, 325, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "vendorCmdGet") < 0)) __PYX_ERR(0, 338, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_req = values[0];
     __pyx_v_bytesToRead = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vendorCmdGet", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 325, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vendorCmdGet", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 338, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.vendorCmdGet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_18vendorCmdGet(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_req, __pyx_v_bytesToRead);
 
@@ -5541,116 +5603,116 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vendorCmdGet", 0);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":328
+  /* "ft4222/ft4222.pyx":341
  *         """Vendor get command"""
  *         cdef:
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *         resize(buf, bytesToRead)
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 328, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 341, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 328, __pyx_L1_error)
+      __PYX_ERR(0, 341, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":329
+  /* "ft4222/ft4222.pyx":342
  *         cdef:
  *             array[uint8] buf = array('B', [])
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)
  *         if status == FT_OK:
  */
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 329, __pyx_L1_error)
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 329, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 342, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":330
+  /* "ft4222/ft4222.pyx":343
  *             array[uint8] buf = array('B', [])
  *         resize(buf, bytesToRead)
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)             # <<<<<<<<<<<<<<
  *         if status == FT_OK:
  *             return bytes(buf)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_UCHAR(__pyx_v_req); if (unlikely((__pyx_t_5 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_USHORT(__pyx_v_bytesToRead); if (unlikely((__pyx_t_6 == ((USHORT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_UCHAR(__pyx_v_req); if (unlikely((__pyx_t_5 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_USHORT(__pyx_v_bytesToRead); if (unlikely((__pyx_t_6 == ((USHORT)-1)) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
   __pyx_v_status = FT_VendorCmdGet(__pyx_v_self->_handle, __pyx_t_5, __pyx_v_buf->data.as_uchars, __pyx_t_6);
 
-  /* "ft4222/ft4222.pyx":331
+  /* "ft4222/ft4222.pyx":344
  *         resize(buf, bytesToRead)
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   __pyx_t_7 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_7) {
 
-    /* "ft4222/ft4222.pyx":332
+    /* "ft4222/ft4222.pyx":345
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)
  *         if status == FT_OK:
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 332, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":331
+    /* "ft4222/ft4222.pyx":344
  *         resize(buf, bytesToRead)
  *         status = FT_VendorCmdGet(self._handle, req, buf.data.as_uchars, bytesToRead)
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":333
+  /* "ft4222/ft4222.pyx":346
  *         if status == FT_OK:
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def vendorCmdSet(self, req, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_Raise(__pyx_t_1, __pyx_t_2, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 333, __pyx_L1_error)
+  __PYX_ERR(0, 346, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":325
+  /* "ft4222/ft4222.pyx":338
  *         raise FT4222DeviceError, status
  * 
  *     def vendorCmdGet(self, req, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Vendor get command"""
  *         cdef:
  */
 
@@ -5672,15 +5734,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":335
+/* "ft4222/ft4222.pyx":348
  *         raise FT4222DeviceError, status
  * 
  *     def vendorCmdSet(self, req, data):             # <<<<<<<<<<<<<<
  *         """Vendor set command"""
  *         if isinstance(data, int):
  */
 
@@ -5715,32 +5777,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_req)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("vendorCmdSet", 1, 2, 2, 1); __PYX_ERR(0, 335, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("vendorCmdSet", 1, 2, 2, 1); __PYX_ERR(0, 348, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "vendorCmdSet") < 0)) __PYX_ERR(0, 335, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "vendorCmdSet") < 0)) __PYX_ERR(0, 348, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_req = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("vendorCmdSet", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 335, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("vendorCmdSet", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 348, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.vendorCmdSet", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_20vendorCmdSet(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_req, __pyx_v_data);
 
@@ -5764,54 +5826,54 @@
   Py_ssize_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("vendorCmdSet", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "ft4222/ft4222.pyx":337
+  /* "ft4222/ft4222.pyx":350
  *     def vendorCmdSet(self, req, data):
  *         """Vendor set command"""
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":338
+    /* "ft4222/ft4222.pyx":351
  *         """Vendor set command"""
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 338, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 338, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 351, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":337
+    /* "ft4222/ft4222.pyx":350
  *     def vendorCmdSet(self, req, data):
  *         """Vendor set command"""
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":339
+  /* "ft4222/ft4222.pyx":352
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -5824,94 +5886,94 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":340
+    /* "ft4222/ft4222.pyx":353
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 bytesSent
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 340, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 340, __pyx_L1_error)
+    __PYX_ERR(0, 353, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":339
+    /* "ft4222/ft4222.pyx":352
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":343
+  /* "ft4222/ft4222.pyx":356
  *         cdef:
  *             uint16 bytesSent
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  *         status = FT_VendorCmdSet(self._handle, req, cdata, len(data))
  *         if status != FT_OK:
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 356, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":344
+  /* "ft4222/ft4222.pyx":357
  *             uint16 bytesSent
  *             uint8* cdata = data
  *         status = FT_VendorCmdSet(self._handle, req, cdata, len(data))             # <<<<<<<<<<<<<<
  *         if status != FT_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_7 = __Pyx_PyInt_As_UCHAR(__pyx_v_req); if (unlikely((__pyx_t_7 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 344, __pyx_L1_error)
-  __pyx_t_8 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_UCHAR(__pyx_v_req); if (unlikely((__pyx_t_7 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 357, __pyx_L1_error)
+  __pyx_t_8 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 357, __pyx_L1_error)
   __pyx_v_status = FT_VendorCmdSet(__pyx_v_self->_handle, __pyx_t_7, __pyx_v_cdata, __pyx_t_8);
 
-  /* "ft4222/ft4222.pyx":345
+  /* "ft4222/ft4222.pyx":358
  *             uint8* cdata = data
  *         status = FT_VendorCmdSet(self._handle, req, cdata, len(data))
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_1 = ((__pyx_v_status != FT_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":346
+    /* "ft4222/ft4222.pyx":359
  *         status = FT_VendorCmdSet(self._handle, req, cdata, len(data))
  *         if status != FT_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def getLatencyTimer(self):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 346, __pyx_L1_error)
+    __PYX_ERR(0, 359, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":345
+    /* "ft4222/ft4222.pyx":358
  *             uint8* cdata = data
  *         status = FT_VendorCmdSet(self._handle, req, cdata, len(data))
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":335
+  /* "ft4222/ft4222.pyx":348
  *         raise FT4222DeviceError, status
  * 
  *     def vendorCmdSet(self, req, data):             # <<<<<<<<<<<<<<
  *         """Vendor set command"""
  *         if isinstance(data, int):
  */
 
@@ -5926,15 +5988,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":348
+/* "ft4222/ft4222.pyx":361
  *             raise FT4222DeviceError, status
  * 
  *     def getLatencyTimer(self):             # <<<<<<<<<<<<<<
  *         """Get the current value of the latency timer.
  * 
  */
 
@@ -5961,73 +6023,73 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("getLatencyTimer", 0);
 
-  /* "ft4222/ft4222.pyx":358
+  /* "ft4222/ft4222.pyx":371
  *         """
  *         cdef UCHAR latency
  *         status = FT_GetLatencyTimer(self._handle, &latency)             # <<<<<<<<<<<<<<
  *         if status == FT_OK:
  *             return latency
  */
   __pyx_v_status = FT_GetLatencyTimer(__pyx_v_self->_handle, (&__pyx_v_latency));
 
-  /* "ft4222/ft4222.pyx":359
+  /* "ft4222/ft4222.pyx":372
  *         cdef UCHAR latency
  *         status = FT_GetLatencyTimer(self._handle, &latency)
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return latency
  *         raise FT2XXDeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":360
+    /* "ft4222/ft4222.pyx":373
  *         status = FT_GetLatencyTimer(self._handle, &latency)
  *         if status == FT_OK:
  *             return latency             # <<<<<<<<<<<<<<
  *         raise FT2XXDeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_UCHAR(__pyx_v_latency); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 360, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_UCHAR(__pyx_v_latency); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":359
+    /* "ft4222/ft4222.pyx":372
  *         cdef UCHAR latency
  *         status = FT_GetLatencyTimer(self._handle, &latency)
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return latency
  *         raise FT2XXDeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":361
+  /* "ft4222/ft4222.pyx":374
  *         if status == FT_OK:
  *             return latency
  *         raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def setLatencyTimer(self, latency):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 361, __pyx_L1_error)
+  __PYX_ERR(0, 374, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":348
+  /* "ft4222/ft4222.pyx":361
  *             raise FT4222DeviceError, status
  * 
  *     def getLatencyTimer(self):             # <<<<<<<<<<<<<<
  *         """Get the current value of the latency timer.
  * 
  */
 
@@ -6039,15 +6101,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":363
+/* "ft4222/ft4222.pyx":376
  *         raise FT2XXDeviceError, status
  * 
  *     def setLatencyTimer(self, latency):             # <<<<<<<<<<<<<<
  *         """Set the current value of the latency timer.
  * 
  */
 
@@ -6074,60 +6136,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setLatencyTimer", 0);
 
-  /* "ft4222/ft4222.pyx":372
+  /* "ft4222/ft4222.pyx":385
  *             FT2XXDeviceError: on error
  *         """
  *         status = FT_SetLatencyTimer(self._handle, latency)             # <<<<<<<<<<<<<<
  *         if status != FT_OK:
  *             raise FT2XXDeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_UCHAR(__pyx_v_latency); if (unlikely((__pyx_t_1 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 372, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_UCHAR(__pyx_v_latency); if (unlikely((__pyx_t_1 == ((UCHAR)-1)) && PyErr_Occurred())) __PYX_ERR(0, 385, __pyx_L1_error)
   __pyx_v_status = FT_SetLatencyTimer(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":373
+  /* "ft4222/ft4222.pyx":386
  *         """
  *         status = FT_SetLatencyTimer(self._handle, latency)
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT2XXDeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":374
+    /* "ft4222/ft4222.pyx":387
  *         status = FT_SetLatencyTimer(self._handle, latency)
  *         if status != FT_OK:
  *             raise FT2XXDeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_Init(self, *args, gpio0=Dir.INPUT, gpio1=Dir.INPUT, gpio2=Dir.INPUT, gpio3=Dir.INPUT):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT2XXDeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 374, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 374, __pyx_L1_error)
+    __PYX_ERR(0, 387, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":373
+    /* "ft4222/ft4222.pyx":386
  *         """
  *         status = FT_SetLatencyTimer(self._handle, latency)
  *         if status != FT_OK:             # <<<<<<<<<<<<<<
  *             raise FT2XXDeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":363
+  /* "ft4222/ft4222.pyx":376
  *         raise FT2XXDeviceError, status
  * 
  *     def setLatencyTimer(self, latency):             # <<<<<<<<<<<<<<
  *         """Set the current value of the latency timer.
  * 
  */
 
@@ -6141,15 +6203,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":376
+/* "ft4222/ft4222.pyx":389
  *             raise FT2XXDeviceError, status
  * 
  *     def gpio_Init(self, *args, gpio0=Dir.INPUT, gpio1=Dir.INPUT, gpio2=Dir.INPUT, gpio3=Dir.INPUT):             # <<<<<<<<<<<<<<
  *         """Initialize the GPIO interface.
  * 
  */
 
@@ -6197,28 +6259,28 @@
         Py_ssize_t index;
         for (index = 0; index < 4 && kw_args > 0; index++) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, 0, "gpio_Init") < 0)) __PYX_ERR(0, 376, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, 0, "gpio_Init") < 0)) __PYX_ERR(0, 389, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) < 0) {
       goto __pyx_L5_argtuple_error;
     } else {
     }
     __pyx_v_gpio0 = values[0];
     __pyx_v_gpio1 = values[1];
     __pyx_v_gpio2 = values[2];
     __pyx_v_gpio3 = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gpio_Init", 0, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 376, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gpio_Init", 0, 0, 0, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 389, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_args); __pyx_v_args = 0;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.gpio_Init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_26gpio_Init(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_gpio0, __pyx_v_gpio1, __pyx_v_gpio2, __pyx_v_gpio3, __pyx_v_args);
@@ -6244,173 +6306,173 @@
   Py_ssize_t __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_Init", 0);
 
-  /* "ft4222/ft4222.pyx":392
+  /* "ft4222/ft4222.pyx":405
  *         cdef:
  *             GPIO_Dir ioDir[4]
  *         if len(args) > 0:             # <<<<<<<<<<<<<<
  *             for i in xrange(len(args)):
  *                 ioDir[i] = args[i]
  */
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 392, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 405, __pyx_L1_error)
   __pyx_t_2 = ((__pyx_t_1 > 0) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":393
+    /* "ft4222/ft4222.pyx":406
  *             GPIO_Dir ioDir[4]
  *         if len(args) > 0:
  *             for i in xrange(len(args)):             # <<<<<<<<<<<<<<
  *                 ioDir[i] = args[i]
  *             for i in xrange(len(args), 4 - len(args)):
  */
-    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 393, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 406, __pyx_L1_error)
     __pyx_t_3 = __pyx_t_1;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "ft4222/ft4222.pyx":394
+      /* "ft4222/ft4222.pyx":407
  *         if len(args) > 0:
  *             for i in xrange(len(args)):
  *                 ioDir[i] = args[i]             # <<<<<<<<<<<<<<
  *             for i in xrange(len(args), 4 - len(args)):
  *                 ioDir[i] = GPIO_INPUT
  */
-      __pyx_t_5 = __Pyx_GetItemInt_Tuple(__pyx_v_args, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 394, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_GetItemInt_Tuple(__pyx_v_args, __pyx_v_i, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_t_5)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 394, __pyx_L1_error)
+      __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_t_5)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 407, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       (__pyx_v_ioDir[__pyx_v_i]) = __pyx_t_6;
     }
 
-    /* "ft4222/ft4222.pyx":395
+    /* "ft4222/ft4222.pyx":408
  *             for i in xrange(len(args)):
  *                 ioDir[i] = args[i]
  *             for i in xrange(len(args), 4 - len(args)):             # <<<<<<<<<<<<<<
  *                 ioDir[i] = GPIO_INPUT
  *         else:
  */
-    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 395, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 408, __pyx_L1_error)
     __pyx_t_3 = (4 - __pyx_t_1);
-    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 395, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 408, __pyx_L1_error)
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_7 = __pyx_t_1; __pyx_t_7 < __pyx_t_4; __pyx_t_7+=1) {
       __pyx_v_i = __pyx_t_7;
 
-      /* "ft4222/ft4222.pyx":396
+      /* "ft4222/ft4222.pyx":409
  *                 ioDir[i] = args[i]
  *             for i in xrange(len(args), 4 - len(args)):
  *                 ioDir[i] = GPIO_INPUT             # <<<<<<<<<<<<<<
  *         else:
  *             ioDir[0] = gpio0
  */
       (__pyx_v_ioDir[__pyx_v_i]) = GPIO_INPUT;
     }
 
-    /* "ft4222/ft4222.pyx":392
+    /* "ft4222/ft4222.pyx":405
  *         cdef:
  *             GPIO_Dir ioDir[4]
  *         if len(args) > 0:             # <<<<<<<<<<<<<<
  *             for i in xrange(len(args)):
  *                 ioDir[i] = args[i]
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":398
+  /* "ft4222/ft4222.pyx":411
  *                 ioDir[i] = GPIO_INPUT
  *         else:
  *             ioDir[0] = gpio0             # <<<<<<<<<<<<<<
  *             ioDir[1] = gpio1
  *             ioDir[2] = gpio2
  */
   /*else*/ {
-    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio0)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 398, __pyx_L1_error)
+    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio0)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 411, __pyx_L1_error)
     (__pyx_v_ioDir[0]) = __pyx_t_6;
 
-    /* "ft4222/ft4222.pyx":399
+    /* "ft4222/ft4222.pyx":412
  *         else:
  *             ioDir[0] = gpio0
  *             ioDir[1] = gpio1             # <<<<<<<<<<<<<<
  *             ioDir[2] = gpio2
  *             ioDir[3] = gpio3
  */
-    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 399, __pyx_L1_error)
+    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio1)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 412, __pyx_L1_error)
     (__pyx_v_ioDir[1]) = __pyx_t_6;
 
-    /* "ft4222/ft4222.pyx":400
+    /* "ft4222/ft4222.pyx":413
  *             ioDir[0] = gpio0
  *             ioDir[1] = gpio1
  *             ioDir[2] = gpio2             # <<<<<<<<<<<<<<
  *             ioDir[3] = gpio3
  *         status = FT4222_GPIO_Init(self._handle, ioDir)
  */
-    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L1_error)
+    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio2)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 413, __pyx_L1_error)
     (__pyx_v_ioDir[2]) = __pyx_t_6;
 
-    /* "ft4222/ft4222.pyx":401
+    /* "ft4222/ft4222.pyx":414
  *             ioDir[1] = gpio1
  *             ioDir[2] = gpio2
  *             ioDir[3] = gpio3             # <<<<<<<<<<<<<<
  *         status = FT4222_GPIO_Init(self._handle, ioDir)
  *         if status != FT4222_OK:
  */
-    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio3)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 401, __pyx_L1_error)
+    __pyx_t_6 = ((GPIO_Dir)__Pyx_PyInt_As_GPIO_Dir(__pyx_v_gpio3)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 414, __pyx_L1_error)
     (__pyx_v_ioDir[3]) = __pyx_t_6;
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":402
+  /* "ft4222/ft4222.pyx":415
  *             ioDir[2] = gpio2
  *             ioDir[3] = gpio3
  *         status = FT4222_GPIO_Init(self._handle, ioDir)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
   __pyx_v_status = FT4222_GPIO_Init(__pyx_v_self->_handle, __pyx_v_ioDir);
 
-  /* "ft4222/ft4222.pyx":403
+  /* "ft4222/ft4222.pyx":416
  *             ioDir[3] = gpio3
  *         status = FT4222_GPIO_Init(self._handle, ioDir)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":404
+    /* "ft4222/ft4222.pyx":417
  *         status = FT4222_GPIO_Init(self._handle, ioDir)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_Read(self, portNum):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 404, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 404, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_Raise(__pyx_t_5, __pyx_t_8, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 404, __pyx_L1_error)
+    __PYX_ERR(0, 417, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":403
+    /* "ft4222/ft4222.pyx":416
  *             ioDir[3] = gpio3
  *         status = FT4222_GPIO_Init(self._handle, ioDir)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":376
+  /* "ft4222/ft4222.pyx":389
  *             raise FT2XXDeviceError, status
  * 
  *     def gpio_Init(self, *args, gpio0=Dir.INPUT, gpio1=Dir.INPUT, gpio2=Dir.INPUT, gpio3=Dir.INPUT):             # <<<<<<<<<<<<<<
  *         """Initialize the GPIO interface.
  * 
  */
 
@@ -6424,15 +6486,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":406
+/* "ft4222/ft4222.pyx":419
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_Read(self, portNum):             # <<<<<<<<<<<<<<
  *         """Read value from selected GPIO
  * 
  */
 
@@ -6460,74 +6522,74 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_Read", 0);
 
-  /* "ft4222/ft4222.pyx":421
+  /* "ft4222/ft4222.pyx":434
  *         cdef:
  *             BOOL value
  *         status = FT4222_GPIO_Read(self._handle, portNum, &value)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return value
  */
-  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 421, __pyx_L1_error)
+  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 434, __pyx_L1_error)
   __pyx_v_status = FT4222_GPIO_Read(__pyx_v_self->_handle, __pyx_t_1, (&__pyx_v_value));
 
-  /* "ft4222/ft4222.pyx":422
+  /* "ft4222/ft4222.pyx":435
  *             BOOL value
  *         status = FT4222_GPIO_Read(self._handle, portNum, &value)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return value
  *         raise FT4222DeviceError, status
  */
   __pyx_t_2 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":423
+    /* "ft4222/ft4222.pyx":436
  *         status = FT4222_GPIO_Read(self._handle, portNum, &value)
  *         if status == FT4222_OK:
  *             return value             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_BOOL(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_BOOL(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":422
+    /* "ft4222/ft4222.pyx":435
  *             BOOL value
  *         status = FT4222_GPIO_Read(self._handle, portNum, &value)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return value
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":424
+  /* "ft4222/ft4222.pyx":437
  *         if status == FT4222_OK:
  *             return value
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_Write(self, portNum, value):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(0, 424, __pyx_L1_error)
+  __PYX_ERR(0, 437, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":406
+  /* "ft4222/ft4222.pyx":419
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_Read(self, portNum):             # <<<<<<<<<<<<<<
  *         """Read value from selected GPIO
  * 
  */
 
@@ -6539,15 +6601,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":426
+/* "ft4222/ft4222.pyx":439
  *         raise FT4222DeviceError, status
  * 
  *     def gpio_Write(self, portNum, value):             # <<<<<<<<<<<<<<
  *         """Write value to given GPIO
  * 
  */
 
@@ -6582,32 +6644,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_portNum)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_value)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("gpio_Write", 1, 2, 2, 1); __PYX_ERR(0, 426, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("gpio_Write", 1, 2, 2, 1); __PYX_ERR(0, 439, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_Write") < 0)) __PYX_ERR(0, 426, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_Write") < 0)) __PYX_ERR(0, 439, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_portNum = values[0];
     __pyx_v_value = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gpio_Write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 426, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gpio_Write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 439, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.gpio_Write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_30gpio_Write(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_portNum, __pyx_v_value);
 
@@ -6626,61 +6688,61 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_Write", 0);
 
-  /* "ft4222/ft4222.pyx":437
+  /* "ft4222/ft4222.pyx":450
  * 
  *         """
  *         status = FT4222_GPIO_Write(self._handle, portNum, value)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 437, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_As_BOOL(__pyx_v_value); if (unlikely((__pyx_t_2 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 437, __pyx_L1_error)
+  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_As_BOOL(__pyx_v_value); if (unlikely((__pyx_t_2 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 450, __pyx_L1_error)
   __pyx_v_status = FT4222_GPIO_Write(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2);
 
-  /* "ft4222/ft4222.pyx":438
+  /* "ft4222/ft4222.pyx":451
  *         """
  *         status = FT4222_GPIO_Write(self._handle, portNum, value)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_3 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "ft4222/ft4222.pyx":439
+    /* "ft4222/ft4222.pyx":452
  *         status = FT4222_GPIO_Write(self._handle, portNum, value)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_SetInputTrigger(self, portNum, trigger):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 439, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 452, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_4, __pyx_t_5, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 439, __pyx_L1_error)
+    __PYX_ERR(0, 452, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":438
+    /* "ft4222/ft4222.pyx":451
  *         """
  *         status = FT4222_GPIO_Write(self._handle, portNum, value)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":426
+  /* "ft4222/ft4222.pyx":439
  *         raise FT4222DeviceError, status
  * 
  *     def gpio_Write(self, portNum, value):             # <<<<<<<<<<<<<<
  *         """Write value to given GPIO
  * 
  */
 
@@ -6694,15 +6756,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":441
+/* "ft4222/ft4222.pyx":454
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_SetInputTrigger(self, portNum, trigger):             # <<<<<<<<<<<<<<
  *         """Set software trigger conditions on the specified GPIO pin.
  * 
  */
 
@@ -6737,32 +6799,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_portNum)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_trigger)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("gpio_SetInputTrigger", 1, 2, 2, 1); __PYX_ERR(0, 441, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("gpio_SetInputTrigger", 1, 2, 2, 1); __PYX_ERR(0, 454, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_SetInputTrigger") < 0)) __PYX_ERR(0, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_SetInputTrigger") < 0)) __PYX_ERR(0, 454, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_portNum = values[0];
     __pyx_v_trigger = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gpio_SetInputTrigger", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gpio_SetInputTrigger", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 454, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.gpio_SetInputTrigger", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_32gpio_SetInputTrigger(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_portNum, __pyx_v_trigger);
 
@@ -6781,61 +6843,61 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_SetInputTrigger", 0);
 
-  /* "ft4222/ft4222.pyx":452
+  /* "ft4222/ft4222.pyx":465
  * 
  *         """
  *         status = FT4222_GPIO_SetInputTrigger(self._handle, portNum, trigger)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 452, __pyx_L1_error)
-  __pyx_t_2 = ((GPIO_Trigger)__Pyx_PyInt_As_GPIO_Trigger(__pyx_v_trigger)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L1_error)
+  __pyx_t_2 = ((GPIO_Trigger)__Pyx_PyInt_As_GPIO_Trigger(__pyx_v_trigger)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L1_error)
   __pyx_v_status = FT4222_GPIO_SetInputTrigger(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2);
 
-  /* "ft4222/ft4222.pyx":453
+  /* "ft4222/ft4222.pyx":466
  *         """
  *         status = FT4222_GPIO_SetInputTrigger(self._handle, portNum, trigger)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_3 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "ft4222/ft4222.pyx":454
+    /* "ft4222/ft4222.pyx":467
  *         status = FT4222_GPIO_SetInputTrigger(self._handle, portNum, trigger)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_GetTriggerStatus(self, portNum):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 467, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_4, __pyx_t_5, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 454, __pyx_L1_error)
+    __PYX_ERR(0, 467, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":453
+    /* "ft4222/ft4222.pyx":466
  *         """
  *         status = FT4222_GPIO_SetInputTrigger(self._handle, portNum, trigger)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":441
+  /* "ft4222/ft4222.pyx":454
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_SetInputTrigger(self, portNum, trigger):             # <<<<<<<<<<<<<<
  *         """Set software trigger conditions on the specified GPIO pin.
  * 
  */
 
@@ -6849,15 +6911,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":456
+/* "ft4222/ft4222.pyx":469
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_GetTriggerStatus(self, portNum):             # <<<<<<<<<<<<<<
  *         """Get the size of trigger event queue.
  * 
  */
 
@@ -6885,74 +6947,74 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_GetTriggerStatus", 0);
 
-  /* "ft4222/ft4222.pyx":471
+  /* "ft4222/ft4222.pyx":484
  *         cdef:
  *             uint16 queueSize
  *         status = FT4222_GPIO_GetTriggerStatus(self._handle, portNum, &queueSize)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return queueSize
  */
-  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 471, __pyx_L1_error)
+  __pyx_t_1 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 484, __pyx_L1_error)
   __pyx_v_status = FT4222_GPIO_GetTriggerStatus(__pyx_v_self->_handle, __pyx_t_1, (&__pyx_v_queueSize));
 
-  /* "ft4222/ft4222.pyx":472
+  /* "ft4222/ft4222.pyx":485
  *             uint16 queueSize
  *         status = FT4222_GPIO_GetTriggerStatus(self._handle, portNum, &queueSize)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return queueSize
  *         raise FT4222DeviceError, status
  */
   __pyx_t_2 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":473
+    /* "ft4222/ft4222.pyx":486
  *         status = FT4222_GPIO_GetTriggerStatus(self._handle, portNum, &queueSize)
  *         if status == FT4222_OK:
  *             return queueSize             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_queueSize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_uint16_t(__pyx_v_queueSize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":472
+    /* "ft4222/ft4222.pyx":485
  *             uint16 queueSize
  *         status = FT4222_GPIO_GetTriggerStatus(self._handle, portNum, &queueSize)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return queueSize
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":474
+  /* "ft4222/ft4222.pyx":487
  *         if status == FT4222_OK:
  *             return queueSize
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def gpio_ReadTriggerQueue(self, portNum, readSize=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(0, 474, __pyx_L1_error)
+  __PYX_ERR(0, 487, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":456
+  /* "ft4222/ft4222.pyx":469
  *             raise FT4222DeviceError, status
  * 
  *     def gpio_GetTriggerStatus(self, portNum):             # <<<<<<<<<<<<<<
  *         """Get the size of trigger event queue.
  * 
  */
 
@@ -6964,15 +7026,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":476
+/* "ft4222/ft4222.pyx":489
  *         raise FT4222DeviceError, status
  * 
  *     def gpio_ReadTriggerQueue(self, portNum, readSize=None):             # <<<<<<<<<<<<<<
  *         """Get events recorded in the trigger event queue.
  * 
  */
 
@@ -7012,15 +7074,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_readSize);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_ReadTriggerQueue") < 0)) __PYX_ERR(0, 476, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gpio_ReadTriggerQueue") < 0)) __PYX_ERR(0, 489, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -7028,15 +7090,15 @@
       }
     }
     __pyx_v_portNum = values[0];
     __pyx_v_readSize = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gpio_ReadTriggerQueue", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 476, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gpio_ReadTriggerQueue", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 489, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.gpio_ReadTriggerQueue", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_36gpio_ReadTriggerQueue(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_portNum, __pyx_v_readSize);
 
@@ -7067,241 +7129,241 @@
   PyObject *__pyx_t_12 = NULL;
   int __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gpio_ReadTriggerQueue", 0);
 
-  /* "ft4222/ft4222.pyx":490
+  /* "ft4222/ft4222.pyx":503
  * 
  *         """
  *         if readSize == None:             # <<<<<<<<<<<<<<
  *             self.gpio_GetTriggerStatus(portNum)
  *         cdef:
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_readSize, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 490, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_readSize, Py_None, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":491
+    /* "ft4222/ft4222.pyx":504
  *         """
  *         if readSize == None:
  *             self.gpio_GetTriggerStatus(portNum)             # <<<<<<<<<<<<<<
  *         cdef:
  *             GPIO_Trigger *events = <GPIO_Trigger*>alloca(portNum * sizeof(GPIO_Trigger))
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_gpio_GetTriggerStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_gpio_GetTriggerStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_v_portNum) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_portNum);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 491, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 504, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ft4222/ft4222.pyx":490
+    /* "ft4222/ft4222.pyx":503
  * 
  *         """
  *         if readSize == None:             # <<<<<<<<<<<<<<
  *             self.gpio_GetTriggerStatus(portNum)
  *         cdef:
  */
   }
 
-  /* "ft4222/ft4222.pyx":493
+  /* "ft4222/ft4222.pyx":506
  *             self.gpio_GetTriggerStatus(portNum)
  *         cdef:
  *             GPIO_Trigger *events = <GPIO_Trigger*>alloca(portNum * sizeof(GPIO_Trigger))             # <<<<<<<<<<<<<<
  *             uint16 sizeRead
  *         status = FT4222_GPIO_ReadTriggerQueue(self._handle, portNum, events, readSize, &sizeRead)
  */
-  __pyx_t_1 = __Pyx_PyInt_FromSize_t((sizeof(GPIO_Trigger))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_FromSize_t((sizeof(GPIO_Trigger))); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_v_portNum, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_v_portNum, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_size_t(__pyx_t_3); if (unlikely((__pyx_t_5 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_events = ((GPIO_Trigger *)alloca(__pyx_t_5));
 
-  /* "ft4222/ft4222.pyx":495
+  /* "ft4222/ft4222.pyx":508
  *             GPIO_Trigger *events = <GPIO_Trigger*>alloca(portNum * sizeof(GPIO_Trigger))
  *             uint16 sizeRead
  *         status = FT4222_GPIO_ReadTriggerQueue(self._handle, portNum, events, readSize, &sizeRead)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             res = []
  */
-  __pyx_t_6 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 495, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_readSize); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 495, __pyx_L1_error)
+  __pyx_t_6 = ((GPIO_Port)__Pyx_PyInt_As_GPIO_Port(__pyx_v_portNum)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_readSize); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 508, __pyx_L1_error)
   __pyx_v_status = FT4222_GPIO_ReadTriggerQueue(__pyx_v_self->_handle, __pyx_t_6, __pyx_v_events, __pyx_t_7, (&__pyx_v_sizeRead));
 
-  /* "ft4222/ft4222.pyx":496
+  /* "ft4222/ft4222.pyx":509
  *             uint16 sizeRead
  *         status = FT4222_GPIO_ReadTriggerQueue(self._handle, portNum, events, readSize, &sizeRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             res = []
  *             for i in xrange(readSize):
  */
   __pyx_t_2 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":497
+    /* "ft4222/ft4222.pyx":510
  *         status = FT4222_GPIO_ReadTriggerQueue(self._handle, portNum, events, readSize, &sizeRead)
  *         if status == FT4222_OK:
  *             res = []             # <<<<<<<<<<<<<<
  *             for i in xrange(readSize):
  *                 res.append(Trigger(events[i]))
  */
-    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_res = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "ft4222/ft4222.pyx":498
+    /* "ft4222/ft4222.pyx":511
  *         if status == FT4222_OK:
  *             res = []
  *             for i in xrange(readSize):             # <<<<<<<<<<<<<<
  *                 res.append(Trigger(events[i]))
  *             return res
  */
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_xrange, __pyx_v_readSize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_xrange, __pyx_v_readSize); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
     } else {
-      __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 498, __pyx_L1_error)
+      __pyx_t_8 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 511, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 498, __pyx_L1_error)
+      __pyx_t_9 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 511, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_9)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 498, __pyx_L1_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 511, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 498, __pyx_L1_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 511, __pyx_L1_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 511, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_9(__pyx_t_1);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 498, __pyx_L1_error)
+            else __PYX_ERR(0, 511, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "ft4222/ft4222.pyx":499
+      /* "ft4222/ft4222.pyx":512
  *             res = []
  *             for i in xrange(readSize):
  *                 res.append(Trigger(events[i]))             # <<<<<<<<<<<<<<
  *             return res
  *         raise FT4222DeviceError, status
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Trigger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Trigger); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 499, __pyx_L1_error)
-      __pyx_t_11 = __Pyx_PyInt_From_GPIO_Trigger((__pyx_v_events[__pyx_t_10])); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_i); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 512, __pyx_L1_error)
+      __pyx_t_11 = __Pyx_PyInt_From_GPIO_Trigger((__pyx_v_events[__pyx_t_10])); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_11);
       __pyx_t_12 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
         __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_4);
         if (likely(__pyx_t_12)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_4, function);
         }
       }
       __pyx_t_3 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_12, __pyx_t_11) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_11);
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 499, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_res, __pyx_t_3); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 499, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyList_Append(__pyx_v_res, __pyx_t_3); if (unlikely(__pyx_t_13 == ((int)-1))) __PYX_ERR(0, 512, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "ft4222/ft4222.pyx":498
+      /* "ft4222/ft4222.pyx":511
  *         if status == FT4222_OK:
  *             res = []
  *             for i in xrange(readSize):             # <<<<<<<<<<<<<<
  *                 res.append(Trigger(events[i]))
  *             return res
  */
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "ft4222/ft4222.pyx":500
+    /* "ft4222/ft4222.pyx":513
  *             for i in xrange(readSize):
  *                 res.append(Trigger(events[i]))
  *             return res             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_res);
     __pyx_r = __pyx_v_res;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":496
+    /* "ft4222/ft4222.pyx":509
  *             uint16 sizeRead
  *         status = FT4222_GPIO_ReadTriggerQueue(self._handle, portNum, events, readSize, &sizeRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             res = []
  *             for i in xrange(readSize):
  */
   }
 
-  /* "ft4222/ft4222.pyx":501
+  /* "ft4222/ft4222.pyx":514
  *                 res.append(Trigger(events[i]))
  *             return res
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_1, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 501, __pyx_L1_error)
+  __PYX_ERR(0, 514, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":476
+  /* "ft4222/ft4222.pyx":489
  *         raise FT4222DeviceError, status
  * 
  *     def gpio_ReadTriggerQueue(self, portNum, readSize=None):             # <<<<<<<<<<<<<<
  *         """Get events recorded in the trigger event queue.
  * 
  */
 
@@ -7318,15 +7380,15 @@
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":504
+/* "ft4222/ft4222.pyx":517
  * 
  * 
  *     def i2cMaster_Init(self, kbps=100):             # <<<<<<<<<<<<<<
  *         """Initialize the FT4222H as an I2C master with the requested I2C speed.
  * 
  */
 
@@ -7359,29 +7421,29 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_kbps);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Init") < 0)) __PYX_ERR(0, 504, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Init") < 0)) __PYX_ERR(0, 517, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_kbps = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("i2cMaster_Init", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 504, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("i2cMaster_Init", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 517, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.i2cMaster_Init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_38i2cMaster_Init(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_kbps);
 
@@ -7405,147 +7467,147 @@
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_Init", 0);
 
-  /* "ft4222/ft4222.pyx":514
+  /* "ft4222/ft4222.pyx":527
  * 
  *         """
  *         status = FT4222_I2CMaster_Init(self._handle, kbps)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_kbps); if (unlikely((__pyx_t_1 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint32_t(__pyx_v_kbps); if (unlikely((__pyx_t_1 == ((uint32)-1)) && PyErr_Occurred())) __PYX_ERR(0, 527, __pyx_L1_error)
   __pyx_v_status = FT4222_I2CMaster_Init(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":515
+  /* "ft4222/ft4222.pyx":528
  *         """
  *         status = FT4222_I2CMaster_Init(self._handle, kbps)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  *         # current version (v1.3) of ftdi's lib can only handle clock rates down to 60kHz
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":516
+    /* "ft4222/ft4222.pyx":529
  *         status = FT4222_I2CMaster_Init(self._handle, kbps)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  *         # current version (v1.3) of ftdi's lib can only handle clock rates down to 60kHz
  *         # although the chip can handle clock rates down to ~23.6kHz
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 516, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 516, __pyx_L1_error)
+    __PYX_ERR(0, 529, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":515
+    /* "ft4222/ft4222.pyx":528
  *         """
  *         status = FT4222_I2CMaster_Init(self._handle, kbps)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  *         # current version (v1.3) of ftdi's lib can only handle clock rates down to 60kHz
  */
   }
 
-  /* "ft4222/ft4222.pyx":520
+  /* "ft4222/ft4222.pyx":533
  *         # although the chip can handle clock rates down to ~23.6kHz
  *         # there's a undocumented ways to achieve this
  *         if kbps < 60:             # <<<<<<<<<<<<<<
  *             #             Operating Clock Freq
  *             # SCL Freq = -----------------------  | M = 6 or 8; N = 1, 2, 3, , 127
  */
-  __pyx_t_4 = PyObject_RichCompare(__pyx_v_kbps, __pyx_int_60, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 520, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_v_kbps, __pyx_int_60, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 533, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":529
+    /* "ft4222/ft4222.pyx":542
  *             #            M * SCL Freq               8 * kbps
  *             #
  *             n = max(min(int(round(24000000.0 / (8 * 1000 * kbps) - 1)), 127), 1)             # <<<<<<<<<<<<<<
  *             self.setClock(SysClock.CLK_24)
  *             self.vendorCmdSet(0x52, n)
  */
     __pyx_t_5 = 1;
     __pyx_t_6 = 0x7F;
-    __pyx_t_4 = PyNumber_Multiply(__pyx_int_8000, __pyx_v_kbps); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_4 = PyNumber_Multiply(__pyx_int_8000, __pyx_v_kbps); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyFloat_TrueDivideCObj(__pyx_float_24000000_0, __pyx_t_4, 24000000.0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFloat_TrueDivideCObj(__pyx_float_24000000_0, __pyx_t_4, 24000000.0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_SubtractObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_round, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyNumber_Int(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_4, Py_LT); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_4, Py_LT); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (__pyx_t_2) {
-      __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_t_6); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 542, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_3 = __pyx_t_8;
       __pyx_t_8 = 0;
     } else {
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_3 = __pyx_t_4;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __pyx_t_4 = __pyx_t_3;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_8, __pyx_t_4, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 529, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 542, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_2) {
-      __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 529, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_5); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 542, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_3 = __pyx_t_7;
       __pyx_t_7 = 0;
     } else {
       __Pyx_INCREF(__pyx_t_4);
       __pyx_t_3 = __pyx_t_4;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __pyx_t_3;
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_n = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":530
+    /* "ft4222/ft4222.pyx":543
  *             #
  *             n = max(min(int(round(24000000.0 / (8 * 1000 * kbps) - 1)), 127), 1)
  *             self.setClock(SysClock.CLK_24)             # <<<<<<<<<<<<<<
  *             self.vendorCmdSet(0x52, n)
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_setClock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_setClock); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SysClock); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_SysClock); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CLK_24); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 530, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_CLK_24); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7553,27 +7615,27 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_8);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 530, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 543, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":531
+    /* "ft4222/ft4222.pyx":544
  *             n = max(min(int(round(24000000.0 / (8 * 1000 * kbps) - 1)), 127), 1)
  *             self.setClock(SysClock.CLK_24)
  *             self.vendorCmdSet(0x52, n)             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_Read(self, addr, bytesToRead):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_vendorCmdSet); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 531, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_vendorCmdSet); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 544, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_8 = NULL;
     __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -7582,56 +7644,56 @@
         __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_int_82, __pyx_v_n};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_4);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_int_82, __pyx_v_n};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_GOTREF(__pyx_t_4);
     } else
     #endif
     {
-      __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_7 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 544, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       if (__pyx_t_8) {
         __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_8); __pyx_t_8 = NULL;
       }
       __Pyx_INCREF(__pyx_int_82);
       __Pyx_GIVEREF(__pyx_int_82);
       PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_9, __pyx_int_82);
       __Pyx_INCREF(__pyx_v_n);
       __Pyx_GIVEREF(__pyx_v_n);
       PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_9, __pyx_v_n);
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 531, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_7, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 544, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":520
+    /* "ft4222/ft4222.pyx":533
  *         # although the chip can handle clock rates down to ~23.6kHz
  *         # there's a undocumented ways to achieve this
  *         if kbps < 60:             # <<<<<<<<<<<<<<
  *             #             Operating Clock Freq
  *             # SCL Freq = -----------------------  | M = 6 or 8; N = 1, 2, 3, , 127
  */
   }
 
-  /* "ft4222/ft4222.pyx":504
+  /* "ft4222/ft4222.pyx":517
  * 
  * 
  *     def i2cMaster_Init(self, kbps=100):             # <<<<<<<<<<<<<<
  *         """Initialize the FT4222H as an I2C master with the requested I2C speed.
  * 
  */
 
@@ -7648,15 +7710,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_n);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":533
+/* "ft4222/ft4222.pyx":546
  *             self.vendorCmdSet(0x52, n)
  * 
  *     def i2cMaster_Read(self, addr, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the specified I2C slave device with START and STOP conditions.
  * 
  */
 
@@ -7691,32 +7753,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_addr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytesToRead)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_Read", 1, 2, 2, 1); __PYX_ERR(0, 533, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_Read", 1, 2, 2, 1); __PYX_ERR(0, 546, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Read") < 0)) __PYX_ERR(0, 533, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Read") < 0)) __PYX_ERR(0, 546, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_addr = values[0];
     __pyx_v_bytesToRead = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("i2cMaster_Read", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 533, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("i2cMaster_Read", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 546, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.i2cMaster_Read", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_40i2cMaster_Read(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_addr, __pyx_v_bytesToRead);
 
@@ -7745,125 +7807,125 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_Read", 0);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":548
+  /* "ft4222/ft4222.pyx":561
  *         """
  *         cdef:
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 548, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 561, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 548, __pyx_L1_error)
+      __PYX_ERR(0, 561, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":550
+  /* "ft4222/ft4222.pyx":563
  *             array[uint8] buf = array('B', [])
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  *         status = FT4222_I2CMaster_Read(self._handle, addr, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  */
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 550, __pyx_L1_error)
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 550, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 563, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 563, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":551
+  /* "ft4222/ft4222.pyx":564
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  *         status = FT4222_I2CMaster_Read(self._handle, addr, buf.data.as_uchars, bytesToRead, &bytesRead)             # <<<<<<<<<<<<<<
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 551, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_6 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_6 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L1_error)
   __pyx_v_status = FT4222_I2CMaster_Read(__pyx_v_self->_handle, __pyx_t_5, __pyx_v_buf->data.as_uchars, __pyx_t_6, (&__pyx_v_bytesRead));
 
-  /* "ft4222/ft4222.pyx":552
+  /* "ft4222/ft4222.pyx":565
  *         resize(buf, bytesToRead)
  *         status = FT4222_I2CMaster_Read(self._handle, addr, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return bytes(buf)
  */
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 552, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 565, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":553
+  /* "ft4222/ft4222.pyx":566
  *         status = FT4222_I2CMaster_Read(self._handle, addr, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   __pyx_t_7 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_7) {
 
-    /* "ft4222/ft4222.pyx":554
+    /* "ft4222/ft4222.pyx":567
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 554, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":553
+    /* "ft4222/ft4222.pyx":566
  *         status = FT4222_I2CMaster_Read(self._handle, addr, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":555
+  /* "ft4222/ft4222.pyx":568
  *         if status == FT4222_OK:
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_Write(self, addr, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 555, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_Raise(__pyx_t_1, __pyx_t_2, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 555, __pyx_L1_error)
+  __PYX_ERR(0, 568, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":533
+  /* "ft4222/ft4222.pyx":546
  *             self.vendorCmdSet(0x52, n)
  * 
  *     def i2cMaster_Read(self, addr, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the specified I2C slave device with START and STOP conditions.
  * 
  */
 
@@ -7885,15 +7947,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":557
+/* "ft4222/ft4222.pyx":570
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_Write(self, addr, data):             # <<<<<<<<<<<<<<
  *         """Write data to the specified I2C slave device with START and STOP conditions.
  * 
  */
 
@@ -7928,32 +7990,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_addr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_Write", 1, 2, 2, 1); __PYX_ERR(0, 557, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_Write", 1, 2, 2, 1); __PYX_ERR(0, 570, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Write") < 0)) __PYX_ERR(0, 557, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_Write") < 0)) __PYX_ERR(0, 570, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_addr = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("i2cMaster_Write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 557, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("i2cMaster_Write", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 570, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.i2cMaster_Write", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_42i2cMaster_Write(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_addr, __pyx_v_data);
 
@@ -7978,54 +8040,54 @@
   Py_ssize_t __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_Write", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "ft4222/ft4222.pyx":571
+  /* "ft4222/ft4222.pyx":584
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":572
+    /* "ft4222/ft4222.pyx":585
  *         """
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 572, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 572, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 585, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":571
+    /* "ft4222/ft4222.pyx":584
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":573
+  /* "ft4222/ft4222.pyx":586
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -8038,108 +8100,108 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":574
+    /* "ft4222/ft4222.pyx":587
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 bytesSent
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 574, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 587, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 574, __pyx_L1_error)
+    __PYX_ERR(0, 587, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":573
+    /* "ft4222/ft4222.pyx":586
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":577
+  /* "ft4222/ft4222.pyx":590
  *         cdef:
  *             uint16 bytesSent
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  *         status = FT4222_I2CMaster_Write(self._handle, addr, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 577, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 590, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":578
+  /* "ft4222/ft4222.pyx":591
  *             uint16 bytesSent
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_Write(self._handle, addr, cdata, len(data), &bytesSent)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return bytesSent
  */
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 578, __pyx_L1_error)
-  __pyx_t_8 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 578, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 591, __pyx_L1_error)
+  __pyx_t_8 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 591, __pyx_L1_error)
   __pyx_v_status = FT4222_I2CMaster_Write(__pyx_v_self->_handle, __pyx_t_7, __pyx_v_cdata, __pyx_t_8, (&__pyx_v_bytesSent));
 
-  /* "ft4222/ft4222.pyx":579
+  /* "ft4222/ft4222.pyx":592
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_Write(self._handle, addr, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":580
+    /* "ft4222/ft4222.pyx":593
  *         status = FT4222_I2CMaster_Write(self._handle, addr, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:
  *             return bytesSent             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 580, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 593, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":579
+    /* "ft4222/ft4222.pyx":592
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_Write(self._handle, addr, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":581
+  /* "ft4222/ft4222.pyx":594
  *         if status == FT4222_OK:
  *             return bytesSent
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_ReadEx(self, addr, flag, bytesToRead):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 594, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 581, __pyx_L1_error)
+  __PYX_ERR(0, 594, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":557
+  /* "ft4222/ft4222.pyx":570
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_Write(self, addr, data):             # <<<<<<<<<<<<<<
  *         """Write data to the specified I2C slave device with START and STOP conditions.
  * 
  */
 
@@ -8152,15 +8214,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":583
+/* "ft4222/ft4222.pyx":596
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_ReadEx(self, addr, flag, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the specified I2C slave device with the specified I2C condition.
  * 
  */
 
@@ -8198,40 +8260,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_addr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, 1); __PYX_ERR(0, 583, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, 1); __PYX_ERR(0, 596, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytesToRead)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, 2); __PYX_ERR(0, 583, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, 2); __PYX_ERR(0, 596, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_ReadEx") < 0)) __PYX_ERR(0, 583, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_ReadEx") < 0)) __PYX_ERR(0, 596, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_addr = values[0];
     __pyx_v_flag = values[1];
     __pyx_v_bytesToRead = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 583, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("i2cMaster_ReadEx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 596, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.i2cMaster_ReadEx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_44i2cMaster_ReadEx(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_addr, __pyx_v_flag, __pyx_v_bytesToRead);
 
@@ -8261,126 +8323,126 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_ReadEx", 0);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":599
+  /* "ft4222/ft4222.pyx":612
  *         """
  *         cdef:
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 599, __pyx_L1_error)
+      __PYX_ERR(0, 612, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":601
+  /* "ft4222/ft4222.pyx":614
  *             array[uint8] buf = array('B', [])
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  *         status = FT4222_I2CMaster_ReadEx(self._handle, addr, flag, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  */
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 601, __pyx_L1_error)
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 601, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 614, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":602
+  /* "ft4222/ft4222.pyx":615
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  *         status = FT4222_I2CMaster_ReadEx(self._handle, addr, flag, buf.data.as_uchars, bytesToRead, &bytesRead)             # <<<<<<<<<<<<<<
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 602, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_uint8_t(__pyx_v_flag); if (unlikely((__pyx_t_6 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 602, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 602, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_uint8_t(__pyx_v_flag); if (unlikely((__pyx_t_6 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 615, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 615, __pyx_L1_error)
   __pyx_v_status = FT4222_I2CMaster_ReadEx(__pyx_v_self->_handle, __pyx_t_5, __pyx_t_6, __pyx_v_buf->data.as_uchars, __pyx_t_7, (&__pyx_v_bytesRead));
 
-  /* "ft4222/ft4222.pyx":603
+  /* "ft4222/ft4222.pyx":616
  *         resize(buf, bytesToRead)
  *         status = FT4222_I2CMaster_ReadEx(self._handle, addr, flag, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return bytes(buf)
  */
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 616, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":604
+  /* "ft4222/ft4222.pyx":617
  *         status = FT4222_I2CMaster_ReadEx(self._handle, addr, flag, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   __pyx_t_8 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_8) {
 
-    /* "ft4222/ft4222.pyx":605
+    /* "ft4222/ft4222.pyx":618
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 618, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":604
+    /* "ft4222/ft4222.pyx":617
  *         status = FT4222_I2CMaster_ReadEx(self._handle, addr, flag, buf.data.as_uchars, bytesToRead, &bytesRead)
  *         resize(buf, bytesRead)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":606
+  /* "ft4222/ft4222.pyx":619
  *         if status == FT4222_OK:
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_WriteEx(self, addr, flag, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 606, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 619, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_Raise(__pyx_t_1, __pyx_t_2, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 606, __pyx_L1_error)
+  __PYX_ERR(0, 619, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":583
+  /* "ft4222/ft4222.pyx":596
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_ReadEx(self, addr, flag, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the specified I2C slave device with the specified I2C condition.
  * 
  */
 
@@ -8402,15 +8464,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":608
+/* "ft4222/ft4222.pyx":621
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_WriteEx(self, addr, flag, data):             # <<<<<<<<<<<<<<
  *         """Write data to the specified I2C slave device with the specified I2C condition.
  * 
  */
 
@@ -8448,40 +8510,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_addr)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flag)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, 1); __PYX_ERR(0, 608, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, 1); __PYX_ERR(0, 621, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, 2); __PYX_ERR(0, 608, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, 2); __PYX_ERR(0, 621, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_WriteEx") < 0)) __PYX_ERR(0, 608, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "i2cMaster_WriteEx") < 0)) __PYX_ERR(0, 621, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_addr = values[0];
     __pyx_v_flag = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 608, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("i2cMaster_WriteEx", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 621, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.i2cMaster_WriteEx", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_46i2cMaster_WriteEx(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_addr, __pyx_v_flag, __pyx_v_data);
 
@@ -8507,54 +8569,54 @@
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_WriteEx", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "ft4222/ft4222.pyx":623
+  /* "ft4222/ft4222.pyx":636
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":624
+    /* "ft4222/ft4222.pyx":637
  *         """
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 624, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 637, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 624, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 637, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":623
+    /* "ft4222/ft4222.pyx":636
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":625
+  /* "ft4222/ft4222.pyx":638
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -8567,109 +8629,109 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":626
+    /* "ft4222/ft4222.pyx":639
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 bytesSent
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 626, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 639, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 626, __pyx_L1_error)
+    __PYX_ERR(0, 639, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":625
+    /* "ft4222/ft4222.pyx":638
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":629
+  /* "ft4222/ft4222.pyx":642
  *         cdef:
  *             uint16 bytesSent
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  *         status = FT4222_I2CMaster_WriteEx(self._handle, addr, flag, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 629, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 642, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":630
+  /* "ft4222/ft4222.pyx":643
  *             uint16 bytesSent
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_WriteEx(self._handle, addr, flag, cdata, len(data), &bytesSent)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return bytesSent
  */
-  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_flag); if (unlikely((__pyx_t_8 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 630, __pyx_L1_error)
-  __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 630, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_uint16_t(__pyx_v_addr); if (unlikely((__pyx_t_7 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_uint8_t(__pyx_v_flag); if (unlikely((__pyx_t_8 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 643, __pyx_L1_error)
+  __pyx_t_9 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 643, __pyx_L1_error)
   __pyx_v_status = FT4222_I2CMaster_WriteEx(__pyx_v_self->_handle, __pyx_t_7, __pyx_t_8, __pyx_v_cdata, __pyx_t_9, (&__pyx_v_bytesSent));
 
-  /* "ft4222/ft4222.pyx":631
+  /* "ft4222/ft4222.pyx":644
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_WriteEx(self._handle, addr, flag, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":632
+    /* "ft4222/ft4222.pyx":645
  *         status = FT4222_I2CMaster_WriteEx(self._handle, addr, flag, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:
  *             return bytesSent             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 632, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 645, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":631
+    /* "ft4222/ft4222.pyx":644
  *             uint8* cdata = data
  *         status = FT4222_I2CMaster_WriteEx(self._handle, addr, flag, cdata, len(data), &bytesSent)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":633
+  /* "ft4222/ft4222.pyx":646
  *         if status == FT4222_OK:
  *             return bytesSent
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_Reset(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 633, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 633, __pyx_L1_error)
+  __PYX_ERR(0, 646, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":608
+  /* "ft4222/ft4222.pyx":621
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_WriteEx(self, addr, flag, data):             # <<<<<<<<<<<<<<
  *         """Write data to the specified I2C slave device with the specified I2C condition.
  * 
  */
 
@@ -8682,15 +8744,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":635
+/* "ft4222/ft4222.pyx":648
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_Reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the I2C master device.
  * 
  */
 
@@ -8716,59 +8778,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_Reset", 0);
 
-  /* "ft4222/ft4222.pyx":645
+  /* "ft4222/ft4222.pyx":658
  * 
  *         """
  *         status = FT4222_I2CMaster_Reset(self._handle)             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
   __pyx_v_status = FT4222_I2CMaster_Reset(__pyx_v_self->_handle);
 
-  /* "ft4222/ft4222.pyx":646
+  /* "ft4222/ft4222.pyx":659
  *         """
  *         status = FT4222_I2CMaster_Reset(self._handle)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_1 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":647
+    /* "ft4222/ft4222.pyx":660
  *         status = FT4222_I2CMaster_Reset(self._handle)
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def i2cMaster_GetStatus(self):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 647, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 647, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 660, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 647, __pyx_L1_error)
+    __PYX_ERR(0, 660, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":646
+    /* "ft4222/ft4222.pyx":659
  *         """
  *         status = FT4222_I2CMaster_Reset(self._handle)
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":635
+  /* "ft4222/ft4222.pyx":648
  *         raise FT4222DeviceError, status
  * 
  *     def i2cMaster_Reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the I2C master device.
  * 
  */
 
@@ -8782,15 +8844,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":649
+/* "ft4222/ft4222.pyx":662
  *             raise FT4222DeviceError, status
  * 
  *     def i2cMaster_GetStatus(self):             # <<<<<<<<<<<<<<
  *         """Read the status of the I2C master controller.
  * 
  */
 
@@ -8819,91 +8881,91 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("i2cMaster_GetStatus", 0);
 
-  /* "ft4222/ft4222.pyx":662
+  /* "ft4222/ft4222.pyx":675
  *         """
  *         cdef uint8 cs
  *         status = FT4222_I2CMaster_GetStatus(self._handle, &cs)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return ControllerStatus(cs)
  */
   __pyx_v_status = FT4222_I2CMaster_GetStatus(__pyx_v_self->_handle, (&__pyx_v_cs));
 
-  /* "ft4222/ft4222.pyx":663
+  /* "ft4222/ft4222.pyx":676
  *         cdef uint8 cs
  *         status = FT4222_I2CMaster_GetStatus(self._handle, &cs)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return ControllerStatus(cs)
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":664
+    /* "ft4222/ft4222.pyx":677
  *         status = FT4222_I2CMaster_GetStatus(self._handle, &cs)
  *         if status == FT4222_OK:
  *             return ControllerStatus(cs)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ControllerStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 664, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_ControllerStatus); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_uint8_t(__pyx_v_cs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 664, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint8_t(__pyx_v_cs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 664, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":663
+    /* "ft4222/ft4222.pyx":676
  *         cdef uint8 cs
  *         status = FT4222_I2CMaster_GetStatus(self._handle, &cs)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return ControllerStatus(cs)
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":665
+  /* "ft4222/ft4222.pyx":678
  *         if status == FT4222_OK:
  *             return ControllerStatus(cs)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 665, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 678, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 665, __pyx_L1_error)
+  __PYX_ERR(0, 678, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":649
+  /* "ft4222/ft4222.pyx":662
  *             raise FT4222DeviceError, status
  * 
  *     def i2cMaster_GetStatus(self):             # <<<<<<<<<<<<<<
  *         """Read the status of the I2C master controller.
  * 
  */
 
@@ -8917,15 +8979,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":668
+/* "ft4222/ft4222.pyx":681
  * 
  * 
  *     def spi_Reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the SPI master or slave device
  * 
  */
 
@@ -8951,59 +9013,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spi_Reset", 0);
 
-  /* "ft4222/ft4222.pyx":675
+  /* "ft4222/ft4222.pyx":688
  * 
  *         """
  *         status = FT4222_SPI_Reset(self._handle);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
   __pyx_v_status = FT4222_SPI_Reset(__pyx_v_self->_handle);
 
-  /* "ft4222/ft4222.pyx":676
+  /* "ft4222/ft4222.pyx":689
  *         """
  *         status = FT4222_SPI_Reset(self._handle);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_1 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":677
+    /* "ft4222/ft4222.pyx":690
  *         status = FT4222_SPI_Reset(self._handle);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spi_ResetTransaction(self, spiIdx):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 677, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 677, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 690, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 677, __pyx_L1_error)
+    __PYX_ERR(0, 690, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":676
+    /* "ft4222/ft4222.pyx":689
  *         """
  *         status = FT4222_SPI_Reset(self._handle);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":668
+  /* "ft4222/ft4222.pyx":681
  * 
  * 
  *     def spi_Reset(self):             # <<<<<<<<<<<<<<
  *         """Reset the SPI master or slave device
  * 
  */
 
@@ -9017,15 +9079,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":679
+/* "ft4222/ft4222.pyx":692
  *             raise FT4222DeviceError, status
  * 
  *     def spi_ResetTransaction(self, spiIdx):             # <<<<<<<<<<<<<<
  *         """Reset the SPI transaction
  * 
  */
 
@@ -9052,60 +9114,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spi_ResetTransaction", 0);
 
-  /* "ft4222/ft4222.pyx":689
+  /* "ft4222/ft4222.pyx":702
  * 
  *         """
  *         status = FT4222_SPI_ResetTransaction(self._handle, spiIdx);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_spiIdx); if (unlikely((__pyx_t_1 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_uint8_t(__pyx_v_spiIdx); if (unlikely((__pyx_t_1 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 702, __pyx_L1_error)
   __pyx_v_status = FT4222_SPI_ResetTransaction(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":690
+  /* "ft4222/ft4222.pyx":703
  *         """
  *         status = FT4222_SPI_ResetTransaction(self._handle, spiIdx);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":691
+    /* "ft4222/ft4222.pyx":704
  *         status = FT4222_SPI_ResetTransaction(self._handle, spiIdx);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spi_SetDrivingStrength(self, clkStrength, ioStrength, ssoStrength):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 691, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 704, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 691, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 704, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 691, __pyx_L1_error)
+    __PYX_ERR(0, 704, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":690
+    /* "ft4222/ft4222.pyx":703
  *         """
  *         status = FT4222_SPI_ResetTransaction(self._handle, spiIdx);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":679
+  /* "ft4222/ft4222.pyx":692
  *             raise FT4222DeviceError, status
  * 
  *     def spi_ResetTransaction(self, spiIdx):             # <<<<<<<<<<<<<<
  *         """Reset the SPI transaction
  * 
  */
 
@@ -9119,15 +9181,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":693
+/* "ft4222/ft4222.pyx":706
  *             raise FT4222DeviceError, status
  * 
  *     def spi_SetDrivingStrength(self, clkStrength, ioStrength, ssoStrength):             # <<<<<<<<<<<<<<
  *         """Reset the SPI master or slave device.
  * 
  */
 
@@ -9165,40 +9227,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_clkStrength)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ioStrength)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, 1); __PYX_ERR(0, 693, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, 1); __PYX_ERR(0, 706, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ssoStrength)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, 2); __PYX_ERR(0, 693, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, 2); __PYX_ERR(0, 706, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spi_SetDrivingStrength") < 0)) __PYX_ERR(0, 693, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spi_SetDrivingStrength") < 0)) __PYX_ERR(0, 706, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_clkStrength = values[0];
     __pyx_v_ioStrength = values[1];
     __pyx_v_ssoStrength = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 693, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spi_SetDrivingStrength", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 706, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spi_SetDrivingStrength", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_56spi_SetDrivingStrength(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_clkStrength, __pyx_v_ioStrength, __pyx_v_ssoStrength);
 
@@ -9218,62 +9280,62 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spi_SetDrivingStrength", 0);
 
-  /* "ft4222/ft4222.pyx":705
+  /* "ft4222/ft4222.pyx":718
  * 
  *         """
  *         status = FT4222_SPI_SetDrivingStrength(self._handle, clkStrength, ioStrength, ssoStrength);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_clkStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 705, __pyx_L1_error)
-  __pyx_t_2 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_ioStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 705, __pyx_L1_error)
-  __pyx_t_3 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_ssoStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 705, __pyx_L1_error)
+  __pyx_t_1 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_clkStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_2 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_ioStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_3 = ((SPI_DrivingStrength)__Pyx_PyInt_As_SPI_DrivingStrength(__pyx_v_ssoStrength)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
   __pyx_v_status = FT4222_SPI_SetDrivingStrength(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2, __pyx_t_3);
 
-  /* "ft4222/ft4222.pyx":706
+  /* "ft4222/ft4222.pyx":719
  *         """
  *         status = FT4222_SPI_SetDrivingStrength(self._handle, clkStrength, ioStrength, ssoStrength);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_4 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "ft4222/ft4222.pyx":707
+    /* "ft4222/ft4222.pyx":720
  *         status = FT4222_SPI_SetDrivingStrength(self._handle, clkStrength, ioStrength, ssoStrength);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_Init(self, mode, clock, cpol, cpha, ssoMap):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 720, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 707, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 720, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_Raise(__pyx_t_5, __pyx_t_6, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 707, __pyx_L1_error)
+    __PYX_ERR(0, 720, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":706
+    /* "ft4222/ft4222.pyx":719
  *         """
  *         status = FT4222_SPI_SetDrivingStrength(self._handle, clkStrength, ioStrength, ssoStrength);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":693
+  /* "ft4222/ft4222.pyx":706
  *             raise FT4222DeviceError, status
  * 
  *     def spi_SetDrivingStrength(self, clkStrength, ioStrength, ssoStrength):             # <<<<<<<<<<<<<<
  *         """Reset the SPI master or slave device.
  * 
  */
 
@@ -9287,15 +9349,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":709
+/* "ft4222/ft4222.pyx":722
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_Init(self, mode, clock, cpol, cpha, ssoMap):             # <<<<<<<<<<<<<<
  *         """Initialize as an SPI master under all modes.
  * 
  */
 
@@ -9339,37 +9401,37 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_clock)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 1); __PYX_ERR(0, 709, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 1); __PYX_ERR(0, 722, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cpol)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 2); __PYX_ERR(0, 709, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 2); __PYX_ERR(0, 722, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cpha)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 3); __PYX_ERR(0, 709, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 3); __PYX_ERR(0, 722, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_ssoMap)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 4); __PYX_ERR(0, 709, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, 4); __PYX_ERR(0, 722, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_Init") < 0)) __PYX_ERR(0, 709, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_Init") < 0)) __PYX_ERR(0, 722, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 5) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
@@ -9380,15 +9442,15 @@
     __pyx_v_clock = values[1];
     __pyx_v_cpol = values[2];
     __pyx_v_cpha = values[3];
     __pyx_v_ssoMap = values[4];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 709, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiMaster_Init", 1, 5, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 722, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiMaster_Init", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_58spiMaster_Init(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_mode, __pyx_v_clock, __pyx_v_cpol, __pyx_v_cpha, __pyx_v_ssoMap);
 
@@ -9410,64 +9472,64 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiMaster_Init", 0);
 
-  /* "ft4222/ft4222.pyx":723
+  /* "ft4222/ft4222.pyx":736
  * 
  *         """
  *         status = FT4222_SPIMaster_Init(self._handle, mode, clock, cpol, cpha, ssoMap);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((FT4222_SPIMode)__Pyx_PyInt_As_FT4222_SPIMode(__pyx_v_mode)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L1_error)
-  __pyx_t_2 = ((FT4222_SPIClock)__Pyx_PyInt_As_FT4222_SPIClock(__pyx_v_clock)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L1_error)
-  __pyx_t_3 = ((FT4222_SPICPOL)__Pyx_PyInt_As_FT4222_SPICPOL(__pyx_v_cpol)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L1_error)
-  __pyx_t_4 = ((FT4222_SPICPHA)__Pyx_PyInt_As_FT4222_SPICPHA(__pyx_v_cpha)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyInt_As_uint8_t(__pyx_v_ssoMap); if (unlikely((__pyx_t_5 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 723, __pyx_L1_error)
+  __pyx_t_1 = ((FT4222_SPIMode)__Pyx_PyInt_As_FT4222_SPIMode(__pyx_v_mode)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_2 = ((FT4222_SPIClock)__Pyx_PyInt_As_FT4222_SPIClock(__pyx_v_clock)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_3 = ((FT4222_SPICPOL)__Pyx_PyInt_As_FT4222_SPICPOL(__pyx_v_cpol)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_4 = ((FT4222_SPICPHA)__Pyx_PyInt_As_FT4222_SPICPHA(__pyx_v_cpha)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint8_t(__pyx_v_ssoMap); if (unlikely((__pyx_t_5 == ((uint8)-1)) && PyErr_Occurred())) __PYX_ERR(0, 736, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_Init(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_t_4, __pyx_t_5);
 
-  /* "ft4222/ft4222.pyx":724
+  /* "ft4222/ft4222.pyx":737
  *         """
  *         status = FT4222_SPIMaster_Init(self._handle, mode, clock, cpol, cpha, ssoMap);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_6 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_6)) {
 
-    /* "ft4222/ft4222.pyx":725
+    /* "ft4222/ft4222.pyx":738
  *         status = FT4222_SPIMaster_Init(self._handle, mode, clock, cpol, cpha, ssoMap);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_SetLines(self, mode):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 725, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 738, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 725, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 738, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_Raise(__pyx_t_7, __pyx_t_8, 0, 0);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __PYX_ERR(0, 725, __pyx_L1_error)
+    __PYX_ERR(0, 738, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":724
+    /* "ft4222/ft4222.pyx":737
  *         """
  *         status = FT4222_SPIMaster_Init(self._handle, mode, clock, cpol, cpha, ssoMap);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":709
+  /* "ft4222/ft4222.pyx":722
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_Init(self, mode, clock, cpol, cpha, ssoMap):             # <<<<<<<<<<<<<<
  *         """Initialize as an SPI master under all modes.
  * 
  */
 
@@ -9481,15 +9543,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":727
+/* "ft4222/ft4222.pyx":740
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_SetLines(self, mode):             # <<<<<<<<<<<<<<
  *         """Switch the FT4222H SPI master to single, dual, or quad mode.
  * 
  */
 
@@ -9516,60 +9578,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiMaster_SetLines", 0);
 
-  /* "ft4222/ft4222.pyx":740
+  /* "ft4222/ft4222.pyx":753
  * 
  *         """
  *         status = FT4222_SPIMaster_SetLines(self._handle, mode);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((FT4222_SPIMode)__Pyx_PyInt_As_FT4222_SPIMode(__pyx_v_mode)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 740, __pyx_L1_error)
+  __pyx_t_1 = ((FT4222_SPIMode)__Pyx_PyInt_As_FT4222_SPIMode(__pyx_v_mode)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 753, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_SetLines(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":741
+  /* "ft4222/ft4222.pyx":754
  *         """
  *         status = FT4222_SPIMaster_SetLines(self._handle, mode);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":742
+    /* "ft4222/ft4222.pyx":755
  *         status = FT4222_SPIMaster_SetLines(self._handle, mode);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_SingleRead(self, bytesToRead, isEndTransaction):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 742, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 755, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 742, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 755, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 742, __pyx_L1_error)
+    __PYX_ERR(0, 755, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":741
+    /* "ft4222/ft4222.pyx":754
  *         """
  *         status = FT4222_SPIMaster_SetLines(self._handle, mode);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":727
+  /* "ft4222/ft4222.pyx":740
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_SetLines(self, mode):             # <<<<<<<<<<<<<<
  *         """Switch the FT4222H SPI master to single, dual, or quad mode.
  * 
  */
 
@@ -9583,15 +9645,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":744
+/* "ft4222/ft4222.pyx":757
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleRead(self, bytesToRead, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Read data from a SPI slave in single mode
  * 
  */
 
@@ -9626,32 +9688,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytesToRead)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_isEndTransaction)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleRead", 1, 2, 2, 1); __PYX_ERR(0, 744, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleRead", 1, 2, 2, 1); __PYX_ERR(0, 757, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleRead") < 0)) __PYX_ERR(0, 744, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleRead") < 0)) __PYX_ERR(0, 757, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_bytesToRead = values[0];
     __pyx_v_isEndTransaction = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleRead", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 744, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleRead", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 757, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiMaster_SingleRead", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_62spiMaster_SingleRead(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_bytesToRead, __pyx_v_isEndTransaction);
 
@@ -9680,125 +9742,125 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiMaster_SingleRead", 0);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":759
+  /* "ft4222/ft4222.pyx":772
  *         """
  *         cdef:
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 759, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 772, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 759, __pyx_L1_error)
+      __PYX_ERR(0, 772, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":761
+  /* "ft4222/ft4222.pyx":774
  *             array[uint8] buf = array('B', [])
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  *         status = FT4222_SPIMaster_SingleRead(self._handle, buf.data.as_uchars, bytesToRead, &bytesRead, isEndTransaction)
  *         if status == FT4222_OK:
  */
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 761, __pyx_L1_error)
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 761, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 774, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 774, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":762
+  /* "ft4222/ft4222.pyx":775
  *             uint16 bytesRead
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_SingleRead(self._handle, buf.data.as_uchars, bytesToRead, &bytesRead, isEndTransaction)             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 762, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_6 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 762, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_6 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 775, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_SingleRead(__pyx_v_self->_handle, __pyx_v_buf->data.as_uchars, __pyx_t_5, (&__pyx_v_bytesRead), __pyx_t_6);
 
-  /* "ft4222/ft4222.pyx":763
+  /* "ft4222/ft4222.pyx":776
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_SingleRead(self._handle, buf.data.as_uchars, bytesToRead, &bytesRead, isEndTransaction)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  */
   __pyx_t_7 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_7) {
 
-    /* "ft4222/ft4222.pyx":764
+    /* "ft4222/ft4222.pyx":777
  *         status = FT4222_SPIMaster_SingleRead(self._handle, buf.data.as_uchars, bytesToRead, &bytesRead, isEndTransaction)
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
-    __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 764, __pyx_L1_error)
+    __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 777, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":765
+    /* "ft4222/ft4222.pyx":778
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 765, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 778, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":763
+    /* "ft4222/ft4222.pyx":776
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_SingleRead(self._handle, buf.data.as_uchars, bytesToRead, &bytesRead, isEndTransaction)
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  */
   }
 
-  /* "ft4222/ft4222.pyx":766
+  /* "ft4222/ft4222.pyx":779
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_SingleWrite(self, data, isEndTransaction):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 766, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 779, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 766, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 779, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_Raise(__pyx_t_1, __pyx_t_2, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 766, __pyx_L1_error)
+  __PYX_ERR(0, 779, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":744
+  /* "ft4222/ft4222.pyx":757
  *             raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleRead(self, bytesToRead, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Read data from a SPI slave in single mode
  * 
  */
 
@@ -9820,15 +9882,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":768
+/* "ft4222/ft4222.pyx":781
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleWrite(self, data, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Write data to a SPI slave in single mode
  * 
  */
 
@@ -9863,32 +9925,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_isEndTransaction)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleWrite", 1, 2, 2, 1); __PYX_ERR(0, 768, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleWrite", 1, 2, 2, 1); __PYX_ERR(0, 781, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleWrite") < 0)) __PYX_ERR(0, 768, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleWrite") < 0)) __PYX_ERR(0, 781, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_data = values[0];
     __pyx_v_isEndTransaction = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleWrite", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 768, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleWrite", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 781, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiMaster_SingleWrite", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_64spiMaster_SingleWrite(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_data, __pyx_v_isEndTransaction);
 
@@ -9913,54 +9975,54 @@
   BOOL __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiMaster_SingleWrite", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "ft4222/ft4222.pyx":782
+  /* "ft4222/ft4222.pyx":795
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":783
+    /* "ft4222/ft4222.pyx":796
  *         """
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 796, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 783, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 796, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":782
+    /* "ft4222/ft4222.pyx":795
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":784
+  /* "ft4222/ft4222.pyx":797
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -9973,108 +10035,108 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":785
+    /* "ft4222/ft4222.pyx":798
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 bytesSent
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 785, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 798, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 785, __pyx_L1_error)
+    __PYX_ERR(0, 798, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":784
+    /* "ft4222/ft4222.pyx":797
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":788
+  /* "ft4222/ft4222.pyx":801
  *         cdef:
  *             uint16 bytesSent
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  *         status = FT4222_SPIMaster_SingleWrite(self._handle, cdata, len(data), &bytesSent, isEndTransaction);
  *         if status == FT4222_OK:
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 788, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 801, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":789
+  /* "ft4222/ft4222.pyx":802
  *             uint16 bytesSent
  *             uint8* cdata = data
  *         status = FT4222_SPIMaster_SingleWrite(self._handle, cdata, len(data), &bytesSent, isEndTransaction);             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return bytesSent
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 789, __pyx_L1_error)
-  __pyx_t_8 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_8 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 789, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 802, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_8 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 802, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_SingleWrite(__pyx_v_self->_handle, __pyx_v_cdata, __pyx_t_7, (&__pyx_v_bytesSent), __pyx_t_8);
 
-  /* "ft4222/ft4222.pyx":790
+  /* "ft4222/ft4222.pyx":803
  *             uint8* cdata = data
  *         status = FT4222_SPIMaster_SingleWrite(self._handle, cdata, len(data), &bytesSent, isEndTransaction);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":791
+    /* "ft4222/ft4222.pyx":804
  *         status = FT4222_SPIMaster_SingleWrite(self._handle, cdata, len(data), &bytesSent, isEndTransaction);
  *         if status == FT4222_OK:
  *             return bytesSent             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 791, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_bytesSent); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 804, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":790
+    /* "ft4222/ft4222.pyx":803
  *             uint8* cdata = data
  *         status = FT4222_SPIMaster_SingleWrite(self._handle, cdata, len(data), &bytesSent, isEndTransaction);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return bytesSent
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":792
+  /* "ft4222/ft4222.pyx":805
  *         if status == FT4222_OK:
  *             return bytesSent
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_SingleReadWrite(self, data, isEndTransaction):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 805, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 792, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 805, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 792, __pyx_L1_error)
+  __PYX_ERR(0, 805, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":768
+  /* "ft4222/ft4222.pyx":781
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleWrite(self, data, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Write data to a SPI slave in single mode
  * 
  */
 
@@ -10087,15 +10149,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":794
+/* "ft4222/ft4222.pyx":807
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleReadWrite(self, data, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Write and read data to and from a SPI slave in single mode
  * 
  */
 
@@ -10130,32 +10192,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_isEndTransaction)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleReadWrite", 1, 2, 2, 1); __PYX_ERR(0, 794, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_SingleReadWrite", 1, 2, 2, 1); __PYX_ERR(0, 807, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleReadWrite") < 0)) __PYX_ERR(0, 794, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_SingleReadWrite") < 0)) __PYX_ERR(0, 807, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_data = values[0];
     __pyx_v_isEndTransaction = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleReadWrite", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 794, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiMaster_SingleReadWrite", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 807, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiMaster_SingleReadWrite", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_66spiMaster_SingleReadWrite(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_data, __pyx_v_isEndTransaction);
 
@@ -10188,54 +10250,54 @@
   __Pyx_RefNannySetupContext("spiMaster_SingleReadWrite", 0);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":808
+  /* "ft4222/ft4222.pyx":821
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":809
+    /* "ft4222/ft4222.pyx":822
  *         """
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 822, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 809, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 822, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":808
+    /* "ft4222/ft4222.pyx":821
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":810
+  /* "ft4222/ft4222.pyx":823
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -10248,158 +10310,158 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":811
+    /* "ft4222/ft4222.pyx":824
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 sizeTransferred
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 811, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 824, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 811, __pyx_L1_error)
+    __PYX_ERR(0, 824, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":810
+    /* "ft4222/ft4222.pyx":823
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":814
+  /* "ft4222/ft4222.pyx":827
  *         cdef:
  *             uint16 sizeTransferred
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  *             array[uint8] buf = array('B', [])
  *         resize(buf, len(data))
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 814, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 827, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":815
+  /* "ft4222/ft4222.pyx":828
  *             uint16 sizeTransferred
  *             uint8* cdata = data
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *         resize(buf, len(data))
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);
  */
-  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 815, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 815, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 828, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_4), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 815, __pyx_L1_error)
+      __PYX_ERR(0, 828, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "ft4222/ft4222.pyx":816
+  /* "ft4222/ft4222.pyx":829
  *             uint8* cdata = data
  *             array[uint8] buf = array('B', [])
  *         resize(buf, len(data))             # <<<<<<<<<<<<<<
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);
  *         if status == FT4222_OK:
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 816, __pyx_L1_error)
-  __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 816, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 829, __pyx_L1_error)
+  __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 829, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":817
+  /* "ft4222/ft4222.pyx":830
  *             array[uint8] buf = array('B', [])
  *         resize(buf, len(data))
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             resize(buf, sizeTransferred)
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 817, __pyx_L1_error)
-  __pyx_t_9 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_9 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 817, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 830, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_BOOL(__pyx_v_isEndTransaction); if (unlikely((__pyx_t_9 == ((BOOL)-1)) && PyErr_Occurred())) __PYX_ERR(0, 830, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_SingleReadWrite(__pyx_v_self->_handle, __pyx_v_buf->data.as_uchars, __pyx_v_cdata, __pyx_t_7, (&__pyx_v_sizeTransferred), __pyx_t_9);
 
-  /* "ft4222/ft4222.pyx":818
+  /* "ft4222/ft4222.pyx":831
  *         resize(buf, len(data))
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, sizeTransferred)
  *             return bytes(buf)
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":819
+    /* "ft4222/ft4222.pyx":832
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);
  *         if status == FT4222_OK:
  *             resize(buf, sizeTransferred)             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
-    __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_sizeTransferred); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 819, __pyx_L1_error)
+    __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_sizeTransferred); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 832, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":820
+    /* "ft4222/ft4222.pyx":833
  *         if status == FT4222_OK:
  *             resize(buf, sizeTransferred)
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 820, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 833, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":818
+    /* "ft4222/ft4222.pyx":831
  *         resize(buf, len(data))
  *         status = FT4222_SPIMaster_SingleReadWrite(self._handle, buf.data.as_uchars, cdata, len(data), &sizeTransferred, isEndTransaction);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, sizeTransferred)
  *             return bytes(buf)
  */
   }
 
-  /* "ft4222/ft4222.pyx":821
+  /* "ft4222/ft4222.pyx":834
  *             resize(buf, sizeTransferred)
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_MultiReadWrite(self, singleWrite, multiWrite, bytesToRead):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 821, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 821, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 834, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 821, __pyx_L1_error)
+  __PYX_ERR(0, 834, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":794
+  /* "ft4222/ft4222.pyx":807
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_SingleReadWrite(self, data, isEndTransaction):             # <<<<<<<<<<<<<<
  *         """Write and read data to and from a SPI slave in single mode
  * 
  */
 
@@ -10422,15 +10484,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":823
+/* "ft4222/ft4222.pyx":836
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_MultiReadWrite(self, singleWrite, multiWrite, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Write and read data to and from a SPI slave in dual- or quad-mode (multi-mode).
  * 
  */
 
@@ -10468,40 +10530,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_singleWrite)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_multiWrite)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, 1); __PYX_ERR(0, 823, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, 1); __PYX_ERR(0, 836, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_bytesToRead)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, 2); __PYX_ERR(0, 823, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, 2); __PYX_ERR(0, 836, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_MultiReadWrite") < 0)) __PYX_ERR(0, 823, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiMaster_MultiReadWrite") < 0)) __PYX_ERR(0, 836, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_singleWrite = values[0];
     __pyx_v_multiWrite = values[1];
     __pyx_v_bytesToRead = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 823, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiMaster_MultiReadWrite", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 836, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiMaster_MultiReadWrite", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_68spiMaster_MultiReadWrite(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_singleWrite, __pyx_v_multiWrite, __pyx_v_bytesToRead);
 
@@ -10537,54 +10599,54 @@
   __Pyx_INCREF(__pyx_v_singleWrite);
   __Pyx_INCREF(__pyx_v_multiWrite);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":838
+  /* "ft4222/ft4222.pyx":851
  * 
  *         """
  *         if isinstance(singleWrite, int):             # <<<<<<<<<<<<<<
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_singleWrite); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":839
+    /* "ft4222/ft4222.pyx":852
  *         """
  *         if isinstance(singleWrite, int):
  *             singleWrite = bytes([singleWrite])             # <<<<<<<<<<<<<<
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 839, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_singleWrite);
     __Pyx_GIVEREF(__pyx_v_singleWrite);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_singleWrite);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 839, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 852, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_singleWrite, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":838
+    /* "ft4222/ft4222.pyx":851
  * 
  *         """
  *         if isinstance(singleWrite, int):             # <<<<<<<<<<<<<<
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":840
+  /* "ft4222/ft4222.pyx":853
  *         if isinstance(singleWrite, int):
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         if isinstance(multiWrite, int):
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_singleWrite); 
@@ -10597,77 +10659,77 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_singleWrite); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":841
+    /* "ft4222/ft4222.pyx":854
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         if isinstance(multiWrite, int):
  *             multiWrite = bytes([multiWrite])
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 841, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 854, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 841, __pyx_L1_error)
+    __PYX_ERR(0, 854, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":840
+    /* "ft4222/ft4222.pyx":853
  *         if isinstance(singleWrite, int):
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         if isinstance(multiWrite, int):
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":842
+  /* "ft4222/ft4222.pyx":855
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         if isinstance(multiWrite, int):             # <<<<<<<<<<<<<<
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_multiWrite); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":843
+    /* "ft4222/ft4222.pyx":856
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         if isinstance(multiWrite, int):
  *             multiWrite = bytes([multiWrite])             # <<<<<<<<<<<<<<
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 843, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_multiWrite);
     __Pyx_GIVEREF(__pyx_v_multiWrite);
     PyList_SET_ITEM(__pyx_t_4, 0, __pyx_v_multiWrite);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 843, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 856, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF_SET(__pyx_v_multiWrite, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "ft4222/ft4222.pyx":842
+    /* "ft4222/ft4222.pyx":855
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         if isinstance(multiWrite, int):             # <<<<<<<<<<<<<<
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  */
     goto __pyx_L6;
   }
 
-  /* "ft4222/ft4222.pyx":844
+  /* "ft4222/ft4222.pyx":857
  *         if isinstance(multiWrite, int):
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         write = singleWrite + multiWrite
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_multiWrite); 
@@ -10680,171 +10742,171 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_multiWrite); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L7_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":845
+    /* "ft4222/ft4222.pyx":858
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         write = singleWrite + multiWrite
  *         cdef:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 845, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 858, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 845, __pyx_L1_error)
+    __PYX_ERR(0, 858, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":844
+    /* "ft4222/ft4222.pyx":857
  *         if isinstance(multiWrite, int):
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         write = singleWrite + multiWrite
  */
   }
   __pyx_L6:;
 
-  /* "ft4222/ft4222.pyx":846
+  /* "ft4222/ft4222.pyx":859
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")
  *         write = singleWrite + multiWrite             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint8* cdata = write
  */
-  __pyx_t_3 = PyNumber_Add(__pyx_v_singleWrite, __pyx_v_multiWrite); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 846, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Add(__pyx_v_singleWrite, __pyx_v_multiWrite); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 859, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_write = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "ft4222/ft4222.pyx":848
+  /* "ft4222/ft4222.pyx":861
  *         write = singleWrite + multiWrite
  *         cdef:
  *             uint8* cdata = write             # <<<<<<<<<<<<<<
  *             array[uint8] buf = array('B', [])
  *             uint32 bytesRead
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_write); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 848, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_write); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 861, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":849
+  /* "ft4222/ft4222.pyx":862
  *         cdef:
  *             uint8* cdata = write
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *             uint32 bytesRead
  *         resize(buf, bytesToRead)
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 862, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 849, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 862, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 849, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 862, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_3), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 849, __pyx_L1_error)
+      __PYX_ERR(0, 862, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "ft4222/ft4222.pyx":851
+  /* "ft4222/ft4222.pyx":864
  *             array[uint8] buf = array('B', [])
  *             uint32 bytesRead
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  *         status = FT4222_SPIMaster_MultiReadWrite(self._handle, buf.data.as_uchars, cdata, len(singleWrite), len(multiWrite), bytesToRead, &bytesRead);
  *         if status == FT4222_OK:
  */
-  __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 851, __pyx_L1_error)
-  __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 851, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_7 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 864, __pyx_L1_error)
+  __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_7); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 864, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":852
+  /* "ft4222/ft4222.pyx":865
  *             uint32 bytesRead
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_MultiReadWrite(self._handle, buf.data.as_uchars, cdata, len(singleWrite), len(multiWrite), bytesToRead, &bytesRead);             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_singleWrite); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 852, __pyx_L1_error)
-  __pyx_t_9 = PyObject_Length(__pyx_v_multiWrite); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 852, __pyx_L1_error)
-  __pyx_t_10 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_10 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 852, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_singleWrite); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 865, __pyx_L1_error)
+  __pyx_t_9 = PyObject_Length(__pyx_v_multiWrite); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 865, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_10 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 865, __pyx_L1_error)
   __pyx_v_status = FT4222_SPIMaster_MultiReadWrite(__pyx_v_self->_handle, __pyx_v_buf->data.as_uchars, __pyx_v_cdata, __pyx_t_7, __pyx_t_9, __pyx_t_10, (&__pyx_v_bytesRead));
 
-  /* "ft4222/ft4222.pyx":853
+  /* "ft4222/ft4222.pyx":866
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_MultiReadWrite(self._handle, buf.data.as_uchars, cdata, len(singleWrite), len(multiWrite), bytesToRead, &bytesRead);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":854
+    /* "ft4222/ft4222.pyx":867
  *         status = FT4222_SPIMaster_MultiReadWrite(self._handle, buf.data.as_uchars, cdata, len(singleWrite), len(multiWrite), bytesToRead, &bytesRead);
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
-    __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 854, __pyx_L1_error)
+    __pyx_t_8 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_bytesRead); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(0, 867, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":855
+    /* "ft4222/ft4222.pyx":868
  *         if status == FT4222_OK:
  *             resize(buf, bytesRead)
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 855, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 868, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":853
+    /* "ft4222/ft4222.pyx":866
  *         resize(buf, bytesToRead)
  *         status = FT4222_SPIMaster_MultiReadWrite(self._handle, buf.data.as_uchars, cdata, len(singleWrite), len(multiWrite), bytesToRead, &bytesRead);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  */
   }
 
-  /* "ft4222/ft4222.pyx":856
+  /* "ft4222/ft4222.pyx":869
  *             resize(buf, bytesRead)
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiMaster_EndTransaction(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 856, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 856, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 869, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(0, 856, __pyx_L1_error)
+  __PYX_ERR(0, 869, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":823
+  /* "ft4222/ft4222.pyx":836
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_MultiReadWrite(self, singleWrite, multiWrite, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Write and read data to and from a SPI slave in dual- or quad-mode (multi-mode).
  * 
  */
 
@@ -10869,15 +10931,15 @@
   __Pyx_XDECREF(__pyx_v_singleWrite);
   __Pyx_XDECREF(__pyx_v_multiWrite);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":858
+/* "ft4222/ft4222.pyx":871
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_EndTransaction(self):             # <<<<<<<<<<<<<<
  *         """End the current SPI transaction.
  * 
  */
 
@@ -10904,70 +10966,70 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiMaster_EndTransaction", 0);
 
-  /* "ft4222/ft4222.pyx":867
+  /* "ft4222/ft4222.pyx":880
  *         cdef:
  *             DWORD bytesSent;
  *         status = FT_Write(self._handle, <unsigned char*>NULL, 0, &bytesSent);             # <<<<<<<<<<<<<<
  *         if status == FT_OK:
  *             return
  */
   __pyx_v_status = FT_Write(__pyx_v_self->_handle, ((unsigned char *)NULL), 0, (&__pyx_v_bytesSent));
 
-  /* "ft4222/ft4222.pyx":868
+  /* "ft4222/ft4222.pyx":881
  *             DWORD bytesSent;
  *         status = FT_Write(self._handle, <unsigned char*>NULL, 0, &bytesSent);
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":869
+    /* "ft4222/ft4222.pyx":882
  *         status = FT_Write(self._handle, <unsigned char*>NULL, 0, &bytesSent);
  *         if status == FT_OK:
  *             return             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":868
+    /* "ft4222/ft4222.pyx":881
  *             DWORD bytesSent;
  *         status = FT_Write(self._handle, <unsigned char*>NULL, 0, &bytesSent);
  *         if status == FT_OK:             # <<<<<<<<<<<<<<
  *             return
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":870
+  /* "ft4222/ft4222.pyx":883
  *         if status == FT_OK:
  *             return
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_Init(self):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 870, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_ULONG(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 883, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 870, __pyx_L1_error)
+  __PYX_ERR(0, 883, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":858
+  /* "ft4222/ft4222.pyx":871
  *         raise FT4222DeviceError, status
  * 
  *     def spiMaster_EndTransaction(self):             # <<<<<<<<<<<<<<
  *         """End the current SPI transaction.
  * 
  */
 
@@ -10979,15 +11041,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":872
+/* "ft4222/ft4222.pyx":885
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_Init(self):             # <<<<<<<<<<<<<<
  *         """Initialize the FT4222H as an SPI slave. Default SPI_SlaveProtocol is SPI_SLAVE_WITH_PROTOCOL.
  * 
  */
 
@@ -11013,59 +11075,59 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_Init", 0);
 
-  /* "ft4222/ft4222.pyx":879
+  /* "ft4222/ft4222.pyx":892
  * 
  *         """
  *         status = FT4222_SPISlave_Init(self._handle);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
   __pyx_v_status = FT4222_SPISlave_Init(__pyx_v_self->_handle);
 
-  /* "ft4222/ft4222.pyx":880
+  /* "ft4222/ft4222.pyx":893
  *         """
  *         status = FT4222_SPISlave_Init(self._handle);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_1 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":881
+    /* "ft4222/ft4222.pyx":894
  *         status = FT4222_SPISlave_Init(self._handle);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_InitEx(self, proto):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 894, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 881, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 894, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 881, __pyx_L1_error)
+    __PYX_ERR(0, 894, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":880
+    /* "ft4222/ft4222.pyx":893
  *         """
  *         status = FT4222_SPISlave_Init(self._handle);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":872
+  /* "ft4222/ft4222.pyx":885
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_Init(self):             # <<<<<<<<<<<<<<
  *         """Initialize the FT4222H as an SPI slave. Default SPI_SlaveProtocol is SPI_SLAVE_WITH_PROTOCOL.
  * 
  */
 
@@ -11079,15 +11141,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":883
+/* "ft4222/ft4222.pyx":896
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_InitEx(self, proto):             # <<<<<<<<<<<<<<
  *         """Initialize as an SPI slave under all modes.
  * 
  */
 
@@ -11114,60 +11176,60 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_InitEx", 0);
 
-  /* "ft4222/ft4222.pyx":893
+  /* "ft4222/ft4222.pyx":906
  * 
  *         """
  *         status = FT4222_SPISlave_InitEx(self._handle,proto);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((SPI_SlaveProtocol)__Pyx_PyInt_As_SPI_SlaveProtocol(__pyx_v_proto)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 893, __pyx_L1_error)
+  __pyx_t_1 = ((SPI_SlaveProtocol)__Pyx_PyInt_As_SPI_SlaveProtocol(__pyx_v_proto)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 906, __pyx_L1_error)
   __pyx_v_status = FT4222_SPISlave_InitEx(__pyx_v_self->_handle, __pyx_t_1);
 
-  /* "ft4222/ft4222.pyx":894
+  /* "ft4222/ft4222.pyx":907
  *         """
  *         status = FT4222_SPISlave_InitEx(self._handle,proto);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_2 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "ft4222/ft4222.pyx":895
+    /* "ft4222/ft4222.pyx":908
  *         status = FT4222_SPISlave_InitEx(self._handle,proto);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_Read(self, bytesToRead):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 895, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 908, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 895, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 908, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_3, __pyx_t_4, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 895, __pyx_L1_error)
+    __PYX_ERR(0, 908, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":894
+    /* "ft4222/ft4222.pyx":907
  *         """
  *         status = FT4222_SPISlave_InitEx(self._handle,proto);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":883
+  /* "ft4222/ft4222.pyx":896
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_InitEx(self, proto):             # <<<<<<<<<<<<<<
  *         """Initialize as an SPI slave under all modes.
  * 
  */
 
@@ -11181,15 +11243,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":897
+/* "ft4222/ft4222.pyx":910
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_Read(self, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the receive queue of the SPI slave device.
  * 
  */
 
@@ -11226,124 +11288,124 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_Read", 0);
   __pyx_pybuffer_buf.pybuffer.buf = NULL;
   __pyx_pybuffer_buf.refcount = 0;
   __pyx_pybuffernd_buf.data = NULL;
   __pyx_pybuffernd_buf.rcbuffer = &__pyx_pybuffer_buf;
 
-  /* "ft4222/ft4222.pyx":911
+  /* "ft4222/ft4222.pyx":924
  *         """
  *         cdef:
  *             array[uint8] buf = array('B', [])             # <<<<<<<<<<<<<<
  *             uint16 sizeRead
  *         resize(buf, bytesToRead)
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 924, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 924, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_n_u_B);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_B);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 911, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_7cpython_5array_array), __pyx_t_2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 924, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_buf.rcbuffer->pybuffer, (PyObject*)((arrayobject *)__pyx_t_1), &__Pyx_TypeInfo_nn_uint8, PyBUF_FORMAT| PyBUF_INDIRECT, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_buf = ((arrayobject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_buf.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 911, __pyx_L1_error)
+      __PYX_ERR(0, 924, __pyx_L1_error)
     } else {__pyx_pybuffernd_buf.diminfo[0].strides = __pyx_pybuffernd_buf.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_buf.diminfo[0].shape = __pyx_pybuffernd_buf.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_buf.diminfo[0].suboffsets = __pyx_pybuffernd_buf.rcbuffer->pybuffer.suboffsets[0];
     }
   }
   __pyx_v_buf = ((arrayobject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":913
+  /* "ft4222/ft4222.pyx":926
  *             array[uint8] buf = array('B', [])
  *             uint16 sizeRead
  *         resize(buf, bytesToRead)             # <<<<<<<<<<<<<<
  * 
  *         status = FT4222_SPISlave_Read(self._handle, buf.data.as_uchars, bytesToRead, &sizeRead);
  */
-  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 913, __pyx_L1_error)
-  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 913, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyIndex_AsSsize_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 926, __pyx_L1_error)
+  __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_t_3); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 926, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":915
+  /* "ft4222/ft4222.pyx":928
  *         resize(buf, bytesToRead)
  * 
  *         status = FT4222_SPISlave_Read(self._handle, buf.data.as_uchars, bytesToRead, &sizeRead);             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             resize(buf, sizeRead)
  */
-  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 915, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_uint16_t(__pyx_v_bytesToRead); if (unlikely((__pyx_t_5 == ((uint16)-1)) && PyErr_Occurred())) __PYX_ERR(0, 928, __pyx_L1_error)
   __pyx_v_status = FT4222_SPISlave_Read(__pyx_v_self->_handle, __pyx_v_buf->data.as_uchars, __pyx_t_5, (&__pyx_v_sizeRead));
 
-  /* "ft4222/ft4222.pyx":916
+  /* "ft4222/ft4222.pyx":929
  * 
  *         status = FT4222_SPISlave_Read(self._handle, buf.data.as_uchars, bytesToRead, &sizeRead);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, sizeRead)
  *             return bytes(buf)
  */
   __pyx_t_6 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_6) {
 
-    /* "ft4222/ft4222.pyx":917
+    /* "ft4222/ft4222.pyx":930
  *         status = FT4222_SPISlave_Read(self._handle, buf.data.as_uchars, bytesToRead, &sizeRead);
  *         if status == FT4222_OK:
  *             resize(buf, sizeRead)             # <<<<<<<<<<<<<<
  *             return bytes(buf)
  *         raise FT4222DeviceError, status
  */
-    __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_sizeRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 917, __pyx_L1_error)
+    __pyx_t_4 = resize(((arrayobject *)__pyx_v_buf), __pyx_v_sizeRead); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 930, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":918
+    /* "ft4222/ft4222.pyx":931
  *         if status == FT4222_OK:
  *             resize(buf, sizeRead)
  *             return bytes(buf)             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 918, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), ((PyObject *)__pyx_v_buf)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":916
+    /* "ft4222/ft4222.pyx":929
  * 
  *         status = FT4222_SPISlave_Read(self._handle, buf.data.as_uchars, bytesToRead, &sizeRead);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             resize(buf, sizeRead)
  *             return bytes(buf)
  */
   }
 
-  /* "ft4222/ft4222.pyx":919
+  /* "ft4222/ft4222.pyx":932
  *             resize(buf, sizeRead)
  *             return bytes(buf)
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_SetMode(self, cpol, cpha):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 919, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 919, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 932, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_Raise(__pyx_t_1, __pyx_t_2, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __PYX_ERR(0, 919, __pyx_L1_error)
+  __PYX_ERR(0, 932, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":897
+  /* "ft4222/ft4222.pyx":910
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_Read(self, bytesToRead):             # <<<<<<<<<<<<<<
  *         """Read data from the receive queue of the SPI slave device.
  * 
  */
 
@@ -11365,15 +11427,15 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_buf);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":921
+/* "ft4222/ft4222.pyx":934
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_SetMode(self, cpol, cpha):             # <<<<<<<<<<<<<<
  *         """Set SPI slave cpol and cpha. The Default value of cpol is (:obj:`ft4222.SPI.Cpol.CLK_IDLE_LOW`) , default value of cpha is (:obj:`ft4222.SPI.Cpol.CLK_LEADING`)
  * 
  */
 
@@ -11408,32 +11470,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cpol)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_cpha)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("spiSlave_SetMode", 1, 2, 2, 1); __PYX_ERR(0, 921, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("spiSlave_SetMode", 1, 2, 2, 1); __PYX_ERR(0, 934, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiSlave_SetMode") < 0)) __PYX_ERR(0, 921, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "spiSlave_SetMode") < 0)) __PYX_ERR(0, 934, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_cpol = values[0];
     __pyx_v_cpha = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("spiSlave_SetMode", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 921, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("spiSlave_SetMode", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 934, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("ft4222.ft4222.FT4222.spiSlave_SetMode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_6ft4222_6ft4222_6FT4222_78spiSlave_SetMode(((struct __pyx_obj_6ft4222_6ft4222_FT4222 *)__pyx_v_self), __pyx_v_cpol, __pyx_v_cpha);
 
@@ -11452,61 +11514,61 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_SetMode", 0);
 
-  /* "ft4222/ft4222.pyx":932
+  /* "ft4222/ft4222.pyx":945
  * 
  *         """
  *         status = FT4222_SPISlave_SetMode(self._handle, cpol, cpha);             # <<<<<<<<<<<<<<
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status
  */
-  __pyx_t_1 = ((FT4222_SPICPOL)__Pyx_PyInt_As_FT4222_SPICPOL(__pyx_v_cpol)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 932, __pyx_L1_error)
-  __pyx_t_2 = ((FT4222_SPICPHA)__Pyx_PyInt_As_FT4222_SPICPHA(__pyx_v_cpha)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 932, __pyx_L1_error)
+  __pyx_t_1 = ((FT4222_SPICPOL)__Pyx_PyInt_As_FT4222_SPICPOL(__pyx_v_cpol)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
+  __pyx_t_2 = ((FT4222_SPICPHA)__Pyx_PyInt_As_FT4222_SPICPHA(__pyx_v_cpha)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 945, __pyx_L1_error)
   __pyx_v_status = FT4222_SPISlave_SetMode(__pyx_v_self->_handle, __pyx_t_1, __pyx_t_2);
 
-  /* "ft4222/ft4222.pyx":933
+  /* "ft4222/ft4222.pyx":946
  *         """
  *         status = FT4222_SPISlave_SetMode(self._handle, cpol, cpha);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   __pyx_t_3 = ((__pyx_v_status != FT4222_OK) != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "ft4222/ft4222.pyx":934
+    /* "ft4222/ft4222.pyx":947
  *         status = FT4222_SPISlave_SetMode(self._handle, cpol, cpha);
  *         if status != FT4222_OK:
  *             raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_GetRxStatus(self):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 934, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 947, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 934, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 947, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_4, __pyx_t_5, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 934, __pyx_L1_error)
+    __PYX_ERR(0, 947, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":933
+    /* "ft4222/ft4222.pyx":946
  *         """
  *         status = FT4222_SPISlave_SetMode(self._handle, cpol, cpha);
  *         if status != FT4222_OK:             # <<<<<<<<<<<<<<
  *             raise FT4222DeviceError, status
  * 
  */
   }
 
-  /* "ft4222/ft4222.pyx":921
+  /* "ft4222/ft4222.pyx":934
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_SetMode(self, cpol, cpha):             # <<<<<<<<<<<<<<
  *         """Set SPI slave cpol and cpha. The Default value of cpol is (:obj:`ft4222.SPI.Cpol.CLK_IDLE_LOW`) , default value of cpha is (:obj:`ft4222.SPI.Cpol.CLK_LEADING`)
  * 
  */
 
@@ -11520,15 +11582,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":936
+/* "ft4222/ft4222.pyx":949
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_GetRxStatus(self):             # <<<<<<<<<<<<<<
  *         """Get number of bytes in the receive queue.
  * 
  */
 
@@ -11555,73 +11617,73 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_GetRxStatus", 0);
 
-  /* "ft4222/ft4222.pyx":949
+  /* "ft4222/ft4222.pyx":962
  *             uint16 pRxSize
  * 
  *         status = FT4222_SPISlave_GetRxStatus(self._handle, &pRxSize);             # <<<<<<<<<<<<<<
  * 
  *         if status == FT4222_OK:
  */
   __pyx_v_status = FT4222_SPISlave_GetRxStatus(__pyx_v_self->_handle, (&__pyx_v_pRxSize));
 
-  /* "ft4222/ft4222.pyx":951
+  /* "ft4222/ft4222.pyx":964
  *         status = FT4222_SPISlave_GetRxStatus(self._handle, &pRxSize);
  * 
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return pRxSize
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":952
+    /* "ft4222/ft4222.pyx":965
  * 
  *         if status == FT4222_OK:
  *             return pRxSize             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_pRxSize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 952, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_uint16_t(__pyx_v_pRxSize); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 965, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":951
+    /* "ft4222/ft4222.pyx":964
  *         status = FT4222_SPISlave_GetRxStatus(self._handle, &pRxSize);
  * 
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return pRxSize
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":953
+  /* "ft4222/ft4222.pyx":966
  *         if status == FT4222_OK:
  *             return pRxSize
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  * 
  *     def spiSlave_Write(self, data):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 966, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 953, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 966, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_2, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 953, __pyx_L1_error)
+  __PYX_ERR(0, 966, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":936
+  /* "ft4222/ft4222.pyx":949
  *             raise FT4222DeviceError, status
  * 
  *     def spiSlave_GetRxStatus(self):             # <<<<<<<<<<<<<<
  *         """Get number of bytes in the receive queue.
  * 
  */
 
@@ -11633,15 +11695,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "ft4222/ft4222.pyx":955
+/* "ft4222/ft4222.pyx":968
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_Write(self, data):             # <<<<<<<<<<<<<<
  *         """Write data to the transmit queue of the SPI slave device.
  * 
  */
 
@@ -11674,54 +11736,54 @@
   Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("spiSlave_Write", 0);
   __Pyx_INCREF(__pyx_v_data);
 
-  /* "ft4222/ft4222.pyx":968
+  /* "ft4222/ft4222.pyx":981
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_data); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "ft4222/ft4222.pyx":969
+    /* "ft4222/ft4222.pyx":982
  *         """
  *         if isinstance(data, int):
  *             data = bytes([data])             # <<<<<<<<<<<<<<
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  */
-    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 969, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 982, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyList_SET_ITEM(__pyx_t_3, 0, __pyx_v_data);
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 969, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 982, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF_SET(__pyx_v_data, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "ft4222/ft4222.pyx":968
+    /* "ft4222/ft4222.pyx":981
  * 
  *         """
  *         if isinstance(data, int):             # <<<<<<<<<<<<<<
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  */
     goto __pyx_L3;
   }
 
-  /* "ft4222/ft4222.pyx":970
+  /* "ft4222/ft4222.pyx":983
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_data); 
@@ -11734,104 +11796,104 @@
   __pyx_t_5 = PyByteArray_Check(__pyx_v_data); 
   __pyx_t_1 = (__pyx_t_5 != 0);
   __pyx_t_2 = __pyx_t_1;
   __pyx_L4_bool_binop_done:;
   __pyx_t_1 = ((!(__pyx_t_2 != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "ft4222/ft4222.pyx":971
+    /* "ft4222/ft4222.pyx":984
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 sizeTransferred
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 971, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 984, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 971, __pyx_L1_error)
+    __PYX_ERR(0, 984, __pyx_L1_error)
 
-    /* "ft4222/ft4222.pyx":970
+    /* "ft4222/ft4222.pyx":983
  *         if isinstance(data, int):
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):             # <<<<<<<<<<<<<<
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")
  *         cdef:
  */
   }
   __pyx_L3:;
 
-  /* "ft4222/ft4222.pyx":974
+  /* "ft4222/ft4222.pyx":987
  *         cdef:
  *             uint16 sizeTransferred
  *             uint8* cdata = data             # <<<<<<<<<<<<<<
  * 
  *         status = FT4222_SPISlave_Write(self._handle, cdata, len(data), &sizeTransferred);
  */
-  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 974, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_AsWritableUString(__pyx_v_data); if (unlikely((!__pyx_t_6) && PyErr_Occurred())) __PYX_ERR(0, 987, __pyx_L1_error)
   __pyx_v_cdata = __pyx_t_6;
 
-  /* "ft4222/ft4222.pyx":976
+  /* "ft4222/ft4222.pyx":989
  *             uint8* cdata = data
  * 
  *         status = FT4222_SPISlave_Write(self._handle, cdata, len(data), &sizeTransferred);             # <<<<<<<<<<<<<<
  *         if status == FT4222_OK:
  *             return sizeTransferred
  */
-  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 976, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_v_data); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 989, __pyx_L1_error)
   __pyx_v_status = FT4222_SPISlave_Write(__pyx_v_self->_handle, __pyx_v_cdata, __pyx_t_7, (&__pyx_v_sizeTransferred));
 
-  /* "ft4222/ft4222.pyx":977
+  /* "ft4222/ft4222.pyx":990
  * 
  *         status = FT4222_SPISlave_Write(self._handle, cdata, len(data), &sizeTransferred);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return sizeTransferred
  *         raise FT4222DeviceError, status
  */
   __pyx_t_1 = ((__pyx_v_status == FT4222_OK) != 0);
   if (__pyx_t_1) {
 
-    /* "ft4222/ft4222.pyx":978
+    /* "ft4222/ft4222.pyx":991
  *         status = FT4222_SPISlave_Write(self._handle, cdata, len(data), &sizeTransferred);
  *         if status == FT4222_OK:
  *             return sizeTransferred             # <<<<<<<<<<<<<<
  *         raise FT4222DeviceError, status
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_sizeTransferred); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 978, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_uint16_t(__pyx_v_sizeTransferred); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 991, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "ft4222/ft4222.pyx":977
+    /* "ft4222/ft4222.pyx":990
  * 
  *         status = FT4222_SPISlave_Write(self._handle, cdata, len(data), &sizeTransferred);
  *         if status == FT4222_OK:             # <<<<<<<<<<<<<<
  *             return sizeTransferred
  *         raise FT4222DeviceError, status
  */
   }
 
-  /* "ft4222/ft4222.pyx":979
+  /* "ft4222/ft4222.pyx":992
  *         if status == FT4222_OK:
  *             return sizeTransferred
  *         raise FT4222DeviceError, status             # <<<<<<<<<<<<<<
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 979, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FT4222DeviceError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 992, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 979, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_FT4222_STATUS(__pyx_v_status); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 992, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_4, __pyx_t_3, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 979, __pyx_L1_error)
+  __PYX_ERR(0, 992, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":955
+  /* "ft4222/ft4222.pyx":968
  *         raise FT4222DeviceError, status
  * 
  *     def spiSlave_Write(self, data):             # <<<<<<<<<<<<<<
  *         """Write data to the transmit queue of the SPI slave device.
  * 
  */
 
@@ -12707,15 +12769,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_6ft4222_6ft4222_FT4222 __pyx_vtable_6ft4222_6ft4222_FT4222;
 
 static PyObject *__pyx_tp_new_6ft4222_6ft4222_FT4222(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_obj_6ft4222_6ft4222_FT4222 *p;
@@ -12891,15 +12953,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -13126,21 +13188,21 @@
   {&__pyx_n_s_write_timeout, __pyx_k_write_timeout, sizeof(__pyx_k_write_timeout), 0, 0, 1, 1},
   {&__pyx_n_s_xrange, __pyx_k_xrange, sizeof(__pyx_k_xrange), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 244, __pyx_L1_error)
   #if PY_MAJOR_VERSION >= 3
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_xrange) __PYX_ERR(0, 406, __pyx_L1_error)
   #else
-  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_builtin_xrange = __Pyx_GetBuiltinName(__pyx_n_s_xrange); if (!__pyx_builtin_xrange) __PYX_ERR(0, 406, __pyx_L1_error)
   #endif
-  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(0, 542, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 109, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
@@ -13162,44 +13224,44 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_self__handle_cannot_be_converted); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "ft4222/ft4222.pyx":340
+  /* "ft4222/ft4222.pyx":353
  *             data = bytes([data])
  *         elif not isinstance(data, (bytes, bytearray)):
  *             raise TypeError("the data argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         cdef:
  *             uint16 bytesSent
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_the_data_argument_must_be_of_typ); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 340, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_the_data_argument_must_be_of_typ); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "ft4222/ft4222.pyx":841
+  /* "ft4222/ft4222.pyx":854
  *             singleWrite = bytes([singleWrite])
  *         elif not isinstance(singleWrite, (bytes, bytearray)):
  *             raise TypeError("the singleWrite argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         if isinstance(multiWrite, int):
  *             multiWrite = bytes([multiWrite])
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_the_singleWrite_argument_must_be); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 841, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_the_singleWrite_argument_must_be); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 854, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "ft4222/ft4222.pyx":845
+  /* "ft4222/ft4222.pyx":858
  *             multiWrite = bytes([multiWrite])
  *         elif not isinstance(multiWrite, (bytes, bytearray)):
  *             raise TypeError("the multiWrite argument must be of type 'int', 'bytes' or 'bytearray'")             # <<<<<<<<<<<<<<
  *         write = singleWrite + multiWrite
  *         cdef:
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_the_multiWrite_argument_must_be); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 845, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_the_multiWrite_argument_must_be); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 858, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self._handle cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -13290,45 +13352,45 @@
   __Pyx_GIVEREF(__pyx_tuple__22);
   __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_getDeviceInfoDetail, 100, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 100, __pyx_L1_error)
 
   /* "ft4222/ft4222.pyx":117
  *     raise FT2XXDeviceError, status
  * 
  * def openBySerial(serial):             # <<<<<<<<<<<<<<
- *     """Open a handle to a usb device by serial number"""
- *     cdef FT_HANDLE handle
+ *     """Open a handle to a usb device by serial number
+ * 
  */
   __pyx_tuple__24 = PyTuple_Pack(4, __pyx_n_s_serial, __pyx_n_s_handle, __pyx_n_s_cserial, __pyx_n_s_status); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
   __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_openBySerial, 117, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 117, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":126
+  /* "ft4222/ft4222.pyx":139
  *     raise FT2XXDeviceError, status
  * 
  * def openByDescription(desc):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by description
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_desc, __pyx_n_s_handle, __pyx_n_s_cdesc, __pyx_n_s_status); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(4, __pyx_n_s_desc, __pyx_n_s_handle, __pyx_n_s_cdesc, __pyx_n_s_status); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_openByDescription, 126, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(1, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_openByDescription, 139, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 139, __pyx_L1_error)
 
-  /* "ft4222/ft4222.pyx":149
+  /* "ft4222/ft4222.pyx":162
  *     raise FT2XXDeviceError, status
  * 
  * def openByLocation(locId):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by location
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_locId, __pyx_n_s_handle, __pyx_n_s_status); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_locId, __pyx_n_s_handle, __pyx_n_s_status); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_openByLocation, 149, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_ft4222_ft4222_pyx, __pyx_n_s_openByLocation, 162, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -13390,38 +13452,38 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_6ft4222_6ft4222__closer = &__pyx_vtable_6ft4222_6ft4222__closer;
   __pyx_vtable_6ft4222_6ft4222__closer.wrap = (PyObject *(*)(FT_HANDLE))__pyx_f_6ft4222_6ft4222_7_closer_wrap;
-  if (PyType_Ready(&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6ft4222_6ft4222__closer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6ft4222_6ft4222__closer.tp_dictoffset && __pyx_type_6ft4222_6ft4222__closer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6ft4222_6ft4222__closer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6ft4222_6ft4222__closer.tp_dict, __pyx_vtabptr_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_closer, (PyObject *)&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 169, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6ft4222_6ft4222__closer.tp_dict, __pyx_vtabptr_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_closer, (PyObject *)&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6ft4222_6ft4222__closer) < 0) __PYX_ERR(0, 182, __pyx_L1_error)
   __pyx_ptype_6ft4222_6ft4222__closer = &__pyx_type_6ft4222_6ft4222__closer;
   __pyx_vtabptr_6ft4222_6ft4222_FT4222 = &__pyx_vtable_6ft4222_6ft4222_FT4222;
   __pyx_vtable_6ft4222_6ft4222_FT4222._get_version = (PyObject *(*)(struct __pyx_obj_6ft4222_6ft4222_FT4222 *))__pyx_f_6ft4222_6ft4222_6FT4222__get_version;
-  if (PyType_Ready(&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_6ft4222_6ft4222_FT4222.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6ft4222_6ft4222_FT4222.tp_dictoffset && __pyx_type_6ft4222_6ft4222_FT4222.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_6ft4222_6ft4222_FT4222.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6ft4222_6ft4222_FT4222.tp_dict, __pyx_vtabptr_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FT4222, (PyObject *)&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_6ft4222_6ft4222_FT4222.tp_dict, __pyx_vtabptr_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FT4222, (PyObject *)&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
   if (__pyx_type_6ft4222_6ft4222_FT4222.tp_weaklistoffset == 0) __pyx_type_6ft4222_6ft4222_FT4222.tp_weaklistoffset = offsetof(struct __pyx_obj_6ft4222_6ft4222_FT4222, __weakref__);
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6ft4222_6ft4222_FT4222) < 0) __PYX_ERR(0, 200, __pyx_L1_error)
   __pyx_ptype_6ft4222_6ft4222_FT4222 = &__pyx_type_6ft4222_6ft4222_FT4222;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -13432,27 +13494,25 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType(__pyx_t_1, "array", "array", sizeof(arrayobject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_0_29_35(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(arrayobject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(2, 58, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -14159,80 +14219,80 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_getDeviceInfoDetail, __pyx_t_1) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "ft4222/ft4222.pyx":117
  *     raise FT2XXDeviceError, status
  * 
  * def openBySerial(serial):             # <<<<<<<<<<<<<<
- *     """Open a handle to a usb device by serial number"""
- *     cdef FT_HANDLE handle
+ *     """Open a handle to a usb device by serial number
+ * 
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6ft4222_6ft4222_5openBySerial, NULL, __pyx_n_s_ft4222_ft4222); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_openBySerial, __pyx_t_1) < 0) __PYX_ERR(0, 117, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":126
+  /* "ft4222/ft4222.pyx":139
  *     raise FT2XXDeviceError, status
  * 
  * def openByDescription(desc):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by description
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6ft4222_6ft4222_7openByDescription, NULL, __pyx_n_s_ft4222_ft4222); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6ft4222_6ft4222_7openByDescription, NULL, __pyx_n_s_ft4222_ft4222); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openByDescription, __pyx_t_1) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openByDescription, __pyx_t_1) < 0) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":149
+  /* "ft4222/ft4222.pyx":162
  *     raise FT2XXDeviceError, status
  * 
  * def openByLocation(locId):             # <<<<<<<<<<<<<<
  *     """Open a handle to a usb device by location
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6ft4222_6ft4222_9openByLocation, NULL, __pyx_n_s_ft4222_ft4222); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6ft4222_6ft4222_9openByLocation, NULL, __pyx_n_s_ft4222_ft4222); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openByLocation, __pyx_t_1) < 0) __PYX_ERR(0, 149, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_openByLocation, __pyx_t_1) < 0) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "ft4222/ft4222.pyx":376
+  /* "ft4222/ft4222.pyx":389
  *             raise FT2XXDeviceError, status
  * 
  *     def gpio_Init(self, *args, gpio0=Dir.INPUT, gpio1=Dir.INPUT, gpio2=Dir.INPUT, gpio3=Dir.INPUT):             # <<<<<<<<<<<<<<
  *         """Initialize the GPIO interface.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dir); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dir); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_k__4 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_k__5 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dir); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Dir); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_k__6 = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Dir); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_INPUT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 389, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_k__7 = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "ft4222/ft4222.pyx":1
@@ -15067,28 +15127,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -16226,61 +16286,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-    #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    #ifndef __PYX_HAVE_RT_ImportType_0_29_35
+#define __PYX_HAVE_RT_ImportType_0_29_35
+static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -17022,15 +17100,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -17586,15 +17667,15 @@
                         } else if (8 * sizeof(DWORD) >= 4 * PyLong_SHIFT) {
                             return (DWORD) (((((((((DWORD)digits[3]) << PyLong_SHIFT) | (DWORD)digits[2]) << PyLong_SHIFT) | (DWORD)digits[1]) << PyLong_SHIFT) | (DWORD)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -17782,15 +17863,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -17978,15 +18059,15 @@
                         } else if (8 * sizeof(ULONG) >= 4 * PyLong_SHIFT) {
                             return (ULONG) (((((((((ULONG)digits[3]) << PyLong_SHIFT) | (ULONG)digits[2]) << PyLong_SHIFT) | (ULONG)digits[1]) << PyLong_SHIFT) | (ULONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -18174,15 +18255,15 @@
                         } else if (8 * sizeof(FT4222_ClockRate) >= 4 * PyLong_SHIFT) {
                             return (FT4222_ClockRate) (((((((((FT4222_ClockRate)digits[3]) << PyLong_SHIFT) | (FT4222_ClockRate)digits[2]) << PyLong_SHIFT) | (FT4222_ClockRate)digits[1]) << PyLong_SHIFT) | (FT4222_ClockRate)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -18408,15 +18489,15 @@
                         } else if (8 * sizeof(BOOL) >= 4 * PyLong_SHIFT) {
                             return (BOOL) (((((((((BOOL)digits[3]) << PyLong_SHIFT) | (BOOL)digits[2]) << PyLong_SHIFT) | (BOOL)digits[1]) << PyLong_SHIFT) | (BOOL)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -18642,15 +18723,15 @@
                         } else if (8 * sizeof(UCHAR) >= 4 * PyLong_SHIFT) {
                             return (UCHAR) (((((((((UCHAR)digits[3]) << PyLong_SHIFT) | (UCHAR)digits[2]) << PyLong_SHIFT) | (UCHAR)digits[1]) << PyLong_SHIFT) | (UCHAR)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -18838,15 +18919,15 @@
                         } else if (8 * sizeof(USHORT) >= 4 * PyLong_SHIFT) {
                             return (USHORT) (((((((((USHORT)digits[3]) << PyLong_SHIFT) | (USHORT)digits[2]) << PyLong_SHIFT) | (USHORT)digits[1]) << PyLong_SHIFT) | (USHORT)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -19072,15 +19153,15 @@
                         } else if (8 * sizeof(GPIO_Dir) >= 4 * PyLong_SHIFT) {
                             return (GPIO_Dir) (((((((((GPIO_Dir)digits[3]) << PyLong_SHIFT) | (GPIO_Dir)digits[2]) << PyLong_SHIFT) | (GPIO_Dir)digits[1]) << PyLong_SHIFT) | (GPIO_Dir)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -19268,15 +19349,15 @@
                         } else if (8 * sizeof(GPIO_Port) >= 4 * PyLong_SHIFT) {
                             return (GPIO_Port) (((((((((GPIO_Port)digits[3]) << PyLong_SHIFT) | (GPIO_Port)digits[2]) << PyLong_SHIFT) | (GPIO_Port)digits[1]) << PyLong_SHIFT) | (GPIO_Port)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -19502,15 +19583,15 @@
                         } else if (8 * sizeof(GPIO_Trigger) >= 4 * PyLong_SHIFT) {
                             return (GPIO_Trigger) (((((((((GPIO_Trigger)digits[3]) << PyLong_SHIFT) | (GPIO_Trigger)digits[2]) << PyLong_SHIFT) | (GPIO_Trigger)digits[1]) << PyLong_SHIFT) | (GPIO_Trigger)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -19698,15 +19779,15 @@
                         } else if (8 * sizeof(uint16_t) >= 4 * PyLong_SHIFT) {
                             return (uint16_t) (((((((((uint16_t)digits[3]) << PyLong_SHIFT) | (uint16_t)digits[2]) << PyLong_SHIFT) | (uint16_t)digits[1]) << PyLong_SHIFT) | (uint16_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -19932,15 +20013,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20166,15 +20247,15 @@
                         } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
                             return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20400,15 +20481,15 @@
                         } else if (8 * sizeof(SPI_DrivingStrength) >= 4 * PyLong_SHIFT) {
                             return (SPI_DrivingStrength) (((((((((SPI_DrivingStrength)digits[3]) << PyLong_SHIFT) | (SPI_DrivingStrength)digits[2]) << PyLong_SHIFT) | (SPI_DrivingStrength)digits[1]) << PyLong_SHIFT) | (SPI_DrivingStrength)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20596,15 +20677,15 @@
                         } else if (8 * sizeof(FT4222_SPIMode) >= 4 * PyLong_SHIFT) {
                             return (FT4222_SPIMode) (((((((((FT4222_SPIMode)digits[3]) << PyLong_SHIFT) | (FT4222_SPIMode)digits[2]) << PyLong_SHIFT) | (FT4222_SPIMode)digits[1]) << PyLong_SHIFT) | (FT4222_SPIMode)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20792,15 +20873,15 @@
                         } else if (8 * sizeof(FT4222_SPIClock) >= 4 * PyLong_SHIFT) {
                             return (FT4222_SPIClock) (((((((((FT4222_SPIClock)digits[3]) << PyLong_SHIFT) | (FT4222_SPIClock)digits[2]) << PyLong_SHIFT) | (FT4222_SPIClock)digits[1]) << PyLong_SHIFT) | (FT4222_SPIClock)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -20988,15 +21069,15 @@
                         } else if (8 * sizeof(FT4222_SPICPOL) >= 4 * PyLong_SHIFT) {
                             return (FT4222_SPICPOL) (((((((((FT4222_SPICPOL)digits[3]) << PyLong_SHIFT) | (FT4222_SPICPOL)digits[2]) << PyLong_SHIFT) | (FT4222_SPICPOL)digits[1]) << PyLong_SHIFT) | (FT4222_SPICPOL)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21184,15 +21265,15 @@
                         } else if (8 * sizeof(FT4222_SPICPHA) >= 4 * PyLong_SHIFT) {
                             return (FT4222_SPICPHA) (((((((((FT4222_SPICPHA)digits[3]) << PyLong_SHIFT) | (FT4222_SPICPHA)digits[2]) << PyLong_SHIFT) | (FT4222_SPICPHA)digits[1]) << PyLong_SHIFT) | (FT4222_SPICPHA)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21380,15 +21461,15 @@
                         } else if (8 * sizeof(SPI_SlaveProtocol) >= 4 * PyLong_SHIFT) {
                             return (SPI_SlaveProtocol) (((((((((SPI_SlaveProtocol)digits[3]) << PyLong_SHIFT) | (SPI_SlaveProtocol)digits[2]) << PyLong_SHIFT) | (SPI_SlaveProtocol)digits[1]) << PyLong_SHIFT) | (SPI_SlaveProtocol)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21576,15 +21657,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -21772,15 +21853,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `ft4222-1.8.0/ft4222/ft4222.pyi` & `ft4222-1.8.1/ft4222/ft4222.pyi`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/ft4222/ft4222.pyx` & `ft4222-1.8.1/ft4222/ft4222.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,28 @@
     if status == FT_OK:
         return {'index': devnum, 'flags': f, 'type': t,
                 'id': i, 'location': l, 'serial': n,
                 'description': d, 'handle': <size_t>h}
     raise FT2XXDeviceError, status
 
 def openBySerial(serial):
-    """Open a handle to a usb device by serial number"""
+    """Open a handle to a usb device by serial number
+
+    Args:
+        serial (bytes, str): Serial number
+
+    Returns:
+        :obj:`FT4222`: Opened device
+
+    Raises:
+        FT2XXDeviceError: on error
+
+    """
+    if isinstance(serial, str):
+        serial = serial.encode('utf-8')
     cdef FT_HANDLE handle
     cdef char* cserial = serial
     status = FT_OpenEx(<PVOID>cserial, FT_OPEN_BY_SERIAL_NUMBER, &handle)
     if status == FT_OK:
         return FT4222(<uintptr_t>handle, update=False)
     raise FT2XXDeviceError, status
```

### Comparing `ft4222-1.8.0/ft4222.egg-info/PKG-INFO` & `ft4222-1.8.1/ft4222.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ft4222
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python wrapper around libFT4222.
 Home-page: https://gitlab.com/msrelectronics/python-ft4222
 Author: Bearsh
 Author-email: me@bearsh.org
 License: MIT
 Keywords: ftdi ft4222
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ft4222-1.8.0/ft4222.egg-info/SOURCES.txt` & `ft4222-1.8.1/ft4222.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/WinTypes.h` & `ft4222-1.8.1/linux/WinTypes.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v6-hf/libft4222.so` & `ft4222-1.8.1/linux/build-arm-v6-hf/libft4222.so`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v6-hf/libft4222.so.1.4.4.170` & `ft4222-1.8.1/linux/build-arm-v6-hf/libft4222.so.1.4.4.170`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v7-hf/libft4222.so` & `ft4222-1.8.1/linux/build-arm-v7-hf/libft4222.so`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v7-hf/libft4222.so.1.4.4.170` & `ft4222-1.8.1/linux/build-arm-v7-hf/libft4222.so.1.4.4.170`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v8/libft4222.so` & `ft4222-1.8.1/linux/build-arm-v8/libft4222.so`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-arm-v8/libft4222.so.1.4.4.170` & `ft4222-1.8.1/linux/build-arm-v8/libft4222.so.1.4.4.170`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-i386/libft4222.so` & `ft4222-1.8.1/linux/build-i386/libft4222.so`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-i386/libft4222.so.1.4.4.44` & `ft4222-1.8.1/linux/build-i386/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-x86_64/libft4222.so` & `ft4222-1.8.1/linux/build-x86_64/libft4222.so`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/build-x86_64/libft4222.so.1.4.4.170` & `ft4222-1.8.1/linux/build-x86_64/libft4222.so.1.4.4.170`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/ftd2xx.h` & `ft4222-1.8.1/linux/ftd2xx.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/linux/libft4222.h` & `ft4222-1.8.1/linux/libft4222.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/WinTypes.h` & `ft4222-1.8.1/osx/WinTypes.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/ftd2xx.h` & `ft4222-1.8.1/osx/ftd2xx.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/libft4222.1.4.4.170.dylib` & `ft4222-1.8.1/osx/libft4222.1.4.4.170.dylib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/libft4222.dylib` & `ft4222-1.8.1/osx/libft4222.dylib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/libft4222.h` & `ft4222-1.8.1/osx/libft4222.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/osx/libftd2xx.dylib` & `ft4222-1.8.1/osx/libftd2xx.dylib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/setup.py` & `ft4222-1.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/LibFT4222.h` & `ft4222-1.8.1/win/LibFT4222.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/amd64/LibFT4222-64.dll` & `ft4222-1.8.1/win/amd64/LibFT4222-64.dll`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/amd64/LibFT4222-64.lib` & `ft4222-1.8.1/win/amd64/LibFT4222-64.lib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/amd64/ftd2xx.dll` & `ft4222-1.8.1/win/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/amd64/ftd2xx.lib` & `ft4222-1.8.1/win/amd64/ftd2xx.lib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/ftd2xx.h` & `ft4222-1.8.1/win/ftd2xx.h`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/i386/LibFT4222.dll` & `ft4222-1.8.1/win/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/i386/LibFT4222.lib` & `ft4222-1.8.1/win/i386/LibFT4222.lib`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/i386/ftd2xx.dll` & `ft4222-1.8.1/win/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `ft4222-1.8.0/win/i386/ftd2xx.lib` & `ft4222-1.8.1/win/i386/ftd2xx.lib`

 * *Files identical despite different names*

