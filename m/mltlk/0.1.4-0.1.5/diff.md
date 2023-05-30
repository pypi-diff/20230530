# Comparing `tmp/mltlk-0.1.4.tar.gz` & `tmp/mltlk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.4.tar", last modified: Tue May 30 11:14:11 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.5.tar", last modified: Tue May 30 12:02:58 2023, max compression
```

## Comparing `mltlk-0.1.4.tar` & `mltlk-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.271453 mltlk-0.1.4/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.4/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.4/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 11:14:11.270533 mltlk-0.1.4/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.4/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.4/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.4/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.4/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    23205 2023-05-30 11:09:49.000000 mltlk-0.1.4/Wikipedia_exploration.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.4/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.249960 mltlk-0.1.4/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.4/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.4/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.4/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.262811 mltlk-0.1.4/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 07:10:19.000000 mltlk-0.1.4/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     7301 2023-05-30 11:01:35.000000 mltlk-0.1.4/mltlk/exploration_textdata.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.4/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.4/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.4/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.4/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.267548 mltlk-0.1.4/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 11:14:10.000000 mltlk-0.1.4/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 11:14:10.000000 mltlk-0.1.4/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 11:14:11.271646 mltlk-0.1.4/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-29 08:47:52.000000 mltlk-0.1.4/setup.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.268732 mltlk-0.1.4/stopwords/
--rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.4/stopwords/custom.csv
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.722649 mltlk-0.1.5/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.5/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.5/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 12:02:58.721975 mltlk-0.1.5/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.5/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.5/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.5/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.5/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    33244 2023-05-30 12:01:38.000000 mltlk-0.1.5/Wikipedia_exploration.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.5/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.703185 mltlk-0.1.5/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.5/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.5/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.5/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.715117 mltlk-0.1.5/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 12:01:12.000000 mltlk-0.1.5/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     8137 2023-05-30 11:59:52.000000 mltlk-0.1.5/mltlk/exploration_textdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.5/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.5/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.5/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.5/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.719463 mltlk-0.1.5/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 12:02:58.722836 mltlk-0.1.5/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 12:01:05.000000 mltlk-0.1.5/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.720635 mltlk-0.1.5/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.5/stopwords/custom.csv
```

### Comparing `mltlk-0.1.4/LICENSE` & `mltlk-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/Spiral.ipynb` & `mltlk-0.1.5/Spiral.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/Weather.ipynb` & `mltlk-0.1.5/Weather.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/Wikipedia.ipynb` & `mltlk-0.1.5/Wikipedia.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/Wikipedia_exploration.ipynb` & `mltlk-0.1.5/Wikipedia_exploration.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9879427083333334%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.5\\n']}}}, 9: {'outputs': {3: {'data': "*

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
-                        "0.1.4\n"
+                        "0.1.5\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -168,15 +168,72 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>24.31%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>24.31%</td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n",
+                        "\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 1</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category 2</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Overlap</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#e2b102;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>0</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td></tr></table>"
+                        ],
+                        "text/plain": [
+                            "<IPython.core.display.HTML object>"
+                        ]
+                    },
+                    "metadata": {},
+                    "output_type": "display_data"
+                },
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                }
+            ],
+            "source": [
+                "overlap_all_categories(corpus)\n",
+                "overlap_all_categories(corpus, similarity=\"oc\")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 6,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "\n"
+                    ]
+                },
+                {
+                    "data": {
+                        "text/html": [
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Unique words</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>No documents</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>36272</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#b40403;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>29802</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'>Total words:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'>53151</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>Overlap:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>12923</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Overlap (Jaccard Similarity):</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>24.31%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Overlap (Overlap Coefficient):</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>43.36%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#3b08d3;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'></td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -186,15 +243,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
-                "overlap_all_categories(corpus)"
+                "overlap(corpus, \"Games\", \"Programming\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `mltlk-0.1.4/Wikipedia_word2vec.ipynb` & `mltlk-0.1.5/Wikipedia_word2vec.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/data/spiral.csv` & `mltlk-0.1.5/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/data/wikipedia_300.csv.gz` & `mltlk-0.1.5/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/mltlk/exploration_textdata.py` & `mltlk-0.1.5/mltlk/exploration_textdata.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from collections import Counter
 from customized_table import *
 from .utils import *
 
 
 # Caches to speed up processing
 cache_topcats = {}
-cache_overlap = {}
+cache_overlap_js = {}
+cache_overlap_oc = {}
+
 
 #
 # Builds a corpus from text data
 #
 def build_corpus(session):
     if session is None:
         error("Session is empty")
@@ -162,57 +164,73 @@
     
     t = CustomizedTable(["Category", "Unique words", "No documents"])
     t.column_style([1,2], {"color": "value"})
     t.add_row([cat1, len(wrds1), corpus["documents_per_category"][cat1]])
     t.cell_style(0, -1, {"color": "name"})
     t.add_row([cat2, len(wrds2), corpus["documents_per_category"][cat2]])
     t.cell_style(0, -1, {"color": "name"})
-    t.add_row(["Both:", len(tot), corpus["documents_per_category"][cat1]+corpus["documents_per_category"][cat2]], style={"border": "top"})
-    t.add_row(["Overlap:", f"{len(overlap)}&nbsp;&nbsp;&nbsp;{len(overlap)/len(tot)*100:.2f}%", ""])
+    t.add_row(["Total words:", len(tot), ""], style={"border": "top"})
+    t.add_row(["Overlap:", len(overlap), ""])
+    t.add_row(["Overlap (Jaccard Similarity):", f"{len(overlap)/len(tot)*100:.2f}%", ""])
+    t.add_row(["Overlap (Overlap Coefficient):", f"{len(overlap)/min(len(wrds1),len(wrds2))*100:.2f}%", ""])
     print()
     t.display()
     print()
     
 
 #
 # Check overlapping words between all categories
 #
-def overlap_all_categories(corpus, n=10, sidx=0):
-    global cache_overlap
-    done = set()
+def overlap_all_categories(corpus, n=10, sidx=0, similarity="jaccard"):
+    global cache_overlap_js, cache_overlap_oc
+    similarity = similarity.lower()
+    
+    # Check all combinations of categories
+    cats = sorted(corpus["categories"])
     tab = []
-    for cat1 in corpus["categories"]:
-        for cat2 in corpus["categories"]:
-            key1 = f"{cat1}-{cat2}"
-            key2 = f"{cat2}-{cat1}"
-            if key1 not in done and key2 not in done and key1 != key2:
-                if key1 in cache_overlap:
-                    pct = cache_overlap[key1]
-                elif key2 in cache_overlap:
-                    pct = cache_overlap[key2]
+    for i in range(0,len(cats)):
+        for j in range(i,len(cats)):
+            if i != j:
+                cat1 = cats[i]
+                cat2 = cats[j]
+                key = f"{cat1}-{cat2}"
+                
+                # Calculate similarity
+                if key in cache_overlap_js and key in cache_overlap_oc:
+                    res_js = cache_overlap_js[key]
+                    res_oc = cache_overlap_oc[key]
                 else:
                     wrds1 = set(corpus["words_per_category"][cat1])
                     wrds2 = set(corpus["words_per_category"][cat2])
                     tot = wrds1.union(wrds2)
                     overlap = wrds1.intersection(wrds2)
-                    pct = len(overlap)/len(tot)
-                    cache_overlap[key1] = pct
-                    cache_overlap[key2] = pct
-                done.add(key1)
-                done.add(key2)
-                tab.append([cat1, cat2, pct])
-    tab = sorted(tab, key=lambda x: x[2], reverse=True)
+                    res_js = [len(overlap)/len(tot), len(wrds1), len(wrds2)]
+                    res_oc = [len(overlap)/min(len(wrds2),len(wrds2)), len(wrds1), len(wrds2)]
+                    cache_overlap_js[key] = res_js
+                    cache_overlap_oc[key] = res_oc
+            
+                # Check similarity to use
+                if similarity in [2, "oc", "overlap coefficient", "overlap"]:
+                    res = res_oc
+                elif similarity in [1, "ji", "jaccard similarity", "jaccard"]:
+                    res = res_js
+                else:
+                    error("Unknown similarity " + colored(similarity, "cyan"))
+                    return
+                tab.append([cat1, res[1], cat2, res[2], res[0]])
+    tab = sorted(tab, key=lambda x: x[4], reverse=True)
     
     # Start and end index
     si = sidx
     if sidx < 0:
         si = len(tab) + sidx
     
-    t = CustomizedTable(["", "Category 1", "Category 2", "Overlap"])
+    t = CustomizedTable(["", "Category 1", "Words", "Category 2", "Words", "Overlap"])
     t.column_style(0, {"color": "size"})
-    t.column_style([1, 2], {"color": "name"})
-    t.column_style(3, {"color": "percent", "num-format": "pct-2"})
+    t.column_style([1, 3], {"color": "name"})
+    t.column_style([2, 4], {"color": "value"})
+    t.column_style(5, {"color": "percent", "num-format": "pct-2"})
     for i,r in enumerate(tab[si:si+n]):
         t.add_row([si+i] + r)
     print()
     t.display()
-    print()
+    print()
```

### Comparing `mltlk-0.1.4/mltlk/ml.py` & `mltlk-0.1.5/mltlk/ml.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/mltlk/resampling.py` & `mltlk-0.1.5/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/mltlk/utils.py` & `mltlk-0.1.5/mltlk/utils.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.4/mltlk/word2vec.py` & `mltlk-0.1.5/mltlk/word2vec.py`

 * *Files identical despite different names*

