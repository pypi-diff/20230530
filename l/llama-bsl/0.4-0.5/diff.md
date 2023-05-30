# Comparing `tmp/llama-bsl-0.4.tar.gz` & `tmp/llama-bsl-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/llama-bsl/dist/tmplc77iyqu/llama-bsl-0.4.tar", last modified: Mon Sep 13 00:32:22 2021, max compression
+gzip compressed data, was "llama-bsl-0.5.tar", last modified: Tue May 30 17:14:05 2023, max compression
```

## Comparing `llama-bsl-0.4.tar` & `llama-bsl-0.5.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-09-13 00:32:22.000000 llama-bsl-0.4/
--rw-r--r--   0 pi        (1000) pi        (1000)      321 2021-09-13 00:22:03.000000 llama-bsl-0.4/.gitignore
--rw-r--r--   0 pi        (1000) pi        (1000)      238 2021-09-13 00:22:03.000000 llama-bsl-0.4/.travis.yml
--rw-r--r--   0 pi        (1000) pi        (1000)      546 2021-09-13 00:31:57.000000 llama-bsl-0.4/Makefile
--rw-r--r--   0 pi        (1000) pi        (1000)     1987 2021-09-13 00:32:22.000000 llama-bsl-0.4/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1183 2021-09-13 00:22:03.000000 llama-bsl-0.4/README.md
--rwxr-xr-x   0 pi        (1000) pi        (1000)    53138 2021-09-13 00:22:03.000000 llama-bsl-0.4/llama-bsl.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1987 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      284 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       72 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2021-09-13 00:32:22.000000 llama-bsl-0.4/llama_bsl.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      103 2021-09-13 00:22:03.000000 llama-bsl-0.4/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       37 2021-09-13 00:22:03.000000 llama-bsl-0.4/requirements.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2021-09-13 00:32:22.000000 llama-bsl-0.4/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     1147 2021-09-13 00:24:43.000000 llama-bsl-0.4/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2021-09-13 00:32:22.000000 llama-bsl-0.4/tests/
--rw-r--r--   0 pi        (1000) pi        (1000)      878 2021-09-13 00:22:03.000000 llama-bsl-0.4/tests/test_cc2538-bsl.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:05.390982 llama-bsl-0.5/
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:05.373932 llama-bsl-0.5/.github/
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:05.381946 llama-bsl-0.5/.github/workflows/
+-rw-rw-rw-   0        0        0      603 2023-05-28 20:31:17.000000 llama-bsl-0.5/.github/workflows/main.yml
+-rw-rw-rw-   0        0        0      350 2021-09-12 11:17:53.000000 llama-bsl-0.5/.gitignore
+-rw-rw-rw-   0        0        0      253 2021-09-10 15:56:32.000000 llama-bsl-0.5/.travis.yml
+-rw-rw-rw-   0        0        0     1541 2023-05-28 20:31:17.000000 llama-bsl-0.5/LICENSE.md
+-rw-rw-rw-   0        0        0      577 2023-05-30 16:57:26.000000 llama-bsl-0.5/Makefile
+-rw-rw-rw-   0        0        0     2058 2023-05-30 17:14:05.389979 llama-bsl-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1209 2021-09-10 21:07:12.000000 llama-bsl-0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:05.386984 llama-bsl-0.5/llama_bsl.egg-info/
+-rw-rw-rw-   0        0        0     2058 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       72 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 17:14:05.000000 llama-bsl-0.5/llama_bsl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    54600 2023-05-30 16:41:05.000000 llama-bsl-0.5/llama_bsl.py
+-rw-rw-rw-   0        0        0      108 2023-05-30 14:50:13.000000 llama-bsl-0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-28 20:31:17.000000 llama-bsl-0.5/requirements-test.txt
+-rw-rw-rw-   0        0        0       39 2021-09-12 11:20:37.000000 llama-bsl-0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 17:14:05.390982 llama-bsl-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1318 2023-05-30 14:50:06.000000 llama-bsl-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:14:05.389979 llama-bsl-0.5/tests/
+-rw-rw-rw-   0        0        0   360448 2019-12-09 23:06:46.000000 llama-bsl-0.5/tests/blink_LED-DIO7_BSL-DIO13_zzh-only.bin
+-rw-rw-rw-   0        0        0      926 2023-05-30 14:50:19.000000 llama-bsl-0.5/tests/test_cc2538-bsl.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 14:50:21.000000 llama-bsl-0.5/tests/test_ext_call.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `llama-bsl-0.4/PKG-INFO` & `llama-bsl-0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1
-Name: llama-bsl
-Version: 0.4
-Summary: Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)
-Home-page: https://github.com/electrolama/llama-bsl
-Author: Omer Kilic
-Author-email: omerkilic@gmail.com
-License: BSD-3-Clause
-Keywords: cc2538,cc1310,cc13xx,bootloader,cc26xx,cc2650,cc2640
-Platform: posix
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.4
-
-# llama-bsl
-
-This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
-
-### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
-
-
-## Why fork?
-
-We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
-
-Any generally applicable additions/fixes will be submitted upstream.
-
-
-## Usage
-
-Documentation for new features will be added once fully tested, refer to commit history to see changes.
-
-Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
-
-
-## Authors
-
-[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
-
-llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
-
-
+Metadata-Version: 2.1
+Name: llama-bsl
+Version: 0.5
+Summary: Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)
+Home-page: https://github.com/electrolama/llama-bsl
+Author: Omer Kilic
+Author-email: omerkilic@gmail.com
+License: BSD-3-Clause
+Keywords: cc2538,cc1310,cc13xx,bootloader,cc26xx,cc2650,cc2640
+Platform: posix
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.4
+License-File: LICENSE.md
+
+# llama-bsl
+
+This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
+
+### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
+
+
+## Why fork?
+
+We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
+
+Any generally applicable additions/fixes will be submitted upstream.
+
+
+## Usage
+
+Documentation for new features will be added once fully tested, refer to commit history to see changes.
+
+Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
+
+
+## Authors
+
+[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
+
+llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
```

### Comparing `llama-bsl-0.4/README.md` & `llama-bsl-0.5/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# llama-bsl
-
-This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
-
-### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
-
-
-## Why fork?
-
-We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
-
-Any generally applicable additions/fixes will be submitted upstream.
-
-
-## Usage
-
-Documentation for new features will be added once fully tested, refer to commit history to see changes.
-
-Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
-
-
-## Authors
-
-[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
-
-llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
+# llama-bsl
+
+This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
+
+### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
+
+
+## Why fork?
+
+We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
+
+Any generally applicable additions/fixes will be submitted upstream.
+
+
+## Usage
+
+Documentation for new features will be added once fully tested, refer to commit history to see changes.
+
+Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
+
+
+## Authors
+
+[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
+
+llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
```

### Comparing `llama-bsl-0.4/llama_bsl.egg-info/PKG-INFO` & `llama-bsl-0.5/llama_bsl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,48 @@
-Metadata-Version: 2.1
-Name: llama-bsl
-Version: 0.4
-Summary: Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)
-Home-page: https://github.com/electrolama/llama-bsl
-Author: Omer Kilic
-Author-email: omerkilic@gmail.com
-License: BSD-3-Clause
-Keywords: cc2538,cc1310,cc13xx,bootloader,cc26xx,cc2650,cc2640
-Platform: posix
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.4
-
-# llama-bsl
-
-This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
-
-### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
-
-
-## Why fork?
-
-We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
-
-Any generally applicable additions/fixes will be submitted upstream.
-
-
-## Usage
-
-Documentation for new features will be added once fully tested, refer to commit history to see changes.
-
-Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
-
-
-## Authors
-
-[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
-
-llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
-
-
+Metadata-Version: 2.1
+Name: llama-bsl
+Version: 0.5
+Summary: Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)
+Home-page: https://github.com/electrolama/llama-bsl
+Author: Omer Kilic
+Author-email: omerkilic@gmail.com
+License: BSD-3-Clause
+Keywords: cc2538,cc1310,cc13xx,bootloader,cc26xx,cc2650,cc2640
+Platform: posix
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.4
+License-File: LICENSE.md
+
+# llama-bsl
+
+This is a nascent fork of the ever-popular [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) script that is widely used with TI's serial bootloader for CC13xx/CC26xx/CC2538 series of chips. 
+
+### Warning: This is an experimental fork with features that can disable BSL on your boards. Do not use if you're not comfortable with JTAG recovery until a fully tested release is published.
+
+
+## Why fork?
+
+We're adding features that only make sense in limited context, therefore unlikely to be ever merged upstream.
+
+Any generally applicable additions/fixes will be submitted upstream.
+
+
+## Usage
+
+Documentation for new features will be added once fully tested, refer to commit history to see changes.
+
+Original README can be found [here](https://github.com/JelmerT/cc2538-bsl/blob/master/README.md).
+
+
+## Authors
+
+[@OmerK](https://twitter.com/omerk) and [contributors](https://github.com/electrolama/llama-bsl/graphs/contributors).
+
+llama-bsl is a fork of [cc2538-bsl.py](https://github.com/JelmerT/cc2538-bsl/) created by Jelmer Tiete <jelmer@tiete.be>, which is in turn based on [stm32loader](https://github.com/jsnyder/stm32loader) by Ivan A-R <ivan@tuxotronic.org>
```

### Comparing `llama-bsl-0.4/setup.py` & `llama-bsl-0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-from setuptools import setup
-
-setup(
-    name="llama-bsl",
-    version="v0.4",
-    description="Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)",
-    long_description=open("README.md", encoding="utf-8").read(),
-    keywords="cc2538, cc1310, cc13xx, bootloader, cc26xx, cc2650, cc2640",
-    url="https://github.com/electrolama/llama-bsl",
-    author="Omer Kilic",
-    author_email="omerkilic@gmail.com",
-    license="BSD-3-Clause",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: BSD License",
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS",
-        "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python :: 3",
-        "Topic :: Scientific/Engineering",
-    ],
-    platforms="posix",
-    python_requires=">=3.4",
-    setup_requires=["setuptools_scm"],
-    install_requires=["pip>=10", "setuptools", "wheel", "pyserial==3.5", "intelhex==2.3.0", "requests==2.26.0"],
-    scripts=["llama-bsl.py"],
-)
+from setuptools import setup
+
+setup(
+    name="llama-bsl",
+    version="v0.5",
+    description="Script to communicate with Texas Instruments CC13xx/CC2538/CC26xx Serial Boot Loader (Fork of cc2538-bsl.py)",
+    long_description=open("README.md", encoding="utf-8").read(),
+    keywords="cc2538, cc1310, cc13xx, bootloader, cc26xx, cc2650, cc2640",
+    url="https://github.com/electrolama/llama-bsl",
+    author="Omer Kilic",
+    author_email="omerkilic@gmail.com",
+    license="BSD-3-Clause",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: BSD License",
+        "Operating System :: POSIX :: Linux",
+        "Operating System :: MacOS",
+        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
+    ],
+    platforms="posix",
+    python_requires=">=3.4",
+    setup_requires=["setuptools_scm"],
+    install_requires=[
+        "pip>=10",
+        "setuptools",
+        "wheel",
+        "pyserial==3.5",
+        "intelhex==2.3.0",
+        "requests==2.26.0",
+    ],
+    entry_points={
+        "console_scripts": [
+            "llama-bsl=llama_bsl:main",
+        ],
+    },
+)
```

