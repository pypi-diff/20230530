# Comparing `tmp/iydon-2023.3.2.tar.gz` & `tmp/iydon-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iydon-2023.3.2.tar", max compression
+gzip compressed data, was "iydon-2023.4.tar", max compression
```

## Comparing `iydon-2023.3.2.tar` & `iydon-2023.4.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      266 2023-03-28 14:28:37.296806 iydon-2023.3.2/iydon/__init__.py
--rw-r--r--   0        0        0       66 2023-03-21 14:54:40.262377 iydon-2023.3.2/iydon/base/__init__.py
--rw-r--r--   0        0        0      326 2023-03-28 14:59:19.407554 iydon-2023.3.2/iydon/base/constant.py
--rw-r--r--   0        0        0      817 2023-03-28 14:35:27.045363 iydon-2023.3.2/iydon/base/type.py
--rw-r--r--   0        0        0       46 2023-03-28 14:36:49.171772 iydon-2023.3.2/iydon/namespace/__init__.py
--rw-r--r--   0        0        0       46 2023-03-28 14:40:21.306083 iydon-2023.3.2/iydon/namespace/brief.py
--rw-r--r--   0        0        0      226 2023-03-28 14:58:59.359564 iydon-2023.3.2/iydon/namespace/full.py
--rw-r--r--   0        0        0      204 2023-03-28 14:41:46.533808 iydon-2023.3.2/iydon/namespace/private.py
--rw-r--r--   0        0        0       78 2023-03-28 14:29:48.482416 iydon-2023.3.2/iydon/test/__init__.py
--rw-r--r--   0        0        0      318 2023-03-28 14:29:29.413206 iydon-2023.3.2/iydon/test/test_glhf.py
--rw-r--r--   0        0        0      254 2023-03-28 14:28:08.272139 iydon-2023.3.2/iydon/test/test_rust.py
--rw-r--r--   0        0        0       46 2023-03-28 14:33:53.095849 iydon-2023.3.2/iydon/util/__init__.py
--rw-r--r--   0        0        0       80 2023-03-27 10:26:00.514888 iydon-2023.3.2/iydon/util/glhf/__init__.py
--rw-r--r--   0        0        0     1821 2023-03-28 14:24:40.190531 iydon-2023.3.2/iydon/util/glhf/end.py
--rw-r--r--   0        0        0      262 2023-03-28 14:25:08.077434 iydon-2023.3.2/iydon/util/glhf/silver_bullet.py
--rw-r--r--   0        0        0      150 2023-03-28 14:26:12.106703 iydon-2023.3.2/iydon/util/rust/__init__.py
--rw-r--r--   0        0        0       66 2023-03-28 14:25:49.036826 iydon-2023.3.2/iydon/util/rust/std/__init__.py
--rw-r--r--   0        0        0    19368 2023-03-28 14:25:51.255666 iydon-2023.3.2/iydon/util/rust/std/option.py
--rw-r--r--   0        0        0    21087 2023-03-28 14:27:54.803371 iydon-2023.3.2/iydon/util/rust/std/result.py
--rw-r--r--   0        0        0    35823 2022-05-01 07:51:55.316123 iydon-2023.3.2/LICENSE.txt
--rw-r--r--   0        0        0     1668 2023-03-28 14:59:19.388320 iydon-2023.3.2/pyproject.toml
--rw-r--r--   0        0        0     8396 2023-03-23 19:03:38.960567 iydon-2023.3.2/README.md
--rw-r--r--   0        0        0     9214 2023-03-28 14:59:27.260791 iydon-2023.3.2/setup.py
--rw-r--r--   0        0        0     9438 2023-03-28 14:59:27.260791 iydon-2023.3.2/PKG-INFO
+-rw-r--r--   0        0        0      266 2023-03-28 14:28:37.296806 iydon-2023.4/iydon/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-21 14:54:40.262377 iydon-2023.4/iydon/base/__init__.py
+-rw-r--r--   0        0        0      324 2023-05-30 09:51:23.365805 iydon-2023.4/iydon/base/constant.py
+-rw-r--r--   0        0        0      817 2023-03-28 15:00:41.839863 iydon-2023.4/iydon/base/type.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:36:49.171772 iydon-2023.4/iydon/namespace/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:40:21.306083 iydon-2023.4/iydon/namespace/brief.py
+-rw-r--r--   0        0        0      226 2023-03-28 15:00:39.012518 iydon-2023.4/iydon/namespace/full.py
+-rw-r--r--   0        0        0      204 2023-03-28 14:41:46.533808 iydon-2023.4/iydon/namespace/private.py
+-rw-r--r--   0        0        0       78 2023-03-28 14:29:48.482416 iydon-2023.4/iydon/test/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-28 14:29:29.413206 iydon-2023.4/iydon/test/test_glhf.py
+-rw-r--r--   0        0        0      254 2023-03-28 14:28:08.272139 iydon-2023.4/iydon/test/test_rust.py
+-rw-r--r--   0        0        0       46 2023-03-28 14:33:53.095849 iydon-2023.4/iydon/util/__init__.py
+-rw-r--r--   0        0        0       80 2023-03-27 10:26:00.514888 iydon-2023.4/iydon/util/glhf/__init__.py
+-rw-r--r--   0        0        0     1821 2023-03-28 14:24:40.190531 iydon-2023.4/iydon/util/glhf/end.py
+-rw-r--r--   0        0        0      262 2023-03-28 14:25:08.077434 iydon-2023.4/iydon/util/glhf/silver_bullet.py
+-rw-r--r--   0        0        0      150 2023-03-28 14:26:12.106703 iydon-2023.4/iydon/util/rust/__init__.py
+-rw-r--r--   0        0        0       66 2023-03-28 14:25:49.036826 iydon-2023.4/iydon/util/rust/std/__init__.py
+-rw-r--r--   0        0        0    19368 2023-03-28 14:25:51.255666 iydon-2023.4/iydon/util/rust/std/option.py
+-rw-r--r--   0        0        0    21087 2023-03-28 14:27:54.803371 iydon-2023.4/iydon/util/rust/std/result.py
+-rw-r--r--   0        0        0    35823 2022-05-01 07:51:55.316123 iydon-2023.4/LICENSE.txt
+-rw-r--r--   0        0        0     1772 2023-05-30 09:51:23.318523 iydon-2023.4/pyproject.toml
+-rw-r--r--   0        0        0     8396 2023-03-23 19:03:38.960567 iydon-2023.4/README.md
+-rw-r--r--   0        0        0     9689 1970-01-01 00:00:00.000000 iydon-2023.4/PKG-INFO
```

### Comparing `iydon-2023.3.2/iydon/base/type.py` & `iydon-2023.4/iydon/base/type.py`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/iydon/util/glhf/end.py` & `iydon-2023.4/iydon/util/glhf/end.py`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/iydon/util/rust/std/option.py` & `iydon-2023.4/iydon/util/rust/std/option.py`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/iydon/util/rust/std/result.py` & `iydon-2023.4/iydon/util/rust/std/result.py`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/LICENSE.txt` & `iydon-2023.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/pyproject.toml` & `iydon-2023.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iydon"
-version = "2023.3.2"  # year.month.iota
+version = "2023.4"  # year.iota
 description = "Iydon's common tools"
 authors = ["Iydon Liang <liangiydon@gmail.com>"]
 keywords = ["utilities"]
 readme = "README.md"
 license = "GPL-3.0-only"
 homepage = "https://github.com/iydon/iydon"
 repository = "https://github.com/iydon/iydon"
@@ -35,19 +35,26 @@
 typing-extensions = {version = "^4.5.0", optional = true}
 
 [tool.poetry.extras]
 type = ["typing-extensions"]
 full = ["typing-extensions"]
 
 [tool.poetry.dev-dependencies]
-PyGithub = "^1.58.1"
-tqdm = "^4.65.0"
-mypy = "^1.1.1"
-pytest = "^7.2.2"
-nox-poetry = "^1.0.2"
+click = "^8.1.3"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.4"
 mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+mypy = "^1.1.1"
+nox-poetry = "^1.0.2"
+PyGithub = "^1.58.1"
+pytest = "^7.2.2"
+tqdm = "^4.65.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.script.config]
+upgrade = [
+    'pyproject.toml',
+    'iydon/base/constant.py',
+]
```

### Comparing `iydon-2023.3.2/README.md` & `iydon-2023.4/README.md`

 * *Files identical despite different names*

### Comparing `iydon-2023.3.2/setup.py` & `iydon-2023.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,154 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: iydon
+Version: 2023.4
+Summary: Iydon's common tools
+Home-page: https://github.com/iydon/iydon
+License: GPL-3.0-only
+Keywords: utilities
+Author: Iydon Liang
+Author-email: liangiydon@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Provides-Extra: full
+Provides-Extra: type
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; extra == "type" or extra == "full"
+Project-URL: Bug Tracker, https://github.com/iydon/iydon/issues
+Project-URL: Repository, https://github.com/iydon/iydon
+Description-Content-Type: text/markdown
+
+<div align="center">
+  <a href="https://github.com/iydon/iydon">
+    🔵⬜🟦⬜🟦<br />
+    ⬜⬜🟦⬜🟦<br />
+    🟦⬜🟦🟦🟦<br />
+    🟦⬜⬜⬜🟦<br />
+    🟦⬜🟦🟦🟦<br />
+  </a>
+
+  <h3 align="center">Iydon (梁钰栋 in Chinese)</h3>
+
+  <p align="center">
+    <a href="https://www.iydon.top">
+      <img src="https://img.shields.io/static/v1?label=Blog&message=iydon.top&color=brightgreen" />
+    </a>
+    ·
+    <a href="https://github.com/iydon">
+      <img src="https://img.shields.io/static/v1?label=GitHub&message=iydon&color=green" />
+    </a>
+    ·
+    <a href="mailto:liangiydon@gmail.com">
+      <img src="https://img.shields.io/static/v1?label=Gmail&message=liangiydon&color=yellowgreen" />
+    </a>
+    ·
+    <a href="https://steamcommunity.com/id/iydon">
+      <img src="https://img.shields.io/static/v1?label=Steam&message=iydon&color=yellow" />
+    </a>
+    ·
+    <img src="https://visitor-badge.glitch.me/badge?page_id=iydon&right_color=orange&left_text=Visitors" />
+    ·
+    <img src="https://img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red" />
+  </p>
+</div>
+
+
+
+<details>
+  <summary><strong>GitHub Statistics</strong></summary>
+  <img src="https://github-readme-stats.vercel.app/api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite" />
+</details>
+
+
+
+<details>
+  <summary><strong>Code Statistics</strong></summary>
+  <pre><code>
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Language            Files        Lines         Code     Comments       Blanks
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Autoconf                9           45           36            0            9
+ BASH                   32           98           34           32           32
+ Batch                   7          343          289            3           51
+ C                      35        4,264        2,477        1,053          734
+ C Header               46        3,370        2,351          485          534
+ C++                    13          611          462           40          109
+ CSS                     6          493          480           12            1
+ Cython                  1           16            7            5            4
+ Dockerfile              3          215           95          100           20
+ Forge Config            2           38           38            0            0
+ FORTRAN Modern          2          201          164            0           37
+ Go                      2          140          118            0           22
+ INI                     1            6            6            0            0
+ JavaScript              2            4            4            0            0
+ JSON                   79       21,932       21,930            0            2
+ Julia                   2          120          105            0           15
+ M4                      2        1,069          927            0          142
+ MATLAB                155        6,266        4,650        1,017          599
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
+ R                       5          256          215            6           35
+ ReStructuredText       21        1,046          705            0          341
+ Shell                   9          158           91           38           29
+ SQL                    22        8,027        7,823          118           86
+ SVG                     6          968          883            1           84
+ TeX Class              26       14,091       10,548        2,413        1,130
+ TeX Definition          3          207          195           12            0
+ TeX                   676      328,270      178,952        3,421      145,897
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
+ XML                     1            7            7            0            0
+ YAML                   93       37,661       35,816        1,147          698
+───────────────────────────────────────────────────────────────────────────────
+ HTML                   32        2,626        2,231          322           73
+ |- CSS                  6          123          122            0            1
+ |- JavaScript          10          530          457           11           62
+ (Total)                          3,279        2,810          333          136
+───────────────────────────────────────────────────────────────────────────────
+ Jupyter Notebooks      11          658          324          270           64
+ |- Markdown             7          288            0          259           29
+ |- Python              10          370          324           11           35
+ (Total)                          1,316          648          540          128
+───────────────────────────────────────────────────────────────────────────────
+ Markdown              377       27,448            0       20,957        6,491
+ |- C                    1            7            6            0            1
+ |- C++                  2           78           63            2           13
+ |- HTML                 2           66           66            0            0
+ |- JSON                 2        1,096        1,096            0            0
+ |- MATLAB               1           62           28           29            5
+ |- Markdown             1           51            0           50            1
+ |- Python              36        2,017        1,621           82          314
+ |- R                    2          214          178           36            0
+ |- Rust                 2          269          237            6           26
+ |- Shell               23        1,027          979            0           48
+ |- SQL                  1            2            2            0            0
+ |- TeX                  2           42           35            0            7
+ |- TOML                 1           13           11            0            2
+ |- XML                  1            8            8            0            0
+ |- YAML                 7          263          234           17           12
+ (Total)                         32,663        4,564       21,179        6,920
+───────────────────────────────────────────────────────────────────────────────
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+ Total               2,822      754,196      364,792      216,825      172,579
+━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
+  </code></pre>
+</details>
 
-packages = \
-['iydon',
- 'iydon.base',
- 'iydon.namespace',
- 'iydon.test',
- 'iydon.util',
- 'iydon.util.glhf',
- 'iydon.util.rust',
- 'iydon.util.rust.std']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'full': ['typing-extensions>=4.5.0,<5.0.0'],
- 'type': ['typing-extensions>=4.5.0,<5.0.0']}
-
-setup_kwargs = {
-    'name': 'iydon',
-    'version': '2023.3.2',
-    'description': "Iydon's common tools",
-    'long_description': '<div align="center">\n  <a href="https://github.com/iydon/iydon">\n    🔵⬜🟦⬜🟦<br />\n    ⬜⬜🟦⬜🟦<br />\n    🟦⬜🟦🟦🟦<br />\n    🟦⬜⬜⬜🟦<br />\n    🟦⬜🟦🟦🟦<br />\n  </a>\n\n  <h3 align="center">Iydon (梁钰栋 in Chinese)</h3>\n\n  <p align="center">\n    <a href="https://www.iydon.top">\n      <img src="https://img.shields.io/static/v1?label=Blog&message=iydon.top&color=brightgreen" />\n    </a>\n    ·\n    <a href="https://github.com/iydon">\n      <img src="https://img.shields.io/static/v1?label=GitHub&message=iydon&color=green" />\n    </a>\n    ·\n    <a href="mailto:liangiydon@gmail.com">\n      <img src="https://img.shields.io/static/v1?label=Gmail&message=liangiydon&color=yellowgreen" />\n    </a>\n    ·\n    <a href="https://steamcommunity.com/id/iydon">\n      <img src="https://img.shields.io/static/v1?label=Steam&message=iydon&color=yellow" />\n    </a>\n    ·\n    <img src="https://visitor-badge.glitch.me/badge?page_id=iydon&right_color=orange&left_text=Visitors" />\n    ·\n    <img src="https://img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red" />\n  </p>\n</div>\n\n\n\n<details>\n  <summary><strong>GitHub Statistics</strong></summary>\n  <img src="https://github-readme-stats.vercel.app/api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite" />\n</details>\n\n\n\n<details>\n  <summary><strong>Code Statistics</strong></summary>\n  <pre><code>\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Language            Files        Lines         Code     Comments       Blanks\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Autoconf                9           45           36            0            9\n BASH                   32           98           34           32           32\n Batch                   7          343          289            3           51\n C                      35        4,264        2,477        1,053          734\n C Header               46        3,370        2,351          485          534\n C++                    13          611          462           40          109\n CSS                     6          493          480           12            1\n Cython                  1           16            7            5            4\n Dockerfile              3          215           95          100           20\n Forge Config            2           38           38            0            0\n FORTRAN Modern          2          201          164            0           37\n Go                      2          140          118            0           22\n INI                     1            6            6            0            0\n JavaScript              2            4            4            0            0\n JSON                   79       21,932       21,930            0            2\n Julia                   2          120          105            0           15\n M4                      2        1,069          927            0          142\n MATLAB                155        6,266        4,650        1,017          599\n Makefile               70        1,322          926           79          317\n Python                844       88,642       76,181        2,127       10,334\n R                       5          256          215            6           35\n ReStructuredText       21        1,046          705            0          341\n Shell                   9          158           91           38           29\n SQL                    22        8,027        7,823          118           86\n SVG                     6          968          883            1           84\n TeX Class              26       14,091       10,548        2,413        1,130\n TeX Definition          3          207          195           12            0\n TeX                   676      328,270      178,952        3,421      145,897\n Plain Text             66      182,314            0      180,122        2,192\n TOML                   15          469          405           10           54\n XML                     1            7            7            0            0\n YAML                   93       37,661       35,816        1,147          698\n───────────────────────────────────────────────────────────────────────────────\n HTML                   32        2,626        2,231          322           73\n |- CSS                  6          123          122            0            1\n |- JavaScript          10          530          457           11           62\n (Total)                          3,279        2,810          333          136\n───────────────────────────────────────────────────────────────────────────────\n Jupyter Notebooks      11          658          324          270           64\n |- Markdown             7          288            0          259           29\n |- Python              10          370          324           11           35\n (Total)                          1,316          648          540          128\n───────────────────────────────────────────────────────────────────────────────\n Markdown              377       27,448            0       20,957        6,491\n |- C                    1            7            6            0            1\n |- C++                  2           78           63            2           13\n |- HTML                 2           66           66            0            0\n |- JSON                 2        1,096        1,096            0            0\n |- MATLAB               1           62           28           29            5\n |- Markdown             1           51            0           50            1\n |- Python              36        2,017        1,621           82          314\n |- R                    2          214          178           36            0\n |- Rust                 2          269          237            6           26\n |- Shell               23        1,027          979            0           48\n |- SQL                  1            2            2            0            0\n |- TeX                  2           42           35            0            7\n |- TOML                 1           13           11            0            2\n |- XML                  1            8            8            0            0\n |- YAML                 7          263          234           17           12\n (Total)                         32,663        4,564       21,179        6,920\n───────────────────────────────────────────────────────────────────────────────\n Rust                  146       11,378        9,824          355        1,199\n |- Markdown             2        2,891           26        2,177          688\n (Total)                         14,269        9,850        2,532        1,887\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n Total               2,822      754,196      364,792      216,825      172,579\n━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━\n  </code></pre>\n</details>\n',
-    'author': 'Iydon Liang',
-    'author_email': 'liangiydon@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/iydon/iydon',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,102 +1,109 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['iydon',
-'iydon.base', 'iydon.namespace', 'iydon.test', 'iydon.util', 'iydon.util.glhf',
-'iydon.util.rust', 'iydon.util.rust.std'] package_data = \ {'': ['*']}
-extras_require = \ {'full': ['typing-extensions>=4.5.0,<5.0.0'], 'type':
-['typing-extensions>=4.5.0,<5.0.0']} setup_kwargs = { 'name': 'iydon',
-'version': '2023.3.2', 'description': "Iydon's common tools",
-'long_description': '
-                           \n \n_ðµâ¬ð¦â¬ð¦
-                             \n_â¬â¬ð¦â¬ð¦
-                            \n_ð¦â¬ð¦ð¦ð¦
-                             \n_ð¦â¬â¬â¬ð¦
-                            \n_ð¦â¬ð¦ð¦ð¦
-                                    \n\n\n
+Metadata-Version: 2.1 Name: iydon Version: 2023.4 Summary: Iydon's common tools
+Home-page: https://github.com/iydon/iydon License: GPL-3.0-only Keywords:
+utilities Author: Iydon Liang Author-email: liangiydon@gmail.com Requires-
+Python: >=3.7,<4.0 Classifier: Environment :: Console Classifier: License ::
+OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
+Language :: Chinese (Simplified) Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Software Development :: User Interfaces
+Classifier: Topic :: Utilities Classifier: Typing :: Typed Provides-Extra: full
+Provides-Extra: type Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; extra
+== "type" or extra == "full" Project-URL: Bug Tracker, https://github.com/
+iydon/iydon/issues Project-URL: Repository, https://github.com/iydon/iydon
+Description-Content-Type: text/markdown
+                              ðµâ¬ð¦â¬ð¦
+                               â¬â¬ð¦â¬ð¦
+                              ð¦â¬ð¦ð¦ð¦
+                               ð¦â¬â¬â¬ð¦
+                              ð¦â¬ð¦ð¦ð¦
                     **** Iydon (æ¢é°æ  in Chinese) ****
-                                     \n\n
-                     \n \n_[https://img.shields.io/static/
-   v1?label=Blog&message=iydon.top&color=brightgreen]\n\n Â·\n \n_[https://
- img.shields.io/static/v1?label=GitHub&message=iydon&color=green]\n\n Â·\n \n_
                         [https://img.shields.io/static/
-  v1?label=Gmail&message=liangiydon&color=yellowgreen]\n\n Â·\n \n_[https://
-  img.shields.io/static/v1?label=Steam&message=iydon&color=yellow]\n\n Â·\n
-                       [https://visitor-badge.glitch.me/
-  badge?page_id=iydon&right_color=orange&left_text=Visitors]\n Â·\n [https://
-     img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red]\n
-                                      \n
-\n\n\n\n\n GitHub Statistics\n [https://github-readme-stats.vercel.app/
-api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite]\n\n\n\n\n\n
-Code Statistics\n
-\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Language            Files        Lines         Code     Comments
-Blanks\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Autoconf                9           45           36            0            9\n
-BASH                   32           98           34           32           32\n
-Batch                   7          343          289            3           51\n
-C                      35        4,264        2,477        1,053          734\n
-C Header               46        3,370        2,351          485          534\n
-C++                    13          611          462           40          109\n
-CSS                     6          493          480           12            1\n
-Cython                  1           16            7            5            4\n
-Dockerfile              3          215           95          100           20\n
-Forge Config            2           38           38            0            0\n
-FORTRAN Modern          2          201          164            0           37\n
-Go                      2          140          118            0           22\n
-INI                     1            6            6            0            0\n
-JavaScript              2            4            4            0            0\n
-JSON                   79       21,932       21,930            0            2\n
-Julia                   2          120          105            0           15\n
-M4                      2        1,069          927            0          142\n
-MATLAB                155        6,266        4,650        1,017          599\n
-Makefile               70        1,322          926           79          317\n
-Python                844       88,642       76,181        2,127       10,334\n
-R                       5          256          215            6           35\n
-ReStructuredText       21        1,046          705            0          341\n
-Shell                   9          158           91           38           29\n
-SQL                    22        8,027        7,823          118           86\n
-SVG                     6          968          883            1           84\n
-TeX Class              26       14,091       10,548        2,413        1,130\n
-TeX Definition          3          207          195           12            0\n
-TeX                   676      328,270      178,952        3,421      145,897\n
-Plain Text             66      182,314            0      180,122        2,192\n
-TOML                   15          469          405           10           54\n
-XML                     1            7            7            0            0\n
-YAML                   93       37,661       35,816        1,147
-698\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-HTML                   32        2,626        2,231          322           73\n
-|- CSS                  6          123          122            0            1\n
-|- JavaScript          10          530          457           11           62\n
-(Total)                          3,279        2,810          333
-136\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Jupyter Notebooks      11          658          324          270           64\n
-|- Markdown             7          288            0          259           29\n
-|- Python              10          370          324           11           35\n
-(Total)                          1,316          648          540
-128\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Markdown              377       27,448            0       20,957        6,491\n
-|- C                    1            7            6            0            1\n
-|- C++                  2           78           63            2           13\n
-|- HTML                 2           66           66            0            0\n
-|- JSON                 2        1,096        1,096            0            0\n
-|- MATLAB               1           62           28           29            5\n
-|- Markdown             1           51            0           50            1\n
-|- Python              36        2,017        1,621           82          314\n
-|- R                    2          214          178           36            0\n
-|- Rust                 2          269          237            6           26\n
-|- Shell               23        1,027          979            0           48\n
-|- SQL                  1            2            2            0            0\n
-|- TeX                  2           42           35            0            7\n
-|- TOML                 1           13           11            0            2\n
-|- XML                  1            8            8            0            0\n
-|- YAML                 7          263          234           17           12\n
-(Total)                         32,663        4,564       21,179
-6,920\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Rust                  146       11,378        9,824          355        1,199\n
-|- Markdown             2        2,891           26        2,177          688\n
-(Total)                         14,269        9,850        2,532
-1,887\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-Total               2,822      754,196      364,792      216,825
-172,579\nâââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ\n
-\n\n', 'author': 'Iydon Liang', 'author_email': 'liangiydon@gmail.com',
-'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/iydon/
-iydon', 'packages': packages, 'package_data': package_data, 'extras_require':
-extras_require, 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
+v1?label=Blog&message=iydon.top&color=brightgreen] Â· [https://img.shields.io/
+ static/v1?label=GitHub&message=iydon&color=green] Â· [https://img.shields.io/
+   static/v1?label=Gmail&message=liangiydon&color=yellowgreen] Â· [https://
+ img.shields.io/static/v1?label=Steam&message=iydon&color=yellow] Â· [https://
+                           visitor-badge.glitch.me/
+    badge?page_id=iydon&right_color=orange&left_text=Visitors] Â· [https://
+      img.shields.io/static/v1?label=WeChat&message=liangiydon&color=red]
+ GitHub Statistics [https://github-readme-stats.vercel.app/
+api?username=iydon&count_private=true&show_icons=true&include_all_commits=true&theme=graywhite]
+Code Statistics
+
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Language            Files        Lines         Code     Comments       Blanks
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Autoconf                9           45           36            0            9
+ BASH                   32           98           34           32           32
+ Batch                   7          343          289            3           51
+ C                      35        4,264        2,477        1,053          734
+ C Header               46        3,370        2,351          485          534
+ C++                    13          611          462           40          109
+ CSS                     6          493          480           12            1
+ Cython                  1           16            7            5            4
+ Dockerfile              3          215           95          100           20
+ Forge Config            2           38           38            0            0
+ FORTRAN Modern          2          201          164            0           37
+ Go                      2          140          118            0           22
+ INI                     1            6            6            0            0
+ JavaScript              2            4            4            0            0
+ JSON                   79       21,932       21,930            0            2
+ Julia                   2          120          105            0           15
+ M4                      2        1,069          927            0          142
+ MATLAB                155        6,266        4,650        1,017          599
+ Makefile               70        1,322          926           79          317
+ Python                844       88,642       76,181        2,127       10,334
+ R                       5          256          215            6           35
+ ReStructuredText       21        1,046          705            0          341
+ Shell                   9          158           91           38           29
+ SQL                    22        8,027        7,823          118           86
+ SVG                     6          968          883            1           84
+ TeX Class              26       14,091       10,548        2,413        1,130
+ TeX Definition          3          207          195           12            0
+ TeX                   676      328,270      178,952        3,421      145,897
+ Plain Text             66      182,314            0      180,122        2,192
+ TOML                   15          469          405           10           54
+ XML                     1            7            7            0            0
+ YAML                   93       37,661       35,816        1,147          698
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ HTML                   32        2,626        2,231          322           73
+ |- CSS                  6          123          122            0            1
+ |- JavaScript          10          530          457           11           62
+ (Total)                          3,279        2,810          333          136
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Jupyter Notebooks      11          658          324          270           64
+ |- Markdown             7          288            0          259           29
+ |- Python              10          370          324           11           35
+ (Total)                          1,316          648          540          128
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Markdown              377       27,448            0       20,957        6,491
+ |- C                    1            7            6            0            1
+ |- C++                  2           78           63            2           13
+ |- HTML                 2           66           66            0            0
+ |- JSON                 2        1,096        1,096            0            0
+ |- MATLAB               1           62           28           29            5
+ |- Markdown             1           51            0           50            1
+ |- Python              36        2,017        1,621           82          314
+ |- R                    2          214          178           36            0
+ |- Rust                 2          269          237            6           26
+ |- Shell               23        1,027          979            0           48
+ |- SQL                  1            2            2            0            0
+ |- TeX                  2           42           35            0            7
+ |- TOML                 1           13           11            0            2
+ |- XML                  1            8            8            0            0
+ |- YAML                 7          263          234           17           12
+ (Total)                         32,663        4,564       21,179        6,920
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Rust                  146       11,378        9,824          355        1,199
+ |- Markdown             2        2,891           26        2,177          688
+ (Total)                         14,269        9,850        2,532        1,887
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+ Total               2,822      754,196      364,792      216,825      172,579
+âââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ
+
+
```

