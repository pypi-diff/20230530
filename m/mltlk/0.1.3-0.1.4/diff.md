# Comparing `tmp/mltlk-0.1.3.tar.gz` & `tmp/mltlk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.3.tar", last modified: Mon May 29 08:26:33 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.4.tar", last modified: Tue May 30 11:14:11 2023, max compression
```

## Comparing `mltlk-0.1.3.tar` & `mltlk-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.419133 mltlk-0.1.3/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.3/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.3/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-29 08:26:33.418026 mltlk-0.1.3/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.3/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-26 11:59:23.000000 mltlk-0.1.3/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-26 11:58:57.000000 mltlk-0.1.3/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50617 2023-05-29 08:24:46.000000 mltlk-0.1.3/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    49905 2023-05-29 08:25:32.000000 mltlk-0.1.3/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.397067 mltlk-0.1.3/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.3/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.3/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.3/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.410925 mltlk-0.1.3/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)       73 2023-05-26 11:47:03.000000 mltlk-0.1.3/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32049 2023-05-29 08:23:55.000000 mltlk-0.1.3/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.3/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-29 06:55:45.000000 mltlk-0.1.3/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.3/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.416013 mltlk-0.1.3/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-29 08:26:32.000000 mltlk-0.1.3/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      412 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-29 08:26:32.000000 mltlk-0.1.3/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-29 08:26:33.000000 mltlk-0.1.3/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-29 08:26:33.419375 mltlk-0.1.3/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-26 11:47:12.000000 mltlk-0.1.3/setup.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-29 08:26:33.416995 mltlk-0.1.3/stopwords/
--rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.3/stopwords/custom.csv
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.271453 mltlk-0.1.4/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.4/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.4/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 11:14:11.270533 mltlk-0.1.4/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.4/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.4/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.4/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.4/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    23205 2023-05-30 11:09:49.000000 mltlk-0.1.4/Wikipedia_exploration.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.4/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.249960 mltlk-0.1.4/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.4/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.4/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.4/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.262811 mltlk-0.1.4/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 07:10:19.000000 mltlk-0.1.4/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     7301 2023-05-30 11:01:35.000000 mltlk-0.1.4/mltlk/exploration_textdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.4/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.4/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.4/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.4/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.267548 mltlk-0.1.4/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 11:14:10.000000 mltlk-0.1.4/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 11:14:10.000000 mltlk-0.1.4/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 11:14:11.000000 mltlk-0.1.4/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 11:14:11.271646 mltlk-0.1.4/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-29 08:47:52.000000 mltlk-0.1.4/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 11:14:11.268732 mltlk-0.1.4/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.4/stopwords/custom.csv
```

### Comparing `mltlk-0.1.3/LICENSE` & `mltlk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.3/Spiral.ipynb` & `mltlk-0.1.4/Spiral.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999824074074074%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.4\\n']}}}, 8: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m7.12\\x1b[0m sec\\n')], delete: [0]}}}}, 10: {'outputs': {0: {'text': "*

 * *            "{insert: [(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m1.21\\x1b[0m sec\\n')], delete: [0]}}}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.3\n"
+                        "0.1.4\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -102,15 +102,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m6.90\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m7.12\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.36%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.33%</td></tr></table>"
@@ -169,15 +169,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.12\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.21\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>97.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>97.76%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>97.67%</td></tr></table>"
```

### Comparing `mltlk-0.1.3/Weather.ipynb` & `mltlk-0.1.4/Weather.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996362433862434%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.4\\n']}}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m1.10\\x1b[0m sec\\n')], delete: [0]}}}}, 9: {'outputs': {0: {'text': "*

 * *            "['\\x1b[1m\\x1b[33mInfo: \\x1b[0mBuilding final model on all data took "*

 * *            "\\x1b[34m0.12\\x1b[0m sec\\n']}}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.3\n"
+                        "0.1.4\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -96,15 +96,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.01\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.10\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>64.29%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>63.24%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>62.86%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>64.29%</td></tr></table>"
@@ -182,15 +182,15 @@
             "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.18\u001b[0m sec\n"
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.12\u001b[0m sec\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)"
             ]
         },
```

### Comparing `mltlk-0.1.3/Wikipedia.ipynb` & `mltlk-0.1.4/Wikipedia.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9717598104056437%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.4\\n']}}}, 7: {'outputs': {0: {'text': {insert: "*

 * *            "[(0, 'Building and evaluating model using 10-fold cross validaton took "*

 * *            "\\x1b[34m0.21\\x1b[0m sec\\n')], delete: [0]}}}}, 10: {'outputs': {0: {'text': "*

 * *            "{insert: [(0, 'Building and evaluating model using train-test split took "*

 * *            "\\x1b[34m0.02\\x1b[0m sec\\n')], delete: [0]}}, 1: {'data': {'text/html': "*

 * *            '["<table><tr><td '*

 * *            "style='color […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.3\n"
+                        "0.1.4\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -103,15 +103,15 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.31\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.21\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
@@ -210,22 +210,22 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m0.32\u001b[0m sec\n",
+                        "Building and evaluating model using train-test split took \u001b[34m0.02\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>95.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>95.37%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>95.33%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.33%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.31%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>94.13%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.33%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -236,15 +236,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>96.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>3.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>5</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>9</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>100.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>22</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>86.96%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>23</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>13.04%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>3</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -255,15 +255,15 @@
                     "text": [
                         "\n"
                     ]
                 }
             ],
             "source": [
                 "evaluate_model(LinearSVC(), session, reload=False, conf={\n",
-                "    \"mode\": \"CV-10\",\n",
+                "    \"mode\": \"split\",\n",
                 "    \"categories\": True,\n",
                 "    \"seed\": 42,\n",
                 "})"
             ]
         },
         {
             "cell_type": "markdown",
@@ -278,76 +278,25 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.04\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.03\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(LinearSVC(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
             ]
         },
         {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Save session\n",
-                "Save session with data, models, preprocessing etc. to file."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 8,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession saved to \u001b[36msessions/wikipedia.gz\u001b[0m\n"
-                    ]
-                }
-            ],
-            "source": [
-                "save_session(session, \"wikipedia\")    "
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "#### Load session and use model"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 9,
-            "metadata": {},
-            "outputs": [
-                {
-                    "name": "stdout",
-                    "output_type": "stream",
-                    "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mSession loaded from \u001b[36msessions/wikipedia.gz\u001b[0m (created at \u001b[34m2023-05-29 10:24:37\u001b[0m from file \u001b[36mdata/wikipedia_300.csv.gz\u001b[0m)\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
-                    ]
-                }
-            ],
-            "source": [
-                "loaded_session = load_session(\"wikipedia\")\n",
-                "predict(\"This is an article about gamers - people who love playing games\", loaded_session)"
-            ]
-        },
-        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
```

### Comparing `mltlk-0.1.3/Wikipedia_word2vec.ipynb` & `mltlk-0.1.4/Wikipedia_word2vec.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996358890778534%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.4\\n']}}}, 3: {'outputs': {0: {'text': {insert: "*

 * *            "[(2, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mWord2vec model generated in "*

 * *            "\\x1b[34m3.10\\x1b[0m sec\\n'), (4, '\\x1b[1m\\x1b[33mInfo: \\x1b[0mWord2vec "*

 * *            "embeddings generated in \\x1b[34m9.68\\x1b[0m sec\\n')], delete: [4, 2]}}}}, 7: "*

 * *            "{'outputs': {0: {'text': {insert: [(0, 'Building and evaluating model using 10-fold "*

 * *            "cross validaton took \\x1b[34m1.89\ […]*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.3\n"
+                        "0.1.4\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
@@ -43,17 +43,17 @@
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\u001b[1m\u001b[33mInfo: \u001b[0mClean texts keeping letters and digits\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoad 180 stopwords from \u001b[36menglish, stopwords/custom.csv\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m5.32\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model generated in \u001b[34m3.10\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec model stored to \u001b[36mword2vec/wikipedia_300_75.w2v\u001b[0m\n",
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m13.96\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings generated in \u001b[34m9.68\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mWord2vec embeddings stored to \u001b[36mword2vec/wikipedia_300_75.emb\u001b[0m\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mLoaded \u001b[34m300\u001b[0m examples in \u001b[34m2\u001b[0m categories\n"
                     ]
                 }
             ],
             "source": [
                 "session = load_data(\"data/wikipedia_300.csv.gz\", conf={\n",
@@ -106,22 +106,22 @@
             "execution_count": 4,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m3.02\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.89\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>92.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>92.70%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>92.67%</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.67%</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -132,15 +132,15 @@
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
-                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.00%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>6.00%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>9</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>91.33%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>8.67%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>13</td></tr></table>"
+                            "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Category</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>Accuracy</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;row-toggle-background:0;'>n</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Games</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>94.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;font:Verdana 12px;'>&nbsp;&nbsp;Programming</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;font:Verdana 12px;'>5.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;font:Verdana 12px;'>8</td></tr><tr><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#048512;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>Programming</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>92.67%</td><td style='text-align:left;background:#eee;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#3b08d3;font-family:Verdana;font-size:12px;border-top:1px solid #aaa;font:Verdana 12px;'>150</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#fd8e8a;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>&nbsp;&nbsp;Games</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;num-format:pct-2;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>7.33%</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;row-toggle-background:0;color:#aaa4fa;font-family:Verdana;font-size:12px;border-bottom:1px solid #aaa;font:Verdana 12px;'>11</td></tr></table>"
                         ],
                         "text/plain": [
                             "<IPython.core.display.HTML object>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
@@ -150,15 +150,15 @@
                     "output_type": "stream",
                     "text": [
                         "\n"
                     ]
                 },
                 {
                     "data": {
-                        "image/png": "iVBORw0KGgoAAAANSUhEUgAAAgAAAAIACAYAAAD0eNT6AAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjYuMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8o6BhiAAAACXBIWXMAAA9hAAAPYQGoP6dpAAA9fElEQVR4nO3deVxU9f7H8fcACrKDJgqCiChuuKZllrmlZi5pZrdcsLRScy3S7P5MzC0rl9SbVpZbmpl5LZdSUTO1TUFNUzER9zVJEJF15veH16kJMKiBMc/r+XjMo+Z7vnPOZ0Zg3vP9fs8Zk8VisQgAABiKk6MLAAAAJY8AAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAANycXQBuLWYzWadOXNGXl5eMplMji4HAFBEFotFV65cUWBgoJycCv6cTwCAjTNnzig4ONjRZQAA/qaTJ0+qUqVKBW4nAMCGl5eXJOnYibfk7V3GwdUAxcPfd4CjSwCKkUWSxfr3vCAEANi4Mezv7V1G3t7uDq4GKC5Mb+F2Z/nTaVwWAQIAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAUEhff52gLp2nKzhouFyc+uqzVXEF9h00YIFcnPrqrRnrbdonTfxc9zabIC+PZ1TWb2ChjmuxWDT2lZWqFDhMnu5Pq+0Dr+vnn8/Z9ElOTlPvXnPl5zNAZf0G6ul+7ystLaPoTxL4E56ebpo6/QklHpuqK+nvaduO/9Odd1a56WPuv7+Gfogbp6sZ83To59fVJ+rePH0GDmqtI0lvKu3ae/rmu1fUuHFYcT0F/A8BACikq1czVbduiGbN7n3Tfqv+G6fvv09UYKBvnm1ZWbnq3r2xnh3QstDHfeP1dZo9a6PenhOlb757RR4erurQfqoyMrKsfXr3ekcHfjqtLze8qM9Wj9C2bYc14NkFhT4GUFjvzntKbR6oo76931X9yH9r44b9Wh87UoGBfvn2Dw0tp8/XPq+tWw6qUf0xmjljg96d95Tatq1j7fNojyZ6c9rjGj/uMzVuOFZ7957UuvXRuuMOr5J6WoZEAPiLzp07p2HDhik8PFxubm4KCAhQs2bNNGfOHKWnpzu6PBSDBx+sq/ETHtHDXRsV2Of06V81bOiHWvThAJUq5Zxne8y4rho+op0iIysV6pgWi0Uz39qgl//dWZ27NFTdusFasPBpnTnzqz5bFS9JOnjwjNZ/uU/vvPeU7rqrqu69t7pmzOypj5d9rzNnfv1rTxbIh5tbKXV75E6NHvmxtm1LUGLiBb06bpWOHLmgAQNb5fuYZwe0UlLSRb0YvUyHDp3V2/+J1acrdmrYiHbWPiOeb695723VwgXbdPDgGQ0asEDp6Vl68qnmJfXUDIkA8BccPXpUDRo00IYNGzRp0iTt3r1b3377rUaOHKk1a9YoNjbW0SXCAcxms6L6vKsXoh9U7dpBdtlnUtJFnTuXotZtalnbfHzc1eSuqvru20RJ0nffHpGvr7vNMGybNrXl5GTSD98ftUsdgCS5uDjLxcVZGRnZNu0Z17LU7N5q+T7m7qbh2hT7k03bhvX7dXfTcElSqVLOatgo1KaPxWLRptifrH1QPAgAf8GgQYPk4uKiXbt2qUePHqpZs6bCwsLUpUsXrV27Vp06dZIkTZs2TZGRkfLw8FBwcLAGDRqktLQ0634WLFggX19frVmzRhEREXJ3d1f37t2Vnp6uhQsXKjQ0VH5+fho6dKhyc3Otj8vMzFR0dLSCgoLk4eGhu+66S1999ZV1+/Hjx9WpUyf5+fnJw8NDtWvX1rp160rs9TGq16esk4uLk4YMfcBu+zx3LkWSFBDgY9MeEOCtc+dTrH3Kl/e22e7i4ix/fw/r4wF7SEvL0Lff/Kx/j+msihV95eRk0hM979HdTcNVoaJvvo8JqOCjC+dTbdounE+Rj4+73NxKqVw5L7m4OOvC+ZQ8fSpUsP25h325OLqAf5pLly5ZP/l7eHjk28dkMkmSnJycNHPmTFWpUkVHjx7VoEGDNHLkSL399tvWvunp6Zo5c6aWLVumK1euqFu3buratat8fX21bt06HT16VI888oiaNWumxx57TJI0ePBgHThwQMuWLVNgYKD++9//qn379tq3b5+qVaum5557TllZWfr666/l4eGhAwcOyNPTM99aMzMzlZmZab2fmpqabz/cXFzcMc2auUE748ZZ//2B21FU73c174N+OnnmLeXk5Gp3/HEt++g7NWwU6ujSUEQEgCI6cuSILBaLIiIibNrLlSunjIzrq66fe+45TZkyRcOHD7duDw0N1YQJEzRgwACbAJCdna05c+aoatWqkqTu3btr8eLFOn/+vDw9PVWrVi21bNlSW7Zs0WOPPaYTJ05o/vz5OnHihAIDAyVJ0dHR+vLLLzV//nxNmjRJJ06c0COPPKLIyEhJUlhYwatpJ0+erHHjxtnltTGy7dsSdOHCFVWp/IK1LTfXrBejl2nmWxuUmDT1L+33xieg8+dTVPF3n7DOn09V/Xoh1j4XLtgGt5ycXCUnX+UTFOzu6NELatVistzdS8vbu4zOnUvR0mWDlHT0Qr79z59LUfkA2xGq8gE+SklJV0ZGtn755YpycnJV/g+jXOUDfBjBKmZMAdjJDz/8oD179qh27drWT9SxsbFq3bq1goKC5OXlpd69e+vSpUs2iwTd3d2tb/6SFBAQoNDQUJtP7AEBAbpw4fov1759+5Sbm6vq1avL09PTetu6dasSE6/PCQ8dOlQTJkxQs2bNNHbsWP34448F1j169GilpKRYbydPnrTr62IUvXo30+694xW3+1XrLTDQVy9EP6h1X0b/5f1WqXKHKlTw0eZNB6xtqanX9MP3ibq76fWfm7ubhuvy5XTFxR2z9tm8+aDMZoua3MWpVCge6elZOncuRb6+7mrbro4+/2x3vv2++/aIWrWuZdPW5oHa+u7bI5Kk7Oxcxccds+ljMpnUqnUtax8UD0YAiig8PFwmk0kJCQk27Tc+ZZcpU0aSdOzYMXXs2FEDBw7UxIkT5e/vr+3bt6tfv37KysqSu7u7JKlUqVI2+zGZTPm2mc1mSVJaWpqcnZ0VFxcnZ2fbVeY3QkP//v3Vrl07rV27Vhs2bNDkyZM1depUDRkyJM/zcXV1laur6199OQwlLS1DR46ct95PSvpFe/Ycl7+/p0JCyqpsWdtpllKlnFWhgo8iIipa206cuKTk5DSdOJGs3FyL9uw5LkkKDw+Qp6ebJKl2zZc0cdKjerhrI5lMJg0d1laTJq5WtWoVFFqlnMa+slKBgX7q8nBDSVLNmoFq1z5SA56Zr//MiVJ2dq6GDVmsx/51V4GnZgF/Vdu2df73N/CswsMD9Nobjynh0FktmL9NkjRx0qMKDPLTk1HvSpLembtZgwa30WtTemj+B9vUslVNPdqjiTo/NM26z+nTvtT8hU8rbleSdv5wVEOHt5OHh6t1nygeBIAiKlu2rB544AHNnj1bQ4YMKXAdQFxcnMxms6ZOnSonp+sDLcuXL//bx2/QoIFyc3N14cIF3XfffQX2Cw4O1oABAzRgwACNHj1a7733Xr4BAIW3a1eS2rSaYr0f/cJHkqQ+Uc30wfynC7WPmLErtWjhDuv9OxuOlSTFbh6lFi1qSpISEs4pJeW3UaIXR3bQ1auZGvDsfF2+nK5m91bX2i9ekJtbaWufxR8+q6FDPlTbNq/Lycmkbt3u1IyZPf/6kwUK4O3jromTH1WlSn5KTr6qlZ/u0ph/r1BOzvWFyhUq+igkxN/a/9ixX9T5oWl6c/oTGjKsrU6d+lXP9P9AGzbst/b5ZPkPuuMOb8W82k0VKvho754Teqj9m3mmtmBfJovFYnF0Ef80iYmJatasmfz8/BQTE6O6devKyclJO3fuVHR0tHr27Kk+ffqofv36mjFjhjp16qQdO3Zo9OjROn36tH799Vf5+vpqwYIFGj58uC5fvmzdd0xMjFatWqU9e/ZY2/r27avLly9r1apVkqRevXppx44dmjp1qho0aKCLFy9q06ZNqlu3rh566CENHz5cDz74oKpXr65ff/1VgwYNUuXKlfXxxx//6XNLTU2Vj4+Pki+/K29vdzu/csCtwcUpytElAMXIIsmslJQUeXt7F9iLEYC/oGrVqtq9e7cmTZqk0aNH69SpU3J1dVWtWrUUHR2tQYMGyd3dXdOmTdOUKVM0evRoNW/eXJMnT1afPn3+9vHnz5+vCRMm6IUXXtDp06dVrlw53X333erYsaMkKTc3V88995xOnTolb29vtW/fXtOnT//bxwUA3D4YAYANRgBgBIwA4PZWuBEAzgIAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAREAAAAwIAIAAAAGRAAAAMCACAAAABgQAQAAAAMiAAAAYEAEAAAADIgAAACAAbkUptPnn39e6B127tz5LxcDAABKRqECwMMPP1yonZlMJuXm5v6degAAQAkoVAAwm83FXQcAAChBf2sNQEZGhr3qAAAAJajIASA3N1fjx49XUFCQPD09dfToUUnSmDFj9P7779u9QAAAYH9FDgATJ07UggUL9Prrr6t06dLW9jp16mjevHl2LQ4AABSPIgeARYsW6d1331XPnj3l7Oxsba9Xr54OHTpk1+IAAEDxKHIAOH36tMLDw/O0m81mZWdn26UoAABQvIocAGrVqqVt27blaV+xYoUaNGhgl6IAAEDxKtRpgL/3yiuvKCoqSqdPn5bZbNbKlSuVkJCgRYsWac2aNcVRIwAAsLMijwB06dJFq1evVmxsrDw8PPTKK6/o4MGDWr16tR544IHiqBEAANhZkUcAJOm+++7Txo0b7V0LAAAoIX8pAEjSrl27dPDgQUnX1wU0atTIbkUBAIDiVeQAcOrUKT3++OPasWOHfH19JUmXL1/WPffco2XLlqlSpUr2rhEAANhZkdcA9O/fX9nZ2Tp48KCSk5OVnJysgwcPymw2q3///sVRIwAAsLMijwBs3bpV33zzjSIiIqxtERERmjVrlu677z67FgcAAIpHkUcAgoOD873gT25urgIDA+1SFAAAKF5FDgBvvPGGhgwZol27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qfbt21sfN3XqVC1YsEAffPCBtm/fruTkZP33v/+96XH79Omjjz76SDNnztTBgwf1zjvvyNPTU8HBwfr0008lSQkJCTp79qzeeustSdLkyZO1aNEizZ07Vz/99JNGjBihXr16aevWrZKuB5Vu3bqpU6dO2rNnj/r376+XXnqpyK+Jl5eXFixYoAMHDuitt97Se++9p+nTp9v0OXLkiJYvX67Vq1fryy+/1O7duzVo0CDr9iVLluiVV17RxIkTdfDgQU2aNEljxozRwoULi1wPUCALABRCVFSUpUuXLhaLxWIxm82WjRs3WlxdXS3R0dHW7QEBAZbMzEzrYxYvXmyJiIiwmM1ma1tmZqalTJkylvXr11ssFoulYsWKltdff926PTs721KpUiXrsSwWi+X++++3DBs2zGKxWCwJCQkWSZaNGzfmW+eWLVsskiy//vqrtS0jI8Pi7u5u+eabb2z69uvXz/L4449bLBaLZfTo0ZZatWrZbB81alSeff2RJMt///vfAre/8cYblkaNGlnvjx071uLs7Gw5deqUte2LL76wODk5Wc6ePWuxWCyWqlWrWpYuXWqzn/Hjx1uaNm1qsVgslqSkJIsky+7duws8LvBnWAMAoNDWrFkjT09PZWdny2w264knnlBMTIx1e2RkpM28/969e3XkyBF5eXnZ7CcjI0OJiYlKSUnR2bNnddddd1m3ubi46M4778wzDXDDnj175OzsrPvvv7/QdR85ckTp6el64IEHbNqzsrLUoEEDSdLBgwdt6pCkpk2bFvoYN3z88ceaOXOmEhMTlZaWppycHHl7e9v0CQkJUVBQkM1xzGazEhIS5OXlpcTERPXr109PP/20tU9OTo58fHyKXA9QEAIAgEJr2bKl5syZo9KlSyswMFAuLrZ/Qn7/bW+SlJaWpkaNGmnJkiV59nXHHXf8pRrKlClT5MekpaVJktauXWvzxivJ5lvr/q5vv/1WPXv21Lhx49SuXTv5+Pho2bJlmjp1apFrfe+99/IEEmdnZ7vVChAAABSah4eHwsPDC92/YcOG+vjjj1W+fPk8n4JvqFixor7//ns1b95c0vVPunFxcWrYsGG+/SMjI2U2m7V161a1adMmz/YbIxC5ubnWtlq1asnV1VUnTpwocOSgZs2a1gWNN3z33Xd//iR/55tvvlHlypX173//29p2/PjxPP1OnDihM2fOKDAw0HocJycnRUREKCAgQIGBgTp69Kh69uxZpOMDRcEiQADFpmfPnipXrpy6dOmibdu2KSkpSV999ZWGDh2qU6dOSZKGDRum1157TatWrdKhQ4c0aNCgm57DHxoaqqioKD311FNatWqVdZ/Lly+XJFWuXFkmk0lr1qzRxYsXlZaWJi8vL0VHR2vEiBFauHChEhMTFR8fr1mzZlkX1g0YMEA///yzXnzxRSUkJGjp0qVasGBBkZ5vtWrVdOLECS1btkyJiYmaOXNmvgsa3dzcFBUVpb1792rbtm0aOnSoevTooQoVKkiSxo0bp8mTJ2vmzJk6fPiw9u3bp/nz52vatGlFqge4GQIAgGLj7u6ur7/+WiEhIerWrZtq1qypfv36KSMjwzoi8MILL6h3796KiopS06ZN5eXlpa5du950v3PmzFH37t01aNAg1ahRQ08//bSuXr0qSQoKCtK4ceP00ksvKSAgQIMHD5YkjR8/XmPGjNHkyZNVs2ZNtW/fXmvXrlWVKlUkXZ+X//TTT7Vq1SrVq1dPc+fO1aRJk4r0fDt37qwRI0Zo8ODBql+/vr755huNGTMmT7/w8HB169ZNHTp0UNu2bVW3bl2b0/z69++vefPmaf78+YqMjNT999+vBQsWWGsF7MFkKWilDQAAuG0xAgAAgAERAAAAMCACAAAABkQAAADAgAgAAAAYEAEAAAADIgAAAGBABAAAAAyIAAAAgAERAAAAMCACAAAABvT/WGfe9yXoYKQAAAAASUVORK5CYII=\n",
+                        "image/png": "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\n",
                         "text/plain": [
                             "<Figure size 640x480 with 1 Axes>"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
@@ -213,15 +213,15 @@
             "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m2.67\u001b[0m sec\n",
+                        "Building and evaluating model using 10-fold cross validaton took \u001b[34m1.70\u001b[0m sec\n",
                         "\n"
                     ]
                 },
                 {
                     "data": {
                         "text/html": [
                             "<table><tr><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'>Results</td><td style='color:black;background:#ddd;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;font-weight:bold;border-top:1px solid #aaa;border-bottom:1px solid #aaa;font:Verdana 12px;text-align:left;'></td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Accuracy:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>F1-score:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);font:Verdana 12px;'>93.67%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>Precision:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(100%);font:Verdana 12px;'>93.68%</td></tr><tr><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>Recall:</td><td style='text-align:left;background:white;padding-top:3px;padding-bottom:3px;padding-left:5px;padding-right:15px;color:#7a03fc;num-format:pct-2;font-family:Verdana;font-size:12px;filter:brightness(96%);border-bottom:1px solid #aaa;font:Verdana 12px;'>93.67%</td></tr></table>"
@@ -281,15 +281,15 @@
             "execution_count": 7,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.26\u001b[0m sec\n",
+                        "\u001b[1m\u001b[33mInfo: \u001b[0mBuilding final model on all data took \u001b[34m0.21\u001b[0m sec\n",
                         "\u001b[1m\u001b[33mInfo: \u001b[0mExample is predicted as \u001b[32mGames\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "build_model(RandomForestClassifier(), session)\n",
                 "predict(\"This is an article about gamers - people who love playing games\", session)"
```

### Comparing `mltlk-0.1.3/data/spiral.csv` & `mltlk-0.1.4/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.3/data/wikipedia_300.csv.gz` & `mltlk-0.1.4/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.3/mltlk/ml.py` & `mltlk-0.1.4/mltlk/ml.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,32 +104,25 @@
         if verbose >= 1:
             s = ""
             for li,ni in cnt.items():
                 if ni < conf["min_samples"]:
                     s += li + ", "
             if s != "":
                 info("Removed minority categories " + colored(s[:-2], "cyan"))
-    
-    # Encode labels
-    if "encode_labels" in conf and conf["encode_labels"]:
-        session["label_encoder"] = LabelEncoder().fit(session["y"])
-        session["y"] = session["label_encoder"].transform(session["y"])
-        if verbose >= 1:
-            info("Labels encoded")
             
     # Check text inputs without text preprocessing
     if conf["preprocess"] not in ["bag-of-words", "bow", "wordtovec", "word2vec"]:
-        if type(X[0]) == str:
+        if type(session["X"][0]) == str:
             error("Input seems to be text but no text-preprocessing is set")
             return None
         
     # Check ordinal features without encoding
     if conf["preprocess"] not in ["one-hot", "onehot", "one hot", "ordinal"]:
-        if type(X[0]) != str:
-            for xi in X[0]:
+        if type(session["X"][0]) != str:
+            for xi in session["X"][0]:
                 if type(xi) == str:
                     error("Input contains ordinal features but no encoding is set (use " + colored("one-hot", "blue") + " or " + colored("ordinal", "blue") + ")")
                     return None
     
     # Clean text inputs
     if "clean_text" in conf and conf["preprocess"] in ["word2vec", "bag-of-words", "bow"]:
         clean = True
@@ -141,38 +134,48 @@
             warning("Invalid clean text mode " + colored(conf["clean_text"], "cyan"))
             clean = False
         if clean:
             for i,xi in enumerate(session["X"]):
                 # Remove new line and whitespaces
                 xi = xi.replace("<br>", " ")
                 xi = xi.replace("&nbsp;", " ")
+                xi = xi.replace("\n", " ")
                 # Remove special chars
                 if conf["clean_text"] in [2, "letters digits", "digits letters"]:
                     xi = re.sub("[^a-zA-Z0-9åäöÅÄÖ ]", " ", xi)
                 else:
                     xi = re.sub("[^a-zA-ZåäöÅÄÖ ]", " ", xi)
                 # Remove multiple whitespaces
                 xi = " ".join(xi.split())
                 # Set to lower case
                 xi = xi.lower()
                 # Strip trailing/leading whitespaces
                 xi = xi.strip()
                 session["X"][i] = xi
+            session["X_original"] = session["X"].copy()
+    
+    # Encode labels
+    if "encode_labels" in conf and conf["encode_labels"]:
+        session["label_encoder"] = LabelEncoder().fit(session["y"])
+        session["y"] = session["label_encoder"].transform(session["y"])
+        if verbose >= 1:
+            info("Labels encoded")
     
     # Bag-of-words representation for input texts
     if conf["preprocess"] in ["bag-of-words", "bow"]:
         sw = load_stopwords(conf, verbose=verbose)
         l = "Used bag-of-words"
         if "stopwords" in conf:
             l += " with stopwords removed"
         elif verbose >= 1:
             l = "Used bag-of-words"
         session["bow"] = CountVectorizer(stop_words=sw).fit(session["X"]) #todo: max_features=max_words, ngram_range=ngram)
         session["X"] = session["bow"].transform(session["X"])
-    
+        session["stopwords"] = sw
+        
         # TF-IDF conversion for bag-of-words
         if "TF-IDF" in conf and conf["TF-IDF"] or "tf-idf" in conf and conf["tf-idf"]:
             session["TF-IDF"] = TfidfTransformer().fit(session["X"])
             session["X"] = session["TF-IDF"].transform(session["X"])
             l += " and TF-IDF"
         if verbose >= 1:
             info(l)
```

### Comparing `mltlk-0.1.3/mltlk/resampling.py` & `mltlk-0.1.4/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.3/mltlk/utils.py` & `mltlk-0.1.4/mltlk/utils.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Basic stuff
 from termcolor import colored
 import time
 from datetime import datetime
+from os.path import exists
+import pandas as pd
 # Stopwords
 from nltk.corpus import stopwords
-import pandas as pd
-from os.path import exists
 
 
 #
 # Error message
 #
 def error(e):
     print(colored("Error: ", "red", attrs=["bold"]) + e)
```

### Comparing `mltlk-0.1.3/mltlk/word2vec.py` & `mltlk-0.1.4/mltlk/word2vec.py`

 * *Files identical despite different names*

