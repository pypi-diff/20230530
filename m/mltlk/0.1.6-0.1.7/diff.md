# Comparing `tmp/mltlk-0.1.6.tar.gz` & `tmp/mltlk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.6.tar", last modified: Tue May 30 13:14:13 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.7.tar", last modified: Tue May 30 13:26:47 2023, max compression
```

## Comparing `mltlk-0.1.6.tar` & `mltlk-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.217481 mltlk-0.1.6/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.6/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.6/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:14:13.216711 mltlk-0.1.6/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.6/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.6/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.6/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.6/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    33244 2023-05-30 13:13:01.000000 mltlk-0.1.6/Wikipedia_exploration.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.6/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.182569 mltlk-0.1.6/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.6/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.6/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.6/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.206134 mltlk-0.1.6/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 13:12:34.000000 mltlk-0.1.6/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     7897 2023-05-30 13:12:12.000000 mltlk-0.1.6/mltlk/exploration_textdata.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.6/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.6/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.6/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.6/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.213591 mltlk-0.1.6/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 13:14:13.000000 mltlk-0.1.6/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 13:14:13.217758 mltlk-0.1.6/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 13:12:25.000000 mltlk-0.1.6/setup.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.214912 mltlk-0.1.6/stopwords/
--rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.6/stopwords/custom.csv
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.289176 mltlk-0.1.7/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.7/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.7/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:26:47.288370 mltlk-0.1.7/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.7/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.7/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.7/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.7/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    33375 2023-05-30 13:24:23.000000 mltlk-0.1.7/Wikipedia_exploration.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.7/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.264558 mltlk-0.1.7/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.7/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.7/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.7/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.278140 mltlk-0.1.7/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 13:22:24.000000 mltlk-0.1.7/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     8047 2023-05-30 13:23:32.000000 mltlk-0.1.7/mltlk/exploration_textdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.7/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.7/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.7/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.7/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.285427 mltlk-0.1.7/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:26:46.000000 mltlk-0.1.7/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 13:26:46.000000 mltlk-0.1.7/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 13:26:47.000000 mltlk-0.1.7/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 13:26:47.289479 mltlk-0.1.7/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 13:22:32.000000 mltlk-0.1.7/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:26:47.286887 mltlk-0.1.7/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.7/stopwords/custom.csv
```

### Comparing `mltlk-0.1.6/LICENSE` & `mltlk-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/Spiral.ipynb` & `mltlk-0.1.7/Spiral.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/Weather.ipynb` & `mltlk-0.1.7/Weather.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/Wikipedia.ipynb` & `mltlk-0.1.7/Wikipedia.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/Wikipedia_exploration.ipynb` & `mltlk-0.1.7/Wikipedia_exploration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998090277777778%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.7\\n']}}}, 9: {'outputs': {1: {'data': "*

 * *            '{\'text/html\': ["<table><tr><td '*

 * *            "style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px "*

 * *            "solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td "*

 * *            "style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padd […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.6\n"
+                        "0.1.7\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -168,15 +168,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>24.31%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap<br><font style='font-weight: normal'>(Jaccard Similarity)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>24.31%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -188,15 +188,15 @@
                         "\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap<br><font style='font-weight: normal'>(Overlap Coefficient)</font></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
```

### Comparing `mltlk-0.1.6/Wikipedia_word2vec.ipynb` & `mltlk-0.1.7/Wikipedia_word2vec.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/data/spiral.csv` & `mltlk-0.1.7/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/data/wikipedia_300.csv.gz` & `mltlk-0.1.7/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/mltlk/exploration_textdata.py` & `mltlk-0.1.7/mltlk/exploration_textdata.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,27 +203,29 @@
                     overlap = wrds1.intersection(wrds2)
                     res = [len(overlap)/len(tot), len(overlap)/min(len(wrds1),len(wrds2)), len(wrds1), len(wrds2)]
                     cache_overlap[key] = res
             
                 # Check similarity to use
                 if similarity in [2, "oc", "overlap coefficient", "overlap"]:
                     tab.append([cat1, res[2], cat2, res[3], res[1]])
+                    lbl = "(Overlap Coefficient)"
                 elif similarity in [1, "ji", "jaccard similarity", "jaccard"]:
                     tab.append([cat1, res[2], cat2, res[3], res[0]])
+                    lbl = "(Jaccard Similarity)"
                 else:
                     error("Unknown similarity " + colored(similarity, "cyan"))
                     return
     tab = sorted(tab, key=lambda x: x[4], reverse=True)
     
     # Start and end index
     si = sidx
     if sidx < 0:
         si = len(tab) + sidx
     
-    t = CustomizedTable(["", "Category 1", "Words", "Category 2", "Words", "Overlap"])
+    t = CustomizedTable(["", "Category 1", "Words", "Category 2", "Words", f"Overlap<br><font style='font-weight: normal'>{lbl}</font>"])
     t.column_style(0, {"color": "size"})
     t.column_style([1, 3], {"color": "name"})
     t.column_style([2, 4], {"color": "value"})
     t.column_style(5, {"color": "percent", "num-format": "pct-2"})
     for i,r in enumerate(tab[si:si+n]):
         t.add_row([si+i] + r)
     print()
```

### Comparing `mltlk-0.1.6/mltlk/ml.py` & `mltlk-0.1.7/mltlk/ml.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/mltlk/resampling.py` & `mltlk-0.1.7/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/mltlk/utils.py` & `mltlk-0.1.7/mltlk/utils.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.6/mltlk/word2vec.py` & `mltlk-0.1.7/mltlk/word2vec.py`

 * *Files identical despite different names*

